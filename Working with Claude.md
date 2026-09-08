# Working with Claude

Notes on how I actually work with Claude day to day -- from connecting GitHub through to building custom skills.

## Git and GitHub, in plain terms

- **Git**: tracks changes to a folder of files (a "repository") over time -- a detailed save history.
- **GitHub**: the website that hosts git repositories online, so people (and tools) can share and collaborate on them. Git is the tool; GitHub is where the repo lives.
- **Repository ("repo")**: the project folder itself, plus its entire history of changes.
- **Commit**: a saved snapshot of changes with a short message describing what and why -- a labeled checkpoint you can always return to.
- **Branch**: a separate line of work split off from the main version, so changes don't touch the "real" version until ready. The default branch is usually `main`; a new piece of work gets its own branch.
- **Push**: uploading local commits to GitHub so they're visible online.
- **Pull / fetch**: the reverse -- downloading the latest changes from GitHub.
- **Pull request (PR)**: a request to merge one branch into another, usually `main` -- literally "please pull my changes in." It's also where comments, requested changes, and automated checks happen before anything lands.
- **Merge**: combining a branch's changes into another, typically closing the PR.
- **Merge conflict**: when two branches changed the same lines differently and git can't decide automatically -- a human (or Claude) resolves it by hand.

## Connecting GitHub

Claude connects to GitHub via an authorization link, not a password -- via claude.ai Settings → Connectors. Access is scoped per repository, not "all of GitHub": someone with admin rights has to explicitly grant which repos Claude can see. If Claude can't reach a repo, that's almost always a permissions issue, not a bug.

Once connected, Claude can read issues and PRs, create branches, commit, push, and open pull requests -- the same actions a person would take through the GitHub website or command line. The repos available to a session are listed explicitly up front; Claude has to add a repo before it can touch it, it can't just guess at a URL.

## Working in a session

Each session works inside its own fresh, isolated copy of a repo. Nothing sticks around after the session ends unless it was **committed and pushed** first -- "did you save it?" really means "did you push it?"

Claude works on its own branch per task, never directly on `main` unless told to -- same as a cautious human contributor. Good etiquette:

- Check what's already there (`git status`) before anything that could discard unsaved work.
- Small, focused commits with clear messages, not one giant "fixed everything" commit.
- Don't skip safety checks or force-push over history without asking -- fix the actual problem instead.

## Pull requests and review

Claude can watch a PR and react automatically to a failed check or a reviewer comment. It treats PRs differently by ownership: one it opened is its responsibility to get mergeable; one it's just watching gets bigger decisions raised as a question rather than changed unilaterally. Every comment or reply it posts on GitHub carries a small signature, so it's always clear it came from Claude.

## Skills

A **skill** is a saved, reusable set of instructions for a task that comes up repeatedly -- a review checklist, a formatting style, a repo-specific process. Trigger one with `/skill-name` instead of re-explaining the same thing every time. Skills can be personal, project-specific (stored in the repo so everyone gets the same playbook), or shared org-wide. Claude will surface a relevant skill on its own when a task matches, and suggest creating one if it notices the same kind of task recurring without one.

### Making your own

The **skill-creator** skill helps build a new skill, edit an existing one, and test whether it actually works before relying on it. What matters most:

- **Trigger description**: the short description Claude checks a request against. Too vague and it never fires; too broad and it fires on the wrong things.
- **Instructions**: write them like a briefing for a smart colleague who's never seen this before -- specific steps and file names, not "do the usual thing."
- **Scope discipline**: one job done well (e.g. "review this code for bugs"), not everything at once.

Skills can be tested and benchmarked before relying on them -- worth doing, since a skill whose description is too generic will simply never trigger.

## Habits that make it smoother

- Being explicit about scope keeps Claude from doing too much or too little.
- Asking Claude to explain its understanding of the code before changing it is a good sanity check.
- For anything with real consequences -- pushing code, sending messages, deleting things -- Claude asks for confirmation by default. Rely on that rather than pre-approving broad, hard-to-undo actions.
