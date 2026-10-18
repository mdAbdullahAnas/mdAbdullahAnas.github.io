<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Md. Abdullah Anas – Mobile &amp; Full-Stack Software Engineer</title>
<meta name="description" content="Software engineer building mobile apps with Kotlin Multiplatform and Flutter, and full-stack products with NestJS, Next.js and PostgreSQL.">
<link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>📱</text></svg>">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@12..96,500;12..96,700;12..96,800&family=IBM+Plex+Sans:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#f5f8fc; --surface:#ffffff; --ink:#0d1b2e; --muted:#4f6079; --line:#dbe4ef;
  --accent:#0a6cf0; --cyan:#00b8f0; --soft:#e6f1ff;
  --display:"Bricolage Grotesque","Segoe UI",system-ui,sans-serif;
  --body:"IBM Plex Sans","Segoe UI",system-ui,sans-serif;
}
@media (prefers-color-scheme:dark){
  :root{--bg:#09111d; --surface:#101c2e; --ink:#e8eef7; --muted:#9db0c9; --line:#22324b; --accent:#4d9bff; --cyan:#27c8ff; --soft:#12253f;}
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--ink);font:400 1.0625rem/1.65 var(--body);-webkit-font-smoothing:antialiased}
a{color:var(--accent);text-decoration:none}
a:hover{text-decoration:underline}
:focus-visible{outline:3px solid var(--cyan);outline-offset:3px;border-radius:4px}
.wrap{max-width:1040px;margin:0 auto;padding:0 24px}

/* top bar */
header{position:sticky;top:0;z-index:10;background:color-mix(in srgb,var(--bg) 88%,transparent);backdrop-filter:blur(10px);border-bottom:1px solid var(--line)}
.bar{display:flex;justify-content:space-between;align-items:center;height:62px}
.logo{font:800 1.15rem var(--display);color:var(--ink)}
.logo:hover{text-decoration:none}
nav{display:flex;gap:22px;font-size:.95rem;font-weight:500}
nav a{color:var(--muted)}
nav a:hover{color:var(--ink);text-decoration:none}

/* hero */
.hero{display:grid;grid-template-columns:1.25fr .75fr;gap:48px;align-items:center;padding:84px 0 72px}
h1{font:800 clamp(2.6rem,6.2vw,4.6rem)/1.02 var(--display);letter-spacing:-.03em}
.role{margin-top:20px;font:500 1.3rem/1.4 var(--display);color:var(--muted)}
.lede{margin-top:20px;max-width:34em;color:var(--muted)}
.cta{display:flex;flex-wrap:wrap;gap:12px;margin-top:32px}
.btn{display:inline-block;padding:12px 22px;border-radius:10px;font-weight:600;border:1.5px solid var(--ink);color:var(--ink)}
.btn:hover{text-decoration:none;background:var(--soft)}
.btn.main{background:var(--accent);border-color:var(--accent);color:#fff}
.btn.main:hover{background:var(--ink);border-color:var(--ink)}
.facts{display:flex;flex-wrap:wrap;gap:8px 28px;margin-top:36px;font-size:.95rem;color:var(--muted)}
.facts b{color:var(--ink);font-weight:600}

/* phone – the one memorable element */
.phone{justify-self:center;width:250px;aspect-ratio:9/18.5;border-radius:38px;padding:11px;background:var(--ink);box-shadow:0 30px 60px -20px rgba(10,60,140,.45);transform:rotate(3deg);animation:rise .9s cubic-bezier(.2,.8,.2,1) both}
.screen{height:100%;border-radius:28px;background:var(--surface);padding:22px 16px 16px;display:flex;flex-direction:column;gap:12px;overflow:hidden;position:relative}
.screen::before{content:"";position:absolute;top:8px;left:50%;width:70px;height:6px;margin-left:-35px;border-radius:9px;background:var(--line)}
.s-title{margin-top:8px;font:700 1rem var(--display)}
.s-total{border-radius:16px;padding:14px;background:linear-gradient(135deg,var(--accent),var(--cyan));color:#fff}
.s-total small{display:block;opacity:.85;font-size:.72rem}
.s-total strong{font:800 1.6rem var(--display)}
.row{display:flex;justify-content:space-between;align-items:center;padding:9px 0;border-bottom:1px solid var(--line);font-size:.8rem}
.row span:last-child{font-weight:600}
.pos{color:#0a8f4e}.neg{color:#d23a3a}
.qr{margin-top:auto;display:grid;grid-template-columns:repeat(7,1fr);gap:2px;width:58px;align-self:center;opacity:.85}
.qr i{aspect-ratio:1;background:var(--ink);border-radius:1px}
.qr i:nth-child(3n),.qr i:nth-child(5n+1){background:transparent}
@keyframes rise{from{opacity:0;transform:translateY(30px) rotate(0)}to{opacity:1;transform:translateY(0) rotate(3deg)}}

/* sections */
section{padding:72px 0;border-top:1px solid var(--line)}
h2{font:800 clamp(1.8rem,3.6vw,2.4rem)/1.1 var(--display);letter-spacing:-.02em;margin-bottom:36px}
h3{font:700 1.3rem/1.25 var(--display)}
.meta{color:var(--muted);font-size:.95rem}

/* experience timeline */
.timeline{position:relative;margin-left:8px;padding-left:34px;border-left:2px solid var(--line)}
.job{position:relative;padding-bottom:44px}
.job:last-child{padding-bottom:0}
.job::before{content:"";position:absolute;left:-43px;top:7px;width:16px;height:16px;border-radius:50%;background:var(--bg);border:3px solid var(--accent)}
.job.now::before{background:var(--accent);box-shadow:0 0 0 6px var(--soft)}
.job ul{margin:14px 0 14px 1.1em;max-width:46em}
.job li{margin-bottom:6px}
.tags{display:flex;flex-wrap:wrap;gap:8px}
.tags span{font-size:.82rem;font-weight:500;padding:3px 11px;border-radius:99px;background:var(--soft);color:var(--accent)}

/* projects */
.proj{display:grid;grid-template-columns:200px 1fr;gap:12px 32px;padding:26px 0;border-bottom:1px solid var(--line)}
.proj:first-of-type{padding-top:0}
.proj:last-of-type{border-bottom:0;padding-bottom:0}
.proj p{max-width:44em;margin:8px 0 12px}

/* skills */
.skills{display:grid;grid-template-columns:repeat(2,1fr);gap:0 56px}
.skill{display:grid;grid-template-columns:130px 1fr;gap:6px 16px;padding:16px 0;border-bottom:1px solid var(--line)}
.skill dt{font-weight:600}
.skill dd{color:var(--muted)}

/* two-col lists */
.duo{display:grid;grid-template-columns:1fr 1fr;gap:56px}
.duo h2{font-size:1.5rem;margin-bottom:22px}
.item{margin-bottom:22px}
.item h3{font-size:1.1rem}

/* contact */
.contact{background:var(--ink);color:#e8eef7;border-radius:24px;padding:56px 48px;margin-bottom:72px}
.contact h2{color:#fff;margin-bottom:14px}
.contact p{color:#b5c4da;max-width:34em}
.links{display:flex;flex-wrap:wrap;gap:12px 28px;margin-top:28px}
.links a{color:#7cc4ff;font-weight:600}
footer{padding:0 0 40px;color:var(--muted);font-size:.9rem}

@media (max-width:820px){
  nav{display:none}
  .hero{grid-template-columns:1fr;padding:48px 0}
  .phone{width:220px;order:-1;justify-self:start}
  .proj{grid-template-columns:1fr}
  .skills,.duo{grid-template-columns:1fr;gap:0}
  .duo>div+div{margin-top:48px}
  .skill{grid-template-columns:1fr}
  .contact{padding:36px 24px}
}
@media (prefers-reduced-motion:reduce){*{animation:none!important;scroll-behavior:auto!important}}
</style>
</head>
<body>

<header>
  <div class="wrap bar">
    <a class="logo" href="#top">Abdullah Anas</a>
    <nav aria-label="Main">
      <a href="#experience">Experience</a>
      <a href="#projects">Projects</a>
      <a href="#skills">Skills</a>
      <a href="#research">Research</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</header>

<main id="top">
<div class="wrap">

  <div class="hero">
    <div>
      <h1>Md. Abdullah Anas</h1>
      <p class="role">Software engineer building mobile apps and the APIs behind them.</p>
      <p class="lede">I work with Kotlin Multiplatform, Flutter and native Android, and build full-stack products with NestJS, Next.js and PostgreSQL. I care about secure, maintainable software that people find easy to use.</p>
      <div class="cta">
        <a class="btn main" href="mailto:anas.official.tech@gmail.com">Email me</a>
        <a class="btn" href="https://github.com/mdAbdullahAnas">View GitHub</a>
        <a class="btn" href="https://www.linkedin.com/in/mdabdullahanas">LinkedIn</a>
      </div>
      <div class="facts">
        <span><b>Now</b> Bdjobs.com, Dhaka</span>
        <span><b>Degree</b> B.Sc. CSE, AIUB</span>
        <span><b>Published</b> IEEE TENCON 2026</span>
      </div>
    </div>

    <div class="phone" role="img" aria-label="Illustration of the SplitMate expense app showing balances and a QR code">
      <div class="screen">
        <div class="s-title">SplitMate</div>
        <div class="s-total"><small>You are owed</small><strong>৳ 1,240</strong></div>
        <div class="row"><span>Rafi</span><span class="pos">+ ৳ 620</span></div>
        <div class="row"><span>Tania</span><span class="pos">+ ৳ 780</span></div>
        <div class="row"><span>Sabbir</span><span class="neg">− ৳ 160</span></div>
        <div class="qr" aria-hidden="true"><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i><i></i></div>
      </div>
    </div>
  </div>

  <section id="experience">
    <h2>Experience</h2>
    <div class="timeline">
      <article class="job now">
        <h3>Mobile Application Developer, Bdjobs.com</h3>
        <p class="meta">October 2026 – Present · On-site</p>
        <ul>
          <li>Migrated the Sales Dashboard app from native Kotlin to Kotlin Multiplatform, so one codebase now serves Android and iOS.</li>
          <li>Fixed bugs and UI layout issues across the main Bdjobs mobile app to improve stability, usability and visual consistency.</li>
        </ul>
        <div class="tags"><span>Kotlin</span><span>KMP</span><span>Android</span><span>iOS</span><span>REST APIs</span></div>
      </article>
      <article class="job">
        <h3>Mobile Apps Developer Intern, NNSEL</h3>
        <p class="meta">July 2026 – September 2026 · Hybrid</p>
        <ul>
          <li>Built a subscription-based HRM app for mobile and web with 15+ modules, including Payroll, Attendance and Leave.</li>
          <li>Integrated 200+ REST API endpoints using Dio and Riverpod for backend functionality and data synchronisation.</li>
          <li>Implemented role-based access control, secure authentication and location-based attendance with OpenStreetMap.</li>
        </ul>
        <div class="tags"><span>Flutter</span><span>Dart</span><span>Riverpod</span><span>Dio</span><span>REST APIs</span></div>
      </article>
    </div>
  </section>

  <section id="projects">
    <h2>Projects</h2>

    <article class="proj">
      <div><h3>Kiddo</h3><p class="meta">Educational learning app</p></div>
      <div>
        <p>A cross-platform app with 6 interactive games and 90 levels each. Includes local data persistence, progress tracking, gamification and Lottie animations.</p>
        <div class="tags"><span>Flutter</span><span>Dart</span><span>Hive</span><span>Lottie</span></div>
      </div>
    </article>

    <article class="proj">
      <div><h3>SplitMate</h3><p class="meta">Expense splitter · Live on Google Play</p></div>
      <div>
        <p>Tracks shared expenses with full CRUD, automatic balance calculation, debt settlement and QR code sharing.</p>
        <div class="tags"><span>Kotlin</span><span>SQLite</span><span>Material Design</span><span>QR Code</span></div>
        <p><a href="https://play.google.com/store/apps/details?id=com.misty.splitmate">Open on Google Play</a></p>
      </div>
    </article>

    <article class="proj">
      <div><h3>Matching</h3><p class="meta">Memory card game · Android</p></div>
      <div>
        <p>A published game with flip-card animations, multiple difficulty levels, custom game modes, performance scoring and level progression.</p>
        <div class="tags"><span>Kotlin</span><span>SQLite</span><span>Material Design</span></div>
      </div>
    </article>

    <article class="proj">
      <div><h3>School Management System</h3><p class="meta">Full-stack web platform</p></div>
      <div>
        <p>A role-based platform for admins, teachers and students, with JWT authentication, REST APIs and student and teacher management on PostgreSQL.</p>
        <div class="tags"><span>Next.js</span><span>NestJS</span><span>PostgreSQL</span><span>TypeScript</span></div>
      </div>
    </article>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <dl class="skills">
      <div class="skill"><dt>Mobile</dt><dd>Kotlin, Kotlin Multiplatform, Flutter, Dart, Android, iOS</dd></div>
      <div class="skill"><dt>Backend</dt><dd>NestJS, REST APIs, JWT, RBAC, PostgreSQL, SQLite, Firebase Firestore</dd></div>
      <div class="skill"><dt>Frontend</dt><dd>Next.js, TypeScript, JavaScript</dd></div>
      <div class="skill"><dt>Languages</dt><dd>Kotlin, Dart, TypeScript, JavaScript, Java, C++, Python</dd></div>
      <div class="skill"><dt>Tools</dt><dd>Git, Docker, Android Studio, VS Code, MCP</dd></div>
      <div class="skill"><dt>Platforms</dt><dd>Android, Web, Windows, Linux, Arduino Uno, Raspberry Pi</dd></div>
    </dl>
  </section>

  <section id="research">
    <div class="duo">
      <div>
        <h2>Research</h2>
        <div class="item">
          <h3>ALIS D-Net: Detecting Drug-Induced Autoimmune Hepatitis Signals</h3>
          <p class="meta">Published at IEEE TENCON 2026</p>
        </div>
        <div class="item">
          <h3>Arduino-Based RADAR System</h3>
          <p class="meta">Published and presented at ICEI 2026</p>
        </div>
      </div>
      <div>
        <h2>Education</h2>
        <div class="item">
          <h3>B.Sc. in Computer Science and Engineering</h3>
          <p class="meta">American International University-Bangladesh (AIUB), Dhaka<br>August 2022 – June 2026 · CGPA 3.45</p>
        </div>
        <div class="item">
          <h3>Recognition</h3>
          <p class="meta">Inter-university competitive programming contests. Cisco Networking Academy: IT Essentials, PC Hardware and Software.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="contact" style="border-top:0;padding-bottom:0">
    <div class="contact">
      <h2>Let’s build something</h2>
      <p>I’m open to mobile and full-stack roles. The quickest way to reach me is email.</p>
      <div class="links">
        <a href="mailto:anas.official.tech@gmail.com">anas.official.tech@gmail.com</a>
        <a href="tel:+8801581966623">+880 1581 966623</a>
        <a href="https://www.linkedin.com/in/mdabdullahanas">LinkedIn</a>
        <a href="https://github.com/mdAbdullahAnas">GitHub</a>
      </div>
    </div>
  </section>

</div>
</main>

<footer>
  <div class="wrap">© 2026 Md. Abdullah Anas</div>
</footer>

</body>
</html>
