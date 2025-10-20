<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>EISSA ABD ALMWLA — الموقع الرسمي</title>
  <meta name="description" content="الموقع الرسمي لعيسى عبد المولى — صفحة تعريف وتواصل وسيرة ذاتية" />
  <meta name="keywords" content="Eissa, عيسى, portfolio, CV, تواصل, دمياط" />
  <meta name="author" content="EISSA ABD ALMWLA" />
  <style>
    :root{
      --bg:#010409; --panel:#0a0f1c; --muted:#bdbdbd; --white:#ffffff;
      --neon:#00eaff; --neon-2:#ff4d9d; --glass:rgba(255,255,255,0.05);
      --accent:#00eaff; --radius:14px; --maxw:1000px; font-family:'Cairo', sans-serif;
    }
    *{box-sizing:border-box;scroll-behavior:smooth}
    html,body{height:100%}
    body{margin:0;background:linear-gradient(135deg,var(--bg),#03050b);color:var(--white);display:flex;align-items:center;justify-content:center;padding:20px}
    a{color:inherit;text-decoration:none}

    .site{width:100%;max-width:var(--maxw);border-radius:20px;padding:18px;background:rgba(255,255,255,0.02);border:1px solid rgba(255,255,255,0.05);box-shadow:0 0 25px rgba(0,234,255,0.05);overflow:hidden}

    header{display:flex;align-items:center;justify-content:space-between;padding:12px 18px;background:linear-gradient(90deg,rgba(255,255,255,0.02),rgba(255,255,255,0.04));border-radius:12px}
    .brand{margin:0 auto;font-weight:800;letter-spacing:1px;font-size:22px;text-align:center;background:linear-gradient(90deg,var(--neon),var(--neon-2));-webkit-background-clip:text;-webkit-text-fill-color:transparent}
    nav{display:flex;gap:10px;align-items:center}
    .nav-btn{background:transparent;border:1px solid rgba(255,255,255,0.1);padding:10px 14px;border-radius:10px;cursor:pointer;font-weight:600;transition:.3s;color:var(--white)}
    .nav-btn:hover{background:rgba(255,255,255,0.1)}
    .nav-btn.active{background:linear-gradient(90deg,var(--neon),var(--neon-2));color:#000}

    .content{display:grid;grid-template-columns:1fr 340px;gap:20px;padding:12px}
    @media(max-width:900px){.content{grid-template-columns:1fr}}

    .card{background:linear-gradient(180deg,var(--panel),rgba(255,255,255,0.02));padding:16px;border-radius:12px;border:1px solid rgba(255,255,255,0.06);transition:.3s;position:relative;overflow:hidden}
    .card:hover{transform:translateY(-6px);box-shadow:0 0 18px rgba(0,234,255,0.1)}
    .card h3{margin:0 0 8px 0;font-size:18px;color:var(--neon)}
    .card p{margin:0;color:var(--muted);font-size:13px}

    .action{background:linear-gradient(90deg,var(--neon),var(--neon-2));color:#000;padding:8px 12px;border:none;border-radius:8px;cursor:pointer;font-weight:600;transition:.3s}
    .action:hover{opacity:0.85}

    aside.panel{background:rgba(255,255,255,0.03);padding:16px;border-radius:12px;border:1px solid rgba(255,255,255,0.04)}
    .cv{background:var(--glass);padding:12px;border-radius:10px;color:var(--white);font-size:14px}

    footer{text-align:center;padding:10px;font-size:13px;color:var(--muted);margin-top:10px}

    .page{display:none;opacity:0;transform:translateY(10px);transition:all .4s}
    .page.active{display:block;opacity:1;transform:none}

    input,textarea{width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.15);background:rgba(255,255,255,0.08);color:var(--white);margin-bottom:8px;font-weight:600}
    input::placeholder,textarea::placeholder{color:#d3d3d3;opacity:0.8}
    input:focus,textarea:focus{outline:none;border-color:var(--neon);box-shadow:0 0 8px rgba(0,234,255,0.4)}
  </style>

  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/emailjs-com@3/dist/email.min.js"></script>
  <script>emailjs.init('h9ZHyKt8zcuCkKIfb');</script>
</head>
<body>
  <div class="site">
    <header>
      <div style="width:100px"></div>
      <div class="brand">EISSA ABD ALMWLA</div>
      <nav>
        <button class="nav-btn active" data-target="home">الرئيسية</button>
        <button class="nav-btn" data-target="contact">تواصل</button>
        <button class="nav-btn" data-target="cv">السيرة الذاتية</button>
      </nav>
    </header>

    <main class="content">
      <section>
        <div id="home" class="page active">
          <h2>أهلاً بيك 👋</h2>
          <p style="color:var(--muted)">دي صفحتي الشخصية الرسمية — ممكن تتواصل معايا أو تبعتلي رسالة سريعة.</p>
          <div class="card">
            <h3>✉️ ابعت رسالة سريعة</h3>
            <form id="quickMsg">
              <input name="from_name" placeholder="اسمك" required>
              <input name="reply_to" type="email" placeholder="بريدك (اختياري)">
              <textarea name="message" placeholder="اكتب الرسالة هنا" required></textarea>
              <button class="action" id="sendBtn" type="button" onclick="sendEmail()">إرسال</button>
            </form>
            <p style="font-size:12px;color:var(--muted)">هتوصل الرسالة على الإيميل: <strong>eissaabdalmwla7@gmail.com</strong></p>
          </div>
        </div>

        <div id="contact" class="page">
          <h2>طرق التواصل</h2>
          <div class="card"><a href="tel:01004167961" class="action">📞 اتصال مباشر</a></div>
          <div class="card"><a href="https://wa.me/201004167961" target="_blank" class="action">💬 WhatsApp</a></div>
          <div class="card"><a href="https://www.facebook.com/share/1GgARrqy14/" target="_blank" class="action">🌐 Facebook</a></div>
        </div>

        <div id="cv" class="page">
          <h2>السيرة الذاتية</h2>
          <div class="cv">
            <p><strong>الاسم:</strong> عيسى عبد المولى صالح محمد</p>
            <p><strong>الميلاد:</strong> 3/7/2006</p>
            <p><strong>الإقامة:</strong> ال28 دمياط الجديدة</p>
          </div>
        </div>
      </section>

      <aside class="panel">
        <h3>معلومات سريعة</h3>
        <p>📞 01004167961</p>
        <p>🌐 <a href="https://www.facebook.com/share/1GgARrqy14/" target="_blank">Facebook</a></p>
      </aside>
    </main>

    <footer>© 2025 EISSA ABD ALMWLA — جميع الحقوق محفوظة</footer>
  </div>

  <script>
    const navBtns=document.querySelectorAll('.nav-btn');
    navBtns.forEach(b=>b.addEventListener('click',()=>{
      document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
      document.getElementById(b.dataset.target).classList.add('active');
      navBtns.forEach(x=>x.classList.remove('active'));
      b.classList.add('active');
    }));

    async function sendEmail(){
      const btn=document.getElementById('sendBtn');
      btn.disabled=true;btn.textContent='جاري الإرسال...';
      try{
        const form=document.getElementById('quickMsg');
        await emailjs.sendForm('service_2swaqon','template_1wl7q4x',form);
        alert('✅ تم إرسال الرسالة بنجاح!');
        form.reset();
      }catch(e){
        alert('⚠️ حصل خطأ في الإرسال، حاول تاني.');
      }finally{
        btn.disabled=false;btn.textContent='إرسال';
      }
    }
  </script>
</body>
</html>
