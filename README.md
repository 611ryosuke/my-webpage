# my-webpage

<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cafe Time | 懐かしい喫茶店</title>
  <link rel="stylesheet" href="style.css">
  <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+JP:wght@400;600;700&display=swap" rel="stylesheet">
</head>
<body>

  <header>
    <div class="logo">☕ Cafe Time</div>
    <nav>
      <a href="#home">HOME</a
      <a href="#about">ABOUT</a>
      <a href="#menu">MENU</a>
      <a href="#access">ACCESS</a>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="hero-content">
        <p class="sub-title">A LITTLE MOMENT OF HAPPINESS</p>
        <h1>懐かしい時間を、<br>ここで。</h1>
        <p>ゆっくり流れる時間と、香ばしいコーヒー。</p>
        <a href="#menu" class="btn">MENUを見る</a>
      </div>
    </section>

    <section class="about section" id="about">
      <p class="section-label">ABOUT OUR CAFE</p>
      <h2>いつもの日常に、<br>小さな休息を。</h2>
      <div class="about-content">
        <img src="https://images.unsplash.com/photo-1442512595331-e89e73853f31?w=900" alt="コーヒーを淹れる様子">
        <div>
          <p>
            Cafe Timeは、どこか懐かしい雰囲気が漂う
            小さな喫茶店です。
          </p>
          <p>
            丁寧に淹れたコーヒーと、手作りのスイーツ。
            忙しい毎日を少しだけ忘れて、
            心安らぐひとときをお過ごしください。
          </p>
        </div>
      </div>
    </section>

    <section class="menu section" id="menu">
      <p class="section-label">OUR MENU</p>
      <h2>おすすめメニュー</h2>

      <div class="menu-list">
        <article class="menu-card">
          <img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93?w=700" alt="コーヒー">
          <h3>ブレンドコーヒー</h3>
          <p>深い香りとコクを楽しむ一杯。</p>
          <span>¥550</span>
        </article>

        <article class="menu-card">
          <img src="https://images.unsplash.com/photo-1572490122747-3968b75cc699?w=700" alt="クリームソーダ">
          <h3>クリームソーダ</h3>
          <p>昔ながらの懐かしい味わい。</p>
          <span>¥650</span>
        </article>

        <article class="menu-card">
          <img src="https://images.unsplash.com/photo-1551024506-0bccd828d307?w=700" alt="ドーナツ">
          <h3>自家製スイーツ</h3>
          <p>コーヒーにぴったりの甘いひととき。</p>
          <span>¥480</span>
        </article>
      </div>
    </section>

    <section class="message section">
      <p>— Take a break —</p>
      <h2>今日も、いい一日になりますように。</h2>
    </section>

    <section class="access section" id="access">
      <p class="section-label">ACCESS</p>
      <h2>店舗情報</h2>
      <div class="access-box">
        <p><strong>店名：</strong>Cafe Time</p>
        <p><strong>住所：</strong>福島県○○市○○町 1-2-3</p>
        <p><strong>営業時間：</strong>10:00 ～ 19:00</p>
        <p><strong>定休日：</strong>毎週水曜日</p>
      </div>
    </section>
  </main>

  <footer>
    <p>☕ Cafe Time</p>
    <small>© 2026 Cafe Time. All Rights Reserved.</small>
  </footer>

  <script src="script.js"></script>
</body>
</html>

/* 基本設定 */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

body {
  background-color: #f3ead8;
  color: #493324;
  font-family: 'Noto Serif JP', serif;
  line-height: 1.9;
}

/* ヘッダー */
header {
  background: #4b3023;
  color: #f3ead8;
  padding: 15px 8%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 4px double #c49a6c;
}

.logo {
  font-size: 25px;
  font-weight: bold;
  letter-spacing: 2px;
}

nav {
  display: flex;
  gap: 25px;
}

nav a {
  color: #f3ead8;
  text-decoration: none;
  font-size: 13px;
  letter-spacing: 2px;
  transition: 0.3s;
}

nav a:hover {
  color: #d9a66b;
}

/* メインビジュアル */
.hero {
  height: 620px;
  background:
    linear-gradient(rgba(35, 21, 13, 0.48), rgba(35, 21, 13, 0.48)),
    url("https://images.unsplash.com/photo-1445116572660-236099ec97a0?w=1800")
    center/cover;
  display: flex;
  align-items: center;
  padding: 0 10%;
  color: #fff3df;
}

.hero-content {
  border-left: 3px solid #d9a66b;
  padding-left: 35px;
}

.sub-title {
  letter-spacing: 4px;
  font-size: 12px;
  margin-bottom: 20px;
}

.hero h1 {
  font-size: clamp(34px, 6vw, 60px);
  line-height: 1.6;
  margin-bottom: 20px;
}

.hero-content p {
  margin-bottom: 25px;
}

.btn {
  display: inline-block;
  padding: 10px 35px;
  border: 1px solid #e4c49a;
  color: white;
  text-decoration: none;
  transition: 0.3s;
}

.btn:hover {
  background: #a45e38;
}

/* 共通セクション */
.section {
  padding: 100px 10%;
  text-align: center;
}

.section-label {
  color: #a45e38;
  font-size: 12px;
  letter-spacing: 4px;
  margin-bottom: 10px;
}

.section h2 {
  font-size: 32px;
  margin-bottom: 45px;
}

/* ABOUT */
.about-content {
  display: flex;
  align-items: center;
  gap: 50px;
  max-width: 900px;
  margin: auto;
  text-align: left;
}

.about-content img {
  width: 50%;
  border: 8px solid #fff9ed;
  box-shadow: 5px 5px 0 #b68c62;
}

.about-content div {
  flex: 1;
}

.about-content p {
  margin-bottom: 20px;
}

/* MENU */
.menu {
  background: #e7d8bf;
  border-top: 1px solid #c4a47d;
  border-bottom: 1px solid #c4a47d;
}

.menu-list {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 30px;
  max-width: 1000px;
  margin: auto;
}

.menu-card {
  background: #f8f0e1;
  padding: 15px 15px 25px;
  border: 1px solid #c4a47d;
  transition: 0.3s;
}

.menu-card:hover {
  transform: translateY(-8px);
  box-shadow: 5px 8px 15px #9b795744;
}

.menu-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.menu-card h3 {
  margin-top: 15px;
  font-size: 18px;
}

.menu-card p {
  font-size: 13px;
  margin: 10px 0;
}

.menu-card span {
  color: #a45e38;
  font-weight: bold;
}

/* メッセージ */
.message {
  background: #593b2b;
  color: #f3ead8;
  padding: 80px 20px;
}

.message p {
  color: #d9a66b;
  letter-spacing: 4px;
}

.message h2 {
  margin: 20px 0 0;
  font-size: 27px;
}

/* ACCESS */
.access-box {
  max-width: 550px;
  margin: auto;
  padding: 35px;
  border: 2px solid #9c7957;
  outline: 1px solid #9c7957;
  outline-offset: 6px;
  text-align: left;
  background: #f8f0e1;
}

/* フッター */
footer {
  background: #38251b;
  color: #f3ead8;
  text-align: center;
  padding: 35px;
}

footer p {
  font-size: 24px;
  margin-bottom: 10px;
}

footer small {
  font-size: 11px;
  color: #c5a98a;
}

/* スマホ対応 */
@media (max-width: 700px) {
  header {
    flex-direction: column;
    gap: 12px;
  }

  nav {
    gap: 15px;
  }

  nav a {
    font-size: 11px;
  }

  .hero {
    height: 500px;
    padding: 0 7%;
  }

  .section {
    padding: 70px 7%;
  }

  .about-content {
    flex-direction: column;
    gap: 25px;
  }

  .about-content img {
    width: 100%;
  }

  .menu-list {
    grid-template-columns: 1fr;
  }

  .section h2 {
    font-size: 25px;
  }
}

// ページ読み込み時のアニメーション
document.addEventListener("DOMContentLoaded", () => {

  const sections = document.querySelectorAll(".section");

  const observer = new IntersectionObserver((entries) => {
    entries.forEach((entry) => {
      if (entry.isIntersecting) {
        entry.target.classList.add("show");
        observer.unobserve(entry.target);
      }
    });
  }, {
    threshold: 0.15
  });

  sections.forEach((section) => {
    section.classList.add("fade-in");
    observer.observe(section);
  });

});
