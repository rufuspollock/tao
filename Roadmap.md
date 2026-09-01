# Roadmap for the TAO

<style>
  .rm-wrap {
    --paper-raised: #fffdf8;
    --accent: #327e09;
    --accent-soft: #e4ecdd;
    --line: #ded7c4;
    --muted: #746b57;
    max-width: 900px;
    margin: 0 auto;
    padding: 1rem 0 2rem;
    font-family: "Wittgenstein", ui-serif, Georgia, serif;
  }
  @media (prefers-color-scheme: dark) {
    .rm-wrap:not([data-theme="light"]) {
      --paper-raised: #202020;
      --accent: #4f9c22;
      --accent-soft: #223122;
      --line: #3a3a37;
      --muted: #a6a08e;
    }
  }
  .rm-tree { display: flex; flex-direction: column; align-items: center; gap: 0; }
  .rm-node {
    position: relative;
    z-index: 2;
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.7rem 1.3rem;
    background: var(--accent);
    color: var(--paper-raised);
    border-radius: 999px;
    font-weight: 600;
    font-size: 1rem;
    text-decoration: none;
    box-shadow: 0 1px 2px rgba(0,0,0,.08);
  }
  .rm-node .rm-n { font-size: 0.7rem; opacity: .75; font-family: ui-sans-serif, system-ui, sans-serif; }
  .rm-node:hover { filter: brightness(0.92); }
  .rm-connector { width: 2px; height: 1.75rem; background: var(--line); }
  .rm-branch-row {
    display: flex;
    align-items: flex-start;
    justify-content: center;
    gap: 2.5rem;
    width: 100%;
    position: relative;
    padding: 1.75rem 0;
  }
  .rm-branch-row::before {
    content: "";
    position: absolute;
    top: 0;
    left: 50%;
    width: 2px;
    height: 100%;
    background: var(--line);
    z-index: 0;
  }
  .rm-branch {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.6rem;
    position: relative;
    z-index: 1;
  }
  .rm-branch::before {
    content: "";
    position: absolute;
    top: -1.75rem;
    left: 50%;
    width: 1px;
    height: 1.75rem;
    background: var(--line);
  }
  .rm-chip {
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    padding: 0.4rem 0.85rem;
    border-radius: 999px;
    background: var(--paper-raised);
    border: 1.5px solid var(--line);
    font-size: 0.82rem;
    font-weight: 500;
    text-decoration: none;
    white-space: nowrap;
  }
  .rm-chip.own { border-color: var(--accent); color: var(--accent); }
  .rm-chip.ext { border-style: dashed; border-color: var(--muted); color: var(--muted); }
  .rm-chip.inline { border-style: dotted; color: var(--muted); }
  .rm-chip:hover { background: var(--accent-soft); }
  .rm-legend {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1.4rem;
    margin-top: 2.5rem;
    font-size: 0.8rem;
    color: var(--muted);
    font-family: ui-sans-serif, system-ui, sans-serif;
  }
  .rm-legend-item { display: flex; align-items: center; gap: 0.4rem; }
  .rm-swatch { width: 1rem; height: 1rem; border-radius: 999px; border: 1.5px solid var(--line); }
  .rm-swatch.own { border-color: var(--accent); }
  .rm-swatch.ext { border-style: dashed; border-color: var(--muted); }
  .rm-swatch.inline { border-style: dotted; border-color: var(--muted); }
</style>

<div class="rm-wrap">
  <div class="rm-tree">

    <a class="rm-node" href="https://tao.rufuspollock.com"><span class="rm-n">01</span> Index</a>
    <div class="rm-connector"></div>

    <a class="rm-node" href="https://lifeitself.org/tao/getting-stuff-done"><span class="rm-n">02</span> Getting Stuff Done</a>
    <div class="rm-branch-row">
      <div class="rm-branch">
        <a class="rm-chip ext" href="https://rufuspollock.com/post/getting-things-done">GTD</a>
        <a class="rm-chip own" href="https://tao.rufuspollock.com/KISS+Principle">KISS Principle</a>
      </div>
      <div class="rm-branch">
        <a class="rm-chip inline" href="https://tao.rufuspollock.com#views">Key Views</a>
      </div>
    </div>

    <a class="rm-node" href="https://tao.rufuspollock.com/Five+levels+of+agency"><span class="rm-n">03</span> Five Levels of Agency</a>
    <div class="rm-connector"></div>

    <a class="rm-node" href="https://tao.rufuspollock.com/Hypotheses"><span class="rm-n">04</span> Hypotheses + Open-Minded Rigour</a>
    <div class="rm-branch-row">
      <div class="rm-branch">
        <a class="rm-chip ext" href="https://tao.lifeitself.org/principles/#experimentation-and-creativity">Experimentation and Creativity</a>
      </div>
      <div class="rm-branch">
        <a class="rm-chip ext" href="https://tao.lifeitself.org/principles/#zen--mindfulness">Zen and Mindfulness</a>
      </div>
    </div>

    <a class="rm-node" href="https://tao.rufuspollock.com/Project+Phase+and+Status"><span class="rm-n">05</span> Project System</a>
    <div class="rm-branch-row">
      <div class="rm-branch">
        <a class="rm-chip own" href="https://tao.rufuspollock.com/Definition+of+Done">Definition of Done</a>
      </div>
      <div class="rm-branch">
        <a class="rm-chip own" href="https://tao.rufuspollock.com/Information+Efficiency">Information Efficiency</a>
        <a class="rm-chip inline" href="https://tao.rufuspollock.com/Issues">Issues need the key info</a>
      </div>
    </div>

    <a class="rm-node" href="https://tao.rufuspollock.com/Standups"><span class="rm-n">06</span> Recurring</a>
    <div class="rm-branch-row" style="padding-bottom: 0;">
      <div class="rm-branch">
        <a class="rm-chip own" href="https://tao.rufuspollock.com/Meetings+Prep">Meetings Prep</a>
      </div>
    </div>

  </div>

  <div class="rm-legend">
    <div class="rm-legend-item"><span class="rm-swatch own"></span> has its own Tao page</div>
    <div class="rm-legend-item"><span class="rm-swatch ext"></span> lives outside the Tao (real external source)</div>
    <div class="rm-legend-item"><span class="rm-swatch inline"></span> covered inside another page, no page of its own</div>
  </div>
</div>
