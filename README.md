<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>TinyHost — Разработка и поддержка сайтов</title>
  <meta name="description" content="Разработка и поддержка сайтов, доменов, SSL, DNS, автоматизация. Сопровождение и администрирование." />
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --accent:#06b6d4;
      --muted:#9aa4b2;
      --glass: rgba(255,255,255,0.03);
      color-scheme: dark;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background:linear-gradient(180deg,#071028 0%, #0f1724 100%);
      color:#e6eef6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
      padding:32px;
    }
    .container{max-width:980px;margin:0 auto;}
    header{display:flex;align-items:center;justify-content:space-between;gap:16px;margin-bottom:28px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{
      width:56px;height:56px;border-radius:10px;
      background:linear-gradient(135deg,var(--accent),#7c3aed);
      display:flex;align-items:center;justify-content:center;font-weight:700;color:#041022;
      box-shadow:0 6px 18px rgba(6,182,212,0.08), inset 0 -4px 10px rgba(255,255,255,0.05);
      font-size:20px;
    }
    h1{margin:0;font-size:28px}
    p.lead{color:var(--muted);margin:6px 0 0;font-size:15px}
    .hero{
      background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
      border-radius:12px;padding:28px;margin-bottom:20px;box-shadow:0 4px 30px rgba(2,6,23,0.6);
      display:flex;gap:20px;align-items:center;
    }
    .hero .left{flex:1}
    .hero .right{width:220px;text-align:right}
    .cta{
      display:inline-block;background:var(--accent);color:#041022;padding:12px 18px;border-radius:10px;font-weight:600;text-decoration:none;
      box-shadow:0 8px 24px rgba(6,182,212,0.12);
    }
    .services{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:14px;margin:18px 0 28px}
    .card{
      background:var(--card);padding:16px;border-radius:10px;border:1px solid rgba(255,255,255,0.03);
      box-shadow:0 6px 18px rgba(2,6,23,0.6);
    }
    .card h3{margin:0 0 8px;font-size:16px}
    .muted{color:var(--muted);font-size:14px}
    footer{margin-top:28px;text-align:center;color:var(--muted);font-size:13px}
    .features{display:flex;flex-direction:column;gap:10px;margin-top:12px}
    .feature{display:flex;gap:12px;align-items:flex-start}
    .feature svg{flex:0 0 34px}
    .contact{display:flex;gap:12px;flex-wrap:wrap;justify-content:flex-start;margin-top:14px}
    .btn{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:10px 14px;border-radius:8px;color:var(--muted);text-decoration:none;font-weight:600}
    .btn-primary{background:var(--accent);color:#041022;border:none}
    .small-muted{color:var(--muted);font-size:13px;margin-top:8px}
    @media (max-width:640px){
      .hero{flex-direction:column;align-items:flex-start}
      .hero .right{text-align:left;width:100%}
      header{flex-direction:column;align-items:flex-start;gap:8px}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">TH</div>
        <div>
          <h1>TinyHost</h1>
          <p class="lead">Разработка и поддержка сайтов · Домены · SSL · DNS · Автоматизация</p>
        </div>
      </div>
      <nav style="display:flex;gap:8px;align-items:center">
        <!-- Вставь свой email/телефон в href -->
        <a class="btn" href="mailto:youremail@example.com">youremail@example.com</a>
        <a class="btn btn-primary" href="tel:+7XXXXXXXXXX">+7 XXX XXX XXXX</a>
      </nav>
    </header>

    <section class="hero">
      <div class="left">
        <h2 style="margin:0 0 8px">Помогаем запустить и поддерживать ваш сайт — без забот</h2>
        <p class="muted">Нужна настройка хостинга, миграция сайта, регистрация домена, выставление SSL или автоматизация процессов — мы сделаем быстро и надёжно.</p>

        <div class="contact">
          <a class="cta" href="mailto:youremail@example.com?subject=За%20хостинг%20и%20поддержку">Заказать поддержку</a>
          <a class="btn" href="#services">Услуги</a>
          <a class="btn" href="#contact">Контакты</a>
        </div>

        <div class="small-muted">Готовы к удалённой работе. Uralsk, Kazakhstan — Open to Remote Opportunities</div>
      </div>

      <div class="right">
        <!-- Небольшая витрина услуг -->
        <div class="card">
          <h3>Быстрое сопровождение</h3>
          <div class="muted">24/7 мониторинг, аварийное восстановление, бэкапы и обновления.</div>
          <div style="height:10px"></div>
          <h3>Хостинг и домены</h3>
          <div class="muted">Регистрация доменов, DNS, transfer, WHOIS и настройка email.</div>
        </div>
      </div>
    </section>

    <section id="services">
      <h2 style="margin:0 0 10px">Наши услуги</h2>
      <div class="services">
        <div class="card">
          <h3>Разработка и развертывание сайтов</h3>
          <div class="muted">Landing, WordPress, CMS, оптимизация производительности.</div>
        </div>

        <div class="card">
          <h3>Хостинг и управление серверами</h3>
          <div class="muted">Установка и администрирование Linux, Plesk/cPanel, VPS, миграции.</div>
        </div>

        <div class="card">
          <h3>Домены, DNS и SSL</h3>
          <div class="muted">Регистрация доменов, настройка DNS, установка и продление SSL-сертификатов.</div>
        </div>

        <div class="card">
          <h3>Автоматизация и скрипты</h3>
          <div class="muted">Автоматизация бэкапов, деплой, мониторинг и отчётность.</div>
        </div>

        <div class="card">
          <h3>Техническая поддержка</h3>
          <div class="muted">Сопровождение сайтов: исправление ошибок, восстановление, оптимизация.</div>
        </div>

        <div class="card">
          <h3>Консалтинг и миграции</h3>
          <div class="muted">Помогаем переехать на другой хостинг или в облако без потерь данных.</div>
        </div>
      </div>
    </section>

    <section id="about" style="margin-top:6px">
      <h2 style="margin:0 0 10px">Почему мы</h2>
      <div class="card">
        <div class="features">
          <div class="feature">
            <svg width="34" height="34" viewBox="0 0 24 24" fill="none" aria-hidden>
              <rect x="1" y="1" width="22" height="22" rx="5" stroke="rgba(255,255,255,0.06)" stroke-width="1.5" fill="rgba(255,255,255,0.02)"></rect>
              <path d="M7 12l3 3 7-7" stroke="white" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"></path>
            </svg>
            <div>
              <strong>Надёжность</strong>
              <div class="muted">Резервные копии, мониторинг и быстрый отклик при проблемах.</div>
            </div>
          </div>

          <div class="feature">
            <svg width="34" height="34" viewBox="0 0 24 24" fill="none" aria-hidden>
              <rect x="1" y="1" width="22" height="22" rx="5" stroke="rgba(255,255,255,0.06)" stroke-width="1.5" fill="rgba(255,255,255,0.02)"></rect>
              <path d="M8 12h8M8 16h5M8 8h10" stroke="white" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"></path>
            </svg>
            <div>
              <strong>Прозрачные условия</strong>
              <div class="muted">Чёткие тарифы и оплата за результат — без скрытых платежей.</div>
            </div>
          </div>

          <div class="feature">
            <svg width="34" height="34" viewBox="0 0 24 24" fill="none" aria-hidden>
              <rect x="1" y="1" width="22" height="22" rx="5" stroke="rgba(255,255,255,0.06)" stroke-width="1.5" fill="rgba(255,255,255,0.02)"></rect>
              <path d="M12 5v14M5 12h14" stroke="white" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"></path>
            </svg>
            <div>
              <strong>Автоматизация</strong>
              <div class="muted">Настроим процессы раз и навсегда — чтобы вы платили меньше за поддержку.</div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="contact" style="margin-top:18px">
      <h2 style="margin:0 0 10px">Контакты</h2>
      <div class="card" style="display:flex;flex-direction:column;gap:10px">
        <div class="muted">Заполните email/телефон в шапке. Ниже — быстрые способы связи:</div>

        <div style="display:flex;gap:8px;flex-wrap:wrap">
          <a class="btn" href="mailto:youremail@example.com?subject=Запрос%20поддержки">Написать на почту</a>
          <a class="btn" href="tel:+7XXXXXXXXXX">Позвонить</a>
          <a class="btn" href="https://t.me/yourtelegram" target="_blank">Telegram</a>
        </div>

        <div class="muted">Работаем с малыми и средними бизнесами, индивидуальными предпринимателями и личными проектами. Готовы к разовым и долгосрочным договорам сопровождения.</div>
      </div>
    </section>

    <footer>
      <div>© <strong>TinyHost</strong> — Услуги по серверам и сайтам • Uralsk, Kazakhstan</div>
      <div style="margin-top:6px" class="muted">Сделано с заботой. Готов помочь с переносом сайта на GitHub Pages или настройкой бесплатной панели.</div>
    </footer>
  </div>
</body>
</html>
