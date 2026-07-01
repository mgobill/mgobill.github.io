---
title: Chable
layout: default
description: Chable download links and game overview
permalink: /chable/
---

{% assign chable_app_store_url = "https://apps.apple.com/app/chable-business-empire/id6762150334" %}
{% assign chable_play_store_url = "https://play.google.com/store/apps/details?id=com.mgobill.chable" %}

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

.download-heading {
  margin: 0 0 0.7rem;
  text-align: center;
  font-size: 1.05rem;
  font-weight: 800;
  color: var(--ink);
}

.store-card {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 0.55rem;
  background: var(--panel);
  border: 1px solid var(--stroke);
  box-shadow: 0 10px 20px rgba(15, 23, 42, 0.08);
  border-radius: 14px;
  padding: 0.45rem;
}

.store-link {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  flex: 0 0 auto;
  min-height: 0;
  border-radius: 10px;
  padding: 0.18rem 0.28rem;
  border: 1px solid #e2e8f0;
  background: #f8fafc;
  line-height: 0;
  transition: background 130ms ease, border-color 130ms ease, transform 130ms ease;
}

.store-link:hover {
  background: #ffffff;
  border-color: #b9d2dd;
  transform: translateY(-1px);
}

.store-link:focus-visible {
  outline: 3px solid rgba(15, 118, 110, 0.28);
  outline-offset: 2px;
}

.store-link img {
  display: block;
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
    display: flex;
    align-items: center;
    max-width: 1040px;
    min-height: 100vh;
    padding: 3rem 1.5rem;
  }

  .shell {
    width: 100%;
    grid-template-columns: minmax(0, 1.08fr) minmax(320px, 0.92fr);
    grid-template-areas:
      "hero overview"
      "download overview";
    grid-template-rows: auto 1fr;
    gap: 0;
    overflow: hidden;
    border: 1px solid rgba(219, 231, 240, 0.9);
    border-radius: 28px;
    background: var(--panel);
    box-shadow: var(--shadow);
  }

  .hero {
    grid-area: hero;
    padding: 2.5rem 2.5rem 1.35rem;
    border-radius: 0;
    box-shadow: none;
  }

  .hero-icon {
    width: 88px;
    height: 88px;
    border-radius: 20px;
  }

  .cta-strip {
    grid-area: download;
    padding: 0.75rem 2.5rem 2.5rem;
    background: linear-gradient(145deg, #0f766e 0%, #115e59 100%);
  }

  .download-heading {
    text-align: left;
    color: #f8fafc;
  }

  .store-card {
    justify-content: flex-start;
    gap: 0.65rem;
    border-color: rgba(255, 255, 255, 0.2);
    background: rgba(255, 255, 255, 0.1);
    box-shadow: none;
  }

  .store-link {
    background: #ffffff;
  }

  .store-link img {
    height: 40px;
  }

  .overview {
    grid-area: overview;
    align-self: stretch;
    padding: 2.5rem;
    border: 0;
    border-left: 1px solid var(--stroke);
    border-radius: 0;
  }
}
</style>

<script>
(() => {
  const appStoreUrl = {{ chable_app_store_url | jsonify }};
  const playStoreUrl = {{ chable_play_store_url | jsonify }};
  const params = new URLSearchParams(window.location.search);

  if (params.get('no_redirect') === '1') {
    return;
  }

  const userAgent = navigator.userAgent || navigator.vendor || window.opera || '';
  const platform = navigator.platform || '';
  const maxTouchPoints = navigator.maxTouchPoints || 0;
  const isiOS = /iPad|iPhone|iPod/.test(userAgent) || (platform === 'MacIntel' && maxTouchPoints > 1);
  const isAndroid = /Android/i.test(userAgent);
  const redirectUrl = isiOS ? appStoreUrl : isAndroid ? playStoreUrl : '';

  if (!redirectUrl) {
    return;
  }

  window.location.replace(redirectUrl);
})();
</script>

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
      Scan real-world places, acquire businesses, and build your empire over time. Chable blends
      exploration, portfolio planning, and financial strategy in one focused game loop.
    </p>
  </section>

  <aside class="cta-strip" aria-label="Download Chable">
    <p class="download-heading">Download Chable</p>
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
      Build your own real-world business empire.
    </p>
    <p>
      Explore your surroundings to discover nearby businesses, acquire locations, and grow your
      conglomerate one store at a time. Every location has its own economic potential based on the
      neighborhood around it, making each acquisition unique.
    </p>
    <p>
      Expand into new industries, track your net worth, and compete against players worldwide to
      build the ultimate business empire.
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
