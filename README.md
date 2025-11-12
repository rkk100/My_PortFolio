<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Rohit Kumar — Portfolio</title>
  <meta name="description" content="Rohit Kumar — BCA Fresher · eCourt Phase Website (Python)" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    :root{
      --bg:#0b1220; --card:#0f1724; --muted:#9fb0c9; --accent:#06b6d4; --accent-2:#7c3aed; --glass: rgba(255,255,255,0.03);
      --radius:12px; --maxw:1100px; font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, Arial; color-scheme:dark;
    }
    body.light{ --bg:#f8fafc; --card:#ffffff; --muted:#61707b; --accent:#0ea5a4; color-scheme:light; color:#071023 }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;background:linear-gradient(180deg,var(--bg),#031025);color:#e8f5ff}
    body.light{background:linear-gradient(180deg,#f8fafc,#eef2f7);color:var(--card)}
    a{color:var(--accent)}
    img{max-width:100%;display:block}
    .wrap{width:min(var(--maxw),94%);margin:0 auto;padding:28px 0}

    header{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:54px;height:54px;border-radius:12px;background:linear-gradient(135deg,var(--accent),var(--accent-2));display:flex;align-items:center;justify-content:center;font-weight:800;color:#041022}
    nav{display:flex;gap:14px;align-items:center}
    .nav-link{font-weight:600;font-size:14px}
    .btn{background:linear-gradient(90deg,var(--accent),var(--accent-2));padding:10px 14px;border-radius:10px;color:#041022;border:none;cursor:pointer}

    .hero{display:grid;grid-template-columns:1fr 380px;gap:28px;align-items:start;margin-top:18px}
    .intro h1{font-size:30px;margin:0}
    .intro p{color:var(--muted);margin:12px 0 16px;line-height:1.5}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));backdrop-filter:blur(6px);padding:16px;border-radius:var(--radius);box-shadow:0 12px 40px rgba(2,6,23,0.6)}
    body.light .card{background:linear-gradient(180deg, rgba(11,17,32,0.02), rgba(255,255,255,0.6));box-shadow:none}

    .stats{display:flex;gap:10px;margin-top:12px}
    .stat{flex:1;background:var(--glass);padding:10px;border-radius:10px;text-align:center}

    .about{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:20px}
    .skills{display:flex;flex-direction:column;gap:10px}
    .skill{display:flex;justify-content:space-between;align-items:center}
    .meter{height:10px;background:rgba(255,255,255,0.05);border-radius:999px;overflow:hidden;width:60%}
    .meter > i{display:block;height:100%;background:linear-gradient(90deg,var(--accent),var(--accent-2))}

    .projects{margin-top:22px;display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
    .project{display:flex;flex-direction:column;gap:8px;padding:12px;border-radius:12px}
    .tags{display:flex;gap:8px;flex-wrap:wrap}
    .tag{padding:6px 8px;background:rgba(255,255,255,0.03);border-radius:999px;font-size:12px;color:var(--muted)}

    .contact{margin-top:22px;display:grid;grid-template-columns:1fr 340px;gap:16px}
    input,textarea,select{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:10px;border-radius:8px;color:inherit}
    body.light input, body.light textarea{border-color:rgba(11,17,32,0.06);background:transparent;color:inherit}
    textarea{min-height:120px}
    .small{font-size:13px;color:var(--muted)}

    footer{margin-top:28px;padding:18px 0;border-top:1px solid rgba(255,255,255,0.02);text-align:center;color:var(--muted)}

    .social-row{display:flex;gap:10px;justify-content:center;margin-top:12px}
    .social-btn{padding:8px 10px;border-radius:8px;background:rgba(255,255,255,0.03);display:inline-flex;gap:8px;align-items:center;text-decoration:none;color:inherit}

    .status{margin-top:8px;font-weight:600}

    @media (max-width:980px){.hero{grid-template-columns:1fr}.about{grid-template-columns:1fr}.projects{grid-template-columns:repeat(2,1fr)}}
    @media (max-width:640px){.projects{grid-template-columns:1fr}.logo{width:44px;height:44px;font-size:16px}header{flex-direction:column;align-items:flex-start}}

  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">RK</div>
        <div>
          <div style="font-weight:800">Rohit Kumar</div>
          <div class="small">BCA • Fresher • Python Developer</div>
        </div>
      </div>

      <nav>
        <a class="nav-link" href="#projects">Projects</a>
        <a class="nav-link" href="#about">About</a>
        <a class="nav-link" href="#contact">Contact</a>
        <button id="modeToggle" class="btn">Toggle theme</button>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div>
          <div class="card">
            <h1>Hi — I’m <span style="color:var(--accent)">Rohit Kumar</span></h1>
            <p class="small">BCA graduate and fresher. Built <strong>eCourt Phase Website</strong> using Python. Looking for internships or junior dev roles.</p>
            <div style="display:flex;gap:12px;margin-top:12px">
              <a class="btn" href="#contact">Get in touch</a>
              <a class="small" href="#projects" style="padding:10px 12px;border-radius:10px;background:transparent;border:1px solid rgba(255,255,255,0.04);">See project</a>
            </div>
            <div class="stats">
              <div class="stat"><div style="font-weight:700">1</div><div class="small">Project</div></div>
              <div class="stat"><div style="font-weight:700">Fresher</div><div class="small">Experience</div></div>
              <div class="stat"><div style="font-weight:700">BCA</div><div class="small">Education</div></div>
            </div>
          </div>

          <section id="projects" style="margin-top:18px">
            <h3>Selected Project</h3>
            <div class="projects">
              <article class="project card">
                <h4>eCourt Phase Website</h4>
                <p class="small">Court case management and public viewing portal built with Python (Flask) — case listing, search and basic workflows.</p>
                <div class="tags"><span class="tag">Python</span><span class="tag">Flask</span><span class="tag">HTML</span></div>
                <div style="margin-top:auto;display:flex;gap:8px;justify-content:flex-end"><a class="small" href="#">Live</a><a class="small" href="#">Source</a></div>
              </article>
            </div>
          </section>
        </div>

        <aside>
          <div class="card" style="text-align:center">
            <img src="https://images.unsplash.com/photo-1599566150163-29194dcaad36?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="Rohit" style="border-radius:10px;margin-bottom:12px;width:140px;height:140px;object-fit:cover"/>
            <div style="font-weight:700">Rohit Kumar</div>
            <div class="small">Based in India</div>

            <div class="social-row" style="justify-content:center">
              <a class="social-btn" href="https://instagram.com/yuvavichar3361" target="_blank"><i class="fab fa-instagram"></i></a>
              <a class="social-btn" href="https://github.com/rkk100" target="_blank"><i class="fab fa-github"></i></a>
              <a class="social-btn" href="https://www.facebook.com/Rohit-K-Singh-Chouhan" target="_blank"><i class="fab fa-facebook"></i></a>
              <a id="lnkLinkedin" class="social-btn" href="https://www.linkedin.com/in/rohit-kumar" target="_blank"><i class="fab fa-linkedin"></i></a>
            </div>

            <div style="margin-top:12px"><a class="btn" href="reumey.pdf" download>Download CV</a></div>
          </div>
        </aside>
      </section>

      <section id="about" class="about">
        <div class="card">
          <h3>About</h3>
          <p class="small">I completed my BCA and built the eCourt Phase Website using Python. I focus on writing simple, maintainable code and solving real problems.</p>
          <ul class="small" style="margin-top:8px">
            <li>Languages & tools: Python, Flask, HTML, CSS, JS (basic)</li>
            <li>Databases: MySQL</li>
            <li>Education: BCA</li>
          </ul>
        </div>

        <div class="card">
          <h4>Skills</h4>
          <div class="skills">
            <div class="skill"><span>Python</span><div class="meter"><i style="width:78%"></i></div></div>
            <div class="skill"><span>HTML & CSS</span><div class="meter"><i style="width:85%"></i></div></div>
            <div class="skill"><span>JavaScript (basic)</span><div class="meter"><i style="width:55%"></i></div></div>
            <div class="skill"><span>MySQL</span><div class="meter"><i style="width:60%"></i></div></div>
          </div>
        </div>
      </section>

      <section id="contact" class="contact">
        <div class="card">
          <h3>Contact</h3>
          <p class="small">Send me a message — I will receive it in my email. (First time: verify FormSubmit email)</p>

          <form id="contactForm">
            <input type="hidden" name="_subject" value="New message from Portfolio" />
            <input type="text" id="cname" name="name" placeholder="Your name" required />
            <input type="email" id="cemail" name="email" placeholder="Your email" required />
            <input type="text" id="csubject" name="subject" placeholder="Subject (optional)" />
            <textarea id="cmessage" name="message" placeholder="Your message" required></textarea>

            <!-- simple math captcha (works everywhere) -->
            <div style="display:flex;gap:8px;align-items:center">
              <div class="small" id="captchaLabel">Verify: </div>
              <input type="text" id="captchaInput" placeholder="Answer" style="width:110px;padding:8px;border-radius:8px;border:1px solid rgba(255,255,255,0.06)" required />
            </div>

            <div style="display:flex;gap:10px;align-items:center;margin-top:8px">
              <button type="submit" id="sendBtn" class="btn">Send message</button>
              <div class="small">Or email: <a href="mailto:rohitbca2005@gmail.com">rohitbca2005@gmail.com</a></div>
            </div>
            <div id="formStatus" class="status"></div>
          </form>
        </div>

        <aside class="card">
          <h4>Quick Info</h4>
          <p class="small"><strong>Location:</strong> India</p>
          <p class="small"><strong>Experience:</strong> Fresher</p>
          <p class="small"><strong>Education:</strong> BCA</p>
          <div style="margin-top:12px"><a class="btn" href="resumey.pdf" download>Download CV</a></div>
        </aside>
      </section>

    </main>

    <footer>
      © <span id="year"></span> Rohit Kumar — Built with❤️
    </footer>
  </div>

  <script>
    // Basic dynamic interactions, math captcha and form send via FormSubmit
    document.getElementById('year').textContent = new Date().getFullYear();

    // Theme toggle
    const modeToggle = document.getElementById('modeToggle');
    // persist theme
    const savedTheme = localStorage.getItem('rk_theme') || 'dark';
    if(savedTheme === 'light') document.body.classList.add('light');
    modeToggle.addEventListener('click', ()=>{
      document.body.classList.toggle('light');
      localStorage.setItem('rk_theme', document.body.classList.contains('light')? 'light':'dark');
    });

    // Simple math captcha generation
    function makeCaptcha(){
      const a = Math.floor(Math.random()*9)+1;
      const b = Math.floor(Math.random()*9)+1;
      const label = document.getElementById('captchaLabel');
      label.textContent = `Verify: ${a} + ${b} = `;
      // store result
      label.dataset.answer = (a+b).toString();
    }
    makeCaptcha();

    // Form submission handler
    const FORM_SUBMIT_URL = 'https://formsubmit.co/ajax/rohitbca2005@gmail.com'; // ajax endpoint
    const form = document.getElementById('contactForm');
    const status = document.getElementById('formStatus');
    form.addEventListener('submit', async (e)=>{
      e.preventDefault();
      status.textContent = '';
      const name = document.getElementById('cname').value.trim();
      const email = document.getElementById('cemail').value.trim();
      const message = document.getElementById('cmessage').value.trim();
      const subject = document.getElementById('csubject').value.trim();
      const captchaInput = document.getElementById('captchaInput').value.trim();
      const captchaLabel = document.getElementById('captchaLabel');

      if(!name || !email || !message){ status.style.color='orange'; status.textContent = 'Please fill required fields.'; return; }
      if(captchaInput !== captchaLabel.dataset.answer){ status.style.color='orange'; status.textContent = 'Captcha incorrect — try again.'; makeCaptcha(); document.getElementById('captchaInput').value=''; return; }

      // prepare payload
      const payload = { name, email, subject, message };

      // disable button
      const btn = document.getElementById('sendBtn'); btn.disabled = true; btn.textContent = 'Sending...';

      try{
        const res = await fetch(FORM_SUBMIT_URL, {
          method: 'POST',
          headers: { 'Content-Type': 'application/json', 'Accept': 'application/json' },
          body: JSON.stringify(payload)
        });
        if(res.ok){
          const data = await res.json();
          status.style.color = 'lightgreen'; status.textContent = '✅ Message sent. Check your inbox.';
          form.reset(); makeCaptcha();
        } else {
          // fallback: try standard form submit by creating hidden form
          status.style.color='red'; status.textContent = 'Send failed via AJAX — trying fallback...';
          // build fallback form
          const f = document.createElement('form');
          f.method='POST'; f.action='https://formsubmit.co/rohitbca2005@gmail.com';
          f.style.display='none';
          f.innerHTML = `<input name="name" value="${encodeHTML(name)}"><input name="email" value="${encodeHTML(email)}"><input name="subject" value="${encodeHTML(subject)}"><input name="message" value="${encodeHTML(message)}">`;
          document.body.appendChild(f); f.submit();
        }
      }catch(err){
        console.error('Send error', err);
        status.style.color='red'; status.textContent = 'Network error. Try again later.';
      }finally{ btn.disabled=false; btn.textContent='Send message'; }
    });

    function encodeHTML(s){ return s.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;'); }

    // small accessibility
    document.querySelectorAll('a').forEach(a=>a.addEventListener('keydown', (e)=>{ if(e.key==='Enter') a.click(); }));
  </script>
</body>
</html>
