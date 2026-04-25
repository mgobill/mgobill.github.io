---
title: Apps by mgobill
layout: default
---

<style>
:root {
  color-scheme: light;
  --ink: #0f172a;
  --muted: #475569;
  --bg: #f8f5f0;
  --panel: #ffffff;
  --outline: #e2e8f0;
  --accent: #0f766e;
  --accent-strong: #115e59;
  --accent-warm: #f59e0b;
  --shadow-soft: 0 22px 50px rgba(15, 23, 42, 0.08);
  --shadow-strong: 0 35px 80px rgba(15, 23, 42, 0.22);
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

body {
  margin: 0;
  background:
    radial-gradient(circle at 20% 10%, rgba(245, 158, 11, 0.18), transparent 45%),
    radial-gradient(circle at 80% 20%, rgba(14, 116, 144, 0.2), transparent 50%),
    linear-gradient(180deg, #fef9f3 0%, #f3f7fb 60%, #f8fafc 100%);
  color: var(--ink);
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
  line-height: 1.6;
}

a {
  color: var(--accent);
}

a:hover {
  color: var(--accent-strong);
}

.page-header,
.site-footer {
  display: none;
}

section.main-content {
  max-width: 1400px;
  padding: 0 1.75rem 4rem;
  margin: 0 auto;
  background: transparent;
  color: inherit;
}

.hero {
  margin: 2.5rem 0 2.5rem;
  padding: clamp(2rem, 4vw, 3.5rem);
  border-radius: 28px;
  background: linear-gradient(140deg, #0f172a 10%, #0f766e 60%, #115e59 100%);
  color: #f8fafc;
  box-shadow: var(--shadow-strong);
  display: grid;
  gap: 2rem;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  position: relative;
  overflow: hidden;
}

.hero::after {
  content: "";
  position: absolute;
  inset: 0;
  background:
    radial-gradient(circle at 15% 25%, rgba(255, 255, 255, 0.16), transparent 45%),
    radial-gradient(circle at 90% 15%, rgba(255, 255, 255, 0.12), transparent 50%);
  pointer-events: none;
}

.hero > * {
  position: relative;
  z-index: 1;
}

.hero h1 {
  font-size: clamp(2.25rem, 6vw, 3.4rem);
  margin: 0.35rem 0 0.85rem;
}

.hero-lede {
  max-width: 560px;
  font-size: 1.1rem;
  color: rgba(248, 250, 252, 0.85);
  margin: 0 0 1.25rem;
}

.eyebrow {
  letter-spacing: 0.28em;
  text-transform: uppercase;
  font-size: 0.75rem;
  font-weight: 700;
  color: rgba(248, 250, 252, 0.75);
}

.hero-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.6rem;
}

.hero-tags span {
  padding: 0.45rem 0.8rem;
  border-radius: 999px;
  background: rgba(248, 250, 252, 0.16);
  border: 1px solid rgba(248, 250, 252, 0.28);
  font-size: 0.9rem;
}

.hero-cards {
  display: grid;
  gap: 1rem;
}

.hero-card {
  padding: 1rem 1.1rem;
  border-radius: 16px;
  background: rgba(15, 23, 42, 0.35);
  border: 1px solid rgba(248, 250, 252, 0.18);
  box-shadow: inset 0 0 0 1px rgba(15, 23, 42, 0.1);
}

.hero-card h3 {
  margin: 0 0 0.35rem;
  font-size: 1.05rem;
}

.hero-card p {
  margin: 0;
  color: rgba(248, 250, 252, 0.75);
}

.catalog-header {
  margin: 2.5rem 0 1.5rem;
  display: grid;
  gap: 0.6rem;
}

.catalog-header h2 {
  margin: 0;
  font-size: clamp(1.75rem, 3vw, 2.4rem);
}

.catalog-lede {
  margin: 0;
  color: var(--muted);
  max-width: 640px;
}

.app-panels {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
  margin-bottom: 2.5rem;
}

.app-panel {
  border-radius: 22px;
  border: 1px solid var(--outline);
  padding: 2rem;
  background: var(--panel);
  box-shadow: var(--shadow-soft);
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.app-header {
  display: flex;
  align-items: flex-start;
  gap: 1.25rem;
  --eyebrow-size: 0.75rem;
  --eyebrow-gap: 0.35rem;
  --icon-offset: calc(var(--eyebrow-size) + var(--eyebrow-gap) + 0.6rem);
}

.app-header > div {
  display: flex;
  flex-direction: column;
  gap: var(--eyebrow-gap);
}

.app-header .eyebrow {
  margin: 0;
  font-size: var(--eyebrow-size);
  line-height: 1;
}

.app-header img {
  width: 96px;
  height: 96px;
  border-radius: 22px;
  box-shadow: 0 18px 32px rgba(15, 23, 42, 0.16);
  object-fit: cover;
  flex-shrink: 0;
}

.app-header img,
.app-header .app-icon {
  margin-top: var(--icon-offset);
}

.app-icon {
  width: 96px;
  height: 96px;
  border-radius: 22px;
  box-shadow: 0 18px 32px rgba(15, 23, 42, 0.16);
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, #0ea5e9, #6ee7b7);
  color: #0f172a;
  font-size: 42px;
  font-weight: 800;
  flex-shrink: 0;
}

.app-header h2 {
  margin: 0;
  font-size: 1.85rem;
}

.app-header .app-lede {
  margin: 0;
}

.app-lede {
  margin: 0.15rem 0 0.5rem;
  color: var(--muted);
  line-height: 1.6;
}

.feature-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1rem;
}

.feature-block {
  border-radius: 16px;
  border: 1px solid var(--outline);
  padding: 1rem 1.25rem;
  background: #f8fafc;
}

.feature-block h3 {
  margin: 0 0 0.4rem;
  font-size: 1.05rem;
}

.feature-list {
  margin: 0;
  padding-left: 1.25rem;
  color: var(--muted);
}

.store-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.9rem;
}

.store-badge {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  border-radius: 14px;
  padding: 0;
  background: transparent;
  border: none;
  line-height: 0;
  box-shadow: none;
  transition: transform 150ms ease;
}

.store-badge img {
  height: 46px;
  display: block;
}

.store-badge:hover {
  transform: translateY(-2px);
}

.policy-links {
  margin: 0;
  padding-left: 1.25rem;
  color: var(--muted);
}

@media (max-width: 640px) {
  section.main-content {
    padding: 0 1.25rem 3.5rem;
  }

  .app-header {
    flex-direction: column;
    align-items: flex-start;
  }

  .app-header img,
  .app-header .app-icon {
    margin-top: 0;
  }

  .store-badge {
    width: 100%;
    justify-content: flex-start;
  }
}
</style>

<div class="hero">
  <div class="hero-copy">
    <p class="eyebrow">MGOBILL APP CATALOG</p>
    <h1>Independent apps for clear, focused workflows.</h1>
    <p class="hero-lede">
      A growing collection of tools built to do one job well—covering everything from aviation
      adventures to clinical reference and daily routines.
    </p>
    <div class="hero-tags">
      <span>Offline-ready</span>
      <span>Privacy-minded</span>
      <span>Human-scale support</span>
    </div>
  </div>
  <div class="hero-cards">
    <div class="hero-card">
      <h3>Designed for real moments</h3>
      <p>Each app is tuned for speed, clarity, and the moments you need answers quickly.</p>
    </div>
    <div class="hero-card">
      <h3>Multiple categories, one vision</h3>
      <p>Aviation, health, parenting, and beyond—diverse apps with a consistent, focused feel.</p>
    </div>
    <div class="hero-card">
      <h3>Always expanding</h3>
      <p>New ideas ship with dedicated support and transparent privacy policies.</p>
    </div>
  </div>
</div>

<div class="catalog-header">
  <p class="eyebrow" style="color:#0f172a; letter-spacing:0.2em;">App Catalog</p>
  <h2>Explore the lineup.</h2>
  <p class="catalog-lede">
    Browse each app’s highlights, find support resources, and jump to the store listings as they go live.
  </p>
</div>

<div class="app-panels">
  <article class="app-panel" id="chable">
    <div class="app-header">
      <img src="{{ '/assets/icon_chable.png' | relative_url }}" alt="Chable app icon" />
      <div>
        <p class="eyebrow" style="color:#0f172a; letter-spacing:0.2em;">Business Strategy Simulation</p>
        <h2>Chable</h2>
        <p class="app-lede">
          Scan real-world places, acquire businesses, and build your company over time. Chable blends
          discovery, portfolio strategy, and financial decisions into a focused business-building game.
        </p>
      </div>
    </div>
    <div class="feature-grid">
      <div class="feature-block">
        <h3>Scan & Acquire</h3>
        <ul class="feature-list">
          <li>Scan nearby locations and match results against official business data.</li>
          <li>Acquire locations using available cash and track each deal in your bank ledger.</li>
          <li>Fallback business-type matching keeps discovery useful when exact listings are unavailable.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Portfolio Management</h3>
        <ul class="feature-list">
          <li>Track stores by chain and rename brands across your holdings.</li>
          <li>Review monthly income, debt, and net worth trends from the dashboard.</li>
          <li>Manage risk with loan settings and changing interest-rate environments.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Admin Curation</h3>
        <ul class="feature-list">
          <li>Maintain official business and type templates in the admin console.</li>
          <li>Queue, review, and approve scan findings into official datasets.</li>
          <li>Bulk import/export queue data with CSV for faster content operations.</li>
        </ul>
      </div>
    </div>
    <div>
      <h3>Store Links</h3>
      <div class="store-badges">
        <a class="store-badge" href="https://apps.apple.com/app/chable/id6762150334" target="_blank" rel="noopener noreferrer" aria-label="Download Chable on the App Store">
          <img src="{{ '/assets/branding/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg' | relative_url }}" alt="Download Chable on the App Store" />
        </a>
        <span class="store-badge" aria-label="Google Play coming soon">
          <img src="{{ '/assets/branding/GetItOnGooglePlay_Badge_Web_color_English.svg' | relative_url }}" alt="Google Play coming soon" style="opacity:0.35;" />
        </span>
      </div>
      <p class="app-lede" style="margin-top:0.5rem; color:#475569;">
        iOS is live on the App Store. Android is on the way. Check back soon.
      </p>
    </div>
    <div>
      <h3>Support & Policies</h3>
      <ul class="policy-links">
        <li><a href="./chable_support">Support Center</a></li>
        <li><a href="./chable_privacy_policy">Privacy Policy</a></li>
      </ul>
    </div>
  </article>
  <article class="app-panel" id="tepes">
    <div class="app-header">
      <img src="{{ '/assets/icon_tepes.png' | relative_url }}" alt="Tepes app icon" />
      <div>
        <p class="eyebrow" style="color:#0f172a; letter-spacing:0.2em;">Location-Based Tips</p>
        <h2>Tepes</h2>
        <p class="app-lede">
          Drop location-based tips for people nearby. Tepes keeps short, useful notes tied to
          real places so the community can share what matters right now.
        </p>
      </div>
    </div>
    <div class="feature-grid">
      <div class="feature-block">
        <h3>Post in the moment</h3>
        <ul class="feature-list">
          <li>Share quick tips anchored to your current location.</li>
          <li>Add a photo to give helpful visual context.</li>
          <li>Choose public or private visibility per tepe.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Discover nearby</h3>
        <ul class="feature-list">
          <li>See tepes plotted on a map and list view.</li>
          <li>Tap markers to highlight the matching entry.</li>
          <li>Use your location to surface what is close to you.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Save and manage</h3>
        <ul class="feature-list">
          <li>Bookmark helpful tepes for later.</li>
          <li>Report or remove posts to keep things clean.</li>
          <li>Control your profile and account settings in-app.</li>
        </ul>
      </div>
    </div>
    <div>
      <h3>Store Links</h3>
      <div class="store-badges">
        <a
          class="store-badge"
          href="https://apps.apple.com/us/app/tepes/id6757442726"
          target="_blank"
          rel="noopener"
          aria-label="Download Tepes on the App Store"
        >
          <img src="{{ '/assets/branding/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg' | relative_url }}" alt="Download on the App Store" />
        </a>
        <span class="store-badge" aria-label="Google Play coming soon">
          <img src="{{ '/assets/branding/GetItOnGooglePlay_Badge_Web_color_English.svg' | relative_url }}" alt="Google Play coming soon" style="opacity:0.35;" />
        </span>
      </div>
      <p class="app-lede" style="margin-top:0.5rem; color:#475569;">
        iOS is live on the App Store. Android is on the way—check back soon.
      </p>
    </div>
    <div>
      <h3>Support & Policies</h3>
      <ul class="policy-links">
        <li><a href="./tepes_support">Support Center</a></li>
        <li><a href="./tepes_privacy_policy">Privacy Policy</a></li>
      </ul>
    </div>
  </article>

  <article class="app-panel" id="flight-atc">
    <div class="app-header">
      <img src="{{ '/assets/icon_flightATC.png' | relative_url }}" alt="Flight ATC app icon" />
      <div>
        <p class="eyebrow" style="color:#0f172a; letter-spacing:0.2em;">Arcade ATC Challenge</p>
        <h2>Flight ATC</h2>
        <p class="app-lede">
          Guide planes safely to their matching airports without collisions in this touch-and-draw
          air traffic control game. Strategy meets reflexes for quick play sessions and endless leaderboards.
        </p>
      </div>
    </div>
    <div class="feature-grid">
      <div class="feature-block">
        <h3>How to Play</h3>
        <ul class="feature-list">
          <li>Tap and hold a plane, sketch its route, then release to lock in the path.</li>
          <li>Match each plane's color to its airport and avoid mid-air collisions.</li>
          <li>Land planes to earn points – the game ends if two aircraft collide.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Why You'll Love It</h3>
        <ul class="feature-list">
          <li>Simple controls anyone can pick up in seconds.</li>
          <li>Endless, scaling difficulty keeps adrenaline high.</li>
          <li>Crisp visuals and a one-tap restart keep you chasing a new personal best.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Feature Highlights</h3>
        <ul class="feature-list">
          <li>Dynamic skies with multiple aircraft on screen at once.</li>
          <li>Color-coded airports that reinforce clarity and challenge.</li>
          <li>Optimized for phones and tablets with smooth performance.</li>
        </ul>
      </div>
    </div>
    <div>
      <h3>Store Links</h3>
      <div class="store-badges">
        <a
          class="store-badge"
          href="https://apps.apple.com/us/app/flight-atc/id6755204257"
          target="_blank"
          rel="noopener"
          aria-label="Download Flight ATC on the App Store"
        >
          <img src="{{ '/assets/branding/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg' | relative_url }}" alt="Download on the App Store" />
        </a>
        <a
          class="store-badge"
          href="https://play.google.com/store/apps/details?id=com.mgobill.flightatc&pcampaignid=web_share"
          target="_blank"
          rel="noopener"
          aria-label="Get Flight ATC on Google Play"
        >
          <img src="{{ '/assets/branding/GetItOnGooglePlay_Badge_Web_color_English.svg' | relative_url }}" alt="Get it on Google Play" />
        </a>
      </div>
    </div>
    <div>
      <h3>Support & Policies</h3>
      <ul class="policy-links">
        <li><a href="./flightatc_support">Support Center</a></li>
        <li><a href="./flightatc_privacy_policy">Privacy Policy</a></li>
      </ul>
    </div>
  </article>

  <article class="app-panel" id="aeronatics">
    <div class="app-header">
      <img src="{{ '/assets/icon_aeronatics.png' | relative_url }}" alt="AeroNatics app icon" />
      <div>
        <p class="eyebrow" style="color:#0f172a; letter-spacing:0.2em;">Spotting & Trip Logging</p>
        <h2>AeroNatics</h2>
        <p class="app-lede">
          Discover aircraft near you, log trips, and share missions with fellow aviation fans worldwide.
          AeroNatics keeps every moment organized, measurable, and easy to celebrate.
        </p>
      </div>
    </div>
    <div class="feature-grid">
      <div class="feature-block">
        <h3>Share & Discover</h3>
        <ul class="feature-list">
          <li>Upload photos with airline, aircraft, and airport tags.</li>
          <li>Post to global or followers-only feeds and keep collections curated.</li>
          <li>Bookmark, search, follow spotters, and stay inspired.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>AeroDex & AeroLog</h3>
        <ul class="feature-list">
          <li>Reorder manufacturers, hide groups, and track which operators you have captured.</li>
          <li>Capture multi-leg trip details including seats, registrations, durations, and cabins.</li>
          <li>Trip Statistics highlight your top routes, longest flights, and preferred seats.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Earn & Protect</h3>
        <ul class="feature-list">
          <li>Unlock collectible badges and climb community leaderboards.</li>
          <li>Background uploads, moderation tools, and reporting keep posts reliable.</li>
          <li>Trip logs stay private while spotting posts can stay public or shared.</li>
        </ul>
      </div>
    </div>
    <div>
      <h3>Store Links</h3>
      <div class="store-badges">
        <a
          class="store-badge"
          href="https://apps.apple.com/app/aeronatics/id6755212824"
          target="_blank"
          rel="noopener"
          aria-label="Download Aeronatics on the App Store"
        >
          <img src="{{ '/assets/branding/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg' | relative_url }}" alt="Download on the App Store" />
        </a>
        <a
          class="store-badge"
          href="https://play.google.com/store/apps/details?id=com.mgobill.aeronatics"
          target="_blank"
          rel="noopener"
          aria-label="Get Aeronatics on Google Play"
        >
          <img src="{{ '/assets/branding/GetItOnGooglePlay_Badge_Web_color_English.svg' | relative_url }}" alt="Get it on Google Play" />
        </a>
      </div>
    </div>
    <div>
      <h3>Support & Policies</h3>
      <ul class="policy-links">
        <li><a href="./aeronatics_support">Support Center</a></li>
        <li><a href="https://discord.gg/yXxE5Yx4" target="_blank" rel="noopener">Join the Discord community</a></li>
        <li><a href="./aeronatics_privacy_policy">Privacy Policy</a></li>
        <li><a href="./aeronatics_csae_policy">CSAE Policy</a></li>
      </ul>
    </div>
  </article>

  <article class="app-panel" id="nestynote">
    <div class="app-header">
      <img src="{{ '/assets/icon_nestynote.png' | relative_url }}" alt="NestyNote app icon" />
      <div>
        <p class="eyebrow" style="color:#0f172a; letter-spacing:0.2em;">Baby Tracking & Care Logs</p>
        <h2>NestyNote</h2>
        <p class="app-lede">
          Track feedings, diapers, naps, and meds in one place. Built to answer the "when was the last time?" question
          so parents can stay in sync and care with confidence.
        </p>
      </div>
    </div>
    <div class="feature-grid">
      <div class="feature-block">
        <h3>Track every routine</h3>
        <ul class="feature-list">
          <li>Log nursing, bottle feeds, pumping sessions, diapers, naps, and meds without slowing down.</li>
          <li>See the last time each care task happened to plan the next one confidently.</li>
          <li>Graphs and daily totals make it easy to spot rhythms and discuss them with your pediatrician.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Built-In Privacy</h3>
        <ul class="feature-list">
          <li>Email-based sign-in with verification.</li>
          <li>Data stored securely in the cloud; your content stays yours.</li>
          <li>Clear controls to update or delete your data anytime.</li>
        </ul>
      </div>
    </div>
    <div>
      <h3>Store Links</h3>
      <div class="store-badges">
        <a
          class="store-badge"
          href="https://apps.apple.com/us/app/nestynote/id6756659587"
          target="_blank"
          rel="noopener"
          aria-label="Download NestyNote on the App Store"
        >
          <img src="{{ '/assets/branding/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg' | relative_url }}" alt="Download on the App Store" />
        </a>
        <span class="store-badge" aria-label="Google Play coming soon">
          <img src="{{ '/assets/branding/GetItOnGooglePlay_Badge_Web_color_English.svg' | relative_url }}" alt="Google Play coming soon" style="opacity:0.35;" />
        </span>
      </div>
      <p class="app-lede" style="margin-top:0.5rem; color:#475569;">
        iOS is live on the App Store. Android is on the way—check back soon.
      </p>
    </div>
    <div>
      <h3>Support & Policies</h3>
      <ul class="policy-links">
        <li><a href="./nestynote_support">Support Center</a></li>
        <li><a href="./nestynote_privacy_policy">Privacy Policy</a></li>
      </ul>
    </div>
  </article>

  <article class="app-panel" id="orad-ddx">
    <div class="app-header">
      <img src="{{ '/assets/icon_oraddx.png' | relative_url }}" alt="ORAD DDx app icon" />
      <div>
        <p class="eyebrow" style="color:#0f172a; letter-spacing:0.2em;">Oral Radiology Differential</p>
        <h2>ORAD DDx</h2>
        <p class="app-lede">
          A focused differential diagnosis assistant for oral radiology. Select imaging factors, then
          scan matching diagnoses grouped by category.
        </p>
      </div>
    </div>
    <div class="feature-grid">
      <div class="feature-block">
        <h3>Factor-Driven</h3>
        <ul class="feature-list">
          <li>Select key imaging factors to narrow the list quickly.</li>
          <li>Exclusive groups keep selections clean and consistent.</li>
          <li>Clear counts show how many diagnoses match.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Organized Results</h3>
        <ul class="feature-list">
          <li>Diagnoses grouped by category for fast scanning.</li>
          <li>Clean two-tab layout: Factors then Diagnoses.</li>
          <li>Built for quick review during study or chairside prep.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Offline Reference</h3>
        <ul class="feature-list">
          <li>Runs fully offline once installed.</li>
          <li>No accounts or logins required.</li>
          <li>Lightweight and fast on iPhone and iPad.</li>
        </ul>
      </div>
    </div>
    <div>
      <h3>Store Links</h3>
      <div class="store-badges">
        <span class="store-badge" aria-label="App Store coming soon">
          <img src="{{ '/assets/branding/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg' | relative_url }}" alt="App Store coming soon" style="opacity:0.35;" />
        </span>
      </div>
      <p class="app-lede" style="margin-top:0.5rem; color:#475569;">
        App Store link will be added after approval.
      </p>
    </div>
    <div>
      <h3>Support & Policies</h3>
      <ul class="policy-links">
        <li><a href="./orad_ddx_support">Support Center</a></li>
        <li><a href="./orad_ddx_privacy_policy">Privacy Policy</a></li>
      </ul>
    </div>
  </article>

  <article class="app-panel" id="suner">
    <div class="app-header">
      <img src="{{ '/assets/icon_suner.png' | relative_url }}" alt="Suner app icon" />
      <div>
        <p class="eyebrow" style="color:#0f172a; letter-spacing:0.2em;">Personal Finance Dashboard</p>
        <h2>Suner</h2>
        <p class="app-lede">
          Track net worth, set goals, and visualize progress with projections. Suner keeps your
          snapshots, transfers, and goal trends organized in one clear financial workspace.
        </p>
      </div>
    </div>
    <div class="feature-grid">
      <div class="feature-block">
        <h3>Net Worth Clarity</h3>
        <ul class="feature-list">
          <li>Log snapshots and transfers to see your full financial picture.</li>
          <li>Track assets and liabilities across custom accounts.</li>
          <li>View trends over time with clean charts.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Goals & Projections</h3>
        <ul class="feature-list">
          <li>Set retirement, FIRE, contributions, or net worth goals.</li>
          <li>Build multi-phase projections with adjustable assumptions.</li>
          <li>Compare progress with goal trend views.</li>
        </ul>
      </div>
      <div class="feature-block">
        <h3>Sync & Control</h3>
        <ul class="feature-list">
          <li>Optional cloud backup with auto-sync across devices.</li>
          <li>Reorder and personalize your dashboard layout.</li>
          <li>Keep data private with account-based access.</li>
        </ul>
      </div>
    </div>
    <div>
      <h3>Store Links</h3>
      <div class="store-badges">
        <a
          class="store-badge"
          href="https://apps.apple.com/us/app/suner/id6757318821"
          target="_blank"
          rel="noopener"
          aria-label="Download Suner on the App Store"
        >
          <img src="{{ '/assets/branding/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg' | relative_url }}" alt="Download on the App Store" />
        </a>
        <span class="store-badge" aria-label="Google Play coming soon">
          <img src="{{ '/assets/branding/GetItOnGooglePlay_Badge_Web_color_English.svg' | relative_url }}" alt="Google Play coming soon" style="opacity:0.35;" />
        </span>
      </div>
      <p class="app-lede" style="margin-top:0.5rem; color:#475569;">
        iOS is live on the App Store. Android is on the way—check back soon.
      </p>
    </div>
    <div>
      <h3>Support & Policies</h3>
      <ul class="policy-links">
        <li><a href="./suner_support">Support Center</a></li>
        <li><a href="./suner_privacy_policy">Privacy Policy</a></li>
      </ul>
    </div>
  </article>
</div>
