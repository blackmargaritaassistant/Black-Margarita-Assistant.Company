# Black-Margarita-Assistant.Company
<!DOCTYPE html>
<html lang="fa">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Black Margarita Assistant Company</title>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
<style>
/* ================== Global Styles ================== */
body {
    margin: 0;
    font-family: 'Montserrat', sans-serif;
    background-color: #0a0a0a;
    color: #f0f0f0;
}
a { text-decoration: none; color: inherit; }

/* ================== Header ================== */
header {
    background: rgba(0,0,0,0.9);
    padding: 20px 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 10px rgba(0,0,0,0.5);
}
header h1 {
    color: #f0f0f0;
    font-weight: 700;
    font-size: 1.8em;
}
nav a {
    margin-left: 25px;
    font-weight: 600;
    transition: color 0.3s;
    padding: 5px 10px;
    border-radius: 6px;
}
nav a:hover { color: #ffccff; background-color: rgba(85,0,85,0.3); }

/* گیلاس مشکی */
#cherry {
    position:absolute; top:20px; right:20px;
    width:30px; height:30px;
    background-color:#000;
    border-radius:50%;
    border:2px solid #cc99ff;
    box-shadow: 0 0 10px #cc99ff;
}

/* ================== Hero Section ================== */
.hero {
    background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1596496055763-0f11044f36d7') no-repeat center center/cover;
    height: 85vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
}
.hero h2 { font-size: 3em; margin: 0; color: #ffccff; text-shadow: 0 0 10px #550055; }
.hero p { font-size: 1.3em; margin-top: 10px; max-width: 650px; }
.hero button {
    margin-top: 25px;
    padding: 15px 35px;
    font-size: 1.1em;
    border: none;
    border-radius: 10px;
    background-color: #550055;
    color: #f0f0f0;
    cursor: pointer;
    transition: 0.3s;
    box-shadow: 0 0 15px #cc99ff;
}
.hero button:hover { background-color: #ffccff; color: #0a0a0a; box-shadow: 0 0 20px #ffccff; }

/* ================== Services Section ================== */
.services {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 60px 20px;
    background-color: #111;
}
.service-card {
    background: rgba(30,0,30,0.85);
    border-radius: 15px;
    padding: 35px;
    width: 320px;
    margin: 20px;
    transition: transform 0.4s, background 0.4s, box-shadow 0.4s;
    box-shadow: 0 0 15px rgba(85,0,85,0.5);
}
.service-card:hover {
    transform: translateY(-15px);
    background: rgba(50,0,50,0.95);
    box-shadow: 0 0 25px #cc99ff;
}
.service-card h3 { color: #ffccff; margin-top: 0; }

/* ================== Booking Form ================== */
#booking {
    background-color: #0a0a0a;
    padding: 60px 20px;
    text-align: center;
}
#booking h2 { color: #ffccff; margin-bottom: 35px; text-shadow: 0 0 10px #550055; }
form {
    max-width: 520px;
    margin: auto;
    background-color: rgba(20,0,20,0.9);
    padding: 35px;
    border-radius: 15px;
    box-shadow: 0 0 20px rgba(85,0,85,0.5);
}
form input, form select, form button {
    width: 100%;
    padding: 14px;
    margin: 12px 0;
    border-radius: 8px;
    border: none;
    font-size: 1em;
}
form button {
    background-color: #550055;
    color: #f0f0f0;
    cursor: pointer;
    font-weight: bold;
    transition: 0.3s;
    box-shadow: 0 0 10px #cc99ff;
}
form button:hover { background-color: #ffccff; color: #0a0a0a; box-shadow: 0 0 15px #ffccff; }

/* ================== Chatbot ================== */
#chatbot {
    position: fixed;
    bottom: 25px;
    right: 25px;
    width: 320px;
    background-color: rgba(30,0,30,0.95);
    border-radius: 15px;
    overflow: hidden;
    font-size: 0.95em;
    box-shadow: 0 0 20px #cc99ff;
}
#chatbot-header {
    background-color: #550055;
    padding: 12px;
    color: #f0f0f0;
    cursor: pointer;
    font-weight: 600;
}
#chatbot-messages {
    height: 230px;
    padding: 12px;
    overflow-y: auto;
    display: none;
    background-color: #1a001a;
}
#chatbot-input {
    display: none;
    padding: 12px;
    border-top: 1px solid #550055;
    display: flex;
    gap: 10px;
}
#chatbot-input input {
    flex: 1;
    padding: 10px;
    border-radius: 8px;
    border: none;
}
#chatbot-input button {
    width: 100px;
    background-color: #ffccff;
    border: none;
    border-radius: 8px;
    color: #0a0a0a;
    font-weight: bold;
    cursor: pointer;
}

/* ================== Footer ================== */
footer {
    background-color: #0a0a0a;
    text-align: center;
    padding: 35px 20px;
    border-top: 1px solid #550055;
    box-shadow: 0 -2px 10px rgba(0,0,0,0.5);
}

/* ================== Responsive ================== */
@media (max-width: 768px) {
    .services { flex-direction: column; align-items: center; }
    nav a { margin-left: 12px; }
}
</style>
</head>
<body>

<header>
    <h1>Black Margarita Assistant Company</h1>
    <nav>
        <a href="#services">خدمات ما</a>
        <a href="#booking">رزرو تکت</a>
        <a href="#hotel">رزرو هوتل</a>
        <a href="#contact">تماس با ما</a>
    </nav>
    <div id="cherry"></div>
</header>

<section class="hero">
    <h2>تجربه‌ای بی‌نظیر از خدمات آنلاین لوکس در سراسر جهان</h2>
    <p>فروش تکت، رزرو هوتل، وقت ملاقات سفارت و سایر خدمات آنلاین</p>
    <button>شروع کنید</button>
</section>

<section class="services" id="services">
    <div class="service-card">
        <h3>فروش تکت هوایی</h3>
        <p>به راحتی تکت خود را برای هر نقطه جهان رزرو کنید.</p>
    </div>
    <div class="service-card">
        <h3>رزرو هوتل</h3>
        <p>هوتل‌های لوکس و مدرن را با بهترین قیمت رزرو کنید.</p>
    </div>
    <div class="service-card">
        <h3>وقت ملاقات سفارت</h3>
        <p>به آسانی وقت ملاقات در سفارتخانه‌ها را رزرو نمایید.</p>
    </div>
    <div class="service-card">
        <h3>سایر خدمات آنلاین</h3>
        <p>تمام خدمات دیگر آنلاین را با امنیت و سرعت بالا دریافت کنید.</p>
    </div>
</section>

<section id="booking">
    <h2>رزرو خدمات</h2>
    <form onsubmit="alert('رزرو شما ثبت شد! (نسخه نمونه)'); return false;">
        <input type="text" placeholder="نام کامل" required>
        <input type="email" placeholder="ایمیل" required>
        <select required>
            <option value="">نوع سرویس</option>
            <option value="ticket">تکت هوایی</option>
            <option value="hotel">رزرو هوتل</option>
            <option value="embassy">وقت ملاقات سفارت</option>
        </select>
        <input type="date" required>
        <button type="submit">رزرو و پرداخت</button>
    </form>
</section>

<div id="chatbot">
    <div id="chatbot-header" onclick="toggleChat()">پشتیبانی آنلاین</div>
    <div id="chatbot-messages"></div>
    <div id="chatbot-input">
        <input type="text" id="userMessage" placeholder="پیام خود را بنویسید">
        <button onclick="sendMessage()">ارسال</button>
    </div>
</div>

<footer id="contact">
    <p>&copy; 2026 Black Margarita Assistant Company | تمام حقوق محفوظ است</p>
    <p>ایمیل: kabuldamaknetclub@gmail.com | تماس افغانستان: 0782479150</p>
</footer>

<script>
function toggleChat(){
    let messages = document.getElementById('chatbot-messages');
    let input = document.getElementById('chatbot-input');
    if(messages.style.display === 'none' || messages.style.display === ''){
        messages.style.display = 'block';
        input.style.display = 'flex';
    } else {
        messages.style.display = 'none';
        input.style.display = 'none';
    }
}

function sendMessage(){
    let userMsg = document.getElementById('userMessage').value;
    if(userMsg.trim() === '') return;
    let messagesDiv = document.getElementById('chatbot-messages');
    let userDiv = document.createElement('div');
    userDiv.textContent = 'شما: ' + userMsg;
    userDiv.style.marginBottom = '10px';
    messagesDiv.appendChild(userDiv);

    // پاسخ هوشمند نمونه
    let botDiv = document.createElement('div');
    botDiv.textContent = 'پشتیبانی: لطفاً نوع سرویس خود را انتخاب و فرم رزرو را تکمیل کنید.';
    botDiv.style.marginBottom = '10px';
    botDiv.style.color = '#ffccff';
    messagesDiv.appendChild(botDiv);

    messagesDiv.scrollTop = messagesDiv.scrollHeight;
    document.getElementById('userMessage').value = '';
}
</script>

</body>
</html>
