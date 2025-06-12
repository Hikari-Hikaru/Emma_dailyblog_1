<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>2025年4月5日 - </title>
  <link rel="stylesheet" href="../style.css">
  <style>
    body {
      background-color: #ffe4e1;
      font-family: "Helvetica Neue", sans-serif;
      color: #333;
    }

    header {
      text-align: center;
      margin-top: 40px;
    }

    header h1 {
      font-family: 'Courier New', Courier, monospace;
      font-size: 2.5em;
      color: #ff69b4;
      letter-spacing: 0.1em;
      text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
    }

    header h2 {
      font-size: 0.9em;
      color: #999;
      margin-top: -10px;
    }

    .secret-link {
      color: #ffe4e1;
      text-decoration: none;
      cursor: pointer;
      animation: blink 1.2s infinite;
    }

    .secret-link:hover {
      color: red;
    }

    @keyframes blink {
      0%, 100% { color: #ffe4e1; }
      50% { color: #ff69b4; }
    }

    #please-message {
      display: flex;
      justify-content: center;
      gap: 5px;
      margin-top: 30px;
    }

    .letter {
      font-size: 1.5em;
      color: #cc0000;
      opacity: 0;
      transform: translateY(-20px) rotate(0deg);
      animation: glitchDrop 0.8s ease-in-out forwards;
    }

    @keyframes glitchDrop {
      0% {
        opacity: 0;
        transform: translateY(-20px) rotate(0deg);
      }
      50% {
        opacity: 1;
        transform: translateY(5px) rotate(10deg);
      }
      100% {
        transform: translateY(0px) rotate(-2deg);
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>2025_04_05</h1>
    <h2>Not everything is what it seems.</h2>
  </header>

  <main>
    <p>
      Today was the entrance ceremony for high school.<br>
      I was born in Japan, but since my parents grew up in U.S.A.,<br><br>
      I stood out in a strange way from the perspective of Japanese people,<br>
      and it was a bit embarrassing.<br><br>
      I even saw a tiny pink dot on the page. Maybe it's nothing.

      <!-- ▼ 秘密のリンク（点滅ドット） -->
      <a href="#" class="secret-link" id="secretDot">.</a>
    </p>

    <!-- ▼ 崩れる「Please...」メッセージ -->
    <div id="please-message"></div>
  </main>

  <!-- ▼ 日付別リンク ▼ -->
  <h2>ブログ一覧</h2>
  <ul>
    <li><a href="https://hikari-hikaru.github.io/Emma_dailyblog_2/">（dairy2ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_3/">（dairy3ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_4/">（dairy4ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_5/">（dairy5ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_6/">（dairy6ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_7/">（dairy7ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_8/">（dairy8ページ）</a></li>
  </ul>
  <script>
    document.getElementById("secretDot").addEventListener("click", function(event) {
      event.preventDefault();

      const container = document.getElementById("please-message");

      if (container.childElementCount === 0) {
        const text = "Please...";
        text.split("").forEach((char, index) => {
          const span = document.createElement("span");
          span.className = "letter";
          span.style.animationDelay = `${index * 0.1}s`;
          span.textContent = char;
          container.appendChild(span);
        });

        setTimeout(() => {
          window.location.href = "https://hikari-hikaru.github.io/thanks/";
        }, 2200); // 約2秒後に遷移
      }
    });
  </script>
</body>
</html>
