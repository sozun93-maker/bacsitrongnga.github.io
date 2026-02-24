<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vì Sao Ung Thư Sớm Đường Tiêu Hóa Dễ Bị Bỏ Sót?</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;0,900;1,700&family=Lora:ital@0;1&family=Be+Vietnam+Pro:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --ink: #1a1208;
    --warm-bg: #fdf8f0;
    --paper: #fff9f0;
    --sienna: #b8450a;
    --sienna-light: #e8632a;
    --teal: #0a6b5e;
    --teal-light: #13a898;
    --gold: #c8922a;
    --muted: #6b5e4e;
    --border: #e8ddd0;
    --highlight: #fff3e0;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'Be Vietnam Pro', sans-serif;
    background: var(--warm-bg);
    color: var(--ink);
    line-height: 1.7;
  }

  /* ---- HERO ---- */
  .hero {
    background: var(--ink);
    min-height: 92vh;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    padding: 60px 48px 56px;
    position: relative;
    overflow: hidden;
  }

  .hero::before {
    content: '';
    position: absolute;
    inset: 0;
    background:
      radial-gradient(ellipse 80% 60% at 30% 20%, rgba(184,69,10,0.18) 0%, transparent 60%),
      radial-gradient(ellipse 60% 80% at 80% 80%, rgba(10,107,94,0.15) 0%, transparent 60%);
  }

  .hero-tag {
    font-size: 0.7rem;
    font-weight: 600;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 24px;
    position: relative;
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .hero-tag::before {
    content: '';
    display: block;
    width: 32px;
    height: 1px;
    background: var(--gold);
  }

  .hero h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2.4rem, 5.5vw, 4.2rem);
    font-weight: 900;
    color: #fff;
    line-height: 1.08;
    letter-spacing: -0.02em;
    max-width: 820px;
    position: relative;
    margin-bottom: 28px;
  }

  .hero h1 em {
    font-style: italic;
    color: var(--sienna-light);
  }

  .hero-sub {
    font-size: 1.05rem;
    color: rgba(255,255,255,0.65);
    max-width: 560px;
    position: relative;
    font-weight: 300;
    margin-bottom: 40px;
  }

  .hero-meta {
    display: flex;
    align-items: center;
    gap: 20px;
    position: relative;
  }

  .author-chip {
    display: flex;
    align-items: center;
    gap: 10px;
    background: rgba(255,255,255,0.08);
    border: 1px solid rgba(255,255,255,0.15);
    border-radius: 999px;
    padding: 8px 16px 8px 8px;
  }

  .author-avatar {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    background: linear-gradient(135deg, var(--teal), var(--sienna));
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.9rem;
  }

  .author-chip span {
    font-size: 0.8rem;
    color: rgba(255,255,255,0.75);
    font-weight: 500;
  }

  .read-time {
    font-size: 0.78rem;
    color: rgba(255,255,255,0.4);
    letter-spacing: 0.05em;
  }

  /* ---- ORNAMENT ---- */
  .ornament {
    text-align: center;
    padding: 40px 0 0;
    color: var(--gold);
    font-size: 1.2rem;
    letter-spacing: 0.5em;
    opacity: 0.5;
  }

  /* ---- ARTICLE BODY ---- */
  .article {
    max-width: 720px;
    margin: 0 auto;
    padding: 48px 24px 80px;
  }

  .lead {
    font-family: 'Lora', serif;
    font-size: 1.22rem;
    color: var(--ink);
    line-height: 1.75;
    margin-bottom: 40px;
    padding-bottom: 40px;
    border-bottom: 1px solid var(--border);
  }

  .lead strong { color: var(--sienna); }

  p {
    font-size: 0.975rem;
    margin-bottom: 20px;
    color: #2e2418;
    line-height: 1.8;
  }

  /* ---- SECTION HEADINGS ---- */
  .section {
    margin: 52px 0 28px;
  }

  .section-number {
    font-size: 0.65rem;
    font-weight: 700;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--sienna);
    display: block;
    margin-bottom: 8px;
  }

  .section h2 {
    font-family: 'Playfair Display', serif;
    font-size: 1.7rem;
    font-weight: 700;
    color: var(--ink);
    line-height: 1.25;
    letter-spacing: -0.01em;
  }

  .section h2 em {
    font-style: italic;
    color: var(--teal);
  }

  /* ---- CALLOUT BOXES ---- */
  .callout {
    border-left: 3px solid var(--sienna);
    background: var(--highlight);
    padding: 20px 24px;
    margin: 32px 0;
    border-radius: 0 10px 10px 0;
  }

  .callout.teal {
    border-color: var(--teal);
    background: #f0faf8;
  }

  .callout.gold {
    border-color: var(--gold);
    background: #fdf6e3;
  }

  .callout p {
    margin: 0;
    font-size: 0.93rem;
    font-style: italic;
    color: var(--ink);
  }

  .callout p strong {
    font-style: normal;
    color: var(--sienna);
  }

  .callout.teal p strong { color: var(--teal); }
  .callout.gold p strong { color: var(--gold); }

  /* ---- STAT CARDS ---- */
  .stats-row {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
    margin: 36px 0;
  }

  .stat-card {
    background: var(--paper);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 20px 16px;
    text-align: center;
  }

  .stat-number {
    font-family: 'Playfair Display', serif;
    font-size: 2.2rem;
    font-weight: 900;
    color: var(--sienna);
    display: block;
    line-height: 1;
    margin-bottom: 6px;
  }

  .stat-label {
    font-size: 0.78rem;
    color: var(--muted);
    line-height: 1.4;
  }

  /* ---- WARNING SIGNS ---- */
  .signs-list {
    list-style: none;
    margin: 24px 0;
  }

  .signs-list li {
    display: flex;
    gap: 14px;
    align-items: flex-start;
    padding: 14px 0;
    border-bottom: 1px solid var(--border);
  }

  .signs-list li:last-child { border-bottom: none; }

  .sign-icon {
    width: 36px;
    height: 36px;
    border-radius: 10px;
    background: var(--highlight);
    border: 1px solid var(--border);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1rem;
    flex-shrink: 0;
    margin-top: 2px;
  }

  .signs-list li .sign-text strong {
    display: block;
    font-size: 0.92rem;
    font-weight: 600;
    color: var(--ink);
    margin-bottom: 3px;
  }

  .signs-list li .sign-text span {
    font-size: 0.83rem;
    color: var(--muted);
    line-height: 1.5;
  }

  /* ---- PULL QUOTE ---- */
  .pull-quote {
    margin: 44px -40px;
    padding: 36px 40px;
    background: var(--ink);
    position: relative;
  }

  .pull-quote p {
    font-family: 'Playfair Display', serif;
    font-size: 1.5rem;
    font-style: italic;
    color: #fff;
    line-height: 1.4;
    margin: 0;
    text-align: center;
  }

  .pull-quote p em { color: var(--sienna-light); font-style: normal; }

  /* ---- ACTION STEPS ---- */
  .steps {
    counter-reset: step;
    margin: 28px 0;
  }

  .step-item {
    display: flex;
    gap: 18px;
    margin-bottom: 20px;
    align-items: flex-start;
  }

  .step-num {
    counter-increment: step;
    width: 36px;
    height: 36px;
    border-radius: 50%;
    background: var(--teal);
    color: #fff;
    font-weight: 700;
    font-size: 0.85rem;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    margin-top: 2px;
  }

  .step-item p {
    margin: 0;
    font-size: 0.93rem;
  }

  .step-item p strong {
    display: block;
    margin-bottom: 4px;
    color: var(--ink);
    font-weight: 600;
  }

  /* ---- DISCLAIMER ---- */
  .disclaimer {
    margin-top: 56px;
    padding: 20px 24px;
    background: var(--paper);
    border: 1px solid var(--border);
    border-radius: 12px;
    font-size: 0.78rem;
    color: var(--muted);
    line-height: 1.6;
    text-align: center;
  }

  /* ---- DIVIDER ---- */
  .divider {
    text-align: center;
    margin: 40px 0;
    color: var(--border);
    font-size: 1.4rem;
    letter-spacing: 0.6em;
  }

  /* ---- ANIMATIONS ---- */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(24px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .hero-tag { animation: fadeUp 0.6s ease both; }
  .hero h1 { animation: fadeUp 0.7s 0.1s ease both; }
  .hero-sub { animation: fadeUp 0.7s 0.2s ease both; }
  .hero-meta { animation: fadeUp 0.7s 0.3s ease both; }

  @media (max-width: 600px) {
    .hero { padding: 40px 24px 44px; min-height: 80vh; }
    .stats-row { grid-template-columns: 1fr 1fr; }
    .pull-quote { margin: 36px -24px; padding: 28px 24px; }
    .pull-quote p { font-size: 1.2rem; }
  }
</style>
</head>
<body>

<!-- HERO -->
<div class="hero">
  <div class="hero-tag">Sức khỏe tiêu hóa · Phát hiện sớm</div>
  <h1>Vì Sao Ung Thư Sớm Đường Tiêu Hóa<br><em>Dễ Bị Bỏ Sót</em>?</h1>
  <p class="hero-sub">Bệnh không phải lúc nào cũng gây đau — và đó chính là lý do nguy hiểm nhất. Hãy cùng hiểu vì sao, để bạn không bỏ lỡ cơ hội chữa khỏi hoàn toàn.</p>
  <div class="hero-meta">
    <div class="author-chip">
      <div class="author-avatar">🔬</div>
      <span>Bác sĩ chuyên khoa Nội soi tiêu hóa</span>
    </div>
    <span class="read-time">⏱ 5 phút đọc</span>
  </div>
</div>

<!-- ARTICLE -->
<div class="ornament">· · ·</div>

<article class="article">

  <p class="lead">
    Mỗi năm, hàng nghìn bệnh nhân ung thư đường tiêu hóa ở Việt Nam được phát hiện ở <strong>giai đoạn đã muộn</strong> — khi khối u đã lan rộng và cơ hội chữa khỏi trở nên rất thấp. Điều đáng tiếc là phần lớn những ca này hoàn toàn <strong>có thể được phát hiện sớm hơn</strong> — nếu chúng ta biết điều cần biết.
  </p>

  <!-- SECTION 1 -->
  <div class="section">
    <span class="section-number">Phần 01</span>
    <h2>Ung thư sớm <em>không gây đau</em></h2>
  </div>

  <p>Đây là sự thật khiến nhiều người bất ngờ: ung thư đường tiêu hóa ở giai đoạn sớm — dạ dày, thực quản, đại tràng — <strong>thường không gây ra bất kỳ triệu chứng rõ ràng nào</strong>. Không đau bụng dữ dội, không nôn ra máu, không sụt cân đột ngột.</p>

  <p>Lúc này, khối u còn rất nhỏ, chỉ nằm trên lớp niêm mạc bề mặt, chưa ăn sâu vào thành ruột hay dạ dày. Chính vì thế cơ thể chưa "cảm thấy" gì. Người bệnh vẫn ăn được, ngủ được, sinh hoạt bình thường — và nghĩ rằng mình hoàn toàn khỏe mạnh.</p>

  <div class="callout">
    <p><strong>Nghịch lý nguy hiểm:</strong> Khi bạn bắt đầu đau — khi cơ thể "la lên" — thường là lúc bệnh đã ở giai đoạn 2, 3 hoặc thậm chí 4. Giai đoạn mà cuộc chiến trở nên khó khăn hơn rất nhiều.</p>
  </div>

  <div class="stats-row">
    <div class="stat-card">
      <span class="stat-number">&gt;90%</span>
      <span class="stat-label">tỷ lệ sống 5 năm nếu phát hiện giai đoạn 1</span>
    </div>
    <div class="stat-card">
      <span class="stat-number">&lt;30%</span>
      <span class="stat-label">tỷ lệ sống 5 năm nếu phát hiện giai đoạn 4</span>
    </div>
    <div class="stat-card">
      <span class="stat-number">~70%</span>
      <span class="stat-label">bệnh nhân VN phát hiện ở giai đoạn muộn</span>
    </div>
  </div>

  <!-- SECTION 2 -->
  <div class="section">
    <span class="section-number">Phần 02</span>
    <h2>Tổn thương nhỏ, <em>mắt thường khó thấy</em></h2>
  </div>

  <p>Ngay cả khi được nội soi, ung thư sớm vẫn có thể bị bỏ sót. Vì sao? Bởi vì tổn thương sớm trông không giống những gì chúng ta tưởng tượng về "ung thư".</p>

  <p>Thay vì một khối u lồi lên rõ ràng, ung thư sớm thường chỉ là <strong>một vùng niêm mạc hơi đổi màu</strong>, hơi phẳng hơn xung quanh, hoặc mất đi vẻ bóng bình thường. Những dấu hiệu tinh tế đến mức nếu không có thiết bị nội soi hiện đại và bác sĩ được đào tạo chuyên sâu, chúng rất dễ bị bỏ qua.</p>

  <div class="callout teal">
    <p><strong>Ví dụ dễ hiểu:</strong> Hãy tưởng tượng bạn đang nhìn một tờ giấy trắng. Ung thư sớm giống như một vùng giấy hơi ngả vàng nhạt ở góc — không phải một vết mực đen rõ ràng. Nếu không chú ý kỹ, bạn sẽ không thấy.</p>
  </div>

  <!-- SECTION 3 -->
  <div class="section">
    <span class="section-number">Phần 03</span>
    <h2>Những <em>dấu hiệu mờ nhạt</em> cần lưu ý</h2>
  </div>

  <p>Mặc dù ung thư sớm thường không có triệu chứng rõ, nhưng đôi khi cơ thể vẫn gửi những tín hiệu rất nhỏ. Đừng bỏ qua:</p>

  <ul class="signs-list">
    <li>
      <div class="sign-icon">😣</div>
      <div class="sign-text">
        <strong>Ợ nóng hoặc khó tiêu kéo dài hơn 2–3 tuần</strong>
        <span>Đặc biệt nếu xuất hiện lần đầu ở người trên 45 tuổi, hoặc không đáp ứng với thuốc thông thường.</span>
      </div>
    </li>
    <li>
      <div class="sign-icon">🩸</div>
      <div class="sign-text">
        <strong>Phân có màu đen hoặc đỏ thẫm</strong>
        <span>Dù chỉ một lần — đây là dấu hiệu chảy máu trong đường tiêu hóa, cần khám ngay.</span>
      </div>
    </li>
    <li>
      <div class="sign-icon">⚖️</div>
      <div class="sign-text">
        <strong>Sụt cân không rõ nguyên nhân</strong>
        <span>Giảm hơn 5% trọng lượng cơ thể trong vòng 6 tháng mà không cố ý giảm cân.</span>
      </div>
    </li>
    <li>
      <div class="sign-icon">🍽️</div>
      <div class="sign-text">
        <strong>Chán ăn hoặc mau no bất thường</strong>
        <span>Cảm giác no nhanh dù ăn rất ít, đặc biệt khi mới xuất hiện gần đây.</span>
      </div>
    </li>
    <li>
      <div class="sign-icon">💨</div>
      <div class="sign-text">
        <strong>Thay đổi thói quen đi vệ sinh kéo dài</strong>
        <span>Tiêu chảy hoặc táo bón xen kẽ, đi cầu thấy không hết — kéo dài hơn 4 tuần.</span>
      </div>
    </li>
  </ul>

  <div class="callout gold">
    <p><strong>Lưu ý quan trọng:</strong> Hầu hết những triệu chứng này đều có nguyên nhân lành tính. Nhưng khi chúng kéo dài hoặc xuất hiện ở người có yếu tố nguy cơ, đó là lúc cần gặp bác sĩ — không phải để lo sợ, mà để <strong>chủ động loại trừ</strong>.</p>
  </div>

  <div class="divider">✦ ✦ ✦</div>

  <!-- PULL QUOTE -->
  <div class="pull-quote">
    <p>"Phát hiện sớm không đến từ may mắn —<br>nó đến từ <em>chủ động hành động</em>."</p>
  </div>

  <!-- SECTION 4 -->
  <div class="section">
    <span class="section-number">Phần 04</span>
    <h2>Ai có <em>nguy cơ cao</em> hơn?</h2>
  </div>

  <p>Bạn nên tầm soát sớm hơn nếu có một hoặc nhiều yếu tố sau:</p>

  <ul class="signs-list">
    <li>
      <div class="sign-icon">👪</div>
      <div class="sign-text">
        <strong>Gia đình có người thân bị ung thư đường tiêu hóa</strong>
        <span>Cha, mẹ, anh chị em ruột bị ung thư dạ dày, đại tràng, thực quản.</span>
      </div>
    </li>
    <li>
      <div class="sign-icon">🦠</div>
      <div class="sign-text">
        <strong>Nhiễm vi khuẩn H. pylori chưa điều trị</strong>
        <span>Vi khuẩn này làm tổn thương niêm mạc dạ dày lâu dài và là yếu tố nguy cơ hàng đầu của ung thư dạ dày.</span>
      </div>
    </li>
    <li>
      <div class="sign-icon">🚬</div>
      <div class="sign-text">
        <strong>Hút thuốc lá, uống rượu bia thường xuyên</strong>
        <span>Đặc biệt làm tăng nguy cơ ung thư thực quản và dạ dày.</span>
      </div>
    </li>
    <li>
      <div class="sign-icon">📅</div>
      <div class="sign-text">
        <strong>Trên 45 tuổi và chưa nội soi lần nào</strong>
        <span>Đây là nhóm tuổi mà tầm soát định kỳ bắt đầu trở nên thực sự quan trọng.</span>
      </div>
    </li>
  </ul>

  <!-- SECTION 5 -->
  <div class="section">
    <span class="section-number">Phần 05</span>
    <h2>Bạn có thể <em>làm gì ngay hôm nay</em>?</h2>
  </div>

  <p>Tin tốt là: nếu phát hiện ở giai đoạn sớm, ung thư đường tiêu hóa <strong>có thể điều trị dứt điểm hoàn toàn</strong> — thậm chí không cần phẫu thuật lớn, chỉ qua nội soi. Dưới đây là những bước bạn nên làm:</p>

  <div class="steps">
    <div class="step-item">
      <div class="step-num">1</div>
      <p><strong>Đánh giá yếu tố nguy cơ của bản thân</strong><br>Hỏi bản thân: trong gia đình có ai bị ung thư tiêu hóa không? Bạn có nhiễm H. pylori không? Bạn đã từng nội soi chưa?</p>
    </div>
    <div class="step-item">
      <div class="step-num">2</div>
      <p><strong>Gặp bác sĩ tiêu hóa để được tư vấn tầm soát</strong><br>Bác sĩ sẽ xác định bạn cần tầm soát theo lịch nào — không phải ai cũng cần nội soi mỗi năm, nhưng biết rõ lịch của mình là quan trọng.</p>
    </div>
    <div class="step-item">
      <div class="step-num">3</div>
      <p><strong>Không trì hoãn khi có triệu chứng bất thường</strong><br>Nếu bạn có bất kỳ dấu hiệu nào ở phần trên kéo dài hơn 2–3 tuần, hãy đặt lịch khám — đừng tự trấn an rằng "chắc không sao".</p>
    </div>
    <div class="step-item">
      <div class="step-num">4</div>
      <p><strong>Chọn cơ sở nội soi có thiết bị NBI/BLI và bác sĩ chuyên sâu</strong><br>Không phải nội soi nào cũng như nhau. Nội soi với công nghệ tăng cường hình ảnh giúp phát hiện những tổn thương cực nhỏ mà nội soi thông thường có thể bỏ sót.</p>
    </div>
  </div>

  <div class="callout teal">
    <p><strong>Điều quan trọng cần nhớ:</strong> Nội soi tầm soát không đáng sợ. Hiện nay có thể nội soi gây mê nhẹ (không đau, không khó chịu), chỉ mất 15–20 phút, và có thể trở về sinh hoạt bình thường ngay trong ngày.</p>
  </div>

  <div class="divider">✦</div>

  <p style="font-family:'Lora',serif; font-style:italic; font-size:1.05rem; color:var(--muted); text-align:center; line-height:1.8;">
    Ung thư sớm không có tiếng động. Nhưng bạn có thể <strong style="font-style:normal;color:var(--teal)">chủ động tìm nó</strong> — trước khi nó tìm bạn.
  </p>

  <!-- DISCLAIMER -->
  <div class="disclaimer">
    ⚕️ <strong>Lưu ý:</strong> Bài viết này mang tính giáo dục sức khỏe, không thay thế cho việc thăm khám và tư vấn trực tiếp từ bác sĩ. Nếu bạn có triệu chứng hoặc lo lắng về sức khỏe tiêu hóa, hãy liên hệ cơ sở y tế để được tư vấn cụ thể.
  </div>

</article>

</body>
</html>
