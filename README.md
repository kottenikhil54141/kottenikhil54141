<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Nikhil's GitHub Upgrade Guide</title>
<link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Syne:wght@400;700;800&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  body { background: #050508; color: #e2e8f0; font-family: 'Syne', sans-serif; padding: 2rem; line-height: 1.6; }
  body::before { content:''; position:fixed; inset:0; background-image:linear-gradient(rgba(255,255,255,0.04) 1px,transparent 1px),linear-gradient(90deg,rgba(255,255,255,0.04) 1px,transparent 1px); background-size:40px 40px; pointer-events:none; z-index:0; }
  .wrap { max-width: 860px; margin: 0 auto; position: relative; z-index: 1; }
  h1 { font-size: 2.4rem; font-weight: 800; margin-bottom: 0.4rem; }
  h1 span { color: #7c3aed; }
  .subtitle { color: #64748b; font-family: 'Space Mono', monospace; font-size: 0.8rem; margin-bottom: 3rem; letter-spacing: 0.15em; }
  .section { margin-bottom: 2.5rem; }
  .section-head {
    display: flex; align-items: center; gap: 0.8rem;
    background: #0e0e16; border: 1px solid rgba(255,255,255,0.07);
    border-radius: 10px 10px 0 0; padding: 1rem 1.4rem;
    border-bottom: 2px solid #7c3aed;
  }
  .step-num { background: #7c3aed; color: #fff; border-radius: 6px; width: 28px; height: 28px; display:flex; align-items:center; justify-content:center; font-family:'Space Mono',monospace; font-size:0.75rem; font-weight:700; flex-shrink:0; }
  .section-title { font-weight: 700; font-size: 1rem; }
  .badge { font-family:'Space Mono',monospace; font-size:0.65rem; padding:0.2rem 0.6rem; border-radius:20px; margin-left:auto; }
  .badge.urgent { background:rgba(239,68,68,0.15); color:#f87171; border:1px solid rgba(239,68,68,0.3); }
  .badge.easy { background:rgba(34,197,94,0.15); color:#4ade80; border:1px solid rgba(34,197,94,0.3); }
  .badge.medium { background:rgba(245,158,11,0.15); color:#fbbf24; border:1px solid rgba(245,158,11,0.3); }
  .section-body { background:#0e0e16; border:1px solid rgba(255,255,255,0.07); border-top:none; border-radius:0 0 10px 10px; padding:1.4rem; }
  .step-list { list-style:none; display:flex; flex-direction:column; gap:0.8rem; }
  .step-list li { display:flex; align-items:flex-start; gap:0.8rem; font-size:0.9rem; color:#94a3b8; }
  .step-list li::before { content:'→'; color:#7c3aed; font-family:'Space Mono',monospace; flex-shrink:0; margin-top:0.05rem; }
  .step-list li strong { color:#e2e8f0; }
  .code-snippet {
    background: #020204; border: 1px solid rgba(255,255,255,0.07); border-radius: 8px;
    padding: 1rem 1.2rem; font-family: 'Space Mono', monospace; font-size: 0.75rem;
    color: #86efac; margin-top: 0.8rem; overflow-x: auto; line-height: 1.8;
  }
  .code-snippet .comment { color: #475569; }
  .code-snippet .key { color: #c084fc; }
  .code-snippet .val { color: #06b6d4; }
  .repo-table { width:100%; border-collapse:collapse; margin-top:0.5rem; font-size:0.83rem; }
  .repo-table th { text-align:left; padding:0.6rem 0.8rem; color:#64748b; font-family:'Space Mono',monospace; font-size:0.68rem; letter-spacing:0.1em; border-bottom:1px solid rgba(255,255,255,0.07); }
  .repo-table td { padding:0.7rem 0.8rem; border-bottom:1px solid rgba(255,255,255,0.04); vertical-align:top; }
  .repo-table tr:last-child td { border:none; }
  .old { color:#f87171; text-decoration:line-through; font-family:'Space Mono',monospace; font-size:0.75rem; }
  .new { color:#4ade80; font-family:'Space Mono',monospace; font-size:0.75rem; }
  .desc-new { color:#94a3b8; font-size:0.8rem; }
  .checklist { display:flex; flex-direction:column; gap:0.5rem; margin-top:0.5rem; }
  .check-item { display:flex; align-items:center; gap:0.8rem; padding:0.7rem 1rem; background:#020204; border-radius:8px; border:1px solid rgba(255,255,255,0.06); font-size:0.85rem; }
  .check-box { width:18px; height:18px; border:2px solid #7c3aed; border-radius:4px; flex-shrink:0; }
  .priority { font-family:'Space Mono',monospace; font-size:0.65rem; color:#64748b; margin-left:auto; }
  .tip { background:rgba(124,58,237,0.08); border:1px solid rgba(124,58,237,0.25); border-radius:8px; padding:0.9rem 1.1rem; margin-top:1rem; font-size:0.83rem; color:#c4b5fd; }
  .tip strong { color:#a78bfa; }
</style>
</head>
<body>
<div class="wrap">
  <h1>GitHub <span>Upgrade</span> Guide</h1>
  <p class="subtitle">KOTTE NIKHIL — kottenikhil54141 — STEP BY STEP ACTIONS</p>

  <!-- STEP 1 -->
  <div class="section">
    <div class="section-head">
      <div class="step-num">1</div>
      <div class="section-title">Create Your Profile README (Most Important!)</div>
      <span class="badge urgent">DO THIS FIRST</span>
    </div>
    <div class="section-body">
      <ul class="step-list">
        <li>Go to <strong>github.com/new</strong></li>
        <li>Set repo name to exactly: <strong>kottenikhil54141</strong> (same as your username)</li>
        <li>Check <strong>"Add a README file"</strong>, set to <strong>Public</strong></li>
        <li>Click <strong>Create repository</strong></li>
        <li>Click the ✏️ pencil icon on the README.md file</li>
        <li>Delete everything and <strong>paste the README.md file</strong> I gave you</li>
        <li>Click <strong>Commit changes</strong> — your profile banner is now LIVE!</li>
      </ul>
      <div class="tip">✨ <strong>Result:</strong> A beautiful animated banner with your bio, tech stack, stats, and projects will appear on your GitHub profile automatically.</div>
    </div>
  </div>

  <!-- STEP 2 -->
  <div class="section">
    <div class="section-head">
      <div class="step-num">2</div>
      <div class="section-title">Add Bio, URL & Social Links</div>
      <span class="badge easy">5 MINUTES</span>
    </div>
    <div class="section-body">
      <ul class="step-list">
        <li>Go to <strong>github.com/settings/profile</strong></li>
        <li><strong>Name:</strong> Kotte Nikhil (already set ✅)</li>
        <li><strong>Bio:</strong> Copy paste this exactly:</li>
      </ul>
      <div class="code-snippet">Full Stack Web Developer & AI/ML Enthusiast | Building intelligent web apps | HTML · CSS · JS · Python | Open to Internships 🚀</div>
      <ul class="step-list" style="margin-top:1rem">
        <li><strong>Website URL:</strong> https://kottenikhil54141.github.io</li>
        <li><strong>Location:</strong> Andhra Pradesh, India</li>
        <li>Social accounts: Add your <strong>LinkedIn</strong> URL</li>
        <li>Click <strong>Update profile</strong></li>
      </ul>
    </div>
  </div>

  <!-- STEP 3 -->
  <div class="section">
    <div class="section-head">
      <div class="step-num">3</div>
      <div class="section-title">Fix Your Repo Names & Descriptions</div>
      <span class="badge medium">30 MINUTES</span>
    </div>
    <div class="section-body">
      <p style="color:#64748b;font-size:0.8rem;margin-bottom:1rem;font-family:'Space Mono',monospace">For each repo → Settings → Rename + add description</p>
      <table class="repo-table">
        <thead>
          <tr>
            <th>Current Name</th>
            <th>New Name</th>
            <th>Add This Description</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><span class="old">pp_beauty_parlour</span></td>
            <td><span class="new">beauty-parlour-website</span></td>
            <td><span class="desc-new">Responsive business website for a beauty parlour — HTML, CSS, JavaScript</span></td>
          </tr>
          <tr>
            <td><span class="old">ppbeautyparlour2</span></td>
            <td><span class="new">beauty-parlour-v2</span></td>
            <td><span class="desc-new">Redesigned beauty parlour site with improved UI/UX and CSS animations</span></td>
          </tr>
          <tr>
            <td><span class="old">ppbeautyparlour3</span></td>
            <td><span class="new">beauty-parlour-v3</span></td>
            <td><span class="desc-new">Latest version with advanced layout and responsive styling</span></td>
          </tr>
          <tr>
            <td><span class="old">list</span></td>
            <td><span class="new">task-manager-app</span></td>
            <td><span class="desc-new">Simple task management app built with vanilla JavaScript</span></td>
          </tr>
          <tr>
            <td><span class="old">github-pages</span></td>
            <td><span class="new">portfolio-site</span></td>
            <td><span class="desc-new">Personal portfolio website hosted on GitHub Pages</span></td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>

  <!-- STEP 4 -->
  <div class="section">
    <div class="section-head">
      <div class="step-num">4</div>
      <div class="section-title">Deploy Portfolio Website on GitHub Pages</div>
      <span class="badge easy">10 MINUTES</span>
    </div>
    <div class="section-body">
      <ul class="step-list">
        <li>Create new repo named: <strong>kottenikhil54141.github.io</strong></li>
        <li>Upload the <strong>index.html</strong> portfolio file I gave you</li>
        <li>Go to repo <strong>Settings → Pages</strong></li>
        <li>Under "Branch" select <strong>main</strong> and click Save</li>
        <li>Wait ~2 minutes — your site is live at:</li>
      </ul>
      <div class="code-snippet">https://kottenikhil54141.github.io</div>
      <ul class="step-list" style="margin-top:0.8rem">
        <li>Add this URL to your GitHub profile <strong>Website</strong> field</li>
      </ul>
    </div>
  </div>

  <!-- STEP 5 -->
  <div class="section">
    <div class="section-head">
      <div class="step-num">5</div>
      <div class="section-title">Pin Your Best Repositories</div>
      <span class="badge easy">2 MINUTES</span>
    </div>
    <div class="section-body">
      <ul class="step-list">
        <li>On your profile page click <strong>"Customize your pins"</strong></li>
        <li>Pin these repos in this order:</li>
        <li><strong>1st:</strong> kottenikhil54141 (Profile README repo)</li>
        <li><strong>2nd:</strong> kottenikhil54141.github.io (Portfolio)</li>
        <li><strong>3rd:</strong> beauty-parlour-website (best project)</li>
        <li><strong>4th:</strong> beauty-parlour-v2</li>
      </ul>
    </div>
  </div>

  <!-- STEP 6 -->
  <div class="section">
    <div class="section-head">
      <div class="step-num">6</div>
      <div class="section-title">Grow Your Contribution Graph (Ongoing)</div>
      <span class="badge medium">WEEKLY HABIT</span>
    </div>
    <div class="section-body">
      <p style="color:#94a3b8;font-size:0.85rem;margin-bottom:1rem">Your graph shows only <strong style="color:#f87171">12 contributions</strong>. This is what recruiters check. Build daily habits:</p>
      <ul class="step-list">
        <li>Commit code <strong>every day</strong> — even small improvements count</li>
        <li>Add <strong>README.md</strong> to all your existing repos (1 commit each)</li>
        <li>Create a <strong>new project every 2 weeks</strong> (ideas below)</li>
        <li>Fix bugs, improve CSS, add features — each = 1 commit</li>
      </ul>
      <div class="tip">
        <strong>🚀 Next Project Ideas (easy wins):</strong><br><br>
        1. <strong>Weather App</strong> — HTML/CSS/JS + fetch OpenWeather API<br>
        2. <strong>Todo App with LocalStorage</strong> — Pure JS<br>
        3. <strong>Python Calculator</strong> — simple CLI project<br>
        4. <strong>Quiz Game</strong> — JS with score tracking<br>
        5. <strong>ML: Iris Flower Classifier</strong> — Python + Scikit-learn (Jupyter Notebook)
      </div>
    </div>
  </div>

  <!-- CHECKLIST -->
  <div class="section">
    <div class="section-head">
      <div class="step-num">✓</div>
      <div class="section-title">Complete Checklist</div>
    </div>
    <div class="section-body">
      <div class="checklist">
        <div class="check-item"><div class="check-box"></div> Create kottenikhil54141 repo + paste README.md <span class="priority">PRIORITY 1</span></div>
        <div class="check-item"><div class="check-box"></div> Add bio to GitHub profile settings <span class="priority">PRIORITY 1</span></div>
        <div class="check-item"><div class="check-box"></div> Create kottenikhil54141.github.io + upload portfolio <span class="priority">PRIORITY 2</span></div>
        <div class="check-item"><div class="check-box"></div> Rename repos with better names <span class="priority">PRIORITY 2</span></div>
        <div class="check-item"><div class="check-box"></div> Add descriptions to all repos <span class="priority">PRIORITY 2</span></div>
        <div class="check-item"><div class="check-box"></div> Customize pinned repos <span class="priority">PRIORITY 3</span></div>
        <div class="check-item"><div class="check-box"></div> Add LinkedIn to social accounts <span class="priority">PRIORITY 3</span></div>
        <div class="check-item"><div class="check-box"></div> Build 1 new project (Weather App / Todo App) <span class="priority">THIS WEEK</span></div>
        <div class="check-item"><div class="check-box"></div> Commit code every day for 30 days <span class="priority">ONGOING</span></div>
      </div>
    </div>
  </div>

</div>
</body>
</html>
