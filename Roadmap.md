# Roadmap for the TAO
<style>
  @import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,600;0,700;1,600&display=swap');
  .rm-wrap {
    --rm-paper: #f8f4ee;
    --rm-paper-raised: #fffdf8;
    --rm-ink: #252113;
    --rm-accent: #327e09;
    --rm-accent-soft: #e4ecdd;
    --rm-line: #ded7c4;
    max-width: 960px;
    margin: 0 auto;
    padding: 2rem 1rem 4rem;
    overflow-x: auto;
    color: var(--rm-ink);
    font-family: "Cormorant Garamond", ui-serif, Georgia, serif;
  }
  @media (prefers-color-scheme: dark) {
    :root:not([data-theme="light"]) .rm-wrap {
      --rm-paper: #171717;
      --rm-paper-raised: #202020;
      --rm-ink: #f8f4ee;
      --rm-accent: #4f9c22;
      --rm-accent-soft: #223122;
      --rm-line: #3a3a37;
    }
  }
  :root[data-theme="dark"] .rm-wrap {
    --rm-paper: #171717;
    --rm-paper-raised: #202020;
    --rm-ink: #f8f4ee;
    --rm-accent: #4f9c22;
    --rm-accent-soft: #223122;
    --rm-line: #3a3a37;
  }
  .rm-title { text-align: center; font-weight: 700; font-size: 1.7rem; margin: 0 0 2rem; }
  .rm-row { position: relative; width: 900px; min-width: 900px; margin: 0 auto; }
  .rm-row svg { position: absolute; top: 0; left: 0; width: 900px; height: 100%; z-index: 0; overflow: visible; }
  .rm-row svg path { fill: none; stroke: var(--rm-line); stroke-width: 2; }
  .rm-spine { position: absolute; top: 0; bottom: 0; left: 449px; width: 2px; background: var(--rm-line); z-index: 0; }
  .rm-box {
    box-sizing: border-box;
    position: absolute;
    z-index: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    text-decoration: none;
    background: var(--rm-paper-raised);
    border: 2px solid var(--rm-accent);
    color: var(--rm-accent);
    border-radius: 0.5rem;
    font-weight: 700;
    line-height: 1.15;
    padding: 0 0.9rem;
  }
  .rm-box:hover { background: var(--rm-accent-soft); }
  .rm-box.rm-center { font-size: 1.05rem; height: 60px; }
  .rm-box.rm-side { font-size: 0.92rem; height: 50px; }
  .rm-box .rm-n { font-family: ui-sans-serif, system-ui, sans-serif; font-size: 0.65rem; font-weight: 500; opacity: 0.7; margin-right: 0.35rem; }
</style>
<div class="rm-wrap">
  <p class="rm-title">The Way of the Tao</p>
  <div class="rm-row" style="height: 90px;">
    <div class="rm-spine"></div>
    <a class="rm-box rm-center" href="https://tao.rufuspollock.com" style="left:375px; top:15px; width:150px;"><span class="rm-n">01</span>Index</a>
  </div>
  <div class="rm-row" style="height: 200px;">
    <div class="rm-spine"></div>
    <svg viewBox="0 0 900 200">
      <path d="M255,45 C300,45 300,100 315,100"/>
      <path d="M255,155 C300,155 300,100 315,100"/>
      <path d="M585,100 C650,100 650,45 745,45"/>
    </svg>
    <a class="rm-box rm-side" href="https://rufuspollock.com/post/getting-things-done" style="left:70px; top:20px; width:185px;">GTD</a>
    <a class="rm-box rm-side" href="https://tao.rufuspollock.com/KISS+Principle" style="left:70px; top:130px; width:185px;">KISS Principle</a>
    <a class="rm-box rm-center" href="https://lifeitself.org/tao/getting-stuff-done" style="left:315px; top:70px; width:270px;"><span class="rm-n">02</span>Getting Stuff Done</a>
    <a class="rm-box rm-side" href="https://tao.lifeitself.org/views" style="left:745px; top:20px; width:185px;">Key Views</a>
  </div>
  <div class="rm-row" style="height: 90px;">
    <div class="rm-spine"></div>
    <a class="rm-box rm-center" href="https://tao.rufuspollock.com/Five+levels+of+agency" style="left:280px; top:15px; width:340px;"><span class="rm-n">03</span>Five Levels of Agency</a>
  </div>
  <div class="rm-row" style="height: 130px;">
    <div class="rm-spine"></div>
    <svg viewBox="0 0 900 130">
      <path d="M255,60 C325,60 325,60 340,60"/>
      <path d="M560,60 C625,60 625,60 645,60"/>
    </svg>
    <a class="rm-box rm-side" href="https://tao.lifeitself.org/principles/#experimentation-and-creativity" style="left:40px; top:35px; width:215px;">Experimentation and Creativity</a>
    <a class="rm-box rm-center" href="https://tao.rufuspollock.com/Hypotheses" style="left:340px; top:22px; width:220px; height:76px;"><span class="rm-n">04</span>Hypotheses + Open-Minded Rigour</a>
    <a class="rm-box rm-side" href="https://tao.lifeitself.org/principles/#zen--mindfulness" style="left:645px; top:35px; width:215px;">Zen and Mindfulness</a>
  </div>
  <div class="rm-row" style="height: 200px;">
    <div class="rm-spine"></div>
    <svg viewBox="0 0 900 200">
      <path d="M255,100 C325,100 325,100 375,100"/>
      <path d="M525,100 C600,100 600,45 645,45"/>
      <path d="M525,100 C600,100 600,155 645,155"/>
    </svg>
    <a class="rm-box rm-side" href="https://tao.rufuspollock.com/Definition+of+Done" style="left:70px; top:75px; width:185px;">Definition of Done</a>
    <a class="rm-box rm-center" href="https://tao.rufuspollock.com/Project+Phase+and+Status" style="left:375px; top:70px; width:150px;"><span class="rm-n">05</span>Project System</a>
    <a class="rm-box rm-side" href="https://tao.rufuspollock.com/Information+Efficiency" style="left:645px; top:20px; width:185px;">Information Efficiency</a>
    <a class="rm-box rm-side" href="https://tao.rufuspollock.com/Issues" style="left:645px; top:130px; width:185px;">Issues need the key info</a>
  </div>
  <div class="rm-row" style="height: 140px;">
    <div class="rm-spine"></div>
    <svg viewBox="0 0 900 140">
      <path d="M255,70 C325,70 325,70 340,70"/>
    </svg>
    <a class="rm-box rm-side" href="https://tao.rufuspollock.com/Meetings+Prep" style="left:60px; top:45px; width:195px;">Meetings Prep</a>
    <a class="rm-box rm-center" href="https://tao.rufuspollock.com/Standups" style="left:340px; top:40px; width:220px;"><span class="rm-n">06</span>Recurring</a>
  </div>
</div>
