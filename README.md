```md
<style>
:root {
  --paper: #f5f1e8;
  --ink: #171717;
  --muted: #68645d;
  --rule: #222;
  --accent: #9b1c1f;
  --soft-rule: #b9b2a5;
  --serif: Georgia, "Times New Roman", serif;
  --sans: Arial, Helvetica, sans-serif;
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  background: var(--paper);
  color: var(--ink);
  font-family: var(--serif);
  line-height: 1.55;
}

a {
  color: inherit;
  text-decoration: none;
}

.page {
  max-width: 1440px;
  margin: 0 auto;
  padding: 0 42px 48px;
}

/* Utility strip */

.utility-bar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid var(--rule);
  padding: 9px 0;
  color: var(--muted);
  font: 11px var(--sans);
  letter-spacing: .08em;
  text-transform: uppercase;
}

.utility-links {
  display: flex;
  gap: 20px;
}

/* Masthead */

.masthead {
  display: grid;
  grid-template-columns: 1fr auto 1fr;
  align-items: center;
  gap: 20px;
  padding: 25px 0 20px;
  border-bottom: 4px double var(--rule);
}

.edition {
  font: 11px var(--sans);
  letter-spacing: .12em;
  text-transform: uppercase;
}

.edition span {
  display: block;
  margin-top: 5px;
  color: var(--muted);
  letter-spacing: .04em;
  text-transform: none;
}

.logo {
  text-align: center;
  font-size: clamp(34px, 6vw, 78px);
  font-weight: 900;
  letter-spacing: -.07em;
  line-height: .85;
  white-space: nowrap;
}

.logo small {
  display: block;
  margin-top: 12px;
  font: 10px var(--sans);
  letter-spacing: .3em;
  text-transform: uppercase;
}

.market-status {
  justify-self: end;
  text-align: right;
  font: 11px var(--sans);
  text-transform: uppercase;
}

.market-status strong {
  color: #237342;
}

/* Navigation */

.navigation {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 25px;
  border-bottom: 1px solid var(--rule);
  padding: 12px 0;
  font: bold 12px var(--sans);
  letter-spacing: .08em;
  text-transform: uppercase;
}

.navigation a:hover {
  color: var(--accent);
}

/* Breaking line */

.news-ticker {
  display: flex;
  gap: 15px;
  align-items: center;
  padding: 10px 0;
  border-bottom: 1px solid var(--soft-rule);
  font: 12px var(--sans);
}

.news-ticker b {
  color: var(--accent);
  letter-spacing: .1em;
  text-transform: uppercase;
}

/* Main layout */

.main-grid {
  display: grid;
  grid-template-columns: minmax(0, 2fr) minmax(260px, .85fr);
  gap: 28px;
  margin-top: 28px;
}

.section-label {
  margin-bottom: 12px;
  color: var(--accent);
  font: bold 11px var(--sans);
  letter-spacing: .18em;
  text-transform: uppercase;
}

/* Lead story */

.lead-story {
  border-bottom: 1px solid var(--rule);
  padding-bottom: 24px;
}

.lead-story h1 {
  max-width: 920px;
  margin: 0;
  font-size: clamp(42px, 6vw, 82px);
  line-height: .94;
  letter-spacing: -.055em;
}

.deck {
  max-width: 800px;
  margin: 22px 0 15px;
  color: #45423c;
  font-size: clamp(18px, 2vw, 25px);
  line-height: 1.25;
}

.byline {
  color: var(--muted);
  font: 11px var(--sans);
  letter-spacing: .08em;
  text-transform: uppercase;
}

/* Side briefing */

.briefing {
  border-left: 1px solid var(--rule);
  padding-left: 25px;
}

.briefing h2 {
  margin: 0 0 12px;
  font-size: 27px;
  line-height: 1;
}

.brief-item {
  border-top: 1px solid var(--soft-rule);
  padding: 16px 0;
}

.brief-item:first-of-type {
  border-top: 3px solid var(--rule);
}

.brief-item h3 {
  margin: 0 0 5px;
  font-size: 19px;
  line-height: 1.1;
}

.brief-item p {
  margin: 0;
  color: var(--muted);
  font-size: 14px;
}

/* Article columns */

.article-section {
  margin-top: 32px;
  border-top: 3px solid var(--rule);
  padding-top: 17px;
}

.article-section h2 {
  margin: 0 0 20px;
  font-size: 32px;
  line-height: 1;
}

.article-columns {
  columns: 3 220px;
  column-gap: 30px;
  column-rule: 1px solid var(--soft-rule);
}

.article-columns p {
  margin-top: 0;
  font-size: 16px;
}

.article-columns p:first-child::first-letter {
  float: left;
  margin: 5px 7px 0 0;
  font-size: 58px;
  line-height: .75;
  font-weight: bold;
}

/* Data panel */

.market-panel {
  margin-top: 34px;
  border-top: 3px solid var(--rule);
  border-bottom: 1px solid var(--rule);
  padding: 16px 0 20px;
}

.market-panel h2 {
  margin: 0 0 15px;
  font-size: 28px;
}

.market-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0;
}

.market-card {
  border-left: 1px solid var(--soft-rule);
  padding: 4px 18px;
}

.market-card:first-child {
  border-left: 0;
  padding-left: 0;
}

.market-card span {
  display: block;
  color: var(--muted);
  font: 11px var(--sans);
  letter-spacing: .08em;
  text-transform: uppercase;
}

.market-card strong {
  display: block;
  margin: 4px 0;
  font-size: 25px;
}

.up {
  color: #237342;
  font: bold 12px var(--sans);
}

.down {
  color: var(--accent);
  font: bold 12px var(--sans);
}

/* Opinion section */

.opinion-grid {
  display: grid;
  grid-template-columns: 1.2fr .8fr .8fr;
  gap: 25px;
  margin-top: 34px;
}

.opinion-card {
  border-top: 3px solid var(--rule);
  padding-top: 15px;
}

.opinion-card h2,
.opinion-card h3 {
  margin: 0 0 10px;
  line-height: 1.05;
}

.opinion-card h2 {
  font-size: 29px;
}

.opinion-card h3 {
  font-size: 21px;
}

.opinion-card p {
  margin: 0;
  color: #45423c;
  font-size: 15px;
}

/* Newsletter CTA */

.newsletter {
  display: grid;
  grid-template-columns: 1fr auto;
  gap: 25px;
  align-items: center;
  margin-top: 38px;
  border: 1px solid var(--rule);
  background: #e8e2d5;
  padding: 25px;
}

.newsletter h2 {
  margin: 0 0 5px;
  font-size: 27px;
}

.newsletter p {
  margin: 0;
  color: var(--muted);
}

.newsletter a {
  display: inline-block;
  background: var(--ink);
  color: var(--paper);
  padding: 12px 19px;
  font: bold 12px var(--sans);
  letter-spacing: .08em;
  text-transform: uppercase;
}

.newsletter a:hover {
  background: var(--accent);
}

/* Footer */

footer {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  margin-top: 30px;
  border-top: 4px double var(--rule);
  padding-top: 15px;
  color: var(--muted);
  font: 11px var(--sans);
  letter-spacing: .05em;
  text-transform: uppercase;
}

/* Responsive */

@media (max-width: 800px) {
  .page {
    padding: 0 20px 30px;
  }

  .masthead {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .edition,
  .market-status {
    justify-self: center;
    text-align: center;
  }

  .main-grid,
  .opinion-grid {
    grid-template-columns: 1fr;
  }

  .briefing {
    border-left: 0;
    border-top: 1px solid var(--rule);
    padding: 22px 0 0;
  }

  .market-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 18px 0;
  }

  .market-card:nth-child(3) {
    border-left: 0;
    padding-left: 0;
  }

  .newsletter {
    grid-template-columns: 1fr;
  }

  footer {
    flex-direction: column;
  }
}

@media (max-width: 500px) {
  .navigation {
    gap: 13px;
    font-size: 10px;
  }

  .logo {
    font-size: 39px;
  }

  .lead-story h1 {
    font-size: 47px;
  }

  .article-columns {
    columns: 1;
  }

  .market-grid {
    grid-template-columns: 1fr 1fr;
  }

  .market-card {
    padding: 4px 10px;
  }
}
</style>

<div class="page">

  <div class="utility-bar">
    <div>Monday, August 21, 2026 · Vol. 01, No. 01</div>
    <div class="utility-links">
      <a href="#newsletter">Subscribe</a>
      <a href="#about">About</a>
    </div>
  </div>

  <header class="masthead">
    <div class="edition">
      Morning Edition
      <span>Independent business reporting</span>
    </div>

    <div class="logo">
      THE LEDGER
      <small>News · Markets · Ideas</small>
    </div>

    <div class="market-status">
      Market open<br>
      <strong>▲ Sentiment positive</strong>
    </div>
  </header>

  <nav class="navigation">
    <a href="#top-story">Top Story</a>
    <a href="#markets">Markets</a>
    <a href="#business">Business</a>
    <a href="#ideas">Ideas</a>
    <a href="#briefing">Briefing</a>
    <a href="#newsletter">Newsletter</a>
  </nav>

  <div class="news-ticker">
    <b>News Alert</b>
    <span>Markets look beyond short-term uncertainty as long-term investment returns to the center of the conversation.</span>
  </div>

  <main id="top-story">

    <div class="main-grid">

      <article class="lead-story">
        <div class="section-label">The Big Read</div>
        <h1>The New Business Cycle Is Being Built in Plain Sight</h1>

        <p class="deck">
          Companies are trading speed for resilience, investors are rewarding
          discipline, and a quieter economic transformation is gathering force.
        </p>

        <div class="byline">
          By Morgan Ellis · Senior Correspondent
        </div>
      </article>

      <aside class="briefing" id="briefing">
        <div class="section-label">The Briefing</div>
        <h2>Five Things Moving Markets</h2>

        <div class="brief-item">
          <h3>Capital gets selective</h3>
          <p>Investors are asking harder questions about durable margins and cash flow.</p>
        </div>

        <div class="brief-item">
          <h3>Efficiency becomes strategy</h3>
          <p>Operational discipline is no longer a back-office concern.</p>
        </div>

        <div class="brief-item">
          <h3>The local advantage</h3>
          <p>Smaller companies are finding strength in specialized markets.</p>
        </div>

        <div class="brief-item">
          <h3>Leadership under review</h3>
          <p>Boards increasingly value clarity over grand promises.</p>
        </div>
      </aside>

    </div>

    <section class="article-section" id="business">
      <div class="section-label">Analysis</div>
      <h2>A More Measured Kind of Growth</h2>

      <div class="article-columns">
        <p>
          For much of the past decade, growth was treated as a race. Businesses
          expanded quickly, entered new markets, and used scale as a substitute
          for certainty. Today, the most consequential decisions are often less
          visible: a redesigned supply chain, a narrower product portfolio, or
          a renewed focus on the customer who already exists.
        </p>

        <p>
          That shift has changed the language of corporate planning. Resilience,
          productivity, and quality of earnings have moved from footnotes to
          headlines. The strongest operators are not necessarily the loudest.
          They are the ones able to turn uncertainty into a series of manageable
          decisions.
        </p>

        <p>
          The result is a business environment that may feel slower while
          becoming stronger underneath. New companies are emerging around
          focused expertise, established companies are rebuilding trust through
          consistency, and investors are distinguishing between momentum that
          lasts and momentum that merely looks impressive.
        </p>
      </div>
    </section>

    <section class="market-panel" id="markets">
      <div class="section-label">Market Snapshot</div>
      <h2>At a Glance</h2>

      <div class="market-grid">
        <div class="market-card">
          <span>Industrial Average</span>
          <strong>38,742.18</strong>
          <div class="up">▲ 1.24%</div>
        </div>

        <div class="market-card">
          <span>Technology Index</span>
          <strong>17,608.44</strong>
          <div class="up">▲ 0.86%</div>
        </div>

        <div class="market-card">
          <span>10-Year Yield</span>
          <strong>4.08%</strong>
          <div class="down">▼ 0.06</div>
        </div>

        <div class="market-card">
          <span>Dollar Basket</span>
          <strong>103.72</strong>
          <div class="up">▲ 0.18%</div>
        </div>
      </div>
    </section>

    <section class="opinion-grid" id="ideas">

      <article class="opinion-card">
        <div class="section-label">Editorial</div>
        <h2>What Durable Companies Understand</h2>
        <p>
          The best businesses do not eliminate uncertainty. They build systems
          that allow people to make good decisions when certainty is unavailable.
        </p>
      </article>

      <article class="opinion-card">
        <div class="section-label">Column</div>
        <h3>The Case for Boring Innovation</h3>
        <p>
          The next major productivity gains may come from improvements few
          customers ever notice.
        </p>
      </article>

      <article class="opinion-card">
        <div class="section-label">Notebook</div>
        <h3>Three Questions for Every Founder</h3>
        <p>
          What compounds? What breaks? What remains valuable when the forecast
          is wrong?
        </p>
      </article>

    </section>

    <section class="newsletter" id="newsletter">
      <div>
        <h2>Start the day informed.</h2>
        <p>
          A concise morning briefing on business, markets, and the ideas shaping
          the economy.
        </p>
      </div>

      <a href="mailto:hello@example.com?subject=Subscribe%20to%20The%20Ledger">
        Subscribe Free
      </a>
    </section>

  </main>

  <footer id="about">
    <span>© 2026 The Ledger</span>
    <span>Independent reporting for a changing economy</span>
    <span><a href="mailto:hello@example.com">Contact the newsroom</a></span>
  </footer>

</div>
```
