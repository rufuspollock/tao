# Standups

Standups are part of the [agile methodology](https://playbook.datopian.com/agile/). They keep the team in sync, identify blockers, and flag changes that require coordination or reprioritisation. Teams can do them live or asynchronously in a shared chat channel.

Standups are there to inform others. When they get too long, people stop reading—and miss the important parts. Keep them concise and consolidate related work into fewer bullets. Prioritise blockers and what you expect to achieve today. Keep routine task details in the relevant work items.

## Format

Put the information people most need to act on first:

1. **Blockers:** What's blocked, who can help, and what they need to do. If there are none, say “None”.
2. **Today:** What will you actually achieve? Name the main outcomes you realistically expect to finish, rather than listing everything you might work on.
3. **Completed:** What changed since your last update? Use the actual day if that was Monday rather than yesterday.
4. **Availability (optional):** Mention changes to your usual availability that affect others.

Aim for three or four grouped bullets overall when possible; for a fuller update, two or three short bullets under each heading can still be easy to scan. These are guides, not quotas. One big outcome for today may be enough, with a second bullet for routine operations if colleagues need to know about them.

Each bullet should tell colleagues **what changed, what will be finished, or where help is needed**. Grouping should shorten the update without losing the concrete details:

- **Name a finish line.** “Progress the website” leaves people guessing. “Send the homepage draft to Asdra for review” tells them what to expect. Use the real intended outcome; don't invent one to make the update sound better.
- **Group related work.** A short bold label such as **Travel paperwork** can bring related tasks together. Keep the bullet to one or two short sentences; don't hide eight tasks inside one long paragraph.
- **Select what matters to colleagues.** “Handled urgent items” is too vague. Name the relevant result or leave it out. Meetings usually only need mentioning when they produced a decision or changed the plan.
- **Link to the detail.** Routine administration can be a brief line with a link to the relevant work items or board. The standup does not need to reproduce the task list.

This is an application of [[Information Efficiency]]: a colleague should be able to skim the message in about 20 seconds and know what matters today.

## Template for posting in chat

```md
### Blockers
- **[Person who can help]:** [Action needed] so I can [blocked outcome]. [Task link]

### Today — [day]
- [Main outcome I expect to finish.]
- [Second outcome or a brief grouped operations item, if useful.]

### Completed — [day of previous work]
- [Concrete result colleagues need to know about.]
- [Another meaningful result, if useful.]
```

Post the update in chat. In a live standup, use the task board to highlight major items and discuss anything that needs coordination.

## Concrete example: refining Fae's standup

Here is a real standup someone sent, followed by two progressively shorter rewrites. Notice the inversion of order: **blocker → today → completed**, so the request for help is visible immediately.

### Original update

Transcribed from Fae's standup screenshot, shared on 23 September 2026. Issue links have been reconstructed from the visible repository and issue numbers. The screenshot's “meeting notes” link had no visible destination, so it is retained as plain text.

> **Monday (21/09/2026) – Done**
>
> - Final edit and submission of Sylvie's personal reference for Boaz and Monica
> - Updated backlog projects and tasks (on GitHub) and reminders for me to give Sylvie, based on meeting notes: Taiwan [life-itself/onboarding#84](https://github.com/life-itself/onboarding/issues/84) / Temple of the Sacred World [life-itself/onboarding#111](https://github.com/life-itself/onboarding/issues/111)
> - Sylvie Email management
> - Updated OML shipment contact to ops@ instead of Sylvie
> - Practice planning exercise from Rufus: `briefings/2026-09-21-asdra-and-fae-planning-practice.md`
> - Prioritised tasks from Sylvie's last meeting – added to GitHub, executed quick/urgent items, checked for any requests from Sylvie while she's away
> - Gave feedback to Asdra on the Life Itself TAO
> - Meeting: standup with Asdra (meeting notes)
> - Meeting: LI Coordination with Rufus and Asdra
>
> **Today (23/09/2026) – planned**
>
> - Review LI Coordination notes/transcript and practise the AI & strategy skills Rufus walked through
> - Apply to ESTA for Sylvie and family
> - French translator – see how far the passport application can get completed without Sylvie or Rufus [life-itself/onboarding#102](https://github.com/life-itself/onboarding/issues/102)
> - Provide feedback to Sylvie [life-itself/onboarding#116](https://github.com/life-itself/onboarding/issues/116)
> - Eternity Magazine – draft announcement and review Google form [life-itself/onboarding#115](https://github.com/life-itself/onboarding/issues/115)
> - SCQH Website
> - Close Framer issue with Asdra
> - Scan Sylvie's emails for any urgent follow ups
>
> **Blockers**
>
> - Payment for PA admin tasks (e.g. passport/visa) – need Rufus to set up a card [life-itself/planning#15 “PA blocker: payment card required”](https://github.com/life-itself/planning/issues/15)

The useful information is there, but the blocker comes last in an 18-bullet update. Major outcomes, routine administration, and meeting attendance all receive similar weight.

### Version 1: group related work and put the blocker first

#### Blocker

- **Payment card:** Rufus to set up a card for PA tasks requiring payment, including passport/visa applications ([#15](https://github.com/life-itself/planning/issues/15)).

#### Today — Wednesday 23 September

- **Travel paperwork:** Complete ESTA applications for Sylvie and family if payment is available; progress the passport application as far as possible without Sylvie or Rufus.
- **Communications and website:** Draft the Eternity Magazine announcement and review the submission form; progress the SCQH website and close the Framer issue with Asdra.
- **Planning and routine support:** Review coordination notes and practise the AI/strategy skills; provide feedback to Sylvie and check her inbox for urgent follow-ups.

#### Completed — Monday 21 September

- **Planning and coordination:** Updated and prioritised the backlog from Sylvie's meeting notes, handled urgent items, and joined team coordination.
- **Learning and feedback:** Completed Rufus's planning exercise and gave Asdra feedback on the Life Itself TAO.
- **PA and administration:** Submitted Sylvie's personal reference for Boaz and Monica, managed her inbox, and updated the OML shipment contact.

This reduces 18 bullets to seven and makes the blocker easy to find. But it is an intermediate edit: “progress the SCQH website” still has no finish line, and “handled urgent items” does not tell colleagues what happened. Grouping alone is not enough.

### Version 2: select the important outcomes and keep them concrete

This version illustrates a narrower daily focus. It assumes these are the day's priorities and that completing the ESTA applications is realistic if the card is available. Omitted tasks belong in the work tracker; leaving them out of the standup does not cancel them.

#### Blocker

- **Rufus:** Please set up the payment card so I can complete PA applications requiring payment ([#15](https://github.com/life-itself/planning/issues/15)).

#### Today — Wednesday

- Draft the Eternity Magazine announcement and review the submission form.
- Complete the family's ESTA applications, subject to the payment card being available.
- Close the Framer issue with Asdra; check Sylvie's inbox for urgent follow-ups.

#### Completed — Monday

- Submitted Sylvie's personal reference for Boaz and Monica.
- Updated the Taiwan and Temple of the Sacred World backlog from meeting notes.
- Completed the planning exercise and gave Asdra feedback on the Life Itself TAO.

The second version keeps the same clear headings but gives each bullet less work to do. It removes meeting attendance and minor administration, names the backlog work, and leaves out the website until its intended outcome is clear. If the website is a priority today, include it with a concrete finish line and make room by removing a lower-priority item.

Keep the detailed checklists in the work tasks. Short standups are easier to read: the priority is making blockers visible and showing what you expect to achieve today.

## Discussion after the update

### Linger topics

To keep the standup focused, if substantive items arise (e.g. discussion around a blocker) add them to a dedicated **"linger" topic** section. These topics are:

- Either dealt with when the formal standup ends during a "linger" time with the relevant parties staying in the meeting (hence the term "linger topic")
- Or: dealt with in separate follow-up meetings e.g. "OK, there's a big question around X, let's schedule a meeting for tomorrow to go over it"

NB: it can be worth scheduling in a dedicated "linger" time in a standup meeting. e.g. if the standup is normally 15m then you add a 15m "linger" segment. If there is no linger material people can just get the time back and use it for something else.
