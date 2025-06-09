<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>hidden</title>
  <style>
    body {
      background-color: #000;
      color: #fff;
      font-family: 'Courier New', Courier, monospace;
      padding: 2em;
      transition: opacity 2s ease-out;
    }
    .faint {
      color: #999;
      font-size: 0.9em;
    }
    .secret {
      color: #111; /* 暗号っぽい色で目立たない */
    }
  </style>
  <script>
    setTimeout(() => {
      document.body.style.opacity = 0; // フェードアウト
    }, 14000);

    setTimeout(() => {
      window.close(); // 一部ブラウザでは効果なし
    }, 15000);
  </script>
</head>

<body onload="console.log('hidden.html loaded')">
  <h2>……ここまで読んでくれてありがとう。</h2>
  <p>
    　でも、もう遅いよね。<br>
    　あのとき、わたしは気づいてた。<br>
    　誰が、わたしを……。
  </p>

  <p>
    　お願い。もしこれを見つけてくれたなら、<br>
    　わたしがなぜ、こんな最後を迎えたのかを知ってほしい。<br>
    　そして、<span class="secret">カナエ</span>を……止めて。
  </p>

  <p class="faint">（このページはすぐに閉じるかもしれない）</p>
</body>
</html>
