
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&family=Inter:wght@300;400;500;600&display=swap');

*{box-sizing:border-box;margin:0;padding:0;}

:root{
  --p:#1a56db;--pd:#1245b8;--pl:#3b82f6;--ps:#eff6ff;
  --a:#60a5fa;--as:#dbeafe;
  --tp:#0f2347;--ts:#3d5a8a;--tm:#7a96c2;
  --bg:#f5f8ff;--bgc:#ffffff;--bdr:#d0e0fa;
  --shd:0 4px 20px rgba(26,86,219,.13);
  --shd2:0 8px 32px rgba(26,86,219,.18);
  --r:12px;
}

body{font-family:'Inter',sans-serif;background:var(--bg);color:var(--tp);}

.wrap{padding:1.5rem 0;}

/* HEADER BRAND */
.brand{display:flex;align-items:center;gap:10px;margin-bottom:1.5rem;}
.brand-icon{width:40px;height:40px;border-radius:10px;background:var(--p);display:flex;align-items:center;justify-content:center;color:#fff;font-family:'Poppins',sans-serif;font-weight:800;font-size:1rem;}
.brand-name{font-family:'Poppins',sans-serif;font-weight:800;font-size:1.1rem;color:var(--p);}
.brand-sub{font-size:12px;color:var(--tm);}

/* TABS */
.tabs{display:flex;gap:6px;margin-bottom:1.5rem;background:var(--ps);border-radius:50px;padding:4px;width:fit-content;}
.tab{padding:6px 18px;border-radius:50px;border:none;background:transparent;cursor:pointer;font-size:13px;font-weight:500;color:var(--ts);transition:all .2s;font-family:'Inter',sans-serif;}
.tab.active{background:var(--p);color:#fff;box-shadow:0 2px 10px rgba(26,86,219,.3);}

/* SECTIONS */
.sec{display:none;}
.sec.active{display:block;}

/* ===== PREVIEW ===== */
.preview-shell{background:linear-gradient(135deg,#0d1117 0%,#0d1f35 100%);border-radius:var(--r);overflow:hidden;border:1px solid #1e3a5f;}

.preview-topbar{background:#161b22;border-bottom:1px solid #21262d;padding:10px 14px;display:flex;align-items:center;gap:8px;}
.dot-r{width:12px;height:12px;border-radius:50%;background:#ff5f56;}
.dot-y{width:12px;height:12px;border-radius:50%;background:#ffbd2e;}
.dot-g{width:12px;height:12px;border-radius:50%;background:#27c93f;}
.tab-pill{background:#21262d;border:1px solid #30363d;border-radius:4px;padding:2px 10px;font-size:11px;color:#8b949e;margin-left:8px;}

.preview-body{padding:1.5rem 1.75rem;color:#e6edf3;font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif;}

.gh-header{display:flex;align-items:flex-start;justify-content:space-between;margin-bottom:1rem;}
.gh-avatar{width:56px;height:56px;border-radius:50%;background:linear-gradient(135deg,#1a56db,#60a5fa);display:flex;align-items:center;justify-content:center;font-size:1.3rem;font-weight:800;color:#fff;border:2px solid #30363d;flex-shrink:0;}
.gh-visitor{background:#21262d;border:1px solid #30363d;border-radius:20px;padding:3px 10px;font-size:11px;color:#8b949e;}

.wave{font-size:1.4rem;display:inline-block;animation:wave 2s ease-in-out infinite;}
@keyframes wave{0%,100%{transform:rotate(0deg);}30%{transform:rotate(20deg);}60%{transform:rotate(-10deg);}}

.name-line{font-size:1.4rem;font-weight:700;color:#e6edf3;margin:4px 0;}
.name-line span{background:linear-gradient(90deg,#3b82f6,#60a5fa);-webkit-background-clip:text;-webkit-text-fill-color:transparent;}
.tagline{font-size:12px;color:#8b949e;margin-bottom:14px;line-height:1.6;}

.section-hdr{font-size:11px;font-weight:600;color:#58a6ff;text-transform:uppercase;letter-spacing:.08em;margin:14px 0 6px;display:flex;align-items:center;gap:6px;}
.section-hdr::after{content:'';flex:1;height:1px;background:#21262d;}

.badges-row{display:flex;flex-wrap:wrap;gap:5px;margin-bottom:10px;}
.badge{display:inline-flex;align-items:center;gap:5px;background:#21262d;border:1px solid #30363d;border-radius:6px;padding:4px 9px;font-size:11px;color:#e6edf3;font-weight:500;}
.badge .dot{width:7px;height:7px;border-radius:50%;flex-shrink:0;}

.project-item{background:#161b22;border:1px solid #21262d;border-radius:8px;padding:10px 12px;margin-bottom:6px;display:flex;align-items:flex-start;gap:10px;}
.proj-icon{width:28px;height:28px;border-radius:6px;background:linear-gradient(135deg,#1a56db22,#60a5fa22);border:1px solid #1a56db44;display:flex;align-items:center;justify-content:center;font-size:13px;flex-shrink:0;}
.proj-name{font-size:12px;font-weight:600;color:#58a6ff;}
.proj-desc{font-size:11px;color:#8b949e;margin-top:2px;}
.proj-tags{display:flex;gap:4px;flex-wrap:wrap;margin-top:4px;}
.proj-tag{font-size:10px;background:#21262d;border:1px solid #30363d;border-radius:4px;padding:1px 6px;color:#7d8590;}

.stats-cards{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin:8px 0;}
.stat-c{background:#161b22;border:1px solid #21262d;border-radius:8px;padding:10px 12px;text-align:center;}
.stat-c .sv{font-size:1.3rem;font-weight:700;color:#58a6ff;}
.stat-c .sl{font-size:10px;color:#8b949e;margin-top:2px;}

.gh-img-card{background:#161b22;border:1px solid #21262d;border-radius:8px;padding:10px 12px;margin-bottom:6px;text-align:center;}
.gh-img-card img{max-width:100%;border-radius:6px;}
.gh-img-placeholder{background:linear-gradient(135deg,#1a56db15,#60a5fa15);border:1px dashed #1a56db44;border-radius:6px;padding:12px;font-size:11px;color:#58a6ff;text-align:center;}

.cert-row{display:flex;flex-wrap:wrap;gap:5px;margin-bottom:8px;}
.cert-badge{background:linear-gradient(90deg,#1a56db22,#60a5fa11);border:1px solid #1a56db44;border-radius:6px;padding:4px 10px;font-size:11px;color:#93c5fd;font-weight:500;}

.contact-row{display:flex;flex-wrap:wrap;gap:5px;margin-top:6px;}
.contact-badge{display:inline-flex;align-items:center;gap:5px;border-radius:6px;padding:5px 10px;font-size:11px;font-weight:600;color:#fff;}

.quote-box{background:linear-gradient(135deg,#1a56db15,transparent);border-left:3px solid #1a56db;padding:8px 12px;border-radius:0 6px 6px 0;margin:8px 0;font-size:11px;color:#8b949e;font-style:italic;}

/* ===== CUSTOMIZE ===== */
.cust-card{background:var(--bgc);border:1px solid var(--bdr);border-radius:var(--r);padding:1rem 1.25rem;margin-bottom:10px;}
.cust-card-title{font-family:'Poppins',sans-serif;font-size:13px;font-weight:600;color:var(--tp);margin-bottom:12px;display:flex;align-items:center;gap:6px;}
.toggle-row{display:flex;align-items:center;justify-content:space-between;padding:8px 0;border-bottom:0.5px solid var(--bdr);}
.toggle-row:last-child{border-bottom:none;}
.toggle-row label{font-size:13px;color:var(--ts);display:flex;align-items:center;gap:6px;}
.toggle{position:relative;width:38px;height:21px;flex-shrink:0;}
.toggle input{opacity:0;width:0;height:0;}
.slider{position:absolute;inset:0;background:#c7d8fa;border-radius:21px;cursor:pointer;transition:.2s;}
.toggle input:checked+.slider{background:var(--p);}
.slider:before{content:'';position:absolute;width:15px;height:15px;left:3px;top:3px;background:#fff;border-radius:50%;transition:.2s;box-shadow:0 1px 3px rgba(0,0,0,.2);}
.toggle input:checked+.slider:before{transform:translateX(17px);}

.theme-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:6px;margin-top:4px;}
.theme-opt{border:2px solid var(--bdr);border-radius:8px;padding:6px 4px;text-align:center;cursor:pointer;font-size:11px;font-weight:500;color:var(--ts);transition:all .2s;}
.theme-opt.sel{border-color:var(--p);background:var(--ps);color:var(--p);}
.theme-opt .th-dot{width:24px;height:8px;border-radius:4px;margin:0 auto 4px;}

.sel-row{display:flex;gap:8px;margin-top:4px;}
.sel-row select{flex:1;padding:7px 10px;border-radius:8px;border:1px solid var(--bdr);background:var(--bgc);color:var(--tp);font-size:13px;font-family:'Inter',sans-serif;}

/* ===== MARKDOWN ===== */
.md-box{background:#0d1117;border:1px solid #1e3a5f;border-radius:var(--r);padding:1rem;font-family:'Courier New',monospace;font-size:11.5px;color:#8b949e;white-space:pre-wrap;word-break:break-all;max-height:380px;overflow-y:auto;line-height:1.7;}
.md-box .kw{color:#ff7b72;}
.md-box .str{color:#a5d6ff;}

.copy-btn{width:100%;padding:11px;background:var(--p);color:#fff;border:none;border-radius:50px;cursor:pointer;font-size:14px;font-weight:600;font-family:'Poppins',sans-serif;margin-top:10px;transition:all .2s;box-shadow:0 4px 16px rgba(26,86,219,.3);display:flex;align-items:center;justify-content:center;gap:6px;}
.copy-btn:hover{background:var(--pd);transform:translateY(-1px);box-shadow:0 6px 20px rgba(26,86,219,.4);}
.copy-btn.done{background:#059669;}

.hint{font-size:12px;color:var(--tm);background:var(--ps);border:1px solid var(--as);border-radius:8px;padding:8px 12px;margin-bottom:12px;display:flex;align-items:flex-start;gap:6px;}
</style>

<div class="wrap">
  <div class="brand">
    <div class="brand-icon">M</div>
    <div>
      <div class="brand-name">GPRM · Madhulika</div>
      <div class="brand-sub">GitHub Profile README Generator</div>
    </div>
  </div>

  <div class="tabs">
    <button class="tab active" onclick="sw('preview',this)">👁 Preview</button>
    <button class="tab" onclick="sw('customize',this)">⚙️ Customize</button>
    <button class="tab" onclick="sw('markdown',this)">📋 Markdown</button>
  </div>

  <!-- ========== PREVIEW ========== -->
  <div class="sec active" id="sec-preview">
    <div class="preview-shell">
      <div class="preview-topbar">
        <div class="dot-r"></div><div class="dot-y"></div><div class="dot-g"></div>
        <div class="tab-pill">📄 README.md</div>
        <div style="flex:1"></div>
        <div style="font-size:11px;color:#8b949e;">MadhulikaDamodara / MadhulikaDamodara</div>
      </div>

      <div class="preview-body">

        <!-- Intro -->
        <div class="gh-header">
          <div>
            <div><span class="wave">👋</span></div>
            <div class="name-line">Hi, I'm <span>Damodara Lakshmi Madhulika!</span></div>
            <div class="tagline">🎓 IT Student @ CBIT Hyderabad · CGPA 9.71/10 · IEEE WIE Vice Chair · Research Author @ ICCSCM 2026<br>📍 Hyderabad, Telangana &nbsp;·&nbsp; 📞 9949619556</div>
          </div>
          <div id="prev-visitor" style="display:flex;flex-direction:column;align-items:flex-end;gap:6px;">
            <div class="gh-avatar">M</div>
            <div class="gh-visitor">👀 Views: 1.2k</div>
          </div>
        </div>

        <div class="quote-box">"Building at the intersection of AI, web, and impact — one commit at a time."</div>

        <!-- Tech Stack -->
        <div id="prev-stack">
          <div class="section-hdr">🛠 Tech Stack</div>
          <div class="badges-row">
            <span class="badge"><span class="dot" style="background:#555"></span>C/C++</span>
            <span class="badge"><span class="dot" style="background:#b07219"></span>Java</span>
            <span class="badge"><span class="dot" style="background:#3572A5"></span>Python</span>
            <span class="badge"><span class="dot" style="background:#f1e05a"></span>JavaScript</span>
            <span class="badge"><span class="dot" style="background:#61dafb"></span>React</span>
            <span class="badge"><span class="dot" style="background:#339933"></span>Node.js</span>
            <span class="badge"><span class="dot" style="background:#000"></span>Express.js</span>
            <span class="badge"><span class="dot" style="background:#47A248"></span>MongoDB</span>
            <span class="badge"><span class="dot" style="background:#336791"></span>PostgreSQL</span>
            <span class="badge"><span class="dot" style="background:#0078D4"></span>Azure</span>
            <span class="badge"><span class="dot" style="background:#F05032"></span>Git</span>
          </div>
        </div>

        <!-- Projects -->
        <div id="prev-projects">
          <div class="section-hdr">🔭 What I'm Building</div>
          <div class="project-item">
            <div class="proj-icon">🛒</div>
            <div>
              <div class="proj-name">SmartRetailManager</div>
              <div class="proj-desc">Full-stack retail intelligence platform for offline stores — inventory, POS, loyalty & B2B marketplace</div>
              <div class="proj-tags"><span class="proj-tag">Node.js</span><span class="proj-tag">React</span><span class="proj-tag">MongoDB</span><span class="proj-tag">PostgreSQL</span></div>
            </div>
          </div>
          <div class="project-item">
            <div class="proj-icon">🌐</div>
            <div>
              <div class="proj-name">Yojantha</div>
              <div class="proj-desc">AI-powered government scheme discovery platform for underserved populations</div>
              <div class="proj-tags"><span class="proj-tag">Python</span><span class="proj-tag">AI/ML</span><span class="proj-tag">React</span><span class="proj-tag">Node.js</span></div>
            </div>
          </div>
          <div class="project-item">
            <div class="proj-icon">📚</div>
            <div>
              <div class="proj-name">Interactive Learning Platform</div>
              <div class="proj-desc">Animated DSA & SQL execution simulations — making abstract concepts visual</div>
              <div class="proj-tags"><span class="proj-tag">React</span><span class="proj-tag">Visualization</span></div>
            </div>
          </div>
        </div>

        <!-- Research -->
        <div id="prev-research">
          <div class="section-hdr">📄 Research & Leadership</div>
          <div class="project-item">
            <div class="proj-icon">🏆</div>
            <div>
              <div class="proj-name">Dynamic Task Scheduler — ICCSCM 2026</div>
              <div class="proj-desc">C++ based task scheduler with subtask hierarchies, dependency management & persistent storage. Published.</div>
              <div class="proj-tags"><span class="proj-tag">C++</span><span class="proj-tag">Published</span></div>
            </div>
          </div>
          <div class="project-item">
            <div class="proj-icon">👩‍💼</div>
            <div>
              <div class="proj-name">IEEE WIE Vice Chair — CBIT</div>
              <div class="proj-desc">Leading initiatives to promote women in technology through events & mentorship (2025–Present)</div>
            </div>
          </div>
        </div>

        <!-- Certs -->
        <div id="prev-certs">
          <div class="section-hdr">🏅 Certifications</div>
          <div class="cert-row">
            <span class="cert-badge">☁️ AZ-900 Microsoft Certified</span>
            <span class="cert-badge">🤖 IBM Applied AI</span>
            <span class="cert-badge">🧠 Generative AI — NPTEL</span>
            <span class="cert-badge">⚡ Salesforce Champion</span>
            <span class="cert-badge">🚀 AI-Driven Autonomous Systems</span>
          </div>
          <div style="font-size:11px;color:#58a6ff;margin-top:4px;">🔄 Currently pursuing AZ-104 — Azure Administrator</div>
        </div>

        <!-- Stats -->
        <div id="prev-stats">
          <div class="section-hdr">📊 GitHub Stats</div>
          <div class="stats-cards">
            <div class="stat-c"><div class="sv">9.71</div><div class="sl">🎓 CGPA / 10.0</div></div>
            <div class="stat-c"><div class="sv">10+</div><div class="sl">📦 Projects</div></div>
            <div class="stat-c"><div class="sv">2</div><div class="sl">📝 Research Papers</div></div>
            <div class="stat-c"><div class="sv">5+</div><div class="sl">🏆 Certifications</div></div>
          </div>
          <div class="gh-img-placeholder" id="prev-stats-img">
            📊 GitHub Stats Card · <span id="prev-theme-label">Radical</span> theme<br>
            <span style="font-size:10px;color:#7d8590;">Replace <strong>MadhulikaDamodara</strong> with your GitHub username</span>
          </div>
        </div>

        <!-- Streak -->
        <div id="prev-streak">
          <div class="section-hdr">🔥 GitHub Streak</div>
          <div class="gh-img-placeholder">🔥 Streak Stats · Updates live on your profile</div>
        </div>

        <!-- Trophies -->
        <div id="prev-trophies" style="display:none">
          <div class="section-hdr">🏆 Trophies</div>
          <div class="gh-img-placeholder">🏆 GitHub Profile Trophies</div>
        </div>

        <!-- Contact -->
        <div id="prev-contact">
          <div class="section-hdr">📫 Connect With Me</div>
          <div class="contact-row">
            <span class="contact-badge" style="background:#0077B5;">in LinkedIn</span>
            <span class="contact-badge" style="background:#24292e;">🐙 GitHub</span>
            <span class="contact-badge" style="background:#D14836;">✉ Gmail</span>
          </div>
          <div style="font-size:11px;color:#8b949e;margin-top:8px;">lakshmimadhulikadamodara@gmail.com &nbsp;·&nbsp; Hyderabad, Telangana</div>
        </div>

        <div style="margin-top:16px;padding-top:12px;border-top:1px solid #21262d;font-size:10px;color:#484f58;text-align:center;">README generated with 💙 · D.L. Madhulika · CBIT 2024–2028</div>
      </div>
    </div>

    <button class="copy-btn" onclick="doCopy(this)" style="margin-top:12px;">📋 Copy README.md Markdown</button>
  </div>

  <!-- ========== CUSTOMIZE ========== -->
  <div class="sec" id="sec-customize">
    <div class="cust-card">
      <div class="cust-card-title">💙 Sections</div>
      <div class="toggle-row"><label>👋 Intro / Greeting</label><label class="toggle"><input type="checkbox" checked onchange="sync()"><span class="slider"></span></label></div>
      <div class="toggle-row"><label>🛠 Tech Stack Badges</label><label class="toggle"><input type="checkbox" checked onchange="sync()"><span class="slider"></span></label></div>
      <div class="toggle-row"><label>🔭 Projects Showcase</label><label class="toggle"><input type="checkbox" checked onchange="sync()"><span class="slider"></span></label></div>
      <div class="toggle-row"><label>📄 Research & Leadership</label><label class="toggle"><input type="checkbox" checked onchange="sync()"><span class="slider"></span></label></div>
      <div class="toggle-row"><label>🏅 Certifications</label><label class="toggle"><input type="checkbox" checked onchange="sync()"><span class="slider"></span></label></div>
      <div class="toggle-row"><label>📊 GitHub Stats Cards</label><label class="toggle"><input type="checkbox" checked onchange="sync()"><span class="slider"></span></label></div>
      <div class="toggle-row"><label>🔥 GitHub Streak Stats</label><label class="toggle"><input type="checkbox" checked onchange="sync()"><span class="slider"></span></label></div>
      <div class="toggle-row"><label>🏆 GitHub Trophies</label><label class="toggle"><input type="checkbox" id="tog-trophies" onchange="sync()"><span class="slider"></span></label></div>
      <div class="toggle-row"><label>👀 Visitor Badge</label><label class="toggle"><input type="checkbox" checked onchange="sync()"><span class="slider"></span></label></div>
      <div class="toggle-row"><label>📫 Contact / Links</label><label class="toggle"><input type="checkbox" checked onchange="sync()"><span class="slider"></span></label></div>
    </div>

    <div class="cust-card">
      <div class="cust-card-title">🎨 Stats Theme</div>
      <div class="theme-grid" id="theme-grid">
        <div class="theme-opt sel" onclick="pickTheme('tokyonight','Tokyo Night',this)"><div class="th-dot" style="background:linear-gradient(90deg,#1a1b27,#70a5fd)"></div>Tokyo Night</div>
        <div class="theme-opt" onclick="pickTheme('radical','Radical',this)"><div class="th-dot" style="background:linear-gradient(90deg,#fe428e,#f8d847)"></div>Radical</div>
        <div class="theme-opt" onclick="pickTheme('cobalt','Cobalt',this)"><div class="th-dot" style="background:linear-gradient(90deg,#193549,#3d89d1)"></div>Cobalt</div>
        <div class="theme-opt" onclick="pickTheme('dark','Dark',this)"><div class="th-dot" style="background:linear-gradient(90deg,#151515,#888)"></div>Dark</div>
        <div class="theme-opt" onclick="pickTheme('gruvbox','Gruvbox',this)"><div class="th-dot" style="background:linear-gradient(90deg,#282828,#d79921)"></div>Gruvbox</div>
        <div class="theme-opt" onclick="pickTheme('merko','Merko',this)"><div class="th-dot" style="background:linear-gradient(90deg,#0a0f0d,#6bca81)"></div>Merko</div>
      </div>
    </div>

    <div class="cust-card">
      <div class="cust-card-title">🔗 GitHub Username</div>
      <input id="gh-user" type="text" value="MadhulikaDamodara" placeholder="Your GitHub username" oninput="sync()" style="width:100%;padding:8px 12px;border-radius:8px;border:1px solid var(--bdr);font-size:13px;font-family:'Inter',sans-serif;color:var(--tp);background:var(--bg);">
      <div style="font-size:11px;color:var(--tm);margin-top:6px;">⚠️ Update to your actual GitHub username for stats cards to work</div>
    </div>
  </div>

  <!-- ========== MARKDOWN ========== -->
  <div class="sec" id="sec-markdown">
    <div class="hint">💡 <span>Paste this into your GitHub profile repo's <strong>README.md</strong> (create a repo named exactly your GitHub username)</span></div>
    <div class="md-box" id="md-out"></div>
    <button class="copy-btn" onclick="doCopy(this)">📋 Copy README.md</button>
  </div>
</div>

<script>
let theme = 'tokyonight', themeLabel = 'Tokyo Night';

function sw(name, btn) {
  document.querySelectorAll('.tab').forEach(t=>t.classList.remove('active'));
  document.querySelectorAll('.sec').forEach(s=>s.classList.remove('active'));
  btn.classList.add('active');
  document.getElementById('sec-'+name).classList.add('active');
  if(name==='markdown') document.getElementById('md-out').textContent = genMD();
}

function pickTheme(val, label, el) {
  theme=val; themeLabel=label;
  document.querySelectorAll('.theme-opt').forEach(o=>o.classList.remove('sel'));
  el.classList.add('sel');
  const lbl = document.getElementById('prev-theme-label');
  if(lbl) lbl.textContent = label;
}

function toggles() {
  return [...document.querySelectorAll('#sec-customize input[type=checkbox]')].map(c=>c.checked);
}

function getGH() { return (document.getElementById('gh-user')?.value||'MadhulikaDamodara').trim(); }

function sync() {
  const [intro,stack,proj,research,certs,stats,streak,trophies,visitor,contact] = toggles();
  document.getElementById('prev-stack').style.display = stack?'':'none';
  document.getElementById('prev-projects').style.display = proj?'':'none';
  document.getElementById('prev-research').style.display = research?'':'none';
  document.getElementById('prev-certs').style.display = certs?'':'none';
  document.getElementById('prev-stats').style.display = stats?'':'none';
  document.getElementById('prev-streak').style.display = streak?'':'none';
  document.getElementById('prev-trophies').style.display = trophies?'':'none';
  document.getElementById('prev-visitor').style.display = visitor?'':'none';
  document.getElementById('prev-contact').style.display = contact?'':'none';
}

function genMD() {
  const [intro,stack,proj,research,certs,stats,streak,trophies,visitor,contact] = toggles();
  const gh = getGH();
  let md = '';

  if(intro) {
    md += `<h1 align="center">\n  <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28"> Hi, I'm Damodara Lakshmi Madhulika!\n</h1>\n\n`;
    md += `<p align="center">\n  <em>🎓 IT Student @ CBIT, Hyderabad &nbsp;·&nbsp; CGPA 9.71/10 &nbsp;·&nbsp; IEEE WIE Vice Chair &nbsp;·&nbsp; Research Author @ ICCSCM 2026</em>\n</p>\n\n`;
    if(visitor) {
      md += `<p align="center">\n  <img src="https://visitcount.itsvg.in/api?id=${gh}&icon=3&color=1" alt="Profile Views"/>\n</p>\n\n`;
    }
    md += `> 💙 *"Building at the intersection of AI, web, and impact — one commit at a time."*\n\n`;
    md += `---\n\n`;
  }

  if(stack) {
    md += `## 🛠 Tech Stack\n\n`;
    md += `**Languages:**\n\n`;
    md += `![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white) `;
    md += `![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white) `;
    md += `![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white) `;
    md += `![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) `;
    md += `![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)\n\n`;
    md += `**Web & Databases:**\n\n`;
    md += `![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB) `;
    md += `![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white) `;
    md += `![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white) `;
    md += `![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white) `;
    md += `![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white) `;
    md += `![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)\n\n`;
    md += `**Data & Analytics:**\n\n`;
    md += `![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) `;
    md += `![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white) `;
    md += `![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)\n\n`;
    md += `**Tools & Platforms:**\n\n`;
    md += `![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white) `;
    md += `![Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white) `;
    md += `![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white) `;
    md += `![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)\n\n`;
    md += `---\n\n`;
  }

  if(proj) {
    md += `## 🔭 What I'm Building\n\n`;
    md += `| Project | Description | Stack |\n`;
    md += `|---|---|---|\n`;
    md += `| 🛒 **[SmartRetailManager](https://github.com/${gh})** | Full-stack retail intelligence platform — inventory, POS, loyalty & B2B marketplace | Node.js · React · MongoDB · PostgreSQL |\n`;
    md += `| 🌐 **[Yojantha](https://github.com/${gh})** | AI-powered government scheme discovery for underserved populations | Python · AI/ML · React · Node.js |\n`;
    md += `| 🌾 **[AgriField](https://github.com/${gh})** | Smart agriculture platform — SIH · AI crop recommendations, farmer community & investor connect | React · Node.js · MongoDB |\n`;
    md += `| 📚 **Interactive Learning Platform** | Animated DSA & SQL execution simulations — making abstract concepts visual | React · Viz Libraries |\n`;
    md += `| ♟ **Chess in C** | Fully functional two-player chess with move validation & checkmate detection | C |\n\n`;
    md += `---\n\n`;
  }

  if(research) {
    md += `## 📄 Research & Leadership\n\n`;
    md += `- 🏆 **Research Author** — *Dynamic Task Scheduler* — Published @ **ICCSCM 2026** *(C++ · subtask hierarchies, dependency mgmt, file persistence)*\n`;
    md += `- 🔬 **Research Contributor** — Traffic Violation Detection using YOLO object detection *(2024)*\n`;
    md += `- 👩‍💼 **Vice Chair** — IEEE Women in Engineering, CBIT Student Branch *(2025–Present)*\n`;
    md += `- 🌟 **Executive Board** — VMedha Technical Club · Co-organized IEEE WIE Women Ideathon *(2024–2025)*\n`;
    md += `- 🤝 **Student Volunteer** — RMC Mathematical Club & Chaitanya Srujana Art & Design Club *(2024–Present)*\n\n`;
    md += `---\n\n`;
  }

  if(certs) {
    md += `## 🏅 Certifications & Achievements\n\n`;
    md += `![AZ-900](https://img.shields.io/badge/AZ--900-Microsoft_Certified-0078D4?style=flat-square&logo=microsoft-azure&logoColor=white) `;
    md += `![IBM AI](https://img.shields.io/badge/Applied_AI-IBM_SkillsBuild-1F70C1?style=flat-square&logo=ibm&logoColor=white) `;
    md += `![NPTEL](https://img.shields.io/badge/Generative_AI-NPTEL-F7941D?style=flat-square&logoColor=white) `;
    md += `![Salesforce](https://img.shields.io/badge/Agent_Blazer_Champion-Salesforce-00A1E0?style=flat-square&logo=salesforce&logoColor=white) `;
    md += `![AI Training](https://img.shields.io/badge/AI_Autonomous_Systems-Intl_Training-6366f1?style=flat-square)\n\n`;
    md += `> 🔄 Currently pursuing **AZ-104** — Microsoft Azure Administrator\n\n`;
    md += `---\n\n`;
  }

  if(stats) {
    md += `## 📊 GitHub Stats\n\n`;
    md += `<p align="center">\n`;
    md += `  <img width="49%" src="https://github-readme-stats.vercel.app/api?username=${gh}&theme=${theme}&hide_border=true&include_all_commits=true&count_private=true&show_icons=true" />\n`;
    md += `  <img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=${gh}&theme=${theme}&hide_border=true&layout=compact&langs_count=8" />\n`;
    md += `</p>\n\n`;
  }

  if(streak) {
    md += `## 🔥 GitHub Streak\n\n`;
    md += `<p align="center">\n`;
    md += `  <img src="https://nirzak-streak-stats.vercel.app/?user=${gh}&theme=${theme}&hide_border=true" />\n`;
    md += `</p>\n\n`;
  }

  if(trophies) {
    md += `## 🏆 GitHub Trophies\n\n`;
    md += `<p align="center">\n`;
    md += `  <img src="https://github-profile-trophy.vercel.app/?username=${gh}&theme=${theme}&no-frame=true&no-bg=false&margin-w=4&column=7" />\n`;
    md += `</p>\n\n`;
  }

  if(contact) {
    md += `## 📫 Let's Connect!\n\n`;
    md += `<p align="left">\n`;
    md += `  <a href="https://linkedin.com/in/madhulika-damodara"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>\n`;
    md += `  <a href="https://github.com/${gh}"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"/></a>\n`;
    md += `  <a href="mailto:lakshmimadhulikadamodara@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>\n`;
    md += `</p>\n\n`;
    md += `📍 Hyderabad, Telangana &nbsp;·&nbsp; 📞 9949619556\n\n`;
  }

  md += `---\n\n`;
  md += `<p align="center">\n  <em>💙 Made with passion by D.L. Madhulika &nbsp;·&nbsp; CBIT 2024–2028</em>\n</p>\n`;
  return md;
}

function doCopy(btn) {
  navigator.clipboard.writeText(genMD()).then(()=>{
    const orig = btn.innerHTML;
    btn.innerHTML = '✅ Copied to clipboard!';
    btn.classList.add('done');
    setTimeout(()=>{ btn.innerHTML=orig; btn.classList.remove('done'); }, 2200);
  });
}
</script>
