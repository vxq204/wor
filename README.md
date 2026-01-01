<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Knowledge | دورات تعليمية احترافية</title>
  <meta name="description" content="Knowledge منصة دورات تعليمية احترافية في عمّان، الأردن. تعلم التسويق الرقمي، البرمجة، التصميم الجرافيكي، إدارة الأعمال، مهارات العرض والإلقاء والتعليم عبر التكنولوجيا." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0b1220;
      --card:#121a2e;
      --muted:#95a0b0;
      --brand:#4cc9f0;
      --accent:#f72585;
      --text:#e9edf5;
      --success:#2ecc71;
      --warn:#f39c12;
      --radius:14px;
      --shadow:0 14px 40px rgba(0,0,0,0.35);
    }
    *{box-sizing:border-box}
    html, body {margin:0; padding:0; background:linear-gradient(180deg,#0b1220 0%, #0e1526 100%); color:var(--text); font-family:"Cairo",system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial; }
    a{color:var(--brand); text-decoration:none}
    img{max-width:100%; display:block}
    /* Layout */
    .container{width:95%; max-width:1200px; margin:0 auto}
    header{
      position:sticky; top:0; z-index:50;
      background:rgba(11,18,32,0.6); backdrop-filter:blur(10px);
      border-bottom:1px solid rgba(255,255,255,0.08);
    }
    .nav{
      display:flex; align-items:center; justify-content:space-between; gap:18px; padding:14px 0;
    }
    .brand{
      display:flex; align-items:center; gap:12px; font-weight:800; letter-spacing:.5px;
    }
    .brand img{width:42px; height:42px}
    .brand .name{font-size:1.3rem}
    .nav-links{display:flex; gap:18px}
    .nav-links a{padding:8px 14px; border-radius:10px; transition:.2s; font-weight:600}
    .nav-links a:hover{background:rgba(255,255,255,0.08)}
    .cta-btn{
      background:linear-gradient(135deg,var(--accent),#7b2cbf); color:#fff;
      padding:10px 18px; border-radius:12px; font-weight:700; box-shadow:var(--shadow);
    }
    /* Hero */
    .hero{
      position:relative; overflow:hidden;
      border-bottom:1px solid rgba(255,255,255,0.08);
      padding:48px 0 36px;
    }
    .hero-grid{
      display:grid; grid-template-columns:1.1fr .9fr; gap:28px; align-items:center;
    }
    .hero h1{font-size:2.2rem; margin:0 0 10px}
    .hero p{color:var(--muted); margin:0 0 18px}
    .badge{
      display:inline-flex; align-items:center; gap:8px;
      background:rgba(76,201,240,0.12); border:1px solid rgba(76,201,240,0.35);
      color:#c8f6ff; padding:8px 12px; border-radius:999px; font-weight:700; margin-bottom:14px;
    }
    .hero-actions{display:flex; gap:12px; flex-wrap:wrap; margin-top:10px}
    .btn{
      padding:12px 18px; border-radius:12px; border:1px solid rgba(255,255,255,0.12);
      background:rgba(255,255,255,0.06); color:#fff; font-weight:700; transition:.2s;
    }
    .btn:hover{transform:translateY(-2px); border-color:rgba(255,255,255,0.25)}
    .btn.primary{background:linear-gradient(135deg,var(--brand),#3a86ff); border:none; box-shadow:var(--shadow)}
    .hero-media{
      position:relative; border-radius:18px; overflow:hidden;
      box-shadow:var(--shadow); border:1px solid rgba(255,255,255,0.1)
    }
    .hero-media img{width:100%; height:100%; object-fit:cover}
    .hero-tag{
      position:absolute; bottom:12px; left:12px;
      background:rgba(0,0,0,0.5); padding:8px 12px; border-radius:999px; font-weight:700; font-size:.95rem;
    }
    /* Sections */
    section{padding:42px 0}
    .section-head{display:flex; align-items:flex-end; justify-content:space-between; gap:14px; margin-bottom:18px}
    .section-head h2{margin:0; font-size:1.8rem}
    .section-head p{color:var(--muted); margin:8px 0 0}
    /* Cards */
    .grid{display:grid; gap:18px}
    .courses{grid-template-columns:repeat(3,1fr)}
    @media (max-width:1000px){ .hero-grid{grid-template-columns:1fr} .courses{grid-template-columns:repeat(2,1fr)} }
    @media (max-width:680px){ .courses{grid-template-columns:1fr} }
    .card{
      background:linear-gradient(180deg,#11182c 0%, #0f172a 100%);
      border:1px solid rgba(255,255,255,0.08);
      border-radius:var(--radius); overflow:hidden; box-shadow:var(--shadow);
    }
    .card-media{height:160px; overflow:hidden}
    .card-media img{width:100%; height:100%; object-fit:cover}
    .card-body{padding:16px}
    .price{display:flex; align-items:center; gap:8px; font-weight:800; color:#c8f6ff}
    .price small{color:var(--muted); font-weight:700}
    .meta{display:flex; gap:10px; flex-wrap:wrap; margin:10px 0}
    .chip{
      font-size:.85rem; padding:6px 10px; border-radius:999px;
      background:rgba(255,255,255,0.06); border:1px solid rgba(255,255,255,0.12);
      color:#cbd5e1; font-weight:700;
    }
    .card-actions{display:flex; gap:10px; margin-top:12px}
    .enroll{background:linear-gradient(135deg,#00d4ff,#00a8ff); color:#001018}
    .outline{background:transparent; border:1px solid rgba(255,255,255,0.16)}
    /* Partners */
    .partners{grid-template-columns:repeat(4,1fr)}
    @media (max-width:900px){ .partners{grid-template-columns:repeat(2,1fr)} }
    .partner{
      background:rgba(255,255,255,0.06); border:1px solid rgba(255,255,255,0.12);
      border-radius:16px; padding:14px; display:flex; align-items:center; gap:12px;
    }
    .partner-logo{
      width:48px; height:48px; border-radius:12px; overflow:hidden; background:#fff; display:flex; align-items:center; justify-content:center;
    }
    .partner-logo img{width:100%; height:100%; object-fit:contain}
    /* CTA band */
    .cta-band{
      background:linear-gradient(135deg, rgba(76,201,240,0.18), rgba(247,37,133,0.18));
      border:1px solid rgba(255,255,255,0.12);
      border-radius:18px; padding:18px; display:flex; align-items:center; justify-content:space-between; gap:14px;
    }
    @media (max-width:720px){ .cta-band{flex-direction:column; align-items:flex-start} }
    /* Footer */
    footer{
      border-top:1px solid rgba(255,255,255,0.08);
      padding:26px 0 42px; color:#cbd5e1;
    }
    .foot{
      display:grid; grid-template-columns:1.2fr .8fr .8fr; gap:18px;
    }
    @media (max-width:900px){ .foot{grid-template-columns:1fr; gap:10px} }
    .foot h3{margin:0 0 10px; color:#fff}
    .list{display:flex; flex-direction:column; gap:8px}
    .contact-item{display:flex; align-items:center; gap:10px}
    .copy{margin-top:16px; color:#94a3b8; font-size:.92rem}
    /* Simple icons (SVG inline styles) */
    .icon{width:18px; height:18px}
    /* Link style inside cards */
    .card a{color:#a5b4fc; text-decoration:none; font-weight:700}
    /* Focus */
    :focus-visible{outline:2px solid var(--brand); outline-offset:2px}
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="container nav">
      <div class="brand">
        <!-- Site logo (inline SVG) -->
        <img alt="Knowledge logo" src="data:image/svg+xml;utf8,
          <svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'>
            <defs>
              <linearGradient id='g' x1='0' y1='0' x2='1' y2='1'>
                <stop offset='0' stop-color='%234cc9f0'/>
                <stop offset='1' stop-color='%23f72585'/>
              </linearGradient>
            </defs>
            <rect x='6' y='10' width='52' height='44' rx='10' fill='url(%23g)'/>
            <path d='M18 26h28v4H18zm0 10h20v4H18z' fill='white' opacity='0.9'/>
            <circle cx='48' cy='40' r='4' fill='white'/>
          </svg>">
        <div class="name">Knowledge</div>
      </div>
      <nav class="nav-links">
        <a href="#courses">الدورات</a>
        <a href="#partners">شركاؤنا</a>
        <a href="#contact">تواصل</a>
        <a class="cta-btn" href="http://walidcourse.com" target="_blank" rel="noopener">ادخل موقعنا</a>
      </nav>
    </div>
  </header>

  <!-- Hero -->
  <section class="hero">
    <div class="container hero-grid">
      <div>
        <div class="badge">تعلم اليوم. ابدأ التغيير غدًا.</div>
        <h1>دورات احترافية تصنع مستقبلك — من عمّان إلى العالم</h1>
        <p>في Knowledge نجمع بين الخبرة العملية والأساليب الحديثة لنمنحك تعلمًا سريعًا، ممتعًا، وفعّالًا. اختر مسارك وباشر رحلة تطويرك بثقة.</p>
        <div class="hero-actions">
          <a class="btn primary" href="#courses">استكشف الدورات</a>
          <a class="btn" href="#contact">احجز استشارة مجانية</a>
        </div>
      </div>
      <div class="hero-media">
        <img alt="طلاب يتعلمون عبر التكنولوجيا في بيئة حديثة" src="https://images.unsplash.com/photo-1529070538774-1843cb3265df?q=80&w=1200&auto=format&fit=crop">
        <div class="hero-tag">عمّان، الأردن • جودة تعليم مضمونة</div>
      </div>
    </div>
  </section>

  <!-- Courses -->
  <section id="courses">
    <div class="container">
      <div class="section-head">
        <div>
          <h2>دوراتنا</h2>
          <p>اختر من باقة دورات عملية مصممة لسوق العمل في الأردن والمنطقة.</p>
        </div>
        <div class="cta-band">
          <div>
            <strong>عروض بداية السنة:</strong> خصم يصل إلى 15% على باقات متعددة.
            <div style="color:#cbd5e1; font-size:.92rem; margin-top:6px">تواصل معنا لمعرفة التفاصيل.</div>
          </div>
          <a class="btn primary" href="http://walidcourse.com" target="_blank" rel="noopener">اشترك الآن</a>
        </div>
      </div>

      <div class="grid courses">
        <!-- 1 التعليم عبر التكنولوجيا -->
        <article class="card">
          <div class="card-media">
            <img alt="التعليم عبر التكنولوجيا" src="https://images.unsplash.com/photo-1550439062-609e1531270e?q=80&w=1200&auto=format&fit=crop">
          </div>
          <div class="card-body">
            <h3>دورة التعليم عبر التكنولوجيا</h3>
            <div class="price">120 JD <small>شاملة المواد الرقمية</small></div>
            <p>اتقِ دمج الأدوات الرقمية داخل الصف أو التدريب عن بعد: منصات إدارة التعلم، تصميم محتوى تفاعلي، تقييمات ذكية، واستراتيجيات تحفيز المتعلمين.</p>
            <div class="meta">
              <span class="chip">مدة: 4 أسابيع</span>
              <span class="chip">مستوى: مبتدئ–متوسط</span>
              <span class="chip">شهادة معتمدة</span>
            </div>
            <p><strong>كلام جذاب:</strong> حوّل الحصة إلى تجربة تفاعلية تبقى في ذهن طلابك. التقنية ليست صعبة… فقط تحتاج دليلًا عمليًا.</p>
            <div class="card-actions">
              <a class="btn enroll" href="http://walidcourse.com" target="_blank" rel="noopener">سجّل الآن</a>
              <a class="btn outline" href="#contact">اسأل عن التفاصيل</a>
            </div>
          </div>
        </article>

        <!-- 2 التسويق الرقمي -->
        <article class="card">
          <div class="card-media">
            <img alt="التسويق الرقمي" src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?q=80&w=1200&auto=format&fit=crop">
          </div>
          <div class="card-body">
            <h3>دورة التسويق الرقمي</h3>
            <div class="price">150 JD <small>يشمل مشاريع عملية</small></div>
            <p>من الاستراتيجية إلى التنفيذ: إعلانات مدفوعة، تحسين محركات البحث، التسويق بالمحتوى وقياس الأداء. تعلّم كيف تبني حملة تنمو بميزانية ذكية.</p>
            <div class="meta">
              <span class="chip">مدة: 5 أسابيع</span>
              <span class="chip">مستوى: مبتدئ</span>
              <span class="chip">نماذج جاهزة</span>
            </div>
            <p><strong>كلام جذاب:</strong> اصنع حضورًا رقمياً يبيع من دون ضغط. اجعل علامتك “مرغوبة” لا “مفروضة”.</p>
            <div class="card-actions">
              <a class="btn enroll" href="http://walidcourse.com" target="_blank" rel="noopener">سجّل الآن</a>
              <a class="btn outline" href="#contact">اسأل عن التفاصيل</a>
            </div>
          </div>
        </article>

        <!-- 3 مهارات العرض والإلقاء -->
        <article class="card">
          <div class="card-media">
            <img alt="مهارات العرض والإلقاء" src="https://images.unsplash.com/photo-1523580846011-d3a5bc25702b?q=80&w=1200&auto=format&fit=crop">
          </div>
          <div class="card-body">
            <h3>دورة مهارات العرض والإلقاء</h3>
            <div class="price">90 JD <small>تمارين على المسرح</small></div>
            <p>ابن ثقة حضورك: هيكلة العروض، سرد القصص، لغة الجسد، ونبرة الصوت. تدريبات واقعية أمام الجمهور وصقل الرسالة لتصل بوضوح.</p>
            <div class="meta">
              <span class="chip">مدة: 3 أسابيع</span>
              <span class="chip">مستوى: كل المستويات</span>
              <span class="chip">تقييم أداء</span>
            </div>
            <p><strong>كلام جذاب:</strong> اجعل كلماتك تُسمَع… ويُعمل بها. الإلقاء القوي يفتح أبوابًا لا يفتحها البريد الإلكتروني.</p>
            <div class="card-actions">
              <a class="btn enroll" href="http://walidcourse.com" target="_blank" rel="noopener">سجّل الآن</a>
              <a class="btn outline" href="#contact">اسأل عن التفاصيل</a>
            </div>
          </div>
        </article>

        <!-- 4 إدارة الأعمال -->
        <article class="card">
          <div class="card-media">
            <img alt="إدارة الأعمال" src="https://images.unsplash.com/photo-1551292831-023188e78222?q=80&w=1200&auto=format&fit=crop">
          </div>
          <div class="card-body">
            <h3>دورة إدارة الأعمال</h3>
            <div class="price">200 JD <small>دراسة حالات أردنية</small></div>
            <p>أساسيات التخطيط، إدارة المشاريع، المالية المبسطة والقيادة. منهج عملي يربط النظريات بتطبيقات سوق الأردن والمنطقة.</p>
            <div class="meta">
              <span class="chip">مدة: 6 أسابيع</span>
              <span class="chip">مستوى: مبتدئ–متوسط</span>
              <span class="chip">قوالب عملية</span>
            </div>
            <p><strong>كلام جذاب:</strong> ادِر بإتقان، قرّر بثقة، ونَمِّ الأرباح بذكاء—من اليوم الأول.</p>
            <div class="card-actions">
              <a class="btn enroll" href="http://walidcourse.com" target="_blank" rel="noopener">سجّل الآن</a>
              <a class="btn outline" href="#contact">اسأل عن التفاصيل</a>
            </div>
          </div>
        </article>

        <!-- 5 البرمجة الأساسية -->
        <article class="card">
          <div class="card-media">
            <img alt="البرمجة الأساسية" src="https://images.unsplash.com/photo-1518770660439-4636190af475?q=80&w=1200&auto=format&fit=crop">
          </div>
          <div class="card-body">
            <h3>دورة البرمجة الأساسية</h3>
            <div class="price">130 JD <small>مشاريع مصغّرة</small></div>
            <p>مبادئ التفكير الخوارزمي، المتغيرات، الحلقات والدوال. تبني تطبيقات بسيطة خطوة بخطوة لتأسيس قاعدة قوية لأي تخصص تقني لاحقًا.</p>
            <div class="meta">
              <span class="chip">مدة: 4 أسابيع</span>
              <span class="chip">مستوى: مبتدئ</span>
              <span class="chip">دعم مجتمعي</span>
            </div>
            <p><strong>كلام جذاب:</strong> اكتب أول سطر كود… وستتفاجأ كيف تتغير طريقة تفكيرك للأفضل.</p>
            <div class="card-actions">
              <a class="btn enroll" href="http://walidcourse.com" target="_blank" rel="noopener">سجّل الآن</a>
              <a class="btn outline" href="#contact">اسأل عن التفاصيل</a>
            </div>
          </div>
        </article>

        <!-- 6 التصميم الجرافيكي -->
        <article class="card">
          <div class="card-media">
            <img alt="التصميم الجرافيكي" src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=1200&auto=format&fit=crop">
          </div>
          <div class="card-body">
            <h3>دورة التصميم الجرافيكي</h3>
            <div class="price">140 JD <small>يشمل ملفات عمل</small></div>
            <p>أساسيات الهوية البصرية، نظرية الألوان، التايبوغرافي وبرامج التصميم. تنتهي بمشروع محفظة يعرض أعمالك باحتراف.</p>
            <div class="meta">
              <span class="chip">مدة: 4 أسابيع</span>
              <span class="chip">مستوى: مبتدئ–متوسط</span>
              <span class="chip">مراجعات أعمال</span>
            </div>
            <p><strong>كلام جذاب:</strong> صِمّم هوية تترك أثرًا قبل أن يتكلم محتواك. الجمال يوصل الرسالة أسرع.</p>
            <div class="card-actions">
              <a class="btn enroll" href="http://walidcourse.com" target="_blank" rel="noopener">سجّل الآن</a>
              <a class="btn outline" href="#contact">اسأل عن التفاصيل</a>
            </div>
          </div>
        </article>
      </div>
    </div>
  </section>

  <!-- Partners -->
  <section id="partners">
    <div class="container">
      <div class="section-head">
        <div>
          <h2>شركاؤنا</h2>
          <p>نفتخر بالتعاون مع مؤسسات تعليمية مرموقة لتعزيز مصداقيتنا وجودة محتوانا.</p>
        </div>
      </div>

      <div class="grid partners">
        <!-- جامعة عمان الأهلية (شعار توضيحي مبسّط) -->
        <div class="partner">
          <div class="partner-logo">
            <img alt="شعار توضيحي لجامعة عمان الأهلية" src="data:image/svg+xml;utf8,
              <svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'>
                <rect x='4' y='8' width='56' height='48' rx='8' fill='%23005f73'/>
                <circle cx='32' cy='30' r='14' fill='%23ffd166'/>
                <path d='M20 44h24' stroke='white' stroke-width='3' stroke-linecap='round'/>
              </svg>">
          </div>
          <div>
            <strong>جامعة عمان الأهلية</strong>
            <div style="color:#94a3b8; font-size:.92rem">شراكة أكاديمية لتعزيز المعايير التعليمية</div>
          </div>
        </div>

        <!-- جامعة البترا (شعار توضيحي مبسّط) -->
        <div class="partner">
          <div class="partner-logo">
            <img alt="شعار توضيحي لجامعة البترا" src="data:image/svg+xml;utf8,
              <svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'>
                <rect x='4' y='8' width='56' height='48' rx='8' fill='%237b2cbf'/>
                <path d='M16 44l16-24 16 24' stroke='white' stroke-width='3' fill='none' stroke-linecap='round'/>
                <circle cx='32' cy='28' r='6' fill='%23ffd6e0'/>
              </svg>">
          </div>
          <div>
            <strong>جامعة البترا</strong>
            <div style="color:#94a3b8; font-size:.92rem">تعاون معرفي ودعم لأنشطة الطلاب</div>
          </div>
        </div>

        <!-- شركاء إضافيون (نماذج) -->
        <div class="partner">
          <div class="partner-logo">
            <img alt="شعار شريك تدريبي" src="data:image/svg+xml;utf8,
              <svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'>
                <rect x='4' y='8' width='56' height='48' rx='8' fill='%233a86ff'/>
                <rect x='18' y='22' width='28' height='20' rx='6' fill='white'/>
              </svg>">
          </div>
          <div>
            <strong>مركز تدريب محترف</strong>
            <div style="color:#94a3b8; font-size:.92rem">ورش عمل متقدمة وشهادات مشاركة</div>
          </div>
        </div>

        <div class="partner">
          <div class="partner-logo">
            <img alt="شعار منصة تقنية" src="data:image/svg+xml;utf8,
              <svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'>
                <rect x='4' y='8' width='56' height='48' rx='8' fill='%23f72585'/>
                <circle cx='24' cy='32' r='10' fill='white'/>
                <circle cx='44' cy='32' r='10' fill='white' opacity='0.7'/>
              </svg>">
          </div>
          <div>
            <strong>منصة تقنية تعليمية</strong>
            <div style="color:#94a3b8; font-size:.92rem">مواد رقمية ومتابعة تعلم إلكتروني</div>
          </div>
        </div>
      </div>

      <div style="margin-top:16px; color:#9aa7b6; font-size:.92rem">
        ملاحظة: الشعارات هنا توضيحية. عند الإطلاق الرسمي يمكن استبدالها بالشعارات المعتمدة من الشركاء بعد موافقة الجهات المعنية.
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <div class="container">
      <div class="section-head">
        <div>
          <h2>تواصل معنا</h2>
          <p>نحن هنا لنساعدك في اختيار الدورة الأنسب لأهدافك.</p>
        </div>
      </div>

      <div class="foot">
        <div>
          <h3>Knowledge — عمّان، الأردن</h3>
          <div class="list">
            <div class="contact-item">
              <svg class="icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="#a5b4fc" d="M12 2C8.13 2 5 5.13 5 9c0 6.33 7 13 7 13s7-6.67 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5S10.62 6.5 12 6.5s2.5 1.12 2.5 2.5S13.38 11.5 12 11.5z"/></svg>
              عمّان — الأردن
            </div>
            <div class="contact-item">
              <svg class="icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="#a5b4fc" d="M6.62 10.79a15.053 15.053 0 006.59 6.59l2.2-2.2a1 1 0 011.06-.24c1.12.37 2.33.57 3.53.57a1 1 0 011 1v3.5a1 1 0 01-1 1C10.4 22 2 13.6 2 3.5a1 1 0 011-1H6.5a1 1 0 011 1c0 1.2.2 2.41.57 3.53a1 1 0 01-.24 1.06l-2.21 2.2z"/></svg>
              0781403097
            </div>
            <div class="contact-item">
              <svg class="icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="#a5b4fc" d="M2 6a2 2 0 012-2h16a2 2 0 012 2v.01L12 13 2 6.01V6zm0 3.24l10 6.25 10-6.25V18a2 2 0 01-2 2H4a2 2 0 01-2-2V9.24z"/></svg>
              vxq204@gmail.com
            </div>
            <div class="contact-item">
              <svg class="icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="#a5b4fc" d="M10.9 2.1a1 1 0 011.2 0l8 6A1 1 0 0120 9H4a1 1 0 01-.6-1.9l7.5-5zM4 11h16v9a2 2 0 01-2 2H6a2 2 0 01-2-2v-9z"/></svg>
              <a href="http://walidcourse.com" target="_blank" rel="noopener">www.walidcourse.com</a>
            </div>
          </div>
        </div>

        <div>
          <h3>مواعيد العمل</h3>
          <div class="list">
            <div>الأحد – الخميس: 9 صباحًا – 6 مساءً</div>
            <div>الجمعة: مغلق</div>
            <div>الدعم عبر البريد: 24/7</div>
          </div>
        </div>

        <div>
          <h3>روابط سريعة</h3>
          <div class="list">
            <a href="#courses">الدورات</a>
            <a href="#partners">الشركاء</a>
            <a href="#contact">تواصل</a>
            <a href="http://walidcourse.com" target="_blank" rel="noopener">اشترك أونلاين</a>
          </div>
        </div>
      </div>

      <div class="copy">© 2026 Knowledge — جميع الحقوق محفوظة. عمّان، الأردن.</div>
    </div>
  </section>

  <!-- Floating enroll button -->
  <a aria-label="سجّل الآن" href="http://walidcourse.com" target="_blank" rel="noopener"
     style="position:fixed; inset-inline-start:16px; bottom:16px; background:linear-gradient(135deg,#00d4ff,#00a8ff); color:#001018; padding:12px 16px; border-radius:999px; font-weight:800; box-shadow:0 12px 24px rgba(0,0,0,0.35); border:1px solid rgba(255,255,255,0.2);">
    سجّل الآن
  </a>

</body>
</html>

