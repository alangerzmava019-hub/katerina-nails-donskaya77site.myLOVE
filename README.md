
<!DOCTYPE html>
<html lang="ru"> 
<head>
<!-- Иконка для добавления на главный экран iOS -->
<link rel="apple-touch-icon" href="https://i.postimg.cc/8PHkzTgX/27394514-5DA8-4C13-8072-537404349281.jpg">
<link rel="apple-touch-icon" sizes="180x180" href="https://i.postimg.cc/8PHkzTgX/27394514-5DA8-4C13-8072-537404349281.jpg">
<link rel="apple-touch-icon" sizes="167x167" href="https://i.postimg.cc/8PHkzTgX/27394514-5DA8-4C13-8072-537404349281.jpg">
<link rel="apple-touch-icon" sizes="152x152" href="https://i.postimg.cc/8PHkzTgX/27394514-5DA8-4C13-8072-537404349281.jpg">
<link rel="apple-touch-icon" sizes="120x120" href="https://i.postimg.cc/8PHkzTgX/27394514-5DA8-4C13-8072-537404349281.jpg">

<!-- Настройки при добавлении на главный экран -->
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<meta name="apple-mobile-web-app-title" content="Knails ⚡">
<meta name="apple-mobile-web-app-orientations" content="portrait">

<!-- Стандартная иконка для других платформ -->
<link rel="icon" type="image/jpeg" href="https://i.postimg.cc/8PHkzTgX/27394514-5DA8-4C13-8072-537404349281.jpg">
<link rel="shortcut icon" type="image/jpeg" href="https://i.postimg.cc/8PHkzTgX/27394514-5DA8-4C13-8072-537404349281.jpg">

<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Knails ⚡ — Katerina Nails</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&family=Roboto:wght@300;400;500;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<!-- Дополнительные мета-теги для лучшего отображения -->
<meta name="theme-color" content="#d9b6b0">
<meta name="msapplication-TileColor" content="#d9b6b0">
<meta name="msapplication-TileImage" content="https://i.postimg.cc/8PHkzTgX/27394514-5DA8-4C13-8072-537404349281.jpg">

<style>
:root{
  --bg:#fdf8f6;
  --primary:#d9b6b0;
  --secondary:#fff4f2;
  --text:#2b2b2b;
  --muted:#8f8a88;
  --accent:#e28c8c;
  --shadow:0 10px 25px rgba(0,0,0,0.1);
  --radius:14px;
}

*{box-sizing:border-box;margin:0;padding:0;}
html,body{height:100%;scroll-behavior:smooth;font-family:'Roboto',sans-serif;background:var(--bg);color:var(--text);}
a{text-decoration:none;color:inherit;}
img{display:block;width:100%;height:auto;border-radius:var(--radius);}

.lightning-bg{position:fixed;top:0;left:0;width:100%;height:100%;pointer-events:none;z-index:0;}
.lightning{position:absolute;font-size:24px;opacity:0.18;animation:lightningFloat 8s ease-in-out infinite;}
.star{position:absolute;font-size:14px;opacity:0.04;animation:twinkle 15s ease-in-out infinite;}

@keyframes lightningFloat{0%,100%{transform:translateY(0) scale(1); opacity:0.15;}50%{transform:translateY(-20px) scale(1.2); opacity:0.25;}}
@keyframes twinkle{0%,100%{opacity:0.04;transform:scale(1)}50%{opacity:0.09;transform:scale(1.06)}}

.logo-title{text-align:center;font-family:'Playfair Display',serif;font-size:80px;font-weight:700;color:var(--primary);margin:40px 0 20px;letter-spacing:4px;z-index:2;position:relative;}

.user-info {
  position: absolute;
  top: 20px;
  left: 20px;
  background: rgba(255,255,255,0.9);
  padding: 10px 20px;
  border-radius: 25px;
  font-size: 14px;
  font-weight: 600;
  box-shadow: var(--shadow);
  border: 1px solid rgba(217,182,176,0.4);
  z-index: 1000;
  display: none;
}

.user-info i {
  color: var(--primary);
  margin-right: 8px;
}

.logout-btn {
  background: var(--accent);
  color: white;
  border: none;
  border-radius: 12px;
  padding: 4px 10px;
  margin-left: 10px;
  font-size: 12px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.logout-btn:hover {
  background: #d87c7c;
  transform: translateY(-1px);
}

.dev-crown {
  color: #FFD700;
  margin-left: 8px;
  font-size: 16px;
  animation: crownGlow 2s ease-in-out infinite alternate;
}

@keyframes crownGlow {
  from { filter: drop-shadow(0 0 2px rgba(255, 215, 0, 0.5)); }
  to { filter: drop-shadow(0 0 6px rgba(255, 215, 0, 0.8)); }
}

.dev-greeting {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background: linear-gradient(135deg, var(--primary), var(--accent));
  color: white;
  padding: 15px;
  text-align: center;
  z-index: 1002;
  animation: slideDown 0.5s cubic-bezier(0.33, 1, 0.68, 1) forwards;
  box-shadow: 0 4px 15px rgba(0,0,0,0.2);
  font-weight: 600;
  display: none;
}

@keyframes slideDown {
  from { transform: translateY(-100%); }
  to { transform: translateY(0); }
}

.dev-promo-panel {
  margin-top: 20px;
  padding: 20px;
  background: rgba(217,182,176,0.1);
  border-radius: var(--radius);
  border: 2px dashed var(--primary);
  animation: fadeInScale 0.4s cubic-bezier(0.33, 1, 0.68, 1) forwards;
}

.dev-prices-panel {
  margin-top: 20px;
  padding: 20px;
  background: rgba(217,182,176,0.1);
  border-radius: var(--radius);
  border: 2px dashed var(--primary);
  animation: fadeInScale 0.4s cubic-bezier(0.33, 1, 0.68, 1) forwards;
}

.dev-polls-panel {
  margin-top: 20px;
  padding: 20px;
  background: rgba(217,182,176,0.1);
  border-radius: var(--radius);
  border: 2px dashed var(--primary);
  animation: fadeInScale 0.4s cubic-bezier(0.33, 1, 0.68, 1) forwards;
}

.dev-contests-panel {
  margin-top: 20px;
  padding: 20px;
  background: rgba(217,182,176,0.1);
  border-radius: var(--radius);
  border: 2px dashed var(--primary);
  animation: fadeInScale 0.4s cubic-bezier(0.33, 1, 0.68, 1) forwards;
}

.dev-reviews-panel {
  margin-top: 20px;
  padding: 20px;
  background: rgba(217,182,176,0.1);
  border-radius: var(--radius);
  border: 2px dashed var(--primary);
  animation: fadeInScale 0.4s cubic-bezier(0.33, 1, 0.68, 1) forwards;
}

.dev-portfolio-panel {
  margin-top: 20px;
  padding: 20px;
  background: rgba(217,182,176,0.1);
  border-radius: var(--radius);
  border: 2px dashed var(--primary);
  animation: fadeInScale 0.4s cubic-bezier(0.33, 1, 0.68, 1) forwards;
}

@keyframes fadeInScale {
  from { opacity: 0; transform: scale(0.95); }
  to { opacity: 1; transform: scale(1); }
}

.dev-promo-header, .dev-prices-header, .dev-polls-header, .dev-contests-header, .dev-reviews-header, .dev-portfolio-header {
  font-family: 'Playfair Display', serif;
  font-size: 18px;
  color: var(--primary);
  margin-bottom: 15px;
  display: flex;
  align-items: center;
  gap: 10px;
}

.dev-promo-list, .dev-prices-list, .dev-polls-list, .dev-contests-list, .dev-reviews-list, .dev-portfolio-list {
  max-height: 200px;
  overflow-y: auto;
  margin-bottom: 15px;
  border: 1px solid rgba(217,182,176,0.3);
  border-radius: var(--radius);
  background: white;
}

.dev-promo-item, .dev-price-item, .dev-poll-item, .dev-contest-item, .dev-review-item, .dev-portfolio-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 15px;
  border-bottom: 1px solid rgba(217,182,176,0.2);
  transition: background 0.3s ease;
}

.dev-promo-item:last-child, .dev-price-item:last-child, .dev-poll-item:last-child, .dev-contest-item:last-child, .dev-review-item:last-child, .dev-portfolio-item:last-child {
  border-bottom: none;
}

.dev-promo-item:hover, .dev-price-item:hover, .dev-poll-item:hover, .dev-contest-item:hover, .dev-review-item:hover, .dev-portfolio-item:hover {
  background: rgba(217,182,176,0.05);
}

.dev-promo-code, .dev-price-name, .dev-poll-name, .dev-contest-name, .dev-review-author, .dev-portfolio-name {
  font-weight: 600;
  color: var(--text);
}

.dev-promo-percent, .dev-price-value, .dev-poll-votes, .dev-contest-participants, .dev-review-date, .dev-portfolio-actions {
  color: var(--primary);
  font-weight: 700;
  margin-left: 10px;
}

.dev-promo-delete, .dev-price-edit, .dev-poll-delete, .dev-contest-delete, .dev-review-pin, .dev-review-delete, .dev-portfolio-edit {
  background: var(--accent);
  color: white;
  border: none;
  padding: 4px 8px;
  border-radius: 4px;
  cursor: pointer;
  font-size: 12px;
  transition: all 0.3s ease;
  margin-left: 5px;
}

.dev-promo-delete:hover, .dev-price-edit:hover, .dev-poll-delete:hover, .dev-contest-delete:hover, .dev-review-pin:hover, .dev-review-delete:hover, .dev-portfolio-edit:hover {
  background: #e57373;
  transform: scale(1.05);
}

.dev-promo-form, .dev-price-form, .dev-poll-form, .dev-contest-form, .dev-portfolio-form {
  display: grid;
  grid-template-columns: 1fr auto auto;
  gap: 10px;
  align-items: end;
}

.dev-promo-input, .dev-price-input, .dev-poll-input, .dev-contest-input, .dev-portfolio-input {
  padding: 10px 12px;
  border: 1px solid rgba(200,190,185,0.6);
  border-radius: var(--radius);
  font-family: 'Roboto', sans-serif;
  transition: all 0.3s;
}

.dev-promo-input:focus, .dev-price-input:focus, .dev-poll-input:focus, .dev-contest-input:focus, .dev-portfolio-input:focus {
  outline: none;
  border-color: var(--primary);
  box-shadow: 0 0 0 2px rgba(217,182,176,0.2);
}

.dev-promo-percent-select {
  padding: 10px 12px;
  border: 1px solid rgba(200,190,185,0.6);
  border-radius: var(--radius);
  background: white;
  font-family: 'Roboto', sans-serif;
  cursor: pointer;
}

.dev-promo-add-btn, .dev-price-add-btn, .dev-poll-add-btn, .dev-contest-add-btn, .dev-portfolio-add-btn {
  background: linear-gradient(135deg, var(--primary), var(--accent));
  color: white;
  border: none;
  padding: 10px 15px;
  border-radius: var(--radius);
  cursor: pointer;
  font-weight: 600;
  transition: all 0.3s ease;
}

.dev-promo-add-btn:hover, .dev-price-add-btn:hover, .dev-poll-add-btn:hover, .dev-contest-add-btn:hover, .dev-portfolio-add-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(217,182,176,0.4);
}

.search-container{display:flex;justify-content:center;margin-bottom:30px;position:relative;z-index:2;}
.search-bar{display:flex;align-items:center;background:white;border-radius:50px;padding:10px 25px;box-shadow:var(--shadow);border:1px solid rgba(217,182,176,0.6);transition:all 0.3s;}
.search-bar:focus-within{box-shadow:0 8px 25px rgba(217,182,176,0.25);border-color:var(--primary);}
.search-bar input{border:none;outline:none;background:transparent;flex:1;font-size:16px;color:var(--text);}
.search-results{position:absolute;top:105%;left:50%;transform:translateX(-50%);width:320px;background:white;border-radius:var(--radius);box-shadow:0 10px 25px rgba(0,0,0,0.15);margin-top:5px;display:none;max-height:300px;overflow-y:auto;z-index:10;}
.search-result-item{padding:14px 18px;border-bottom:1px solid rgba(200,190,185,0.3);cursor:pointer;transition:background 0.2s;}
.search-result-item:hover{background:rgba(217,182,176,0.1);}
.search-result-title{font-weight:600;margin-bottom:4px;}
.search-result-price{color:var(--primary);font-weight:700;font-size:14px;}
.search-result-type{font-size:12px;color:var(--muted);background:rgba(217,182,176,0.1);padding:2px 6px;border-radius:10px;display:inline-block;margin-top:4px;}

.container{max-width:1200px;margin:0 auto;padding:20px;position:relative;z-index:2;}
.main-grid{display:grid;grid-template-columns:1fr 350px;gap:20px;}
.paper{background:var(--secondary);border-radius:var(--radius);padding:20px;box-shadow:var(--shadow);border:1px solid rgba(200,190,185,0.5);position:relative;overflow:hidden;transition:transform 0.3s;}
.paper:hover{transform:translateY(-5px) scale(1.01);}
.pin{position:absolute;top:12px;right:12px;font-size:24px;color:var(--primary);}

.services-columns{display:grid;grid-template-columns:repeat(2,1fr);gap:16px;margin-top:18px;}
.note{background:linear-gradient(180deg,rgba(255,255,255,0.85),rgba(250,244,242,0.9));padding:22px;display:flex;flex-direction:column;justify-content:center;position:relative;cursor:pointer;border-radius:var(--radius);border:1px solid rgba(200,190,185,0.3);box-shadow:0 5px 15px rgba(0,0,0,0.05);transition:all 0.3s;}
.note:hover{transform:translateY(-8px) rotate(-0.3deg) scale(1.02);box-shadow:0 12px 25px rgba(0,0,0,0.08);}
.note-title{font-family:'Playfair Display',serif;font-size:20px;font-weight:600;margin-bottom:6px;}
.note-sub{color:var(--muted);font-style:italic;margin-bottom:8px;}
.note-price{color:var(--primary);font-weight:700;font-size:18px;text-align:right;flex:0 0 90px;}
.note-row{display:flex;width:100%;align-items:center;gap:10px;justify-content:space-between;}

.contact-card{text-align:center;padding:20px;display:flex;flex-direction:column;gap:15px;}
.contact-btn{display:flex;flex-direction:column;align-items:center;gap:6px;text-decoration:none;padding:14px;background:linear-gradient(180deg,#fff,#fbf7f5);border-radius:var(--radius);box-shadow:var(--shadow);border:1px solid rgba(200,190,185,0.5);transition:transform 0.25s ease;color:var(--text);}
.contact-btn:hover{transform:translateY(-6px);}
.contact-btn i{font-size:28px;color:var(--primary);}
.contact-btn span{font-weight:600;font-size:14px;}

.portfolio-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin-top:15px;}
.portfolio-item{position:relative;overflow:hidden;border-radius:var(--radius);}
.portfolio-item img{transition:transform 0.6s ease;}
.portfolio-item:hover img{transform:scale(1.08);}

.portfolio-like {
  position: absolute;
  bottom: 10px;
  right: 10px;
  background: rgba(255,255,255,0.9);
  border-radius: 50%;
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 0.3s ease;
  border: 2px solid var(--primary);
  z-index: 5;
}

.portfolio-like:hover {
  transform: scale(1.1);
  background: rgba(255,255,255,1);
}

.portfolio-like.liked {
  background: var(--accent);
  border-color: var(--accent);
}

.portfolio-like.liked i {
  color: white;
}

.portfolio-like i {
  color: var(--primary);
  font-size: 18px;
  transition: all 0.3s ease;
}

.portfolio-likes-count {
  position: absolute;
  bottom: 10px;
  left: 10px;
  background: rgba(255,255,255,0.9);
  border-radius: 20px;
  padding: 4px 10px;
  font-size: 12px;
  font-weight: 600;
  color: var(--text);
  border: 1px solid rgba(217,182,176,0.3);
}

.master-section {
  background: linear-gradient(135deg, #fff8f6 0%, #fff0ed 100%);
  border-radius: 20px;
  padding: 30px;
  position: relative;
  overflow: hidden;
  border: 1px solid rgba(217,182,176,0.3);
  box-shadow: 0 15px 35px rgba(0,0,0,0.1);
}

.master-section::before {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  width: 200px;
  height: 200px;
  background: radial-gradient(circle, rgba(217,182,176,0.1) 0%, transparent 70%);
  border-radius: 50%;
}

.master-header {
  text-align: center;
  margin-bottom: 30px;
  position: relative;
}

.master-title {
  font-family: 'Playfair Display', serif;
  font-size: 32px;
  font-weight: 700;
  color: var(--primary);
  margin-bottom: 10px;
  position: relative;
  display: inline-block;
}

.master-title::after {
  content: "";
  position: absolute;
  bottom: -8px;
  left: 50%;
  transform: translateX(-50%);
  width: 80px;
  height: 3px;
  background: linear-gradient(90deg, transparent, var(--primary), transparent);
  border-radius: 2px;
}

.master-subtitle {
  font-size: 18px;
  color: var(--muted);
  font-style: italic;
}

.master-content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
  align-items: start;
}

.master-stats {
  display: grid;
  grid-template-columns: repeat(2,1fr);
  gap: 15px;
  margin-bottom: 25px;
}

.stat-card {
  background: white;
  padding: 20px;
  border-radius: 15px;
  text-align: center;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
  border: 1px solid rgba(217,182,176,0.2);
  transition: transform 0.3s ease;
}

.stat-card:hover {
  transform: translateY(-5px);
}

.stat-number {
  font-family: 'Playfair Display', serif;
  font-size: 28px;
  font-weight: 700;
  color: var(--primary);
  display: block;
  margin-bottom: 5px;
}

.stat-label {
  font-size: 14px;
  color: var(--muted);
  font-weight: 500;
}

.master-highlights-grid {
  display: grid;
  gap: 12px;
}

.highlight-card {
  background: rgba(255,255,255,0.8);
  padding: 16px;
  border-radius: 12px;
  border-left: 4px solid var(--primary);
  box-shadow: 0 4px 12px rgba(0,0,0,0.05);
  transition: all 0.3s ease;
}

.highlight-card:hover {
  transform: translateX(5px);
  box-shadow: 0 6px 18px rgba(0,0,0,0.1);
}

.highlight-icon {
  font-size: 20px;
  margin-right: 10px;
  color: var(--primary);
}

.inspiration-box {
  background: linear-gradient(135deg, rgba(217,182,176,0.1) 0%, rgba(226,140,140,0.05) 100%);
  padding: 25px;
  border-radius: 15px;
  border: 1px solid rgba(217,182,176,0.2);
  position: relative;
  margin: 25px 0;
  box-shadow: 0 5px 15px rgba(0,0,0,0.03);
}

.inspiration-box::before {
  content: """;
  position: absolute;
  top: 15px;
  left: 20px;
  font-size: 60px;
  font-family: 'Playfair Display', serif;
  color: rgba(217,182,176,0.3);
  line-height: 1;
}

.inspiration-text {
  font-style: italic;
  line-height: 1.7;
  color: var(--text);
  font-size: 16px;
  margin-left: 10px;
  position: relative;
  z-index: 2;
}

.cta-section {
  text-align: center;
  margin-top: 30px;
  padding-top: 25px;
  border-top: 1px solid rgba(217,182,176,0.2);
}

.cta-text {
  font-size: 14px;
  color: var(--muted);
  margin-bottom: 15px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
}

.cta-icon {
  font-size: 18px;
  color: var(--primary);
}

.instagram-btn {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
  color: white;
  padding: 14px 28px;
  border-radius: 50px;
  font-weight: 700;
  text-decoration: none;
  box-shadow: 0 8px 25px rgba(217,182,176,0.4);
  transition: all 0.3s ease;
  border: none;
  cursor: pointer;
  font-size: 16px;
}

.instagram-btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 12px 30px rgba(217,182,176,0.6);
}

.master-photo {
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 15px 35px rgba(0,0,0,0.12);
  position: relative;
}

.master-photo::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 40%;
  background: linear-gradient(transparent, rgba(0,0,0,0.1));
  pointer-events: none;
}

footer{margin-top:40px;text-align:center;color:var(--muted);font-size:14px;padding:40px 0;}

.modal{display:none;position:fixed;top:0;left:0;width:100%;height:100%;background:rgba(0,0,0,0.55);z-index:1000;justify-content:center;align-items:center;}
.modal-content{background:var(--secondary);padding:30px;border-radius:var(--radius);max-width:600px;width:90%;position:relative;animation:fadeIn 0.3s;box-shadow:0 20px 40px rgba(0,0,0,0.15);}
.close-modal{position:absolute;top:15px;right:15px;font-size:24px;cursor:pointer;background:var(--primary);color:white;width:36px;height:36px;border-radius:50%;display:flex;align-items:center;justify-content:center;border:none;box-shadow:0 4px 8px rgba(0,0,0,0.1);}
.contact-options{display:flex;flex-direction:row;gap:15px;margin:25px 0;justify-content:center;}
.contact-option{display:flex;align-items:center;padding:20px;background:#f8f4f0;border-radius:var(--radius);text-decoration:none;color:var(--text);transition:background 0.3s;flex:1;justify-content:center;box-shadow:0 4px 8px rgba(0,0,0,0.05);}
.contact-option:hover{background:#eee6de;}
.contact-option i{margin-right:15px;font-size:28px;color:var(--primary);}
.promo-section{margin-top:20px;padding-top:20px;border-top:1px solid rgba(200,190,185,0.6);}
.promo-codes{display:flex;flex-wrap:wrap;gap:10px;justify-content:center;}
.promo-code{padding:8px 15px;background:#f0e9e3;border-radius:6px;font-size:14px;font-weight:500;position:relative;box-shadow:0 3px 6px rgba(0,0,0,0.05);}
.promo-discount{position:absolute;top:-8px;right:-8px;background:var(--primary);color:white;font-size:10px;padding:2px 6px;border-radius:10px;font-weight:600;}

@keyframes fadeIn{from{opacity:0;transform:translateY(-20px);}to{opacity:1;transform:translateY(0);}}

.book-all-btn {
  background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
  color: white;
  border: none;
  padding: 16px 40px;
  border-radius: 50px;
  font-weight: 700;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 18px;
  box-shadow: 0 8px 25px rgba(217,182,176,0.4);
  display: block;
  margin: 25px auto 0;
  width: fit-content;
  font-family: 'Playfair Display', serif;
  letter-spacing: 1px;
}

.book-all-btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 12px 30px rgba(217,182,176,0.6);
}

.contact-section {
  text-align: center;
  margin-top: 40px;
  padding: 30px;
  background: linear-gradient(135deg, #fff8f6 0%, #fff0ed 100%);
  border-radius: 20px;
  border: 1px solid rgba(217,182,176,0.3);
}

.contact-heading {
  font-family: 'Playfair Display', serif;
  font-size: 32px;
  font-weight: 700;
  color: var(--primary);
  margin-bottom: 25px;
  position: relative;
}

.contact-heading::after {
  content: "";
  position: absolute;
  bottom: -8px;
  left: 50%;
  transform: translateX(-50%);
  width: 80px;
  height: 3px;
  background: linear-gradient(90deg, transparent, var(--primary), transparent);
  border-radius: 2px;
}

.contact-buttons {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}

.contact-button {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100px;
  height: 100px;
  background: white;
  border-radius: 20px;
  text-decoration: none;
  box-shadow: 0 8px 20px rgba(0,0,0,0.1);
  transition: all 0.3s ease;
  color: var(--text);
}

.contact-button:hover {
  transform: translateY(-5px);
  box-shadow: 0 12px 25px rgba(0,0,0,0.15);
}

.contact-button i {
  font-size: 36px;
  margin-bottom: 8px;
  color: var(--primary);
}

.contact-button span {
  font-weight: 600;
  font-size: 14px;
}

.top-right-menu {
  position: fixed;
  top: 20px;
  right: 20px;
  z-index: 1000;
  cursor: move;
  touch-action: none;
  user-select: none;
}

.menu-button {
  background: rgba(255, 255, 255, 0.9);
  border: 1px solid rgba(217,182,176,0.4);
  border-radius: 50%;
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transition: all 0.3s ease;
  font-size: 20px;
  color: var(--primary);
}

.menu-button:hover {
  transform: scale(1.05);
  box-shadow: 0 6px 15px rgba(0,0,0,0.15);
}

.menu-dropdown {
  position: absolute;
  top: 60px;
  right: 0;
  background: white;
  border-radius: var(--radius);
  box-shadow: 0 10px 25px rgba(0,0,0,0.15);
  padding: 15px;
  width: 250px;
  display: none;
  border: 1px solid rgba(217,182,176,0.3);
  max-height: 400px;
  overflow-y: auto;
}

.menu-item {
  padding: 12px 15px;
  border-radius: 8px;
  cursor: pointer;
  transition: background 0.2s;
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 5px;
}

.menu-item:hover {
  background: rgba(217,182,176,0.1);
}

.menu-item i {
  color: var(--primary);
  width: 20px;
  text-align: center;
}

.auth-modal, .fortune-modal, .review-modal, .promo-modal, .prices-modal, .account-modal, .polls-modal, .contests-modal, .search-user-modal, .manage-polls-modal, .manage-contests-modal, .manage-reviews-modal, .manage-portfolio-modal {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.55);
  z-index: 1000;
  justify-content: center;
  align-items: center;
}

.auth-content, .fortune-content, .review-content, .promo-content, .prices-content, .account-content, .polls-content, .contests-content, .search-user-content, .manage-polls-content, .manage-contests-content, .manage-reviews-content, .manage-portfolio-content {
  background: var(--secondary);
  padding: 30px;
  border-radius: var(--radius);
  max-width: 450px;
  width: 90%;
  position: relative;
  animation: fadeIn 0.3s;
  box-shadow: 0 20px 40px rgba(0,0,0,0.15);
  text-align: center;
}

.auth-form {
  display: flex;
  flex-direction: column;
  gap: 15px;
  margin-top: 20px;
}

.form-group {
  text-align: left;
}

.form-group label {
  display: block;
  margin-bottom: 5px;
  font-weight: 500;
  color: var(--text);
}

.form-group input, .form-group textarea, .form-group select {
  width: 100%;
  padding: 12px 15px;
  border-radius: var(--radius);
  border: 1px solid rgba(200,190,185,0.6);
  background: white;
  font-family: 'Roboto', sans-serif;
  transition: all 0.3s;
}

.form-group input:focus, .form-group textarea:focus, .form-group select:focus {
  outline: none;
  border-color: var(--primary);
  box-shadow: 0 0 0 2px rgba(217,182,176,0.2);
}

.submit-btn {
  background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
  color: white;
  border: none;
  padding: 14px;
  border-radius: var(--radius);
  font-weight: 700;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 16px;
  margin-top: 10px;
}

.submit-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(217,182,176,0.4);
}

.submit-btn:disabled {
  background: #cccccc;
  cursor: not-allowed;
  transform: none;
  box-shadow: none;
}

.success-message {
  color: #2ecc71;
  font-weight: 600;
  margin-top: 15px;
  display: none;
}

.fortune-wheel-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  margin-top: 20px;
  position: relative;
}

.fortune-wheel {
  width: 400px;
  height: 400px;
  position: relative;
  border-radius: 50%;
  overflow: hidden;
  box-shadow: 0 10px 25px rgba(0,0,0,0.15);
  border: 8px solid var(--primary);
}

.wheel-inner {
  width: 100%;
  height: 100%;
  position: relative;
  transition: transform 5s cubic-bezier(0.17, 0.67, 0.83, 0.67);
}

.wheel-segment {
  position: absolute;
  width: 50%;
  height: 50%;
  transform-origin: bottom right;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

.segment-content {
  position: absolute;
  width: 140px;
  text-align: center;
  transform: rotate(45deg);
  font-weight: 600;
  color: white;
  text-shadow: 1px 1px 3px rgba(0,0,0,0.5);
  font-size: 14px;
  line-height: 1.3;
  padding: 5px;
}

.segment-discount {
  font-size: 10px;
  opacity: 0.9;
  display: block;
  margin-top: 2px;
}

.wheel-center {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 80px;
  height: 80px;
  background: white;
  border-radius: 50%;
  z-index: 10;
  box-shadow: 0 0 15px rgba(0,0,0,0.3);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 28px;
  color: var(--text);
  border: 3px solid var(--text);
}

.wheel-pointer {
  position: absolute;
  top: 40%;
  left: 10px;
  transform: translateY(-50%) rotate(90deg);
  width: 30px;
  height: 40px;
  background: #000000;
  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
  z-index: 15;
  box-shadow: 0 3px 6px rgba(0,0,0,0.3);
  border-bottom: none;
}

.paw-pointer {
  display: none;
}

.spin-button, .claim-button {
  background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
  color: white;
  border: none;
  padding: 14px 30px;
  border-radius: 50px;
  font-weight: 700;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 18px;
  box-shadow: 0 8px 25px rgba(217,182,176,0.4);
}

.spin-button:hover, .claim-button:hover {
  transform: translateY(-3px);
  box-shadow: 0 12px 30px rgba(217,182,176,0.6);
}

.spin-button:disabled {
  opacity: 0.7;
  cursor: not-allowed;
  transform: none;
}

.result-message {
  margin-top: 20px;
  padding: 15px;
  border-radius: var(--radius);
  background: rgba(217,182,176,0.1);
  display: none;
  font-size: 18px;
  font-weight: 600;
}

.result-prize {
  font-size: 24px;
  margin: 10px 0;
}

.confetti {
  position: fixed;
  width: 12px;
  height: 12px;
  background: var(--primary);
  opacity: 0;
  z-index: 1001;
  pointer-events: none;
}

.reviews-section {
  margin-top: 40px;
  padding: 30px;
  background: linear-gradient(135deg, #fff8f6 0%, #fff0ed 100%);
  border-radius: 20px;
  border: 1px solid rgba(217,182,176,0.3);
  position: relative;
}

.reviews-heading {
  font-family: 'Playfair Display', serif;
  font-size: 32px;
  font-weight: 700;
  color: var(--primary);
  margin-bottom: 25px;
  text-align: center;
  position: relative;
}

.reviews-heading::after {
  content: "";
  position: absolute;
  bottom: -8px;
  left: 50%;
  transform: translateX(-50%);
  width: 80px;
  height: 3px;
  background: linear-gradient(90deg, transparent, var(--primary), transparent);
  border-radius: 2px;
}

.review-form {
  display: flex;
  flex-direction: column;
  gap: 15px;
  max-width: 500px;
  margin: 0 auto;
}

.locked-feature {
  text-align: center;
  padding: 40px 20px;
  background: rgba(255,255,255,0.7);
  border-radius: var(--radius);
  border: 2px dashed var(--primary);
  margin-top: 20px;
}

.locked-icon {
  font-size: 48px;
  margin-bottom: 15px;
  color: var(--muted);
}

.locked-message {
  color: var(--muted);
  font-size: 16px;
  margin-bottom: 20px;
}

.close-right {
  position: absolute;
  top: 15px;
  right: 15px;
  font-size: 24px;
  cursor: pointer;
  background: var(--primary);
  color: white;
  width: 36px;
  height: 36px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  border: none;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  z-index: 10;
}

.prize-modal {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.7);
  z-index: 1001;
  justify-content: center;
  align-items: center;
}

.prize-content {
  background: white;
  padding: 40px;
  border-radius: 20px;
  max-width: 400px;
  width: 90%;
  text-align: center;
  position: relative;
  animation: fadeIn 0.5s;
  box-shadow: 0 20px 40px rgba(0,0,0,0.3);
}

.prize-icon {
  font-size: 80px;
  margin-bottom: 20px;
}

.prize-title {
  font-family: 'Playfair Display', serif;
  font-size: 28px;
  font-weight: 700;
  color: var(--primary);
  margin-bottom: 10px;
}

.prize-description {
  font-size: 18px;
  color: var(--text);
  margin-bottom: 25px;
}

.promo-list { 
  margin-top: 20px; 
  display: flex; 
  flex-direction: column; 
  gap: 12px; 
  position: relative; 
}

.promo-item { 
  opacity: 0; 
  transform: translateY(15px); 
  animation: fadeIn 0.6s forwards; 
  background: white;
  border: 1px solid rgba(217,182,176,0.3);
  border-radius: var(--radius); 
  padding: 15px; 
  font-weight: 600; 
  text-align: center; 
  position: relative; 
  z-index: 1;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08);
  transition: transform 0.3s ease;
}

.promo-item:hover {
  transform: translateY(-3px);
}

.heart { 
  position: absolute; 
  font-size: 18px; 
  animation: floatUp 2s forwards; 
  pointer-events: none; 
  z-index: 100;
}

@keyframes floatUp { 
  0% { 
    opacity: 1; 
    transform: translateY(0) scale(1); 
  } 
  100% { 
    opacity: 0; 
    transform: translateY(-60px) scale(1.2); 
  } 
}

.reviews-display {
  margin-top: 20px;
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.review-item {
  background: rgba(255,255,255,0.8);
  padding: 15px;
  border-radius: var(--radius);
  border-left: 4px solid var(--primary);
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
}

.review-item.pinned {
  border-left: 4px solid var(--accent);
  background: rgba(226,140,140,0.1);
  position: relative;
}

.review-item.pinned::before {
  content: "📌";
  position: absolute;
  top: 10px;
  right: 10px;
  font-size: 16px;
}

.review-author {
  font-weight: 600;
  color: var(--primary);
  margin-bottom: 5px;
}

.review-text {
  color: var(--text);
  font-size: 14px;
  line-height: 1.4;
}

.no-reviews {
  text-align: center;
  color: var(--muted);
  font-style: italic;
  padding: 20px;
}

.modal-content {
  animation: modalAppear 0.35s cubic-bezier(0.33, 1, 0.68, 1) forwards;
}

@keyframes modalAppear {
  from { 
    opacity: 0; 
    transform: scale(0.9) translateY(-20px); 
  }
  to { 
    opacity: 1; 
    transform: scale(1) translateY(0); 
  }
}

.achievements-section {
  margin-top: 20px;
}

.achievements-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 15px;
  margin-top: 20px;
}

.achievement-card {
  background: white;
  padding: 20px;
  border-radius: 15px;
  text-align: center;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
  border: 2px solid transparent;
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.achievement-card.locked {
  opacity: 0.6;
  background: #f8f8f8;
}

.achievement-card.unlocked {
  border-color: var(--primary);
  transform: translateY(-5px);
}

.achievement-icon {
  font-size: 40px;
  margin-bottom: 10px;
}

.achievement-title {
  font-weight: 600;
  color: var(--text);
  margin-bottom: 5px;
}

.achievement-desc {
  font-size: 12px;
  color: var(--muted);
}

.achievement-badge {
  position: absolute;
  top: 10px;
  right: 10px;
  background: var(--accent);
  color: white;
  width: 25px;
  height: 25px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 12px;
}

.loyalty-program {
  background: linear-gradient(135deg, #ffd700, #ffed4e);
  padding: 25px;
  border-radius: 20px;
  margin: 20px 0;
  color: #8B4513;
  text-align: center;
}

.loyalty-stats {
  display: flex;
  justify-content: space-around;
  margin: 20px 0;
}

.loyalty-stat {
  text-align: center;
}

.loyalty-number {
  font-size: 32px;
  font-weight: 700;
  display: block;
}

.loyalty-label {
  font-size: 14px;
  opacity: 0.8;
}

.progress-tracker {
  margin: 30px 0;
}

.progress-bar {
  height: 20px;
  background: var(--secondary);
  border-radius: 10px;
  overflow: hidden;
  margin: 10px 0;
}

.progress-fill {
  height: 100%;
  background: linear-gradient(135deg, var(--primary), var(--accent));
  border-radius: 10px;
  transition: width 0.5s ease;
  position: relative;
}

.progress-fill::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
  animation: shimmer 2s infinite;
}

@keyframes shimmer {
  0% { transform: translateX(-100%); }
  100% { transform: translateX(100%); }
}

.poll-options {
  display: flex;
  flex-direction: column;
  gap: 12px;
  margin: 20px 0;
}

.poll-option {
  padding: 15px 20px;
  background: var(--secondary);
  border: 2px solid transparent;
  border-radius: var(--radius);
  cursor: pointer;
  transition: all 0.3s ease;
  text-align: left;
  font-size: 16px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.poll-option:hover {
  border-color: var(--primary);
  transform: translateX(5px);
}

.poll-option.selected {
  border-color: var(--accent);
  background: rgba(226,140,140,0.1);
}

.poll-results {
  margin-top: 20px;
}

.poll-result-item {
  margin: 10px 0;
}

.poll-result-bar {
  height: 20px;
  background: var(--secondary);
  border-radius: 10px;
  overflow: hidden;
  margin: 5px 0;
}

.poll-result-fill {
  height: 100%;
  background: linear-gradient(135deg, var(--primary), var(--accent));
  border-radius: 10px;
  transition: width 0.5s ease;
}

.trend-tracker {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 20px;
  border-radius: var(--radius);
  margin: 20px 0;
  position: relative;
  overflow: hidden;
}

.trend-item {
  display: flex;
  align-items: center;
  gap: 15px;
  padding: 10px;
  background: rgba(255,255,255,0.1);
  border-radius: var(--radius);
  margin: 10px 0;
}

.gamification-badge {
  position: fixed;
  top: 50%;
  right: 20px;
  transform: translateY(-50%);
  background: linear-gradient(135deg, var(--primary), var(--accent));
  color: white;
  padding: 15px;
  border-radius: var(--radius);
  box-shadow: var(--shadow);
  z-index: 999;
  animation: slideInRight 0.5s ease;
}

@keyframes slideInRight {
  from { transform: translateX(100px) translateY(-50%); opacity: 0; }
  to { transform: translateX(0) translateY(-50%); opacity: 1; }
}

.user-search-results {
  margin-top: 20px;
  max-height: 300px;
  overflow-y: auto;
}

.user-result-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px;
  background: white;
  border-radius: var(--radius);
  margin-bottom: 10px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
}

.user-visit-controls {
  display: flex;
  gap: 10px;
  align-items: center;
}

.visit-btn {
  padding: 8px 15px;
  border-radius: var(--radius);
  border: none;
  cursor: pointer;
  font-weight: 600;
  transition: all 0.3s ease;
}

.visit-add {
  background: #2ecc71;
  color: white;
}

.visit-remove {
  background: #e74c3c;
  color: white;
}

.visit-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
}

.visit-count {
  font-weight: 600;
  color: var(--primary);
  min-width: 30px;
  text-align: center;
}

.vote-button {
  background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
  color: white;
  border: none;
  padding: 12px 25px;
  border-radius: 50px;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 16px;
  box-shadow: 0 4px 12px rgba(217,182,176,0.3);
  margin-top: 15px;
}

.vote-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 15px rgba(217,182,176,0.4);
}

.vote-button:disabled {
  background: #cccccc;
  cursor: not-allowed;
  transform: none;
  box-shadow: none;
}

* {
  transition: all 0.3s ease;
}

.show-all-reviews-btn {
  background: var(--secondary);
  color: var(--text);
  border: 1px solid rgba(200,190,185,0.6);
  padding: 10px 20px;
  border-radius: var(--radius);
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 14px;
  margin: 20px auto;
  display: block;
}

.show-all-reviews-btn:hover {
  background: rgba(217,182,176,0.1);
  transform: translateY(-2px);
}

.review-with-photo {
  position: relative;
}

.review-image {
  max-width: 100%;
  border-radius: var(--radius);
  margin-top: 10px;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.review-image:hover {
  transform: scale(1.02);
}

.achievements-toggle {
  background: var(--secondary);
  color: var(--text);
  border: 1px solid rgba(200,190,185,0.6);
  padding: 8px 15px;
  border-radius: var(--radius);
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 14px;
  margin: 10px 0;
}

.achievements-toggle:hover {
  background: rgba(217,182,176,0.1);
  transform: translateY(-1px);
}

.avatar-selection {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  gap: 10px;
  margin-top: 10px;
}

.avatar-option {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 20px;
  cursor: pointer;
  border: 2px solid transparent;
  transition: all 0.3s ease;
  background: rgba(217,182,176,0.1);
}

.avatar-option:hover {
  transform: scale(1.1);
  border-color: var(--primary);
}

.avatar-option.selected {
  border-color: var(--accent);
  background: rgba(226,140,140,0.2);
  transform: scale(1.1);
}

.change-avatar-btn {
  background: var(--secondary);
  color: var(--text);
  border: 1px solid rgba(200,190,185,0.6);
  padding: 8px 15px;
  border-radius: var(--radius);
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 14px;
  margin-top: 10px;
}

.change-avatar-btn:hover {
  background: rgba(217,182,176,0.1);
  transform: translateY(-1px);
}

.dev-review-clear-all {
  background: #e74c3c;
  color: white;
  border: none;
  padding: 10px 15px;
  border-radius: var(--radius);
  cursor: pointer;
  font-weight: 600;
  transition: all 0.3s ease;
  margin-top: 15px;
  width: 100%;
}

.dev-review-clear-all:hover {
  background: #c0392b;
  transform: translateY(-2px);
}

.add-service-form {
  display: grid;
  grid-template-columns: 1fr 1fr auto;
  gap: 10px;
  margin-top: 20px;
  padding-top: 20px;
  border-top: 1px solid rgba(217,182,176,0.3);
}

.add-service-input {
  padding: 10px 12px;
  border: 1px solid rgba(200,190,185,0.6);
  border-radius: var(--radius);
  font-family: 'Roboto', sans-serif;
  transition: all 0.3s;
}

.add-service-input:focus {
  outline: none;
  border-color: var(--primary);
  box-shadow: 0 0 0 2px rgba(217,182,176,0.2);
}

.add-service-btn {
  background: linear-gradient(135deg, var(--primary), var(--accent));
  color: white;
  border: none;
  padding: 10px 15px;
  border-radius: var(--radius);
  cursor: pointer;
  font-weight: 600;
  transition: all 0.3s ease;
}

.add-service-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(217,182,176,0.4);
}

.review-pin-icon {
  position: absolute;
  top: 10px;
  right: 10px;
  font-size: 16px;
  color: var(--accent);
}

@media (max-width: 768px) {
  .logo-title {
    font-size: 50px;
    margin: 30px 0 15px;
  }
  
  .user-info {
    position: relative;
    top: 0;
    left: 0;
    margin: 10px auto;
    text-align: center;
    display: inline-block;
  }
  
  .search-bar {
    width: 90%;
    max-width: 320px;
    padding: 8px 20px;
  }
  
  .search-results {
    width: 90%;
    max-width: 320px;
  }
  
  .container {
    padding: 15px;
  }
  
  .main-grid {
    grid-template-columns: 1fr;
    gap: 15px;
  }
  
  .services-columns {
    grid-template-columns: 1fr;
    gap: 12px;
  }
  
  .note {
    padding: 18px;
  }
  
  .note-price {
    font-size: 16px;
    flex: 0 0 80px;
  }
  
  .master-section {
    padding: 20px;
    border-radius: 16px;
  }
  
  .master-title {
    font-size: 26px;
  }
  
  .master-content {
    grid-template-columns: 1fr;
    gap: 20px;
  }
  
  .master-stats {
    grid-template-columns: 1fr;
    gap: 12px;
  }
  
  .master-photo {
    order: -1;
    margin-bottom: 20px;
  }
  
  .portfolio-grid {
    grid-template-columns: 1fr;
    gap: 10px;
  }
  
  .contact-options {
    flex-direction: column;
  }
  
  .contact-btn {
    padding: 12px;
  }
  
  .instagram-btn {
    padding: 12px 24px;
    font-size: 14px;
  }
  
  .cta-text {
    flex-direction: column;
    gap: 5px;
  }
  
  .modal-content {
    padding: 20px;
  }
  
  .contact-option {
    padding: 15px;
  }
  
  .contact-buttons {
    gap: 15px;
  }
  
  .contact-button {
    width: 85px;
    height: 85px;
  }
  
  .contact-button i {
    font-size: 30px;
  }
  
  .book-all-btn {
    padding: 14px 30px;
    font-size: 16px;
  }
  
  .top-right-menu {
    top: 15px;
    right: 15px;
  }
  
  .menu-button {
    width: 45px;
    height: 45px;
    font-size: 18px;
  }
  
  .menu-dropdown {
    width: 220px;
  }
  
  .fortune-wheel {
    width: 300px;
    height: 300px;
  }
  
  .segment-content {
    font-size: 12px;
    width: 110px;
  }
  
  .wheel-pointer {
    left: 8px;
    width: 25px;
    height: 30px;
  }
  
  .dev-promo-form, .dev-price-form, .dev-poll-form, .dev-contest-form, .dev-portfolio-form {
    grid-template-columns: 1fr;
    gap: 8px;
  }
  
  .dev-promo-item, .dev-price-item, .dev-poll-item, .dev-contest-item, .dev-portfolio-item {
    flex-direction: column;
    align-items: flex-start;
    gap: 8px;
  }
  
  .dev-promo-actions, .dev-price-actions, .dev-poll-actions, .dev-contest-actions, .dev-portfolio-actions {
    align-self: flex-end;
  }
  
  .dev-greeting {
    padding: 12px 15px;
    font-size: 14px;
  }
  
  .achievements-grid {
    grid-template-columns: 1fr;
  }
  
  .gamification-badge {
    position: relative;
    top: auto;
    right: auto;
    transform: none;
    margin: 20px auto;
    max-width: 300px;
  }
}

@media (max-width: 480px) {
  .logo-title {
    font-size: 40px;
    margin: 20px 0 10px;
  }
  
  .paper {
    padding: 15px;
  }
  
  .master-title {
    font-size: 22px;
  }
  
  .stat-card {
    padding: 15px;
  }
  
  .stat-number {
    font-size: 24px;
  }
  
  .highlight-card {
    padding: 12px;
  }
  
  .inspiration-box {
    padding: 18px;
  }
  
  .inspiration-text {
    font-size: 14px;
  }
  
  .contact-card {
    padding: 15px;
  }
  
  .contact-heading {
    font-size: 26px;
  }
  
  .contact-buttons {
    gap: 10px;
  }
  
  .contact-button {
    width: 75px;
    height: 75px;
  }
  
  .contact-button i {
    font-size: 26px;
  }
  
  .contact-button span {
    font-size: 12px;
  }
  
  .note-price {
    font-size: 16px;
    flex: 0 0 70px;
  }
  
  .fortune-wheel {
    width: 250px;
    height: 250px;
  }
  
  .segment-content {
    font-size: 10px;
    width: 90px;
  }
  
  .wheel-pointer {
    left: 6px;
    width: 20px;
    height: 25px;
  }
  
  .dev-promo-panel, .dev-prices-panel, .dev-polls-panel, .dev-contests-panel, .dev-portfolio-panel {
    padding: 15px;
  }
  
  .dev-promo-header, .dev-prices-header, .dev-polls-header, .dev-contests-header, .dev-portfolio-header {
    font-size: 16px;
  }
  
  .dev-crown {
    font-size: 14px;
    margin-left: 5px;
  }
}

@media (max-width: 360px) {
  .logo-title {
    font-size: 36px;
  }
  
  .search-bar {
    padding: 6px 15px;
  }
  
  .search-bar input {
    font-size: 14px;
  }
  
  .note {
    padding: 15px;
  }
  
  .note-title {
    font-size: 18px;
  }
  
  .note-price {
    font-size: 16px;
    flex: 0 0 65px;
  }
  
  .master-section {
    padding: 15px;
  }
  
  .master-title {
    font-size: 20px;
  }
  
  .master-subtitle {
    font-size: 16px;
  }
  
  .contact-heading {
    font-size: 22px;
  }
  
  .fortune-wheel {
    width: 220px;
    height: 220px;
  }
  
  .segment-content {
    font-size: 9px;
    width: 80px;
  }
  
  .wheel-pointer {
    left: 5px;
    width: 18px;
    height: 22px;
  }
}
</style>
</head>
<body>

<div class="lightning-bg" id="lightning-bg"></div>

<div class="dev-greeting" id="dev-greeting" style="display: none;"></div>

<div class="user-info" id="userInfo">
  <i class="fas fa-user"></i> <span id="userName"></span>
  <span class="dev-crown" id="dev-crown" style="display: none;">👑</span>
  <button class="logout-btn" onclick="logout()">Выйти</button>
</div>

<div class="top-right-menu" id="draggable-menu">
  <div class="menu-button" id="menu-button">
    <i class="fas fa-ellipsis-v"></i>
  </div>
  <div class="menu-dropdown" id="menu-dropdown">
    <div class="menu-item" id="account-button" style="display: none;">
      <i class="fas fa-user-circle"></i>
      <span>Аккаунт</span>
    </div>
    
    <div class="menu-item" id="auth-button">
      <i class="fas fa-sign-in-alt"></i>
      <span id="auth-menu-text">Вход</span>
    </div>
    
    <div class="menu-item" id="fortune-button">
      <i class="fas fa-gift"></i>
      <span>Колесо фортуны</span>
    </div>
    
    <div class="menu-item" id="review-button">
      <i class="fas fa-star"></i>
      <span>Оставить отзыв</span>
    </div>
    
    <div class="menu-item" id="promo-button">
      <i class="fas fa-tag"></i>
      <span>Промокоды</span>
    </div>
    
    <div class="menu-item" id="polls-button">
      <i class="fas fa-poll"></i>
      <span>Опросы</span>
    </div>
    
    <div class="menu-item" id="contests-button">
      <i class="fas fa-trophy"></i>
      <span>Конкурсы</span>
    </div>
    
    <div class="menu-item" id="prices-button" style="display: none;">
      <i class="fas fa-edit"></i>
      <span>Управление ценами</span>
    </div>
    
    <div class="menu-item" id="search-user-button" style="display: none;">
      <i class="fas fa-search"></i>
      <span>Поиск клиента</span>
    </div>
    
    <div class="menu-item" id="manage-polls-button" style="display: none;">
      <i class="fas fa-poll-h"></i>
      <span>Управление опросами</span>
    </div>
    
    <div class="menu-item" id="manage-contests-button" style="display: none;">
      <i class="fas fa-trophy"></i>
      <span>Управление конкурсами</span>
    </div>
    
    <div class="menu-item" id="manage-reviews-button" style="display: none;">
      <i class="fas fa-star"></i>
      <span>Управление отзывами</span>
    </div>
    
    <div class="menu-item" id="manage-portfolio-button" style="display: none;">
      <i class="fas fa-images"></i>
      <span>Управление портфолио</span>
    </div>
  </div>
</div>

<div class="logo-title">Knails ⚡</div>

<div class="search-container">
  <div class="search-bar">
    <input type="text" id="search-input" placeholder="Hello Kitty...">
    <i class="fas fa-search" style="color: var(--primary);"></i>
  </div>
  <div class="search-results" id="search-results"></div>
</div>

<main class="container">
  <div class="main-grid">
    <div>
      <div class="paper">
        <div style="display:flex;align-items:center;justify-content:space-between;">
          <h2 style="font-family:'Playfair Display', serif;">Услуги и цены</h2>
          <div class="pin">⚡</div>
        </div>
        <div class="services-columns" id="services-container">
        </div>
        <button class="book-all-btn" onclick="openBookingModal()">Записаться на услугу</button>
      </div>

      <div class="master-section" style="margin-top:20px;">
        <div class="master-header">
          <h2 class="master-title">Привет! Меня зовут Катя)</h2>
          <div class="master-subtitle">Мастер маникюра с любовью к деталям</div>
        </div>
        
        <div class="master-content">
          <div>
            <div class="master-stats">
              <div class="stat-card">
                <span class="stat-number">3+</span>
                <span class="stat-label">года опыта</span>
              </div>
              <div class="stat-card">
                <span class="stat-number">1000+</span>
                <span class="stat-label">довольных клиенток</span>
              </div>
            </div>
            
            <div class="master-highlights-grid">
              <div class="highlight-card">
                <span class="highlight-icon">⚡</span>
                Работаю быстро, но без потери качества
              </div>
              <div class="highlight-card">
                <span class="highlight-icon">⚡</span>
                Коррекция всего за 1 час
              </div>
              <div class="highlight-card">
                <span class="highlight-icon">⚡</span>
                Исправляю «проблемные» ногти
              </div>
              <div class="highlight-card">
                <span class="highlight-icon">⚡</span>
                Стойкий и эстетичный результат
              </div>
            </div>
          </div>
          
          <div class="master-photo">
            <img src="https://i.postimg.cc/hjBThm9n/IMG-0059.jpg" alt="Катя - мастер маникюра">
          </div>
        </div>
        
        <div class="inspiration-box">
          <div class="inspiration-text">
            Моя цель — создавать не просто маникюр, а настоящее произведение искусства, которое будет радовать вас каждый день. Красивые ухоженные ногти — важная часть уверенности и самовыражения.
          </div>
        </div>
        
        <div class="cta-section">
          <div class="cta-text">
            <span class="cta-icon">📍</span>
            Запись в ЛС
            <span class="cta-icon">📆</span>
            Места быстро разбирают — не откладывай красоту
          </div>
          <a href="https://www.instagram.com/kateina_nails" class="instagram-btn" target="_blank">
            <i class="fab fa-instagram"></i>
            Мой Instagram
          </a>
        </div>
      </div>

      <div class="paper" style="margin-top:20px;">
        <h3 style="font-family:'Playfair Display', serif;">Портфолио</h3>
        <div class="portfolio-grid" id="portfolio-grid">
        </div>
        <div id="portfolio-dev-panel" style="display: none;"></div>
      </div>

      <div class="contact-section">
        <h2 class="contact-heading">Связаться со мной</h2>
        <div class="contact-buttons">
          <a href="https://t.me/Lazaryan0" class="contact-button" target="_blank">
            <i class="fab fa-telegram"></i>
            <span>Telegram</span>
          </a>
          <a href="https://www.instagram.com/kateina_nails" class="contact-button" target="_blank">
            <i class="fab fa-instagram"></i>
            <span>Instagram</span>
          </a>
          <a href="https://wa.me/79881605058" class="contact-button" target="_blank">
            <i class="fab fa-whatsapp"></i>
            <span>WhatsApp</span>
          </a>
        </div>
      </div>

      <div class="reviews-section">
        <h2 class="reviews-heading">Отзывы</h2>
        <div class="reviews-display" id="reviews-display">
        </div>
        <button class="show-all-reviews-btn" id="show-all-reviews-btn" style="display: none;">Раскрыть все отзывы</button>
      </div>
    </div>

    <aside>
      <div class="paper">
        <div class="contact-card">
          <h3>Промокоды</h3>
          <div style="margin-top:20px; font-size:14px; color:var(--muted); text-align:left;">
            <div style="margin-top:5px;" id="default-promocodes">
              <strong style="color:var(--primary)">FIRSTVISIT</strong> - первое посещение -10%<br>
              <strong style="color:var(--primary)">GEL5</strong> - гель-лак -5%<br>
              <strong style="color:var(--primary)">NAILS8</strong> - наращивание -8%<br>
              <strong style="color:var(--primary)">LOVE3</strong> - любые услуги -3%
            </div>
          </div>

          <div id="activated-promos"></div>

          <div style="margin-top:15px; display:flex; gap:10px; justify-content:center;">
            <button onclick="scrollToSection('portfolio')" style="padding:8px 12px; border-radius:12px; border:1px solid rgba(200,190,185,0.6); background:transparent; color:var(--text); font-weight:600; cursor:pointer; box-shadow:0 2px 4px rgba(0,0,0,0.05);">Портфолио</button>
          </div>
        </div>
      </div>
    </aside>
  </div>
</main>

<div class="modal" id="booking-modal">
  <div class="modal-content">
    <button class="close-modal">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Записаться на услугу</h2>
    <p style="color:var(--muted);">Выберите удобный способ связи для записи:</p>
    <div class="contact-options">
      <a href="https://t.me/Lazaryan0" class="contact-option" target="_blank">
        <i class="fab fa-telegram"></i>
        <div>
          <strong>Telegram</strong><br>@Lazaryan0
        </div>
      </a>
      <a href="https://wa.me/79881605058" class="contact-option" target="_blank">
        <i class="fab fa-whatsapp"></i>
        <div>
          <strong>WhatsApp</strong><br>+7 988 160 50 58
        </div>
      </a>
    </div>
    <div class="promo-section">
      <h3 style="font-family:'Playfair Display', serif; margin-bottom:15px;">Промокоды для скидок</h3>
      <div class="promo-codes" id="booking-promocodes">
        <div class="promo-code">FIRSTVISIT<div class="promo-discount">-10%</div></div>
        <div class="promo-code">GEL5<div class="promo-discount">-5%</div></div>
        <div class="promo-code">NAILS8<div class="promo-discount">-8%</div></div>
        <div class="promo-code">LOVE3<div class="promo-discount">-3%</div></div>
      </div>
      <p style="margin-top:15px; font-size:14px; color:var(--muted);" id="booking-promo-description">
        <strong>FIRSTVISIT</strong> - скидка 10% на первое посещение<br>
        <strong>GEL5</strong> - скидка 5% на гель-лак<br>
        <strong>NAILS8</strong> - скидка 8% на наращивание<br>
        <strong>LOVE3</strong> - скидка 3% на любые услуги
      </p>
    </div>
  </div>
</div>

<div class="auth-modal" id="auth-modal">
  <div class="auth-content">
    <button class="close-right" onclick="closeAuthModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;" id="auth-title">Регистрация / Вход</h2>
    <p style="color:var(--muted);" id="auth-subtitle">Создайте аккаунт или войдите в существующий:</p>
    
    <div class="auth-form-extended">
      <div class="form-group">
        <label for="username">Никнейм</label>
        <input type="text" id="username" placeholder="Придумайте уникальный никнейм">
      </div>
      
      <div class="form-group">
        <label for="phone">Номер телефона</label>
        <input type="tel" id="phone" placeholder="+7 (XXX) XXX-XX-XX">
      </div>
      
      <div class="form-group">
        <label for="password">Пароль</label>
        <input type="password" id="password" placeholder="Придумайте надежный пароль">
      </div>
      
      <div class="form-group">
        <label>Выберите аватар</label>
        <div class="avatar-selection" id="avatar-selection">
          <div class="avatar-option" data-avatar="💅">💅</div>
          <div class="avatar-option" data-avatar="🐻">🐻</div>
          <div class="avatar-option" data-avatar="🧸">🧸</div>
          <div class="avatar-option" data-avatar="🌸">🌸</div>
          <div class="avatar-option" data-avatar="💕">💕</div>
          <div class="avatar-option" data-avatar="⚡">⚡</div>
          <div class="avatar-option" data-avatar="🎰">🎰</div>
          <div class="avatar-option" data-avatar="🚩">🚩</div>
          <div class="avatar-option" data-avatar="💋">💋</div>
          <div class="avatar-option" data-avatar="🫦">🫦</div>
          <div class="avatar-option" data-avatar="👠">👠</div>
          <div class="avatar-option" data-avatar="👸">👸</div>
          <div class="avatar-option" data-avatar="👑">👑</div>
        </div>
      </div>
      
      <button class="submit-btn" onclick="submitAuthExtended()">Продолжить</button>
      
      <div class="success-message" id="auth-success">Вы авторизированы!</div>
    </div>
  </div>
</div>

<div class="fortune-modal" id="fortune-modal">
  <div class="fortune-content">
    <button class="close-right" onclick="closeFortuneModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Колесо фортуны</h2>
    <div id="fortune-content">
      <p style="color:var(--muted);">Покрутите колесо и выиграйте приз!</p>
      
      <div class="fortune-wheel-container">
        <div class="wheel-pointer"></div>
        <div class="fortune-wheel">
          <div class="wheel-inner" id="wheel-inner">
          </div>
          <div class="wheel-center">🐾</div>
        </div>
        <button class="spin-button" id="spin-button">Крутить</button>
        <button class="claim-button" id="claim-button" style="display:none;">Забрать</button>
        <div class="result-message" id="result-message">
        </div>
      </div>
    </div>
    <div id="fortune-locked" class="locked-feature" style="display: none;">
      <div class="locked-icon">🔒</div>
      <div class="locked-message">Для использования колеса фортуны необходимо авторизоваться</div>
      <button class="submit-btn" onclick="openAuthModal()">
        <i class="fas fa-sign-in-alt"></i> Войти
      </button>
    </div>
  </div>
</div>

<div class="review-modal" id="review-modal">
  <div class="review-content">
    <button class="close-right" onclick="closeReviewModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Оставить отзыв</h2>
    <p style="color:var(--muted);">Поделитесь вашими впечатлениями:</p>
    <div class="review-form">
      <div class="form-group">
        <label for="modal-review-name">Ваше имя</label>
        <input type="text" id="modal-review-name" placeholder="Введите ваше имя">
      </div>
      <div class="form-group">
        <label for="modal-review-text">Ваш отзыв</label>
        <textarea id="modal-review-text" rows="4" placeholder="Напишите ваш отзыв здесь..."></textarea>
      </div>
      <div class="form-group">
        <label for="modal-review-image">Прикрепить фото (опционально)</label>
        <input type="file" id="modal-review-image" accept="image/*">
      </div>
      <button class="submit-btn" id="modal-submit-review">Отправить отзыв</button>
      <div class="success-message" id="modal-review-success">Отзыв отправлен!</div>
    </div>
  </div>
</div>

<div class="promo-modal" id="promo-modal">
  <div class="promo-content">
    <button class="close-right" onclick="closePromoModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Промокоды</h2>
    <p style="color:var(--muted);">Введите ключ для получения промокодов:</p>
    <div class="auth-form">
      <div class="form-group">
        <input type="password" id="modal-promoKey" placeholder="Введите ключ для промокодов">
      </div>
      <button class="submit-btn" onclick="checkPromo()">Показать промокоды</button>
      <div class="promo-list" id="modal-promoList"></div>
    </div>
  </div>
</div>

<div class="prices-modal" id="prices-modal">
  <div class="prices-content">
    <button class="close-right" onclick="closePricesModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Управление ценами</h2>
    <p style="color:var(--muted);">Изменение цен применяется для всех пользователей:</p>
    <div class="dev-prices-panel">
      <div class="dev-prices-header">
        <i class="fas fa-edit"></i>
        Редактирование прайса
      </div>
      
      <div class="dev-prices-list" id="dev-prices-list">
      </div>
    </div>
  </div>
</div>

<div class="prize-modal" id="prize-modal">
  <div class="prize-content">
    <div class="prize-icon" id="prize-icon">🎁</div>
    <h2 class="prize-title">Поздравляем!</h2>
    <p class="prize-description" id="prize-description">Вы выиграли приз!</p>
    <button class="claim-button" id="exchange-prize-button" onclick="exchangePrizeForDiscount()">Обменять на скидку <span id="exchange-discount-value">5%</span></button>
    <button class="claim-button" onclick="closePrizeModal()" style="margin-top: 10px; background: var(--muted);">Забрать приз</button>
  </div>
</div>

<div class="account-modal" id="account-modal">
  <div class="account-content">
    <button class="close-right" onclick="closeAccountModal()">&times;</button>
    
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Мой аккаунт</h2>
    
    <div class="user-profile">
      <div class="profile-header" style="display: flex; align-items: center; margin-bottom: 20px;">
        <div class="profile-avatar" id="profile-avatar" style="font-size: 40px; margin-right: 15px;"></div>
        <div>
          <h3 id="profile-username" style="margin: 0; color: var(--primary);"></h3>
          <p id="profile-phone" style="margin: 0; color: var(--muted); font-size: 14px;"></p>
          <button class="change-username-btn" onclick="openChangeUsernameModal()">
            <i class="fas fa-edit"></i> Сменить никнейм
          </button>
        </div>
      </div>
      
      <div class="profile-stats" style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 15px; margin-bottom: 20px;">
        <div class="stat-card">
          <span class="stat-number" id="profile-joined-date">-</span>
          <span class="stat-label">С нами с</span>
        </div>
      </div>
    </div>
    
    <div class="loyalty-program">
      <h3>Программа лояльности</h3>
      <div class="loyalty-stats">
        <div class="loyalty-stat">
          <span class="loyalty-number" id="account-visits-count">0</span>
          <span class="loyalty-label">Посещений</span>
        </div>
        <div class="loyalty-stat">
          <span class="loyalty-number" id="account-points-count">0</span>
          <span class="loyalty-label">Баллов</span>
        </div>
        <div class="loyalty-stat">
          <span class="loyalty-number" id="account-discount-percent">0%</span>
          <span class="loyalty-label">Скидка</span>
        </div>
      </div>
      <div class="progress-tracker">
        <div class="progress-bar">
          <div class="progress-fill" id="account-loyalty-progress" style="width: 0%"></div>
        </div>
        <p>До следующего уровня: <span id="account-points-to-next">100</span> баллов</p>
      </div>
    </div>
    
    <button class="achievements-toggle" onclick="toggleAchievements()">Скрыть достижения</button>
    
    <div class="achievements-section" id="achievements-section">
      <h3 style="font-family:'Playfair Display', serif; text-align: center; margin-bottom: 20px;">Мои достижения</h3>
      <div class="achievements-grid" id="account-achievements-container">
      </div>
    </div>
  </div>
</div>

<div class="polls-modal" id="polls-modal">
  <div class="polls-content">
    <button class="close-right" onclick="closePollsModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Опросы</h2>
    
    <div id="current-poll">
      <h3 style="color: var(--primary); margin-bottom: 15px;" id="poll-question">Какой дизайн вам нравится больше?</h3>
      <div class="poll-options" id="poll-options">
      </div>
      
      <button class="vote-button" id="vote-button" onclick="submitVote()">Голосовать</button>
      
      <div class="poll-results" id="poll-results" style="display: none;">
        <h4 style="margin-bottom: 15px;">Результаты голосования:</h4>
        <div id="poll-results-container">
        </div>
      </div>
      
      <div class="trend-tracker" style="margin-top: 30px;">
        <h2 style="color: white; text-align: center;">Сейчас в тренде</h2>
        <div class="trend-item">
          <span style="font-size: 24px;">🎨</span>
          <div>
            <strong>Однотонные цвета</strong>
            <p>Классика всегда в моде - бежевые, розовые и nude оттенки</p>
          </div>
        </div>
        <div class="trend-item">
          <span style="font-size: 24px;">💎</span>
          <div>
            <strong>Минимализм</strong>
            <p>Чистые линии и сдержанная элегантность</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="contests-modal" id="contests-modal">
  <div class="contests-content">
    <button class="close-right" onclick="closeContestsModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Конкурсы</h2>
    
    <div id="contests-container">
    </div>
  </div>
</div>

<div class="search-user-modal" id="search-user-modal">
  <div class="search-user-content">
    <button class="close-right" onclick="closeSearchUserModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Поиск клиента</h2>
    
    <div class="auth-form">
      <div class="form-group">
        <label for="search-user-input">Номер телефона или email</label>
        <input type="text" id="search-user-input" placeholder="Введите данные клиента">
      </div>
      <button class="submit-btn" onclick="searchUser()">Найти</button>
    </div>
    
    <div class="user-search-results" id="user-search-results">
    </div>
  </div>
</div>

<div class="manage-polls-modal" id="manage-polls-modal">
  <div class="manage-polls-content">
    <button class="close-right" onclick="closeManagePollsModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Управление опросами</h2>
    
    <div class="dev-polls-panel">
      <div class="dev-polls-header">
        <i class="fas fa-poll-h"></i>
        Управление опросами
      </div>
      
      <div class="dev-polls-list" id="dev-polls-list">
      </div>
      
      <div class="dev-poll-form">
        <input type="text" class="dev-poll-input" id="new-poll-question" 
               placeholder="Вопрос опроса" maxlength="100">
        <input type="text" class="dev-poll-input" id="new-poll-options" 
               placeholder="Варианты через запятую" maxlength="200">
        <button class="dev-poll-add-btn" onclick="addNewPoll()">
          <i class="fas fa-plus"></i> Добавить опрос
        </button>
      </div>
    </div>
  </div>
</div>

<div class="manage-contests-modal" id="manage-contests-modal">
  <div class="manage-contests-content">
    <button class="close-right" onclick="closeManageContestsModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Управление конкурсами</h2>
    
    <div class="dev-contests-panel">
      <div class="dev-contests-header">
        <i class="fas fa-trophy"></i>
        Управление конкурсами
      </div>
      
      <div class="dev-contests-list" id="dev-contests-list">
      </div>
      
      <div class="dev-contest-form">
        <input type="text" class="dev-contest-input" id="new-contest-title" 
               placeholder="Название конкурса" maxlength="50">
        <input type="text" class="dev-contest-input" id="new-contest-description" 
               placeholder="Описание конкурса" maxlength="200">
        <button class="dev-contest-add-btn" onclick="addNewContest()">
          <i class="fas fa-plus"></i> Добавить конкурс
        </button>
      </div>
    </div>
  </div>
</div>

<div class="manage-reviews-modal" id="manage-reviews-modal">
  <div class="manage-reviews-content">
    <button class="close-right" onclick="closeManageReviewsModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Управление отзывами</h2>
    
    <div class="dev-reviews-panel">
      <div class="dev-reviews-header">
        <i class="fas fa-star"></i>
        Управление отзывами
      </div>
      
      <div class="dev-reviews-list" id="dev-reviews-list">
      </div>
    </div>
  </div>
</div>

<div class="manage-portfolio-modal" id="manage-portfolio-modal">
  <div class="manage-portfolio-content">
    <button class="close-right" onclick="closeManagePortfolioModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Управление портфолио</h2>
    
    <div class="dev-portfolio-panel">
      <div class="dev-portfolio-header">
        <i class="fas fa-images"></i>
        Управление портфолио
      </div>
      
      <div class="dev-portfolio-list" id="dev-portfolio-list">
      </div>
      
      <div class="dev-portfolio-form">
        <input type="text" class="dev-portfolio-input" id="new-portfolio-url" 
               placeholder="URL нового изображения">
        <input type="text" class="dev-portfolio-input" id="new-portfolio-alt" 
               placeholder="Описание изображения">
        <button class="dev-portfolio-add-btn" onclick="addNewPortfolioItem()">
          <i class="fas fa-plus"></i> Добавить фото
        </button>
      </div>
    </div>
  </div>
</div>

<div class="auth-modal" id="change-username-modal">
  <div class="auth-content">
    <button class="close-right" onclick="closeChangeUsernameModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Сменить никнейм</h2>
    <p style="color:var(--muted);">Введите новый никнейм:</p>
    
    <div class="auth-form">
      <div class="form-group">
        <label for="new-username">Новый никнейм</label>
        <input type="text" id="new-username" placeholder="Введите новый никнейм">
      </div>
      
      <button class="submit-btn" onclick="changeUsername()">Сменить никнейм</button>
      <div class="success-message" id="change-username-success" style="display: none;">Никнейм успешно изменен!</div>
    </div>
  </div>
</div>

<div class="auth-modal" id="change-avatar-modal">
  <div class="auth-content">
    <button class="close-right" onclick="closeChangeAvatarModal()">&times;</button>
    <h2 style="font-family:'Playfair Display', serif; margin-bottom:10px;">Сменить аватар</h2>
    <p style="color:var(--muted);">Выберите новый аватар:</p>
    
    <div class="avatar-selection" id="avatar-selection-modal">
      <div class="avatar-option" data-avatar="💅">💅</div>
      <div class="avatar-option" data-avatar="🐻">🐻</div>
      <div class="avatar-option" data-avatar="🧸">🧸</div>
      <div class="avatar-option" data-avatar="🌸">🌸</div>
      <div class="avatar-option" data-avatar="💕">💕</div>
      <div class="avatar-option" data-avatar="⚡">⚡</div>
      <div class="avatar-option" data-avatar="🎰">🎰</div>
      <div class="avatar-option" data-avatar="🚩">🚩</div>
      <div class="avatar-option" data-avatar="💋">💋</div>
      <div class="avatar-option" data-avatar="🫦">🫦</div>
      <div class="avatar-option" data-avatar="👠">👠</div>
      <div class="avatar-option" data-avatar="👸">👸</div>
      <div class="avatar-option" data-avatar="👑">👑</div>
      <div class="avatar-option" data-avatar="✨">✨</div>
      <div class="avatar-option" data-avatar="🌟">🌟</div>
      <div class="avatar-option" data-avatar="🎀">🎀</div>
      <div class="avatar-option" data-avatar="🎨">🎨</div>
      <div class="avatar-option" data-avatar="🦄">🦄</div>
    </div>
    
    <button class="submit-btn" onclick="changeAvatar()" style="margin-top: 20px;">Сменить аватар</button>
    <div class="success-message" id="change-avatar-success" style="display: none;">Аватар успешно изменен!</div>
  </div>
</div>

<footer class="container">
  <p>Katerina Nails © 2025 — Все права защищены</p>
</footer>

<script>
// ===== ОСНОВНЫЕ ПЕРЕМЕННЫЕ =====
let currentUser = null;
let isLoggedIn = false;
let selectedPollOption = null;

const DEV_ACCOUNTS = {
    '+79881605058': {
        password: 'katerinanails',
        greeting: 'Здравствуйте, повелительница ногтей 👸💅',
        name: 'Катерина'
    },
    '+79409373796': {
        password: 'Alanchik', 
        greeting: 'Здравствуйте, повелитель борьбы 🫅🤼',
        name: 'Алан'
    }
};

const ACHIEVEMENTS = {
    firstVisit: {
        id: 'firstVisit',
        title: 'Первая запись',
        description: 'Записалась на первый маникюр',
        icon: '🎉',
        unlocked: false
    },
    fifthVisit: {
        id: 'fifthVisit',
        title: 'Постоянная клиентка',
        description: '5 успешных посещений',
        icon: '⭐',
        unlocked: false
    },
    seasonChange: {
        id: 'seasonChange',
        title: 'Сезонный дизайн',
        description: 'Смена дизайна по сезону',
        icon: '🍂',
        unlocked: false
    },
    designLover: {
        id: 'designLover',
        title: 'Любительница экспериментов',
        description: 'Попробовала 3+ разных стиля',
        icon: '🎨',
        unlocked: false
    },
    reviewMaster: {
        id: 'reviewMaster',
        title: 'Эксперт по отзывам',
        description: 'Оставила 3 отзыва с фото',
        icon: '📸',
        unlocked: false
    },
    socialButterfly: {
        id: 'socialButterfly',
        title: 'Социальная бабочка',
        description: 'Привела 2 подруги',
        icon: '🦋',
        unlocked: false
    }
};

const LOYALTY_SYSTEM = {
    visits: 0,
    points: 0,
    level: 1,
    discount: 0
};

const keys = {
  lovertx: [0,1,2,3,4],
  alanchik: [1,2,4],
  kathy228: [0,3,4],
  pinklove: [2,4],
  softy: [1,3],
  sweety15: [2],
  lovely15: [2],
  discount15: [2],
  dreamy21: [3],
  cozy21: [3],
  relax21: [3],
  cafe25: [0],
  sweet25: [0],
  choco25: [0],
  glam30: [1],
  glossy30: [1],
  beauty30: [1],
  plush35: [4],
  gift35: [4],
  pinky35: [4]
};

let reviews = JSON.parse(localStorage.getItem("reviews") || "[]");
let searchData = [
  {title:"FIRSTVISIT",price:"скидка 10%",type:"промокод",description:"первое посещение"},
  {title:"GEL5",price:"скидка 5%",type:"промокод",description:"гель-лак"},
  {title:"NAILS8",price:"скидка 8%",type:"промокод",description:"наращивание"},
  {title:"LOVE3",price:"скидка 3%",type:"промокод",description:"любые услуги"},
  {title:"Наращивание",price:"1.900₽",type:"услуга",description:"макс. длина 4"},
  {title:"Гель-лак",price:"1.500₽",type:"услуга",description:""},
  {title:"Маникюр без покрытия",price:"800₽",type:"услуга",description:""},
  {title:"Снятие чужой работы",price:"300₽",type:"услуга",description:""},
  {title:"Ремонт одного ногтя",price:"200₽",type:"услуга",description:""}
];

// ===== НОВЫЙ МАССИВ ПРИЗОВ ДЛЯ КОЛЕСА ФОРТУНЫ =====
const fortunePrizes = [
    { name: 'Сладкий кофе-шоколадка', icon: '☕️🍫', discount: 5, weight: 25, color: '#8B4513' },
    { name: 'Уходный подарок', icon: '💄🧴', discount: 8, weight: 20, color: '#F5DEB3' },
    { name: 'Дефузер домашний', icon: '🕯️', discount: 10, weight: 18, color: '#FFD700' },
    { name: 'СПА набор', icon: '💆‍♀️🧼', discount: 13, weight: 22, color: '#FFFFFF' },
    { name: 'Сумка "Лонг чамп"', icon: '👜', discount: 15, weight: 5, color: '#A0522D' },
    { name: 'Плюшевая игрушка', icon: '🧸', discount: 12, weight: 10, color: '#808080' }
];

// ===== ВСПОМОГАТЕЛЬНЫЕ ФУНКЦИИ =====
function simpleHash(str) {
    let hash = 0;
    for (let i = 0; i < str.length; i++) {
        const char = str.charCodeAt(i);
        hash = ((hash << 5) - hash) + char;
        hash = hash & hash;
    }
    return hash.toString();
}

const HASHED_PASSWORDS = {
    '+79881605058': simpleHash('katerinanails'),
    '+79409373796': simpleHash('Alanchik')
};

function checkDevAccount(phone, password) {
    const account = DEV_ACCOUNTS[phone];
    if (!account) return false;
    
    const hashedInput = simpleHash(password);
    return HASHED_PASSWORDS[phone] === hashedInput;
}

function setDevMode(userData) {
    userData.devMode = true;
    localStorage.setItem('currentUser', JSON.stringify(userData));
    showDevGreeting(userData.greeting);
    updateUIForDevMode();
}

function showDevGreeting(greeting) {
    const greetingElement = document.getElementById('dev-greeting');
    greetingElement.textContent = greeting;
    greetingElement.style.display = 'block';
    
    setTimeout(() => {
        greetingElement.style.display = 'none';
    }, 5000);
}

function updateUIForDevMode() {
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    if (currentUser && currentUser.devMode) {
        document.getElementById('dev-crown').style.display = 'inline';
        document.getElementById('prices-button').style.display = 'block';
        document.getElementById('search-user-button').style.display = 'block';
        document.getElementById('manage-polls-button').style.display = 'block';
        document.getElementById('manage-contests-button').style.display = 'block';
        document.getElementById('manage-reviews-button').style.display = 'block';
        document.getElementById('manage-portfolio-button').style.display = 'block';
        showDevPromoPanel();
        showDevPortfolioPanel();
    }
}

function showDevPromoPanel() {
    const activatedPromosContainer = document.getElementById('activated-promos');
    const devPanelHTML = `
        <div class="dev-promo-panel">
            <div class="dev-promo-header">
                <i class="fas fa-tools"></i>
                Панель управления промокодами
            </div>
            
            <div class="dev-promo-list" id="dev-promo-list">
            </div>
            
            <div class="dev-promo-form">
                <input type="text" class="dev-promo-input" id="new-promo-code" 
                       placeholder="Новый промокод" maxlength="20">
                <select class="dev-promo-percent-select" id="new-promo-percent">
                    <option value="5">5%</option>
                    <option value="10">10%</option>
                    <option value="15">15%</option>
                    <option value="20">20%</option>
                    <option value="25">25%</option>
                    <option value="30">30%</option>
                    <option value="35">35%</option>
                    <option value="40">40%</option>
                </select>
                <button class="dev-promo-add-btn" onclick="addNewPromoCode()">
                    <i class="fas fa-plus"></i> Добавить
                </button>
            </div>
        </div>
    `;
    
    activatedPromosContainer.innerHTML = devPanelHTML;
    loadDevPromoList();
}

function showDevPortfolioPanel() {
    const portfolioDevPanel = document.getElementById('portfolio-dev-panel');
    const devPanelHTML = `
        <div class="dev-portfolio-panel">
            <div class="dev-portfolio-header">
                <i class="fas fa-images"></i>
                Панель управления портфолио
            </div>
            
            <div class="dev-portfolio-list" id="dev-portfolio-list">
            </div>
            
            <div class="dev-portfolio-form">
                <input type="text" class="dev-portfolio-input" id="new-portfolio-url" 
                       placeholder="URL нового изображения">
                <input type="text" class="dev-portfolio-input" id="new-portfolio-alt" 
                       placeholder="Описание изображения">
                <button class="dev-portfolio-add-btn" onclick="addNewPortfolioItem()">
                    <i class="fas fa-plus"></i> Добавить фото
                </button>
            </div>
        </div>
    `;
    
    portfolioDevPanel.innerHTML = devPanelHTML;
    portfolioDevPanel.style.display = 'block';
    loadDevPortfolioList();
}

function loadDevPortfolioList() {
    const portfolioItems = JSON.parse(localStorage.getItem('portfolioItems') || '[]');
    const devPortfolioList = document.getElementById('dev-portfolio-list');
    
    if (portfolioItems.length === 0) {
        devPortfolioList.innerHTML = '<div style="padding: 20px; text-align: center; color: var(--muted);">Нет элементов в портфолио</div>';
        return;
    }
    
    devPortfolioList.innerHTML = portfolioItems.map((item, index) => `
        <div class="dev-portfolio-item">
            <div>
                <span class="dev-portfolio-name">${item.alt}</span>
            </div>
            <div>
                <button class="dev-portfolio-edit" onclick="editPortfolioItem(${index})">
                    <i class="fas fa-edit"></i> Изменить
                </button>
                <button class="dev-portfolio-delete" onclick="deletePortfolioItem(${index})">
                    <i class="fas fa-trash"></i> Удалить
                </button>
            </div>
        </div>
    `).join('');
}

function addNewPortfolioItem() {
    const urlInput = document.getElementById('new-portfolio-url');
    const altInput = document.getElementById('new-portfolio-alt');
    
    const url = urlInput.value.trim();
    const alt = altInput.value.trim();
    
    if (!url) {
        alert('Введите URL изображения');
        return;
    }
    
    if (!alt) {
        alert('Введите описание изображения');
        return;
    }
    
    const portfolioItems = JSON.parse(localStorage.getItem('portfolioItems') || '[]');
    
    const newItem = {
        src: url,
        alt: alt,
        id: 'custom-' + Date.now()
    };
    
    portfolioItems.push(newItem);
    localStorage.setItem('portfolioItems', JSON.stringify(portfolioItems));
    
    urlInput.value = '';
    altInput.value = '';
    
    loadDevPortfolioList();
    displayPortfolio();
    
    showSuccessMessage('Новое фото добавлено в портфолио!');
}

function editPortfolioItem(index) {
    const portfolioItems = JSON.parse(localStorage.getItem('portfolioItems') || '[]');
    const item = portfolioItems[index];
    
    const newUrl = prompt('Введите новый URL изображения:', item.src);
    if (newUrl === null) return;
    
    const newAlt = prompt('Введите новое описание изображения:', item.alt);
    if (newAlt === null) return;
    
    portfolioItems[index].src = newUrl.trim();
    portfolioItems[index].alt = newAlt.trim();
    
    localStorage.setItem('portfolioItems', JSON.stringify(portfolioItems));
    
    loadDevPortfolioList();
    displayPortfolio();
    
    showSuccessMessage('Фото обновлено!');
}

function deletePortfolioItem(index) {
    if (!confirm('Удалить это фото из портфолио?')) return;
    
    const portfolioItems = JSON.parse(localStorage.getItem('portfolioItems') || '[]');
    portfolioItems.splice(index, 1);
    
    localStorage.setItem('portfolioItems', JSON.stringify(portfolioItems));
    
    loadDevPortfolioList();
    displayPortfolio();
    
    showSuccessMessage('Фото удалено из портфолио');
}

function loadDevPromoList() {
    const allPromoCodes = JSON.parse(localStorage.getItem('allPromoCodes') || '[]');
    const devPromoList = document.getElementById('dev-promo-list');
    
    if (allPromoCodes.length === 0) {
        devPromoList.innerHTML = '<div style="padding: 20px; text-align: center; color: var(--muted);">Нет активных промокодов</div>';
        return;
    }
    
    devPromoList.innerHTML = allPromoCodes.map(promo => `
        <div class="dev-promo-item">
            <div>
                <span class="dev-promo-code">${promo.code}</span>
                <span class="dev-promo-percent">-${promo.percent}%</span>
            </div>
            <button class="dev-promo-delete" onclick="deletePromoCode('${promo.code}')">
                <i class="fas fa-trash"></i> Удалить
            </button>
        </div>
    `).join('');
}

function addNewPromoCode() {
    const codeInput = document.getElementById('new-promo-code');
    const percentSelect = document.getElementById('new-promo-percent');
    
    const code = codeInput.value.trim().toUpperCase();
    const percent = parseInt(percentSelect.value);
    
    if (!code) {
        alert('Введите код промокода');
        return;
    }
    
    if (code.length < 3) {
        alert('Код промокода должен содержать минимум 3 символа');
        return;
    }
    
    const allPromoCodes = JSON.parse(localStorage.getItem('allPromoCodes') || '[]');
    
    if (allPromoCodes.find(promo => promo.code === code)) {
        alert('Промокод с таким кодом уже существует');
        return;
    }
    
    const newPromo = {
        code: code,
        percent: percent,
        createdBy: JSON.parse(localStorage.getItem('currentUser')).phone,
        createdAt: new Date().toISOString()
    };
    
    allPromoCodes.push(newPromo);
    localStorage.setItem('allPromoCodes', JSON.stringify(allPromoCodes));
    
    updatePromoCodesForAllUsers();
    
    codeInput.value = '';
    
    showSuccessMessage(`Промокод ${code} добавлен!`);
}

function updatePromoCodesForAllUsers() {
    const allPromoCodes = JSON.parse(localStorage.getItem('allPromoCodes') || '[]');
    
    const defaultPromocodes = document.getElementById('default-promocodes');
    if (allPromoCodes.length > 0) {
        defaultPromocodes.innerHTML = allPromoCodes.map(promo => 
            `<strong style="color:var(--primary)">${promo.code}</strong> - скидка ${promo.percent}%<br>`
        ).join('');
    }
    
    const bookingPromocodes = document.getElementById('booking-promocodes');
    const bookingPromoDescription = document.getElementById('booking-promo-description');
    
    if (allPromoCodes.length > 0) {
        bookingPromocodes.innerHTML = allPromoCodes.map(promo => 
            `<div class="promo-code">${promo.code}<div class="promo-discount">-${promo.percent}%</div></div>`
        ).join('');
        
        bookingPromoDescription.innerHTML = allPromoCodes.map(promo => 
            `<strong>${promo.code}</strong> - скидка ${promo.percent}%<br>`
        ).join('');
    }
}

function deletePromoCode(code) {
    if (!confirm(`Удалить промокод ${code}?`)) return;
    
    const allPromoCodes = JSON.parse(localStorage.getItem('allPromoCodes') || '[]');
    const updatedPromoCodes = allPromoCodes.filter(promo => promo.code !== code);
    
    localStorage.setItem('allPromoCodes', JSON.stringify(updatedPromoCodes));
    
    updatePromoCodesForAllUsers();
    
    showSuccessMessage(`Промокод ${code} удален`);
}

function loadServices() {
    let services = JSON.parse(localStorage.getItem('services'));
    
    if (!services) {
        services = [
            { id: 1, name: 'Наращивание', description: '(макс. длина 4)', price: '1.900₽', originalPrice: 1900 },
            { id: 2, name: 'Гель-лак', description: '', price: '1.500₽', originalPrice: 1500 },
            { id: 3, name: 'Маникюр без покрытия', description: '', price: '800₽', originalPrice: 800 },
            { id: 4, name: 'Снятие чужой работы', description: '', price: '300₽', originalPrice: 300 },
            { id: 5, name: 'Ремонт одного ногтя', description: '', price: '200₽', originalPrice: 200 }
        ];
        localStorage.setItem('services', JSON.stringify(services));
    }
    
    return services;
}

function saveServices(services) {
    localStorage.setItem('services', JSON.stringify(services));
}

function displayServices() {
    const services = loadServices();
    const servicesContainer = document.getElementById('services-container');
    
    servicesContainer.innerHTML = services.map(service => `
        <div class="note" data-service="${service.name}">
            <div class="note-row">
                <div>
                    <div class="note-title">${service.name}</div>
                    ${service.description ? `<div class="note-sub">${service.description}</div>` : ''}
                </div>
                <div class="note-price">${service.price}</div>
            </div>
        </div>
    `).join('');
    
    updateSearchData(services);
}

function updateSearchData(services) {
    searchData = searchData.filter(item => item.type !== 'услуга');
    
    services.forEach(service => {
        searchData.push({
            title: service.name,
            price: service.price,
            type: 'услуга',
            description: service.description
        });
    });
}

function openPricesModal() {
    document.getElementById('prices-modal').style.display = 'flex';
    loadPricesForEditing();
}

function closePricesModal() {
    document.getElementById('prices-modal').style.display = 'none';
}

function loadPricesForEditing() {
    const services = loadServices();
    const pricesList = document.getElementById('dev-prices-list');
    
    pricesList.innerHTML = services.map(service => `
        <div class="dev-price-item">
            <div>
                <span class="dev-price-name">${service.name}</span>
                <span class="dev-price-value">${service.price}</span>
            </div>
            <div>
                <input type="number" class="dev-price-input" id="price-${service.id}" 
                       value="${service.originalPrice}" style="width: 80px; margin-right: 10px;">
                <button class="dev-price-edit" onclick="updateServicePrice(${service.id})">
                    <i class="fas fa-save"></i> Сохранить
                </button>
                <button class="dev-price-delete" onclick="deleteService(${service.id})" style="background: #e74c3c; margin-left: 5px;">
                    <i class="fas fa-trash"></i> Удалить
                </button>
            </div>
        </div>
    `).join('');
    
    pricesList.innerHTML += `
        <div class="add-service-form">
            <input type="text" class="add-service-input" id="new-service-name" placeholder="Название услуги">
            <input type="text" class="add-service-input" id="new-service-description" placeholder="Описание (необязательно)">
            <input type="number" class="add-service-input" id="new-service-price" placeholder="Цена" min="0">
            <button class="add-service-btn" onclick="addNewService()" style="grid-column: 1 / -1;">
                <i class="fas fa-plus"></i> Добавить услугу
            </button>
        </div>
    `;
}

function updateServicePrice(serviceId) {
    const newPriceInput = document.getElementById(`price-${serviceId}`);
    const newPrice = parseInt(newPriceInput.value);
    
    if (isNaN(newPrice) || newPrice < 0) {
        alert('Введите корректную цену');
        return;
    }
    
    let services = loadServices();
    const serviceIndex = services.findIndex(service => service.id === serviceId);
    
    if (serviceIndex !== -1) {
        services[serviceIndex].originalPrice = newPrice;
        services[serviceIndex].price = `${newPrice.toLocaleString()}₽`;
        
        saveServices(services);
        displayServices();
        
        showSuccessMessage(`Цена для "${services[serviceIndex].name}" обновлена!`);
    }
}

function addNewService() {
    const nameInput = document.getElementById('new-service-name');
    const descriptionInput = document.getElementById('new-service-description');
    const priceInput = document.getElementById('new-service-price');
    
    const name = nameInput.value.trim();
    const description = descriptionInput.value.trim();
    const price = parseInt(priceInput.value);
    
    if (!name) {
        alert('Введите название услуги');
        return;
    }
    
    if (isNaN(price) || price < 0) {
        alert('Введите корректную цену');
        return;
    }
    
    let services = loadServices();
    const newId = services.length > 0 ? Math.max(...services.map(s => s.id)) + 1 : 1;
    
    const newService = {
        id: newId,
        name: name,
        description: description,
        price: `${price.toLocaleString()}₽`,
        originalPrice: price
    };
    
    services.push(newService);
    saveServices(services);
    displayServices();
    
    nameInput.value = '';
    descriptionInput.value = '';
    priceInput.value = '';
    
    showSuccessMessage(`Услуга "${name}" добавлена!`);
}

function deleteService(serviceId) {
    if (!confirm('Удалить эту услугу?')) return;
    
    let services = loadServices();
    const serviceIndex = services.findIndex(service => service.id === serviceId);
    
    if (serviceIndex !== -1) {
        const serviceName = services[serviceIndex].name;
        services.splice(serviceIndex, 1);
        saveServices(services);
        displayServices();
        loadPricesForEditing();
        
        showSuccessMessage(`Услуга "${serviceName}" удалена!`);
    }
}

function initUserDatabase() {
    if (!localStorage.getItem('userDatabase')) {
        localStorage.setItem('userDatabase', JSON.stringify([]));
    }
}

function saveUserToDatabase(userData) {
    const userDatabase = JSON.parse(localStorage.getItem('userDatabase') || '[]');
    
    const existingUserIndex = userDatabase.findIndex(user => 
        user.phone === userData.phone || user.email === userData.email
    );
    
    if (existingUserIndex !== -1) {
        userDatabase[existingUserIndex] = {
            ...userDatabase[existingUserIndex],
            ...userData,
            lastLogin: new Date().toISOString()
        };
    } else {
        userData.id = generateUserId();
        userData.registrationDate = new Date().toISOString();
        userData.lastLogin = new Date().toISOString();
        userData.visits = 0;
        userData.points = 0;
        userDatabase.push(userData);
        
        if (userDatabase.length > 500) {
            userDatabase.shift();
        }
    }
    
    localStorage.setItem('userDatabase', JSON.stringify(userDatabase));
}

function generateUserId() {
    return 'user_' + Date.now() + '_' + Math.random().toString(36).substr(2, 9);
}

function searchUserInDatabase(query) {
    const userDatabase = JSON.parse(localStorage.getItem('userDatabase') || '[]');
    
    return userDatabase.filter(user => 
        user.phone.includes(query) || 
        user.email.includes(query) ||
        user.username.toLowerCase().includes(query.toLowerCase())
    );
}

function initPortfolioLikes() {
    if (!localStorage.getItem('portfolioLikes')) {
        const defaultLikes = {
            'IMG-0064.jpg': { likes: 0, userLikes: {} },
            'IMG-0066.jpg': { likes: 0, userLikes: {} },
            'IMG-0067.jpg': { likes: 0, userLikes: {} },
            'IMG-0023.jpg': { likes: 0, userLikes: {} },
            'IMG-0025.jpg': { likes: 0, userLikes: {} },
            'IMG-0027.jpg': { likes: 0, userLikes: {} },
            'IMG-0028.jpg': { likes: 0, userLikes: {} }
        };
        localStorage.setItem('portfolioLikes', JSON.stringify(defaultLikes));
    }
}

function displayPortfolio() {
    const portfolioLikes = JSON.parse(localStorage.getItem('portfolioLikes') || '{}');
    const portfolioGrid = document.getElementById('portfolio-grid');
    
    let portfolioItems = JSON.parse(localStorage.getItem('portfolioItems') || '[]');
    
    // Добавляем стандартные элементы, если пользовательские отсутствуют
    if (portfolioItems.length === 0) {
        portfolioItems = [
            { src: 'https://i.postimg.cc/g04rPcvB/IMG-0064.jpg', alt: 'Наращивание ногтей', id: 'IMG-0064.jpg' },
            { src: 'https://i.postimg.cc/25C3JLBM/IMG-0066.jpg', alt: 'Гель-лак дизайн', id: 'IMG-0066.jpg' },
            { src: 'https://i.postimg.cc/FRMLr2gk/IMG-0067.jpg', alt: 'Маникюр с росписью', id: 'IMG-0067.jpg' },
            { src: 'https://i.postimg.cc/cJRdP2kC/IMG-0023.jpg', alt: 'Френч маникюр', id: 'IMG-0023.jpg' },
            { src: 'https://i.postimg.cc/Dzr7RHpZ/IMG-0025.jpg', alt: 'Свадебный маникюр', id: 'IMG-0025.jpg' },
            { src: 'https://i.postimg.cc/YS6tTZDC/IMG-0027.jpg', alt: 'Вечерний маникюр', id: 'IMG-0027.jpg' },
            { src: 'https://i.postimg.cc/9fdcsKgf/IMG-0028.jpg', alt: 'Повседневный маникюр', id: 'IMG-0028.jpg' }
        ];
        localStorage.setItem('portfolioItems', JSON.stringify(portfolioItems));
    }
    
    portfolioGrid.innerHTML = portfolioItems.map(item => {
        const likesData = portfolioLikes[item.id] || { likes: 0, userLikes: {} };
        const currentUser = JSON.parse(localStorage.getItem('currentUser'));
        const isLiked = currentUser && likesData.userLikes[currentUser.id];
        
        return `
            <div class="portfolio-item">
                <a href="${item.src}" target="_blank">
                    <img src="${item.src}" alt="${item.alt}">
                </a>
                <div class="portfolio-like ${isLiked ? 'liked' : ''}" onclick="togglePortfolioLike('${item.id}')">
                    <i class="fas fa-heart"></i>
                </div>
                <div class="portfolio-likes-count">${likesData.likes}</div>
            </div>
        `;
    }).join('');
}

function togglePortfolioLike(photoId) {
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    if (!currentUser) {
        alert('Для оценки фото необходимо авторизоваться!');
        openAuthModal();
        return;
    }
    
    const portfolioLikes = JSON.parse(localStorage.getItem('portfolioLikes') || '{}');
    if (!portfolioLikes[photoId]) {
        portfolioLikes[photoId] = { likes: 0, userLikes: {} };
    }
    
    const likesData = portfolioLikes[photoId];
    
    if (likesData.userLikes[currentUser.id]) {
        likesData.likes--;
        delete likesData.userLikes[currentUser.id];
    } else {
        likesData.likes++;
        likesData.userLikes[currentUser.id] = true;
    }
    
    localStorage.setItem('portfolioLikes', JSON.stringify(portfolioLikes));
    displayPortfolio();
}

function initPollSystem() {
    if (!localStorage.getItem('polls')) {
        const defaultPoll = {
            id: 1,
            question: "Какой дизайн вам нравится больше?",
            options: [
                { id: 'french', name: "Френч", votes: 0 },
                { id: 'gradient', name: "Градиент", votes: 0 },
                { id: 'marble', name: "Мрамор", votes: 0 }
            ],
            userVotes: {},
            active: true
        };
        localStorage.setItem('polls', JSON.stringify([defaultPoll]));
    }
}

function getActivePolls() {
    const polls = JSON.parse(localStorage.getItem('polls') || '[]');
    return polls.filter(poll => poll.active);
}

function displayCurrentPoll() {
    const polls = getActivePolls();
    if (polls.length === 0) {
        document.getElementById('current-poll').innerHTML = '<p>В настоящее время нет активных опросов</p>';
        return;
    }
    
    const currentPoll = polls[0];
    document.getElementById('poll-question').textContent = currentPoll.question;
    
    const pollOptions = document.getElementById('poll-options');
    pollOptions.innerHTML = '';
    
    currentPoll.options.forEach(option => {
        const optionElement = document.createElement('div');
        optionElement.className = 'poll-option';
        optionElement.innerHTML = `
            <span>${option.name}</span>
            <span id="${option.id}-count">${option.votes}</span>
        `;
        optionElement.onclick = () => selectPollOption(option.id);
        pollOptions.appendChild(optionElement);
    });
    
    selectedPollOption = null;
    document.getElementById('vote-button').disabled = true;
    
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    if (currentUser && currentPoll.userVotes[currentUser.id]) {
        showPollResults();
    } else {
        document.getElementById('poll-results').style.display = 'none';
        document.getElementById('vote-button').style.display = 'block';
    }
}

function selectPollOption(optionId) {
    document.querySelectorAll('.poll-option').forEach(option => {
        option.classList.remove('selected');
    });
    
    const selectedOption = Array.from(document.querySelectorAll('.poll-option')).find(option => 
        option.querySelector('span:first-child').textContent === getOptionName(optionId)
    );
    if (selectedOption) {
        selectedOption.classList.add('selected');
    }
    
    selectedPollOption = optionId;
    document.getElementById('vote-button').disabled = false;
}

function getOptionName(optionId) {
    const polls = JSON.parse(localStorage.getItem('polls') || '[]');
    const currentPoll = polls[0];
    const option = currentPoll.options.find(opt => opt.id === optionId);
    return option ? option.name : '';
}

function submitVote() {
    if (!selectedPollOption) {
        alert('Пожалуйста, выберите вариант для голосования');
        return;
    }
    
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    if (!currentUser) {
        alert('Для голосования необходимо авторизоваться!');
        openAuthModal();
        return;
    }
    
    const polls = JSON.parse(localStorage.getItem('polls') || '[]');
    const currentPoll = polls[0];
    
    if (currentPoll.userVotes[currentUser.id]) {
        alert('Вы уже голосовали в этом опросе!');
        return;
    }
    
    const optionIndex = currentPoll.options.findIndex(opt => opt.id === selectedPollOption);
    if (optionIndex !== -1) {
        currentPoll.options[optionIndex].votes++;
        currentPoll.userVotes[currentUser.id] = selectedPollOption;
        
        localStorage.setItem('polls', JSON.stringify(polls));
        
        addLoyaltyPoints(10, 'Участие в опросе');
        
        showSuccessMessage('Спасибо за ваш голос!');
        showPollResults();
    }
}

function showPollResults() {
    const polls = JSON.parse(localStorage.getItem('polls') || '[]');
    const currentPoll = polls[0];
    
    const totalVotes = currentPoll.options.reduce((sum, option) => sum + option.votes, 0);
    
    if (totalVotes > 0) {
        const resultsContainer = document.getElementById('poll-results-container');
        resultsContainer.innerHTML = '';
        
        currentPoll.options.forEach(option => {
            const percent = Math.round((option.votes / totalVotes) * 100);
            const resultItem = document.createElement('div');
            resultItem.className = 'poll-result-item';
            resultItem.innerHTML = `
                <div>${option.name}: <span>${percent}%</span></div>
                <div class="poll-result-bar">
                    <div class="poll-result-fill" style="width: ${percent}%"></div>
                </div>
            `;
            resultsContainer.appendChild(resultItem);
        });
        
        document.getElementById('poll-results').style.display = 'block';
        document.getElementById('vote-button').style.display = 'none';
    }
}

function initContestSystem() {
    if (!localStorage.getItem('contests')) {
        const defaultContests = [
            {
                id: 1,
                title: "Лучший маникюр месяца",
                description: "Присылайте фото вашего маникюра в Instagram с хештегом #KnailsContest",
                participants: [],
                active: true
            },
            {
                id: 2,
                title: "Сезонный конкурс",
                description: "Осенний маникюр - можно выиграть скидку",
                participants: [],
                active: true
            }
        ];
        localStorage.setItem('contests', JSON.stringify(defaultContests));
    }
}

function getActiveContests() {
    const contests = JSON.parse(localStorage.getItem('contests') || '[]');
    return contests.filter(contest => contest.active);
}

function displayContests() {
    const contests = getActiveContests();
    const contestsContainer = document.getElementById('contests-container');
    
    if (contests.length === 0) {
        contestsContainer.innerHTML = '<p>В настоящее время нет активных конкурсов</p>';
        return;
    }
    
    contestsContainer.innerHTML = contests.map(contest => `
        <div class="contest-item" style="background: white; padding: 20px; border-radius: var(--radius); margin-bottom: 20px; box-shadow: var(--shadow);">
            <h3 style="color: var(--primary); margin-bottom: 10px;">${contest.title}</h3>
            <p style="color: var(--muted); margin-bottom: 15px;">${contest.description}</p>
            <button class="submit-btn" onclick="participateContest(${contest.id})">
                <i class="fas fa-trophy"></i> Участвовать
            </button>
        </div>
    `).join('');
}

function participateContest(contestId) {
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    if (!currentUser) {
        alert('Для участия в конкурсе необходимо авторизоваться!');
        openAuthModal();
        return;
    }
    
    const contests = JSON.parse(localStorage.getItem('contests') || '[]');
    const contestIndex = contests.findIndex(contest => contest.id === contestId);
    
    if (contestIndex !== -1) {
        const contest = contests[contestIndex];
        
        if (contest.participants.includes(currentUser.id)) {
            alert('Вы уже участвуете в этом конкурсе!');
            return;
        }
        
        contest.participants.push(currentUser.id);
        localStorage.setItem('contests', JSON.stringify(contests));
        
        addLoyaltyPoints(20, 'Участие в конкурсе');
        
        alert(`Вы успешно зарегистрировались в конкурсе "${contest.title}"!`);
        unlockAchievement('socialButterfly');
    }
}

function openManagePollsModal() {
    document.getElementById('manage-polls-modal').style.display = 'flex';
    loadPollsForEditing();
}

function closeManagePollsModal() {
    document.getElementById('manage-polls-modal').style.display = 'none';
}

function loadPollsForEditing() {
    const polls = JSON.parse(localStorage.getItem('polls') || '[]');
    const pollsList = document.getElementById('dev-polls-list');
    
    if (polls.length === 0) {
        pollsList.innerHTML = '<div style="padding: 20px; text-align: center; color: var(--muted);">Нет активных опросов</div>';
        return;
    }
    
    pollsList.innerHTML = polls.map(poll => `
        <div class="dev-poll-item">
            <div>
                <span class="dev-poll-name">${poll.question}</span>
                <span class="dev-poll-votes">${poll.options.reduce((sum, opt) => sum + opt.votes, 0)} голосов</span>
            </div>
            <div>
                <button class="dev-poll-delete" onclick="deletePoll(${poll.id})">
                    <i class="fas fa-trash"></i> Удалить
                </button>
            </div>
        </div>
    `).join('');
}

function addNewPoll() {
    const questionInput = document.getElementById('new-poll-question');
    const optionsInput = document.getElementById('new-poll-options');
    
    const question = questionInput.value.trim();
    const optionsText = optionsInput.value.trim();
    
    if (!question) {
        alert('Введите вопрос опроса');
        return;
    }
    
    if (!optionsText) {
        alert('Введите варианты ответов через запятую');
        return;
    }
    
    const options = optionsText.split(',').map(opt => ({
        id: generateOptionId(opt.trim()),
        name: opt.trim(),
        votes: 0
    })).filter(opt => opt.name.length > 0);
    
    if (options.length < 2) {
        alert('Должно быть как минимум 2 варианта ответа');
        return;
    }
    
    const polls = JSON.parse(localStorage.getItem('polls') || '[]');
    
    polls.forEach(poll => {
        poll.active = false;
    });
    
    const newPoll = {
        id: polls.length > 0 ? Math.max(...polls.map(p => p.id)) + 1 : 1,
        question: question,
        options: options,
        userVotes: {},
        active: true
    };
    
    polls.push(newPoll);
    localStorage.setItem('polls', JSON.stringify(polls));
    
    loadPollsForEditing();
    displayCurrentPoll();
    
    questionInput.value = '';
    optionsInput.value = '';
    
    showSuccessMessage('Новый опрос добавлен!');
}

function generateOptionId(optionName) {
    return optionName.toLowerCase().replace(/[^a-z0-9]/g, '_');
}

function deletePoll(pollId) {
    if (!confirm('Удалить этот опрос?')) return;
    
    const polls = JSON.parse(localStorage.getItem('polls') || '[]');
    const updatedPolls = polls.filter(poll => poll.id !== pollId);
    
    localStorage.setItem('polls', JSON.stringify(updatedPolls));
    loadPollsForEditing();
    displayCurrentPoll();
    
    showSuccessMessage('Опрос удален');
}

function openManageContestsModal() {
    document.getElementById('manage-contests-modal').style.display = 'flex';
    loadContestsForEditing();
}

function closeManageContestsModal() {
    document.getElementById('manage-contests-modal').style.display = 'none';
}

function loadContestsForEditing() {
    const contests = JSON.parse(localStorage.getItem('contests') || '[]');
    const contestsList = document.getElementById('dev-contests-list');
    
    if (contests.length === 0) {
        contestsList.innerHTML = '<div style="padding: 20px; text-align: center; color: var(--muted);">Нет активных конкурсов</div>';
        return;
    }
    
    contestsList.innerHTML = contests.map(contest => `
        <div class="dev-contest-item">
            <div>
                <span class="dev-contest-name">${contest.title}</span>
                <span class="dev-contest-participants">${contest.participants.length} участников</span>
            </div>
            <div>
                <button class="dev-contest-delete" onclick="deleteContest(${contest.id})">
                    <i class="fas fa-trash"></i> Удалить
                </button>
            </div>
        </div>
    `).join('');
}

function addNewContest() {
    const titleInput = document.getElementById('new-contest-title');
    const descriptionInput = document.getElementById('new-contest-description');
    
    const title = titleInput.value.trim();
    const description = descriptionInput.value.trim();
    
    if (!title) {
        alert('Введите название конкурса');
        return;
    }
    
    if (!description) {
        alert('Введите описание конкурса');
        return;
    }
    
    const contests = JSON.parse(localStorage.getItem('contests') || '[]');
    
    if (contests.length >= 3) {
        alert('Максимальное количество конкурсов - 3. Удалите один из существующих конкурсов, чтобы добавить новый.');
        return;
    }
    
    const newContest = {
        id: contests.length > 0 ? Math.max(...contests.map(c => c.id)) + 1 : 1,
        title: title,
        description: description,
        participants: [],
        active: true
    };
    
    contests.push(newContest);
    localStorage.setItem('contests', JSON.stringify(contests));
    
    loadContestsForEditing();
    displayContests();
    
    titleInput.value = '';
    descriptionInput.value = '';
    
    showSuccessMessage('Новый конкурс добавлен!');
}

function deleteContest(contestId) {
    if (!confirm('Удалить этот конкурс?')) return;
    
    const contests = JSON.parse(localStorage.getItem('contests') || '[]');
    const updatedContests = contests.filter(contest => contest.id !== contestId);
    
    localStorage.setItem('contests', JSON.stringify(updatedContests));
    loadContestsForEditing();
    displayContests();
    
    showSuccessMessage('Конкурс удален');
}

function openManageReviewsModal() {
    document.getElementById('manage-reviews-modal').style.display = 'flex';
    loadReviewsForEditing();
}

function closeManageReviewsModal() {
    document.getElementById('manage-reviews-modal').style.display = 'none';
}

function loadReviewsForEditing() {
    const reviews = JSON.parse(localStorage.getItem("reviews") || "[]");
    const reviewsList = document.getElementById('dev-reviews-list');
    
    if (reviews.length === 0) {
        reviewsList.innerHTML = '<div style="padding: 20px; text-align: center; color: var(--muted);">Нет отзывов</div>';
        return;
    }
    
    reviewsList.innerHTML = reviews.map((review, index) => `
        <div class="dev-review-item">
            <div>
                <span class="dev-review-author">
                    <span style="font-size: 16px; margin-right: 5px;">${review.authorAvatar || '💅'}</span>
                    ${review.author}
                    ${review.pinned ? '<span style="color: var(--accent); margin-left: 5px;">📌</span>' : ''}
                </span>
                <span class="dev-review-date">${new Date(review.date).toLocaleDateString()}</span>
            </div>
            <div>
                <button class="dev-review-pin" onclick="toggleReviewPin(${index})">
                    <i class="fas fa-thumbtack"></i> ${review.pinned ? 'Открепить' : 'Закрепить'}
                </button>
                <button class="dev-review-delete" onclick="deleteReview(${index})">
                    <i class="fas fa-trash"></i> Удалить
                </button>
            </div>
        </div>
    `).join('');
    
    if (reviews.length > 0) {
        reviewsList.innerHTML += `
            <button class="dev-review-clear-all" onclick="clearAllReviews()">
                <i class="fas fa-trash-alt"></i> Очистить все отзывы
            </button>
        `;
    }
}

function toggleReviewPin(index) {
    const reviews = JSON.parse(localStorage.getItem("reviews") || "[]");
    reviews[index].pinned = !reviews[index].pinned;
    localStorage.setItem("reviews", JSON.stringify(reviews));
    loadReviewsForEditing();
    displayReviews();
    showSuccessMessage(`Отзыв ${reviews[index].pinned ? 'закреплен' : 'откреплен'}!`);
}

function deleteReview(index) {
    if (!confirm('Удалить этот отзыв?')) return;
    
    const reviews = JSON.parse(localStorage.getItem("reviews") || "[]");
    reviews.splice(index, 1);
    localStorage.setItem("reviews", JSON.stringify(reviews));
    loadReviewsForEditing();
    displayReviews();
    showSuccessMessage('Отзыв удален');
}

function clearAllReviews() {
    if (!confirm('Вы уверены, что хотите удалить ВСЕ отзывы? Это действие нельзя отменить.')) {
        return;
    }
    
    localStorage.setItem("reviews", JSON.stringify([]));
    reviews = [];
    displayReviews();
    loadReviewsForEditing();
    
    showSuccessMessage('Все отзывы удалены!');
}

function openManagePortfolioModal() {
    document.getElementById('manage-portfolio-modal').style.display = 'flex';
    loadDevPortfolioList();
}

function closeManagePortfolioModal() {
    document.getElementById('manage-portfolio-modal').style.display = 'none';
}

function loadAchievements() {
    const saved = JSON.parse(localStorage.getItem('userAchievements') || '{}');
    Object.keys(ACHIEVEMENTS).forEach(key => {
        ACHIEVEMENTS[key].unlocked = saved[key] || false;
    });
    displayAchievements();
}

function displayAchievements() {
    const container = document.getElementById('account-achievements-container');
    container.innerHTML = Object.values(ACHIEVEMENTS).map(achievement => `
        <div class="achievement-card ${achievement.unlocked ? 'unlocked' : 'locked'}">
            ${achievement.unlocked ? '<div class="achievement-badge">✓</div>' : ''}
            <div class="achievement-icon">${achievement.icon}</div>
            <div class="achievement-title">${achievement.title}</div>
            <div class="achievement-desc">${achievement.description}</div>
        </div>
    `).join('');
}

function unlockAchievement(achievementId) {
    if (ACHIEVEMENTS[achievementId] && !ACHIEVEMENTS[achievementId].unlocked) {
        ACHIEVEMENTS[achievementId].unlocked = true;
        localStorage.setItem('userAchievements', JSON.stringify(
            Object.fromEntries(
                Object.entries(ACHIEVEMENTS).map(([key, value]) => [key, value.unlocked])
            )
        ));
        
        showAchievementNotification(ACHIEVEMENTS[achievementId]);
        displayAchievements();
    }
}

function showAchievementNotification(achievement) {
    const notification = document.createElement('div');
    notification.className = 'gamification-badge';
    notification.innerHTML = `
        <div style="text-align: center;">
            <div style="font-size: 32px; margin-bottom: 8px;">${achievement.icon}</div>
            <div style="font-weight: 600; margin-bottom: 4px;">Достижение разблокировано!</div>
            <div style="font-size: 14px;">${achievement.title}</div>
        </div>
    `;
    document.body.appendChild(notification);
    
    setTimeout(() => {
        notification.remove();
    }, 5000);
}

function loadLoyaltyData() {
    const saved = JSON.parse(localStorage.getItem('loyaltyData') || '{}');
    Object.assign(LOYALTY_SYSTEM, saved);
    updateLoyaltyDisplay();
}

function updateLoyaltyDisplay() {
    document.getElementById('account-visits-count').textContent = LOYALTY_SYSTEM.visits;
    document.getElementById('account-points-count').textContent = LOYALTY_SYSTEM.points;
    document.getElementById('account-discount-percent').textContent = LOYALTY_SYSTEM.discount + '%';
    
    const progress = (LOYALTY_SYSTEM.points % 100) / 100 * 100;
    document.getElementById('account-loyalty-progress').style.width = progress + '%';
    document.getElementById('account-points-to-next').textContent = 100 - (LOYALTY_SYSTEM.points % 100);
}

function addLoyaltyPoints(points, reason) {
    LOYALTY_SYSTEM.points += points;
    LOYALTY_SYSTEM.visits++;
    
    const newLevel = Math.floor(LOYALTY_SYSTEM.points / 100) + 1;
    if (newLevel > LOYALTY_SYSTEM.level) {
        LOYALTY_SYSTEM.level = newLevel;
        LOYALTY_SYSTEM.discount = Math.min(25, (newLevel - 1) * 5);
        showLevelUpNotification(newLevel);
    }
    
    localStorage.setItem('loyaltyData', JSON.stringify(LOYALTY_SYSTEM));
    updateLoyaltyDisplay();
    
    if (LOYALTY_SYSTEM.visits === 1) unlockAchievement('firstVisit');
    if (LOYALTY_SYSTEM.visits === 5) unlockAchievement('fifthVisit');
}

function showLevelUpNotification(level) {
    const notification = document.createElement('div');
    notification.className = 'gamification-badge';
    notification.innerHTML = `
        <div style="text-align: center;">
            <div style="font-size: 32px; margin-bottom: 8px;">🎊</div>
            <div style="font-weight: 600; margin-bottom: 4px;">Новый уровень!</div>
            <div style="font-size: 14px;">Теперь у вас ${level * 5}% скидка</div>
        </div>
    `;
    document.body.appendChild(notification);
    
    setTimeout(() => {
        notification.remove();
    }, 5000);
}

function searchUser() {
    const searchInput = document.getElementById('search-user-input').value.trim();
    if (!searchInput) {
        alert('Введите данные для поиска');
        return;
    }
    
    const userDatabase = JSON.parse(localStorage.getItem('userDatabase') || '[]');
    const results = userDatabase.filter(user => 
        user.phone.includes(searchInput) || 
        user.email.includes(searchInput) ||
        user.username.toLowerCase().includes(searchInput.toLowerCase())
    );
    
    displayUserResults(results);
}

function displayUserResults(users) {
    const resultsContainer = document.getElementById('user-search-results');
    
    if (users.length === 0) {
        resultsContainer.innerHTML = '<div style="text-align: center; color: var(--muted); padding: 20px;">Пользователи не найдены</div>';
        return;
    }
    
    resultsContainer.innerHTML = users.map(user => `
        <div class="user-result-item">
            <div>
                <div style="font-weight: 600;">${user.username}</div>
                <div style="font-size: 12px; color: var(--muted);">${user.phone} • ${user.email}</div>
                <div style="font-size: 12px; color: var(--primary);">Посещений: <span class="visit-count">${user.visits || 0}</span>/100</div>
            </div>
            <div class="user-visit-controls">
                <button class="visit-btn visit-add" onclick="addUserVisit('${user.id}')" ${(user.visits || 0) >= 100 ? 'disabled style="opacity:0.5"' : ''}>+</button>
                <button class="visit-btn visit-remove" onclick="removeUserVisit('${user.id}')" ${(user.visits || 0) <= 0 ? 'disabled style="opacity:0.5"' : ''}>-</button>
            </div>
        </div>
    `).join('');
}

function addUserVisit(userId) {
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    
    if (!currentUser || !currentUser.devMode) {
        alert('Только администраторы могут добавлять посещения');
        return;
    }
    
    const userDatabase = JSON.parse(localStorage.getItem('userDatabase') || '[]');
    const userIndex = userDatabase.findIndex(user => user.id === userId);
    
    if (userIndex !== -1) {
        const currentVisits = userDatabase[userIndex].visits || 0;
        if (currentVisits >= 100) {
            alert('Максимальное количество посещений - 100');
            return;
        }
        
        userDatabase[userIndex].visits = currentVisits + 1;
        localStorage.setItem('userDatabase', JSON.stringify(userDatabase));
        showSuccessMessage('Посещение добавлено!');
        
        searchUser();
    }
}

function removeUserVisit(userId) {
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    
    if (!currentUser || !currentUser.devMode) {
        alert('Только администраторы могут удалять посещения');
        return;
    }
    
    const userDatabase = JSON.parse(localStorage.getItem('userDatabase') || '[]');
    const userIndex = userDatabase.findIndex(user => user.id === userId);
    
    if (userIndex !== -1 && userDatabase[userIndex].visits > 0) {
        userDatabase[userIndex].visits = userDatabase[userIndex].visits - 1;
        localStorage.setItem('userDatabase', JSON.stringify(userDatabase));
        showSuccessMessage('Посещение удалено!');
        
        searchUser();
    }
}

function initUserSystem() {
    if (!localStorage.getItem('users')) {
        localStorage.setItem('users', JSON.stringify([]));
    }
}

function submitAuthExtended() {
    const username = document.getElementById('username').value.trim();
    const phone = document.getElementById('phone').value.trim();
    const password = document.getElementById('password').value;
    const selectedAvatar = document.querySelector('.avatar-option.selected');
    
    if (!username || !phone || !password) {
        alert('Пожалуйста, заполните все поля');
        return;
    }
    
    if (!selectedAvatar) {
        alert('Пожалуйста, выберите аватар');
        return;
    }
    
    const avatar = selectedAvatar.getAttribute('data-avatar');
    
    let isDevAccount = false;
    let devAccountData = null;
    
    for (const devPhone in DEV_ACCOUNTS) {
        if ((phone === devPhone || username === DEV_ACCOUNTS[devPhone].name) && 
            checkDevAccount(devPhone, password)) {
            isDevAccount = true;
            devAccountData = {
                ...DEV_ACCOUNTS[devPhone],
                phone: devPhone,
                username: DEV_ACCOUNTS[devPhone].name,
                avatar: avatar,
                id: generateUserId()
            };
            break;
        }
    }
    
    if (isDevAccount) {
        setDevMode(devAccountData);
        document.getElementById('auth-success').style.display = 'block';
        
        setTimeout(() => {
            closeAuthModal();
            initUI();
            showWelcomeMessage(devAccountData.username, devAccountData.greeting);
        }, 1500);
        return;
    }
    
    const users = JSON.parse(localStorage.getItem('users') || '[]');
    
    const existingUser = users.find(user => user.phone === phone);
    
    if (existingUser) {
        if (existingUser.password !== password) {
            alert('Неверный пароль');
            return;
        }
        
        if (existingUser.avatar !== avatar) {
            existingUser.avatar = avatar;
            localStorage.setItem('users', JSON.stringify(users));
        }
        
        const userData = {
            ...existingUser,
            lastLogin: new Date().toISOString()
        };
        
        localStorage.setItem('currentUser', JSON.stringify(userData));
        saveUserToDatabase(userData);
        
    } else {
        if (users.find(user => user.username === username)) {
            alert('Этот никнейм уже занят. Пожалуйста, выберите другой.');
            return;
        }
        
        const userData = {
            id: generateUserId(),
            username: username,
            phone: phone,
            password: password,
            avatar: avatar,
            registrationDate: new Date().toISOString(),
            lastLogin: new Date().toISOString()
        };
        
        users.push(userData);
        localStorage.setItem('users', JSON.stringify(users));
        localStorage.setItem('currentUser', JSON.stringify(userData));
        saveUserToDatabase(userData);
    }
    
    document.getElementById('auth-success').style.display = 'block';
    
    setTimeout(() => {
        closeAuthModal();
        initUI();
        showWelcomeMessage(username);
    }, 1500);
}

function showWelcomeMessage(username, customGreeting = null) {
    const greeting = customGreeting || `Привет, ${username}! 💖💕✨`;
    alert(greeting);
}

function updateAccountInfo() {
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    
    if (currentUser) {
        document.getElementById('profile-avatar').textContent = currentUser.avatar;
        document.getElementById('profile-username').textContent = currentUser.username;
        document.getElementById('profile-phone').textContent = currentUser.phone;
        
        const registrationDate = new Date(currentUser.registrationDate);
        document.getElementById('profile-joined-date').textContent = registrationDate.toLocaleDateString('ru-RU');
        
        const visits = LOYALTY_SYSTEM.visits || 0;
        let status = "Новичок 💅";
        if (visits >= 10) status = "Лучшая ✨";
        else if (visits >= 5) status = "Хорошая клиентка 💋";
        else if (visits >= 1) status = "Наша клиентка 💖";
        
        document.getElementById('profile-status').textContent = status;
    }
}

function openChangeUsernameModal() {
    document.getElementById('change-username-modal').style.display = 'flex';
}

function closeChangeUsernameModal() {
    document.getElementById('change-username-modal').style.display = 'none';
}

function changeUsername() {
    const newUsername = document.getElementById('new-username').value.trim();
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    
    if (!newUsername) {
        alert('Пожалуйста, введите новый никнейм');
        return;
    }
    
    if (newUsername === currentUser.username) {
        alert('Этот никнейм уже используется');
        return;
    }
    
    const users = JSON.parse(localStorage.getItem('users') || '[]');
    if (users.find(user => user.username === newUsername && user.id !== currentUser.id)) {
        alert('Этот никнейм уже занят. Пожалуйста, выберите другой.');
        return;
    }
    
    const userIndex = users.findIndex(user => user.id === currentUser.id);
    if (userIndex !== -1) {
        users[userIndex].username = newUsername;
        localStorage.setItem('users', JSON.stringify(users));
    }
    
    currentUser.username = newUsername;
    localStorage.setItem('currentUser', JSON.stringify(currentUser));
    
    document.getElementById('change-username-success').style.display = 'block';
    
    setTimeout(() => {
        closeChangeUsernameModal();
        initUI();
        showSuccessMessage('Никнейм успешно изменен!');
    }, 1500);
}

function openChangeAvatarModal() {
    document.getElementById('change-avatar-modal').style.display = 'flex';
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    if (currentUser && currentUser.avatar) {
        document.querySelectorAll('#avatar-selection-modal .avatar-option').forEach(option => {
            if (option.getAttribute('data-avatar') === currentUser.avatar) {
                option.classList.add('selected');
            }
        });
    }
}

function closeChangeAvatarModal() {
    document.getElementById('change-avatar-modal').style.display = 'none';
}

function changeAvatar() {
    const selectedAvatar = document.querySelector('#avatar-selection-modal .avatar-option.selected');
    if (!selectedAvatar) {
        alert('Пожалуйста, выберите аватар');
        return;
    }
    
    const newAvatar = selectedAvatar.getAttribute('data-avatar');
    const currentUser = JSON.parse(localStorage.getItem('currentUser'));
    
    if (currentUser) {
        currentUser.avatar = newAvatar;
        localStorage.setItem('currentUser', JSON.stringify(currentUser));
        
        const users = JSON.parse(localStorage.getItem('users') || '[]');
        const userIndex = users.findIndex(user => user.id === currentUser.id);
        if (userIndex !== -1) {
            users[userIndex].avatar = newAvatar;
            localStorage.setItem('users', JSON.stringify(users));
        }
        
        const userDatabase = JSON.parse(localStorage.getItem('userDatabase') || '[]');
        const dbUserIndex = userDatabase.findIndex(user => user.id === currentUser.id);
        if (dbUserIndex !== -1) {
            userDatabase[dbUserIndex].avatar = newAvatar;
            localStorage.setItem('userDatabase', JSON.stringify(userDatabase));
        }
        
        document.getElementById('change-avatar-success').style.display = 'block';
        
        setTimeout(() => {
            closeChangeAvatarModal();
            initUI();
            showSuccessMessage('Аватар успешно изменен!');
        }, 1500);
    }
}

function toggleAchievements() {
    const achievementsSection = document.getElementById('achievements-section');
    const toggleButton = document.querySelector('.achievements-toggle');
    
    if (achievementsSection.style.display === 'none') {
        achievementsSection.style.display = 'block';
        toggleButton.textContent = 'Скрыть достижения';
    } else {
        achievementsSection.style.display = 'none';
        toggleButton.textContent = 'Показать достижения';
    }
}

// ===== ФУНКЦИИ ДЛЯ ОСНОВНОГО ИНТЕРФЕЙСА =====
function createBackgroundElements(){
  const cont = document.getElementById('lightning-bg');
  
  for(let i=0; i<30; i++){
    const el = document.createElement('div');
    el.className = 'lightning';
    el.style.left = Math.random()*100 + '%';
    el.style.top = Math.random()*100 + '%';
    el.style.animationDelay = (Math.random()*8) + 's';
    el.style.animationDuration = (6 + Math.random()*6) + 's';
    el.textContent = '⚡';
    cont.appendChild(el);
  }
  
  const starPos=[{l:'10%',t:'10%',d:'2s',dur:'18s'},{l:'90%',t:'15%',d:'5s',dur:'20s'},{l:'20%',t:'90%',d:'8s',dur:'16s'},{l:'80%',t:'85%',d:'12s',dur:'22s'}];
  const starChars=['★','☆','✦','✧'];
  starPos.forEach((pos,i)=>{
    const el=document.createElement('div');el.className='star';el.style.left=pos.l;el.style.top=pos.t;el.style.animationDelay=pos.d;el.style.animationDuration=pos.dur;el.textContent=starChars[i];cont.appendChild(el);
  });
}

function initUI() {
  const savedUser = localStorage.getItem('currentUser');
  if (savedUser) {
    const userData = JSON.parse(savedUser);
    currentUser = userData.username;
    isLoggedIn = true;
    
    updateUIForLoggedInUser();
    updateAccountInfo();
  } else {
    updateUIForGuest();
  }
  
  initUserSystem();
  initUserDatabase();
  initPollSystem();
  initContestSystem();
  initPortfolioLikes();
  
  displayReviews();
  displayServices();
  updatePromoCodesForAllUsers();
  loadLoyaltyData();
  loadAchievements();
  displayCurrentPoll();
  displayContests();
  displayPortfolio();
  
  const currentUserData = JSON.parse(localStorage.getItem('currentUser'));
  if (currentUserData && currentUserData.devMode) {
    updateUIForDevMode();
  }
}

function updateUIForLoggedInUser() {
  document.getElementById('userInfo').style.display = 'block';
  document.getElementById('userName').textContent = currentUser;
  document.getElementById('auth-menu-text').textContent = 'Профиль';
  document.getElementById('account-button').style.display = 'block';
  document.getElementById('auth-button').style.display = 'none';
}

function updateUIForGuest() {
  document.getElementById('userInfo').style.display = 'none';
  document.getElementById('auth-menu-text').textContent = 'Вход';
  document.getElementById('account-button').style.display = 'none';
  document.getElementById('auth-button').style.display = 'block';
}

function displayReviews() {
  const reviewsDisplay = document.getElementById('reviews-display');
  const showAllButton = document.getElementById('show-all-reviews-btn');
  reviewsDisplay.innerHTML = '';
  
  if (reviews.length === 0) {
    reviewsDisplay.innerHTML = '<div class="no-reviews">Пока нет отзывов. Будьте первым!</div>';
    showAllButton.style.display = 'none';
    return;
  }
  
  // Сначала показываем закрепленные отзывы
  const pinnedReviews = reviews.filter(review => review.pinned);
  const unpinnedReviews = reviews.filter(review => !review.pinned);
  
  let reviewsToShow = [...pinnedReviews, ...unpinnedReviews];
  
  if (reviewsToShow.length > 3) {
    reviewsToShow = reviewsToShow.slice(-3);
    showAllButton.style.display = 'block';
    showAllButton.onclick = showAllReviews;
  } else {
    showAllButton.style.display = 'none';
  }
  
  reviewsToShow.forEach(review => {
    const reviewItem = document.createElement('div');
    reviewItem.className = review.image ? `review-item review-with-photo ${review.pinned ? 'pinned' : ''}` : `review-item ${review.pinned ? 'pinned' : ''}`;
    
    const authorAvatar = review.authorAvatar || '💅';
    
    reviewItem.innerHTML = `
      <div class="review-author">
        <span style="font-size: 16px; margin-right: 8px;">${authorAvatar}</span>
        ${review.author}
        ${review.pinned ? '<span class="review-pin-icon">📌</span>' : ''}
      </div>
      <div class="review-text">${review.text}</div>
      ${review.image ? `<img src="${review.image}" class="review-image" alt="Фото отзыва">` : ''}
    `;
    reviewsDisplay.appendChild(reviewItem);
  });
}

function showAllReviews() {
  const reviewsDisplay = document.getElementById('reviews-display');
  reviewsDisplay.innerHTML = '';
  
  // Сначала показываем закрепленные отзывы
  const pinnedReviews = reviews.filter(review => review.pinned);
  const unpinnedReviews = reviews.filter(review => !review.pinned);
  
  const allReviews = [...pinnedReviews, ...unpinnedReviews];
  
  allReviews.forEach(review => {
    const reviewItem = document.createElement('div');
    reviewItem.className = review.image ? `review-item review-with-photo ${review.pinned ? 'pinned' : ''}` : `review-item ${review.pinned ? 'pinned' : ''}`;
    reviewItem.innerHTML = `
      <div class="review-author">
        <span style="font-size: 16px; margin-right: 8px;">${review.authorAvatar || '💅'}</span>
        ${review.author}
        ${review.pinned ? '<span class="review-pin-icon">📌</span>' : ''}
      </div>
      <div class="review-text">${review.text}</div>
      ${review.image ? `<img src="${review.image}" class="review-image" alt="Фото отзыва">` : ''}
    `;
    reviewsDisplay.appendChild(reviewItem);
  });
  
  document.getElementById('show-all-reviews-btn').style.display = 'none';
}

function addReview(author, text, image = null) {
  const currentUser = JSON.parse(localStorage.getItem('currentUser'));
  const authorAvatar = currentUser ? currentUser.avatar : '💅';
  
  const newReview = { 
    author, 
    text, 
    image, 
    date: new Date().toISOString(), 
    pinned: false,
    authorAvatar: authorAvatar
  };
  reviews.push(newReview);
  
  if (reviews.length > 100) {
    reviews = reviews.slice(-100);
  }
  
  localStorage.setItem("reviews", JSON.stringify(reviews));
  displayReviews();
}

const searchInput=document.getElementById('search-input');
const searchResults=document.getElementById('search-results');

searchInput.addEventListener('input',function(){
  const query=this.value.toLowerCase().trim();
  searchResults.innerHTML='';
  if(query.length<2){searchResults.style.display='none';return;}
  const filtered=searchData.filter(item=>item.title.toLowerCase().includes(query)||(item.description && item.description.toLowerCase().includes(query))||item.price.toLowerCase().includes(query));
  if(filtered.length>0){
    filtered.forEach(item=>{
      const div=document.createElement('div');div.className='search-result-item';
      div.innerHTML=`<div class="search-result-title">${item.title}</div><div class="search-result-price">${item.price}</div><div class="search-result-type">${item.type}</div>${item.description?`<div style="font-size:12px;color:var(--muted);margin-top:3px;">${item.description}</div>`:''}`;
      div.addEventListener('click',function(){searchInput.value=item.title;searchResults.style.display='none';if(item.type==='услуга')openBookingModal(item.title);});
      searchResults.appendChild(div);
    });
    searchResults.style.display='block';
  } else searchResults.style.display='none';
});
document.addEventListener('click',function(e){if(!e.target.closest('.search-container'))searchResults.style.display='none';});

const modal=document.getElementById('booking-modal');
const closeModal=document.querySelector('.close-modal');
function openBookingModal(service=''){if(service){modal.querySelector('h2').textContent=`Записаться на ${service}`;}modal.style.display='flex';}

document.addEventListener('click', function(e) {
  if (e.target.closest('.note')) {
    const service = e.target.closest('.note').dataset.service;
    openBookingModal(service);
  }
});

closeModal.addEventListener('click',()=>modal.style.display='none');
window.addEventListener('click',e=>{if(e.target===modal)modal.style.display='none';});

function scrollToSection(id){const el=document.getElementById(id);if(el)el.scrollIntoView({behavior:'smooth'});}
document.querySelector('.portfolio-grid').parentElement.parentElement.id='portfolio';

const draggableMenu = document.getElementById('draggable-menu');
let isDragging = false;
let currentX;
let currentY;
let initialX;
let initialY;
let xOffset = 0;
let yOffset = 0;

draggableMenu.addEventListener("mousedown", dragStart);
draggableMenu.addEventListener("touchstart", dragStart);

function dragStart(e) {
  if (e.type === "touchstart") {
    initialX = e.touches[0].clientX - xOffset;
    initialY = e.touches[0].clientY - yOffset;
  } else {
    initialX = e.clientX - xOffset;
    initialY = e.clientY - yOffset;
  }

  if (e.target === draggableMenu || e.target === document.getElementById('menu-button')) {
    isDragging = true;
    
    document.getElementById('menu-dropdown').style.display = 'none';
  }
}

document.addEventListener("mousemove", drag);
document.addEventListener("touchmove", drag);

function drag(e) {
  if (isDragging) {
    e.preventDefault();
    
    if (e.type === "touchmove") {
      currentX = e.touches[0].clientX - initialX;
      currentY = e.touches[0].clientY - initialY;
    } else {
      currentX = e.clientX - initialX;
      currentY = e.clientY - initialY;
    }

    xOffset = currentX;
    yOffset = currentY;

    setTranslate(currentX, currentY, draggableMenu);
  }
}

document.addEventListener("mouseup", dragEnd);
document.addEventListener("touchend", dragEnd);

function dragEnd(e) {
  initialX = currentX;
  initialY = currentY;
  isDragging = false;
}

function setTranslate(xPos, yPos, el) {
  el.style.transform = "translate3d(" + xPos + "px, " + yPos + "px, 0)";
}

const menuButton = document.getElementById('menu-button');
const menuDropdown = document.getElementById('menu-dropdown');
const authButton = document.getElementById('auth-button');
const accountButton = document.getElementById('account-button');
const fortuneButton = document.getElementById('fortune-button');
const reviewButton = document.getElementById('review-button');
const promoButton = document.getElementById('promo-button');
const pollsButton = document.getElementById('polls-button');
const contestsButton = document.getElementById('contests-button');
const pricesButton = document.getElementById('prices-button');
const searchUserButton = document.getElementById('search-user-button');
const managePollsButton = document.getElementById('manage-polls-button');
const manageContestsButton = document.getElementById('manage-contests-button');
const manageReviewsButton = document.getElementById('manage-reviews-button');
const managePortfolioButton = document.getElementById('manage-portfolio-button');

menuButton.addEventListener('click', function(e) {
  e.stopPropagation();
  menuDropdown.style.display = menuDropdown.style.display === 'block' ? 'none' : 'block';
});

document.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
});

authButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openAuthModal();
});

accountButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openAccountModal();
});

fortuneButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openFortuneModal();
});

reviewButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openReviewModal();
});

promoButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openPromoModal();
});

pollsButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openPollsModal();
});

contestsButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openContestsModal();
});

pricesButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openPricesModal();
});

searchUserButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openSearchUserModal();
});

managePollsButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openManagePollsModal();
});

manageContestsButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openManageContestsModal();
});

manageReviewsButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openManageReviewsModal();
});

managePortfolioButton.addEventListener('click', function() {
  menuDropdown.style.display = 'none';
  openManagePortfolioModal();
});

function openAuthModal() {
  if (isLoggedIn) {
    alert(`Вы уже авторизованы как ${currentUser}`);
    return;
  }
  document.getElementById('auth-modal').style.display = 'flex';
}

function closeAuthModal() {
  document.getElementById('auth-modal').style.display = 'none';
}

function openAccountModal() {
  document.getElementById('account-modal').style.display = 'flex';
}

function closeAccountModal() {
  document.getElementById('account-modal').style.display = 'none';
}

function openPollsModal() {
  document.getElementById('polls-modal').style.display = 'flex';
}

function closePollsModal() {
  document.getElementById('polls-modal').style.display = 'none';
}

function openContestsModal() {
  document.getElementById('contests-modal').style.display = 'flex';
}

function closeContestsModal() {
  document.getElementById('contests-modal').style.display = 'none';
}

function openSearchUserModal() {
  document.getElementById('search-user-modal').style.display = 'flex';
}

function closeSearchUserModal() {
  document.getElementById('search-user-modal').style.display = 'none';
}

function openManagePollsModal() {
  document.getElementById('manage-polls-modal').style.display = 'flex';
}

function closeManagePollsModal() {
  document.getElementById('manage-polls-modal').style.display = 'none';
}

function openManageContestsModal() {
  document.getElementById('manage-contests-modal').style.display = 'flex';
}

function closeManageContestsModal() {
  document.getElementById('manage-contests-modal').style.display = 'none';
}

function openManageReviewsModal() {
  document.getElementById('manage-reviews-modal').style.display = 'flex';
}

function closeManageReviewsModal() {
  document.getElementById('manage-reviews-modal').style.display = 'none';
}

function openManagePortfolioModal() {
  document.getElementById('manage-portfolio-modal').style.display = 'flex';
}

function closeManagePortfolioModal() {
  document.getElementById('manage-portfolio-modal').style.display = 'none';
}

function logout() {
  currentUser = null;
  isLoggedIn = false;
  localStorage.removeItem("currentUser");
  updateUIForGuest();
  alert("Вы вышли из системы");
}

function openFortuneModal() {
  document.getElementById('fortune-modal').style.display = 'flex';
  if (isLoggedIn) {
    document.getElementById('fortune-content').style.display = 'block';
    document.getElementById('fortune-locked').style.display = 'none';
    createWheel();
  } else {
    document.getElementById('fortune-content').style.display = 'none';
    document.getElementById('fortune-locked').style.display = 'block';
  }
}

function closeFortuneModal() {
  document.getElementById('fortune-modal').style.display = 'none';
  document.getElementById('wheel-inner').style.transform = 'rotate(0deg)';
  document.getElementById('result-message').style.display = 'none';
  document.getElementById('spin-button').disabled = false;
  document.getElementById('spin-button').style.display = 'block';
  document.getElementById('claim-button').style.display = 'none';
}

function openPrizeModal(prize) {
  document.getElementById('prize-icon').textContent = prize.icon;
  document.getElementById('prize-description').textContent = `Вы выиграли: ${prize.name} (скидка ${prize.discount}%)`;
  
  const exchangeButton = document.getElementById('exchange-prize-button');
  const discountSpan = document.getElementById('exchange-discount-value');
  discountSpan.textContent = prize.discount + '%';
  
  exchangeButton.onclick = function() {
    exchangePrizeForDiscount(prize.discount);
  };
  
  document.getElementById('prize-modal').style.display = 'flex';
}

function closePrizeModal() {
  document.getElementById('prize-modal').style.display = 'none';
  closeFortuneModal();
}

function exchangePrizeForDiscount(discount) {
    alert(`🎉 Поздравляем! Вы обменяли подарок на скидку ${discount}%! (В реальном проекте здесь будет логика применения скидки)`);
    closePrizeModal();
}

function openReviewModal() {
  document.getElementById('review-modal').style.display = 'flex';
}

function closeReviewModal() {
  document.getElementById('review-modal').style.display = 'none';
  document.getElementById('modal-review-success').style.display = 'none';
}

function openPromoModal() {
  document.getElementById('promo-modal').style.display = 'flex';
}

function closePromoModal() {
  document.getElementById('promo-modal').style.display = 'none';
}

function createWheel() {
  const wheelInner = document.getElementById('wheel-inner');
  wheelInner.innerHTML = '';
  
  let currentAngle = 0;
  const angleStep = 360 / fortunePrizes.length;
  
  fortunePrizes.forEach((prize) => {
    const segment = document.createElement('div');
    segment.className = 'wheel-segment';
    segment.style.backgroundColor = prize.color;
    segment.style.transform = `rotate(${currentAngle}deg)`;
    
    const content = document.createElement('div');
    content.className = 'segment-content';
    content.innerHTML = `${prize.icon}<br><span style="font-size:12px;">${prize.name}</span><span class="segment-discount">скидка ${prize.discount}%</span>`;
    
    segment.appendChild(content);
    wheelInner.appendChild(segment);
    
    currentAngle += angleStep;
  });
}

document.getElementById('spin-button').addEventListener('click', function() {
  if (!isLoggedIn) {
    alert("Для использования колеса фортуны необходимо авторизоваться!");
    openAuthModal();
    return;
  }
  
  const spinButton = document.getElementById('spin-button');
  const claimButton = document.getElementById('claim-button');
  const wheelInner = document.getElementById('wheel-inner');
  const resultMessage = document.getElementById('result-message');
  
  spinButton.disabled = true;
  
  const totalWeight = fortunePrizes.reduce((sum, prize) => sum + prize.weight, 0);
  
  let randomValue = Math.random() * totalWeight;
  let selectedPrizeIndex = 0;
  let weightSum = 0;
  
  for (let i = 0; i < fortunePrizes.length; i++) {
    weightSum += fortunePrizes[i].weight;
    if (randomValue <= weightSum) {
      selectedPrizeIndex = i;
      break;
    }
  }
  
  const segmentAngle = 360 / fortunePrizes.length;
  const spins = 5 + Math.floor(Math.random() * 5);
  const finalAngle = spins * 360 + (360 - (selectedPrizeIndex * segmentAngle + segmentAngle / 2));
  
  const duration = 4000 + Math.random() * 2000;
  
  wheelInner.style.transition = `transform ${duration/1000}s cubic-bezier(0.2, 0.8, 0.3, 1)`;
  wheelInner.style.transform = `rotate(${finalAngle}deg)`;
  
  setTimeout(() => {
    openPrizeModal(fortunePrizes[selectedPrizeIndex]);
    
    createConfetti();
    
    addLoyaltyPoints(30, 'Выигрыш в колесе фортуны');
  }, duration);
});

function createConfetti() {
  const colors = ['#d9b6b0', '#e28c8c', '#fff4f2', '#fdf8f6', '#ff69b4', '#8B4513'];
  
  for (let i = 0; i < 200; i++) {
    const confetti = document.createElement('div');
    confetti.className = 'confetti';
    confetti.style.left = Math.random() * 100 + 'vw';
    confetti.style.top = '-10px';
    confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
    confetti.style.transform = `rotate(${Math.random() * 360}deg)`;
    confetti.style.width = Math.random() * 10 + 5 + 'px';
    confetti.style.height = Math.random() * 10 + 5 + 'px';
    
    document.body.appendChild(confetti);
    
    const animation = confetti.animate([
      { top: '-10px', opacity: 1, transform: `rotate(0deg) scale(1)` },
      { top: '100vh', opacity: 0, transform: `rotate(${Math.random() * 360}deg) scale(0.5)` }
    ], {
      duration: Math.random() * 8000 + 6000,
      easing: 'cubic-bezier(0.1, 0.8, 0.2, 1)'
    });
    
    animation.onfinish = () => {
      confetti.remove();
    };
  }
}

function checkPromo(){
  const val = document.getElementById('modal-promoKey').value.trim().toLowerCase();
  const promoBox = document.getElementById('modal-promoList');
  promoBox.innerHTML = '';
  if (!keys[val]) return promoBox.innerHTML = "<div class='promo-item' style='color:red;text-align:center;'>Неверный ключ ❌</div>";
  keys[val].forEach((i,idx) => {
    const div = document.createElement('div');
    div.className = 'promo-item';
    div.style.animationDelay = `${idx*0.1}s`;
    div.textContent = fortunePrizes[i].name + ' - скидка ' + fortunePrizes[i].discount + '%';
    promoBox.appendChild(div);
    createHeartAnimation(div);
  });
}

function createHeartAnimation(target){
  for(let j=0;j<3;j++){
    const heart = document.createElement('div');
    heart.className = 'heart';
    heart.textContent = '💖';
    heart.style.left = (Math.random()*80+10)+'%';
    heart.style.bottom = '0px';
    heart.style.animationDuration = '2s';
    target.appendChild(heart);
    setTimeout(() => heart.remove(), 2000);
  }
}

document.getElementById('modal-submit-review').addEventListener('click', function() {
  const name = document.getElementById('modal-review-name').value;
  const text = document.getElementById('modal-review-text').value;
  const imageInput = document.getElementById('modal-review-image');
  const imageFile = imageInput.files[0];
  
  if (name && text) {
    if (imageFile) {
      const reader = new FileReader();
      reader.onload = function(e) {
        const imageData = e.target.result;
        addReview(name, text, imageData);
        document.getElementById('modal-review-success').style.display = 'block';
        document.getElementById('modal-review-name').value = '';
        document.getElementById('modal-review-text').value = '';
        imageInput.value = '';
        
        setTimeout(() => {
          document.getElementById('modal-review-success').style.display = 'none';
          closeReviewModal();
        }, 1500);
      };
      reader.readAsDataURL(imageFile);
    } else {
      addReview(name, text);
      document.getElementById('modal-review-success').style.display = 'block';
      document.getElementById('modal-review-name').value = '';
      document.getElementById('modal-review-text').value = '';
      
      setTimeout(() => {
        document.getElementById('modal-review-success').style.display = 'none';
        closeReviewModal();
      }, 1500);
    }
  }
});

function showSuccessMessage(message) {
  alert(message);
}

// ===== ИНИЦИАЛИЗАЦИЯ ВЫБОРА АВАТАРА =====
document.addEventListener('DOMContentLoaded', function() {
  const avatarOptions = document.querySelectorAll('#avatar-selection .avatar-option');
  avatarOptions.forEach(option => {
    option.addEventListener('click', function() {
      avatarOptions.forEach(opt => {
        opt.classList.remove('selected');
      });
      this.classList.add('selected');
    });
  });
  
  const avatarOptionsModal = document.querySelectorAll('#avatar-selection-modal .avatar-option');
  avatarOptionsModal.forEach(option => {
    option.addEventListener('click', function() {
      avatarOptionsModal.forEach(opt => {
        opt.classList.remove('selected');
      });
      this.classList.add('selected');
    });
  });
});

// ===== ЗАПУСК ПРИЛОЖЕНИЯ =====
document.addEventListener('DOMContentLoaded', function() {
  createBackgroundElements();
  initUI();
});

</script>
</body>
</html>