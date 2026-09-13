<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Home Page</title>
  <style>
    :root {
      --card: #ffffff;
      --text: #2b2f38;
      --muted: #6b7280;
      --accent: #fb7299;          /* B 站粉 */
      --accent-dark: #f25c87;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 24px;
      background: linear-gradient(135deg, #eef2ff, #fdf2f8);
      font-family: system-ui, -apple-system, "Segoe UI", "Microsoft YaHei", sans-serif;
      color: var(--text);
    }

    .card {
      width: 100%;
      max-width: 560px;
      background: var(--card);
      border-radius: 20px;
      padding: 36px 28px 40px;
      text-align: center;
      box-shadow: 0 12px 40px rgba(31, 41, 55, .12);
    }

    h1 {
      margin: 0 0 8px;
      font-size: clamp(1.6rem, 5vw, 2.2rem);
      letter-spacing: .5px;
    }

    .subtitle {
      margin: 0 0 28px;
      color: var(--muted);
      font-size: .95rem;
    }

    .avatar {
      display: block;
      margin: 0 auto 32px;
      width: 180px;
      height: 180px;
      max-width: 60vw;
      max-height: 60vw;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid #fff;
      box-shadow: 0 8px 24px rgba(251, 114, 153, .35);
    }

    .section-title {
      margin: 0 0 20px;
      font-weight: 700;
      font-size: 1.05rem;
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 2px;
    }

    .link {
      display: inline-block;
      padding: 12px 32px;
      border-radius: 999px;
      background: var(--accent);
      color: #fff;
      text-decoration: none;
      font-weight: 600;
      box-shadow: 0 6px 16px rgba(251, 114, 153, .4);
      transition: transform .15s ease, box-shadow .15s ease, background .15s ease;
    }

    .link:hover {
      background: var(--accent-dark);
      transform: translateY(-2px);
      box-shadow: 0 10px 22px rgba(251, 114, 153, .5);
    }

    .link:active { transform: translateY(0); }

    /* 尊重用户的“减少动画”偏好 */
    @media (prefers-reduced-motion: reduce) {
      .link { transition: none; }
      .link:hover { transform: none; }
    }
  </style>
</head>
<body>
  <main class="card">
    <h1>Hello my friend! 👋</h1>
    <p class="subtitle">欢迎来到我的主页</p>

    <img class="avatar"
         src="https://cdn.luogu.com.cn/upload/usericon/1315217.png"
         alt="我的头像"
         loading="lazy">

    <p class="section-title">Some webpage</p>

    <a class="link"
       href="https://www.bilibili.com"
       target="_blank"
       rel="noopener noreferrer">前往 Bilibili</a>
  </main>
</body>
</html>
