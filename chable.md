---
title: Chable
layout: default
description: Chable download links and game overview
permalink: /chable/
---

{% assign chable_app_store_url = "https://apps.apple.com/app/chable/id6762150334" %}
{% assign chable_play_store_url = "https://play.google.com/store/search?q=chable&c=apps" %}

<style>
:root {
  color-scheme: light;
  --ink: #0f172a;
  --muted: #475569;
  --bg-start: #f4f7fb;
  --bg-end: #fefcf7;
  --panel: #ffffff;
  --stroke: #dbe7f0;
  --teal: #0f766e;
  --teal-strong: #115e59;
  --gold: #f59e0b;
  --shadow: 0 22px 50px rgba(15, 23, 42, 0.12);
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

body {
  margin: 0;
  min-height: 100vh;
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
  color: var(--ink);
  background:
    radial-gradient(circle at 12% 12%, rgba(15, 118, 110, 0.16), transparent 42%),
    radial-gradient(circle at 90% 8%, rgba(245, 158, 11, 0.16), transparent 42%),
    linear-gradient(180deg, var(--bg-start) 0%, var(--bg-end) 100%);
}

.page-header,
.site-footer {
  display: none;
}

section.main-content {
  max-width: 960px;
  margin: 0 auto;
  padding: 1rem 1rem 2.5rem;
  background: transparent;
}

.shell {
  display: grid;
  gap: 1rem;
}

.hero {
  background: linear-gradient(145deg, #0f172a 10%, #0f766e 62%, #115e59 100%);
  color: #f8fafc;
  border-radius: 24px;
  box-shadow: var(--shadow);
  padding: 1.15rem;
}

.hero-top {
  display: flex;
  align-items: center;
  gap: 0.9rem;
}

.hero-icon {
  width: 70px;
  height: 70px;
  border-radius: 16px;
  object-fit: cover;
  flex-shrink: 0;
  box-shadow: 0 14px 26px rgba(2, 6, 23, 0.45);
}

.eyebrow {
  margin: 0;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  font-size: 0.68rem;
  color: rgba(248, 250, 252, 0.74);
}

h1 {
  margin: 0.15rem 0 0;
  font-size: clamp(1.7rem, 8vw, 2.45rem);
  line-height: 1.1;
}

.hero p {
  margin: 0.7rem 0 0;
  color: rgba(248, 250, 252, 0.87);
}

.cta-strip {
  display: block;
}

.store-card {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.65rem;
  background: var(--panel);
  border: 1px solid var(--stroke);
  box-shadow: 0 10px 20px rgba(15, 23, 42, 0.08);
  border-radius: 14px;
  padding: 0.6rem;
}

.store-link {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 52px;
  border-radius: 10px;
  padding: 0.35rem 0.5rem;
  transition: background 130ms ease;
}

.store-link:hover {
  background: #f1f5f9;
}

.store-link img {
  height: 38px;
  width: auto;
  max-width: 100%;
}

.overview {
  background: var(--panel);
  border: 1px solid var(--stroke);
  border-radius: 20px;
  padding: 1rem;
}

.overview h2 {
  margin: 0 0 0.45rem;
  font-size: 1.2rem;
}

.overview p {
  margin: 0;
  color: var(--muted);
}

.feature-list {
  margin: 0.95rem 0 0;
  padding-left: 1.15rem;
  color: #1e293b;
}

.feature-list li + li {
  margin-top: 0.45rem;
}

.meta {
  font-size: 0.95rem;
  color: var(--muted);
}

.actions {
  margin-top: 0.9rem;
  padding-top: 0.9rem;
  border-top: 1px solid var(--stroke);
  display: grid;
  gap: 0.6rem;
}

.quick-links {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.6rem;
}

.quick-link {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 42px;
  border-radius: 12px;
  border: 1px solid var(--stroke);
  background: #f8fbfd;
  color: var(--teal);
  text-decoration: none;
  font-weight: 700;
  font-size: 0.93rem;
}

.quick-link:hover {
  background: #eef6f7;
  color: var(--teal-strong);
}

.back-link {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 44px;
  border-radius: 12px;
  border: 1px dashed #b9d2dd;
  background: rgba(15, 118, 110, 0.06);
  color: #0f5f66;
  font-weight: 700;
  text-decoration: none;
}

.back-link:hover {
  background: rgba(15, 118, 110, 0.12);
}

@media (min-width: 760px) {
  section.main-content {
    padding: 1.35rem 1.4rem 3rem;
  }

  .shell {
    grid-template-columns: 1.14fr 0.86fr;
    align-items: start;
    gap: 1.15rem;
  }

  .hero {
    padding: 1.35rem;
  }

  .hero-icon {
    width: 82px;
    height: 82px;
    border-radius: 18px;
  }

  .cta-strip {
    position: sticky;
    top: 1rem;
  }
}
</style>

<div class="shell">
  <section class="hero">
    <div class="hero-top">
      <img class="hero-icon" src="{{ '/assets/icon_chable.png' | relative_url }}" alt="Chable app icon" />
      <div>
        <p class="eyebrow">Business Strategy Simulation</p>
        <h1>Chable</h1>
      </div>
    </div>
    <p>
      Scan real-world places, acquire businesses, and build your company over time. Chable blends
      exploration, portfolio planning, and financial strategy in one focused game loop.
    </p>
  </section>

  <aside class="cta-strip" aria-label="Download Chable">
    <div class="store-card">
      <a class="store-link" href="{{ chable_app_store_url }}" target="_blank" rel="noopener noreferrer" aria-label="Download Chable on the App Store">
        <img src="{{ '/assets/branding/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg' | relative_url }}" alt="Download on the App Store" />
      </a>
      <a class="store-link" href="{{ chable_play_store_url }}" target="_blank" rel="noopener noreferrer" aria-label="Get Chable on Google Play">
        <img src="{{ '/assets/branding/GetItOnGooglePlay_Badge_Web_color_English.svg' | relative_url }}" alt="Get it on Google Play" />
      </a>
    </div>
  </aside>

  <section class="overview">
    <h2>What you do in Chable</h2>
    <p>
      Start with limited capital and grow into a multi-store business by making good acquisition
      choices, balancing debt, and keeping your portfolio healthy.
    </p>
    <ul class="feature-list">
      <li>Scan nearby locations and match them against structured business templates.</li>
      <li>Acquire stores and track transactions through your in-game bank ledger.</li>
      <li>Review net worth, income, and debt trends while expanding your holdings.</li>
    </ul>
    <p class="meta">
      Store availability can vary by country/region.
    </p>
    <div class="actions">
      <div class="quick-links">
        <a class="quick-link" href="{{ '/chable_support' | relative_url }}">Support Center</a>
        <a class="quick-link" href="{{ '/chable_privacy_policy' | relative_url }}">Privacy Policy</a>
      </div>
      <a class="back-link" href="{{ '/' | relative_url }}">← Back to App Launchpad</a>
    </div>
  </section>
</div>
