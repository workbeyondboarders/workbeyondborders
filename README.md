<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Work Beyond Borders — Home</title>
  <meta name="description" content="Work Beyond Borders — Apply for global job opportunities.">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/intl-tel-input/17.0.19/css/intlTelInput.min.css">
  <style>
    :root{--accent:#0b63d5;--accent-dark:#084f9b;--card:#fff;--muted:#6b7280;--radius:12px;--shadow:0 6px 20px rgba(9,30,66,0.08);--maxw:1000px}
    *{box-sizing:border-box}body{margin:0;font-family:Inter,system-ui,Arial;background:linear-gradient(180deg,#eaf4ff 0%,#f8fbff 100%);color:#000;-webkit-font-smoothing:antialiased}
    header{max-width:var(--maxw);margin:20px auto;display:flex;align-items:center;padding:0 18px;gap:14px}
    .logo-symbol{width:54px;height:54px;border-radius:10px;display:flex;align-items:center;justify-content:center;background:linear-gradient(135deg,var(--accent),var(--accent-dark));color:#fff;font-size:20px}
    .site-title{font-weight:800;font-size:18px}
    nav{margin-left:auto}nav a{margin-left:12px;text-decoration:none;color:var(--accent-dark);font-weight:600}
    main{max-width:var(--maxw);margin:12px auto;padding:18px}
    .hero{background:var(--card);padding:28px;border-radius:var(--radius);box-shadow:var(--shadow);text-align:center}
    .hero h1{margin:0;font-size:28px}
    .muted{color:var(--muted)}
    .cta{margin-top:14px;display:flex;gap:12px;justify-content:center;flex-wrap:wrap}
    .btn{padding:10px 16px;border-radius:10px;border:2px solid transparent;cursor:pointer;font-weight:700}
    .btn-primary{background:white;border:2px solid var(--accent);color:var(--accent-dark)}
    .btn-outline{background:transparent;border:2px solid var(--accent);color:var(--accent)}
    .sections{display:grid;grid-template-columns:1fr;gap:18px;margin-top:20px}
    @media(min-width:900px){.sections{grid-template-columns:2fr 1fr}}
    .card{background:var(--card);padding:16px;border-radius:12px;box-shadow:var(--shadow)}
    .live{font-weight:700;color:var(--accent-dark)}
    .test-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
    @media(min-width:700px){.test-grid{grid-template-columns:repeat(3,1fr)}}
    .test{display:flex;gap:10px;align-items:flex-start;padding:10px;border-radius:10px;background:linear-gradient(180deg,#fff,#fbfdff);border:1px solid #eef7ff}
    .avatar{width:48px;height:48px;border-radius:50%;display:flex;align-items:center;justify-content:center;background:#f1f7ff;color:#084f9b;font-weight:700}
    footer{max-width:var(--maxw);margin:20px auto;padding:18px;color:var(--muted);font-size:14px}
    a.pill{display:inline-block;padding:6px 10px;border-radius:10px;border:1px solid #e6f0ff;background:#f8fbff;color:var(--accent-dark);text-decoration:none;font-weight:700}
  </style>
</head>
<body>
  <header>
    <div style="display:flex;gap:12px;align-items:center">
      <div class="logo-symbol" aria-hidden>✈️</div>
      <div>
        <div class="site-title">Work Beyond Borders</div>
        <div class="muted" style="font-size:13px">Apply for Jobs Worldwide</div>
      </div>
    </div>
    <nav>
      <a href="index.html">Home</a>
      <a href="jobs.html">Available Jobs</a>
      <a href="apply.html">Apply</a>
      <a href="contact.html">Contact</a>
    </nav>
  </header>

  <main>
    <section class="hero card">
      <h1>Work Beyond Borders</h1>
      <p class="muted">Apply for global job opportunities with Work Beyond Borders</p>
      <div class="cta">
        <a class="btn btn-outline" href="jobs.html">See Available Jobs</a>
        <a class="btn btn-primary" href="apply.html">Apply Now</a>
      </div>
      <div style="margin-top:14px" class="muted">Live: <span id="live" class="live">Caregivers in Canada • Technicians in Germany • Cleaners in UAE</span></div>
    </section>

    <div class="sections">
      <div>
        <section class="card" style="margin-top:18px">
          <h3 style="margin-top:0">About Work Beyond Borders</h3>
          <p class="muted">Work Beyond Borders connects job seekers with verified and trusted opportunities around the world. We list available roles by country and make it easy to apply directly from the website.</p>
        </section>

        <section class="card" style="margin-top:14px">
          <h3 style="margin-top:0">Highlights</h3>
          <p class="muted">We update job postings frequently. Explore by continent and country to find roles like caregiver, factory worker, hospitality staff, drivers, and more.</p>
          <div style="margin-top:12px;display:flex;gap:8px;flex-wrap:wrap">
            <a class="pill" href="jobs.html#Europe">Europe</a>
            <a class="pill" href="jobs.html#Asia">Asia</a>
            <a class="pill" href="jobs.html#North America">North America</a>
            <a class="pill" href="jobs.html#South America">South America</a>
            <a class="pill" href="jobs.html#Africa">Africa</a>
          </div>
        </section>
      </div>

      <aside>
        <section class="card">
          <h4 style="margin-top:0">Testimonials</h4>
          <p class="muted">Real stories from applicants (sample testimonials)</p>
          <div class="test-grid" id="testHome">
            <!-- JS fills these -->
          </div>
        </section>

        <section class="card" style="margin-top:14px">
          <h4 style="margin-top:0">Contact</h4>
          <p class="muted">Email: <a href="mailto:workbeyondboarders@gmail.com">workbeyondboarders@gmail.com</a></p>
          <p class="muted">Follow us: Telegram • Facebook (links added later)</p>
        </section>
      </aside>
    </div>
  </main>

  <footer>
    © <span id="year"></span> Work Beyond Borders — All rights reserved
  </footer>

  <script>
    // year
    document.getElementById('year').textContent = new Date().getFullYear();

    // live highlights rotate
    const highlights = ['Caregivers in Canada','Technicians in Germany','Cleaners in UAE','Warehouse roles in USA','Hospitality in Spain'];
    let i = 0;
    setInterval(()=>{i=(i+1)%highlights.length;document.getElementById('live').textContent = highlights[i];},4000);

    // sample testimonials (30)
    const testimonials = [
      {n:'Maria G., Spain',t:'I found a caregiver role in Canada through Work Beyond Borders. Thank you!',g:'female'},
      {n:'Samuel K., Nigeria',t:'The application process was easy and quick. I got an interview within days.',g:'male'},
      {n:'Fatima L., Philippines',t:'Very helpful and professional. I now work as a hotel staff in UAE.',g:'female'},
      {n:'John D., USA',t:'Great platform for international job leads. Clean and simple UI.',g:'male'},
      {n:'Aisha N., Kenya',t:'I applied and received guidance on documents. Highly recommended.',g:'female'},
      {n:'Carlos M., Brazil',t:'Found factory work in Germany. Site looks legit and trustworthy.',g:'male'},
      {n:'Li Na, China',t:'Clear job listings and an easy form. Thank you for connecting me.',g:'female'},
      {n:'Omar R., Egypt',t:'Professional team and fast replies. Helped me secure a position.',g:'male'},
      {n:'Nora S., Ireland',t:'Very friendly service. I got a position in hospitality.',g:'female'},
      {n:'Miguel T., Mexico',t:'Worked well for my job search abroad. Simple and effective.',g:'male'},
      {n:'Elena V., Russia',t:'I appreciate the clarity of job posts and instructions.',g:'female'},
      {n:'Ahmed B., Morocco',t:'Good listings and quick feedback. I now work overseas.',g:'male'},
      {n:'Priya P., India',t:'Easy to use and very helpful. The phone-format is great.',g:'female'},
      {n:'Paul R., Canada',t:'Useful portal, neat layout. Helped me find a local role.',g:'male'},
      {n:'Zainab K., UAE',t:'Received timely updates and clear steps. Very supportive.',g:'female'},
      {n:'Diego F., Argentina',t:'Helpful platform, found a job quickly. Thanks!',g:'male'},
      {n:'Sofia M., Italy',t:'Friendly and professional. I recommend Work Beyond Borders.',g:'female'},
      {n:'Kwame A., Ghana',t:'Good opportunities and clear instructions to apply.',g:'male'},
      {n:'Hana L., Japan',t:'Accessible site, good opportunities. Thank you!',g:'female'},
      {n:'Marcus Y., Sweden',t:'Practical job listings and easy contact method.',g:'male'},
      {n:'Lina R., Colombia',t:'I got an interview quickly. The testimonials inspired me to apply.',g:'female'},
      {n:'Tariq H., Pakistan',t:'Excellent service. Straightforward application process.',g:'male'},
      {n:'Marta O., Poland',t:'Clean design, easy to use on mobile. Found a job fast.',g:'female'},
      {n:'Ben S., Australia',t:'Legit and user-friendly. Good luck to applicants!',g:'male'},
      {n:'Yara A., Lebanon',t:'Supportive guidance and responsive. Great experience.',g:'female'},
      {n:'Ibrahim S., Algeria',t:'Found opportunities I did not see elsewhere. Helpful.',g:'male'},
      {n:'Cristina D., Chile',t:'The form was clear and the process smooth. Recommended.',g:'female'},
      {n:'Ethan W., UK',t:'Easily found job categories and applied successfully.',g:'male'},
      {n:'Zoe N., Greece',t:'Positive experience. Friendly tone and good listings.',g:'female'}
    ];
    const testHome = document.getElementById('testHome');
    testimonials.slice(0,9).forEach(t=>{
      const div=document.createElement('div');div.className='test';
      div.innerHTML=`<div class="avatar">${t.g==='female'?'♀':'♂'}</div><div><strong>${t.n}</strong><div style="margin-top:6px">${t.t}</div><small class="muted">Verified applicant</small></div>`;
      testHome.appendChild(div);
    });
  </script>
</body>
</html>
