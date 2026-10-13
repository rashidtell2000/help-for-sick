# help-for-sick
you can help child
<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>קמפיין תרומות | حملة تبرع | Donation Campaign</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&family=Frank+Ruhl+Libre:wght@500;700;900&family=Heebo:wght@400;500;700&family=Noto+Naskh+Arabic:wght@500;700&display=swap" rel="stylesheet">
<style>
:root{
 --bg:#F4F8F9;--surface:#FFFFFF;--ink:#14272F;--muted:#52666E;--line:#D5E1E5;
 --teal:#1B6B73;--teal-ink:#FFFFFF;--sun:#F0A23B;--sun-soft:#FCEBCF;--focus:#0B4F9E;
 --serif:"Frank Ruhl Libre","Times New Roman",serif;
 --sans:"Heebo",Arial,sans-serif;
 box-sizing:border-box;
 padding-top:env(safe-area-inset-top,0px);
 padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme: dark){
 :root:not([data-theme="light"]){
 --bg:#0F1D22;--surface:#162A31;--ink:#EAF2F4;--muted:#A5B9C0;--line:#2A4048;
 --teal:#5CC2CB;--teal-ink:#08262B;--sun:#F5B258;--sun-soft:#3A2D14;--focus:#8DB8F5;
 }
}
:root[data-theme="dark"]{
 --bg:#0F1D22;--surface:#162A31;--ink:#EAF2F4;--muted:#A5B9C0;--line:#2A4048;
 --teal:#5CC2CB;--teal-ink:#08262B;--sun:#F5B258;--sun-soft:#3A2D14;--focus:#8DB8F5;
}
:root[lang="ar"]{--serif:"Noto Naskh Arabic","Times New Roman",serif;--sans:"Cairo","Heebo",Arial,sans-serif}
html{scroll-behavior:smooth;scroll-padding-top:env(safe-area-inset-top,0px)}
*,*::before,*::after{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font-family:var(--sans);font-size:18px;line-height:1.7;-webkit-text-size-adjust:100%}
a{color:inherit}
:focus-visible{outline:3px solid var(--focus);outline-offset:3px;border-radius:6px}
.wrap{max-width:960px;margin:0 auto;padding:0 22px}

/* language switch */
.top{padding:18px 0 0}
.top .wrap{display:flex;justify-content:flex-end}
.langs{display:inline-flex;border:1.5px solid var(--line);border-radius:999px;overflow:hidden;background:var(--surface)}
.langs button{border:0;background:transparent;color:var(--muted);font:500 16px var(--sans);min-height:42px;padding:0 18px;cursor:pointer}
.langs button[aria-pressed="true"]{background:var(--teal);color:var(--teal-ink);font-weight:700}

/* hero */
.hero{position:relative;overflow:hidden;padding:48px 0 64px;border-bottom:1px solid var(--line)}
.rays{position:absolute;bottom:-2px;inset-inline-start:-40px;width:min(560px,92vw);height:auto;color:var(--sun);pointer-events:none}
.hero .wrap{position:relative}
h1{font-family:var(--serif);font-weight:900;font-size:clamp(42px,9vw,88px);line-height:1.12;margin:0 0 24px;max-width:13ch}
:root[lang="ar"] h1{font-weight:700;line-height:1.35}
.lead{max-width:30em;font-size:clamp(19px,2.6vw,23px);margin:0 0 32px}
.btns{display:flex;flex-wrap:wrap;gap:12px}
.btn{display:inline-flex;align-items:center;justify-content:center;min-height:52px;padding:0 30px;border-radius:999px;border:2px solid var(--teal);background:var(--teal);color:var(--teal-ink);font:700 18px var(--sans);text-decoration:none;cursor:pointer}
.btn:hover{filter:brightness(1.07)}
.btn.ghost{background:transparent;color:var(--teal)}

/* sections */
section{padding:60px 0}
h2{font-family:var(--serif);font-weight:700;font-size:clamp(28px,4.5vw,40px);line-height:1.25;margin:0 0 10px}
.sub{color:var(--muted);margin:0 0 30px;max-width:34em}
.panel{background:var(--surface);border:1px solid var(--line);border-radius:18px;padding:28px;max-width:660px;margin-bottom:24px}
.panel h3{margin:0 0 20px;font-size:22px}
.k{display:block;font-size:15px;color:var(--muted);margin-bottom:6px}
.row{display:flex;gap:8px;align-items:stretch;margin-bottom:18px}
.row code{flex:1;min-width:0;direction:ltr;text-align:left;background:var(--bg);border:1px solid var(--line);border-radius:12px;padding:12px 14px;font:500 15px/1.45 ui-monospace,Menlo,Consolas,monospace;overflow-wrap:anywhere}
.row button, .row a.paypal-link{flex:none;min-width:88px;border-radius:12px;border:1.5px solid var(--teal);background:transparent;color:var(--teal);font:700 16px var(--sans);cursor:pointer;display:inline-flex;align-items:center;justify-content:center;text-decoration:none;padding:0 16px}
.row button.done{background:var(--teal);color:var(--teal-ink)}
.warn{margin:0;padding:14px 16px;border-radius:12px;background:var(--sun-soft);font-size:16px}
.steps{margin:34px 0 0;padding:0;list-style:none;max-width:660px;counter-reset:s}
.steps li{counter-increment:s;display:flex;gap:16px;padding:16px 0;border-top:1px solid var(--line)}
.steps li:last-child{border-bottom:1px solid var(--line)}
.steps li::before{content:counter(s);flex:none;width:34px;height:34px;border-radius:50%;background:var(--sun);color:#1b1b1b;font-weight:700;display:grid;place-items:center}
.contact{font-size:20px}
.contact a{color:var(--teal);font-weight:700;direction:ltr;unicode-bidi:embed}
footer{border-top:1px solid var(--line);padding:28px 0 48px;color:var(--muted);font-size:15px}
footer p{margin:0;max-width:48em}
@media (prefers-reduced-motion:reduce){html{scroll-behavior:auto}}
</style>
</head>
<body>

<div class="top"><div class="wrap">
 <div class="langs" role="group" aria-label="Language / שפה / اللغة">
 <button type="button" data-lang="he">עברית</button>
 <button type="button" data-lang="ar">العربية</button>
 <button type="button" data-lang="en">English</button>
 </div>
</div></div>

<header class="hero">
 <svg class="rays" viewBox="0 0 620 300" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" aria-hidden="true">
 <path d="M40 300a270 270 0 0 1 540 0" opacity=".35"/>
 <path d="M110 300a200 200 0 0 1 400 0" opacity=".6"/>
 <path d="M180 300a130 130 0 0 1 260 0"/>
 </svg>
 <div class="wrap">
 <h1 data-i="slogan"></h1>
 <p class="lead" data-i="lead"></p>
 <div class="btns">
 <a class="btn" href="#donate" data-i="donateBtn"></a>
 <button class="btn ghost" type="button" id="share" data-i="share"></button>
 </div>
 </div>
</header>

<main>
<section id="donate">
 <div class="wrap">
 <h2 data-i="howTitle"></h2>
 <p class="sub" data-i="howSub"></p>

 <!-- قسم PayPal -->
 <div class="panel">
 <h3 data-i="paypalTitle"></h3>
 <span class="k" data-i="paypalEmailLabel"></span>
 <div class="row">
   <code id="paypalEmail">info@comme-il-faut.com</code>
   <button type="button" id="copyPaypal" data-i="copy"></button>
 </div>
 <span class="k" data-i="paypalLinkLabel"></span>
 <div class="row">
   <code>https://www.paypal.com/transfer/homepage</code>
   <a href="https://www.paypal.com/transfer/homepage" target="_blank" rel="noopener" class="paypal-link" data-i="payViaPaypal"></a>
 </div>
 </div>

 <!-- قسم العملات الرقمية -->
 <div class="panel">
 <h3 data-i="walletTitle"></h3>
 <span class="k" data-i="coinLabel"></span>
 <div class="row"><code id="coin">USDT</code></div>
 <span class="k" data-i="netLabel"></span>
 <div class="row"><code id="net">BSC (BNB Smart Chain)</code></div>
 <span class="k" data-i="addrLabel"></span>
 <div class="row"><code id="addr">0x835894ae97eec971d99892171b3fd21fd3582d54</code><button type="button" id="copy" data-i="copy"></button></div>
 <p class="warn" data-i="warn"></p>
 </div>

 <ol class="steps">
 <li data-i="s1"></li>
 <li data-i="s2"></li>
 <li data-i="s3"></li>
 </ol>
 </div>
</section>

<section style="padding-top:0">
 <div class="wrap">
 <h2 data-i="contactTitle"></h2>
 <p class="contact"><span data-i="contactText"></span> <a href="mailto:negev.bread96@gmail.com">negev.bread96@gmail.com</a></p>
 </div>
</section>
</main>

<footer><div class="wrap"><p data-i="foot"></p></div></footer>

<script>
const T = {
 he:{
 title:"קמפיין תרומות לחולים שאין באפשרותם לשלם",
 slogan:"אף חולה לא נשאר מאחור",
 lead:"קמפיין תרומות לעזרה לחולים שאין באפשרותם לשלם עבור טיפול בבתי החולים.",
 donateBtn:"לתרומה", share:"שיתוף", copy:"העתקה", copied:"הועתק",
 howTitle:"איך אפשר לתרום",
 howSub:"התרומה עוברת ישירות לחשבון או לארנק המצוין כאן, בלי גורם מתווך.",
 paypalTitle:"תרומה באמצעות PayPal",
 paypalEmailLabel:"אימייל לחשבון PayPal",
 paypalLinkLabel:"קישור ישיר לתרומה",
 payViaPaypal:"מעבר ל-PayPal",
 walletTitle:"תרומה במטבע דיגיטלי",
 coinLabel:"מטבע", netLabel:"רשת", addrLabel:"כתובת הארנק",
 warn:"ודאו שבחרתם את הרשת BSC לפני השליחה. שליחה ברשת אחרת עלולה לאבד את הכסף.",
 s1:"העתיקו את כתובת הארנק או פרטי ה-PayPal.",
 s2:"בצעו את ההעברה דרך אפליקציית PayPal או ארנק הקריפטו שלכם.",
 s3:"הזינו את הסכום ואשרו את השליחה.",
 contactTitle:"שאלות ובירורים",
 contactText:"לשאלות, לאישור קבלת תרומה או לבירורים:",
 foot:"התרומות מועברות ישירות לחשבון/ארנק המצוין בדף. אם קיבלתם את הקישור ממישהו שאתם לא מכירים, ודאו את פרטי הקמפיין מול המארגנים לפני שאתם תורמים."
 },
 ar:{
 title:"حملة تبرع للمرضى غير القادرين على الدفع",
 slogan:"لا مريض يُترك بلا علاج",
 lead:"حملة تبرع لمساعدة المرضى غير القادرين على دفع تكاليف العلاج في المستشفيات.",
 donateBtn:"تبرّع الآن", share:"مشاركة", copy:"نسخ", copied:"تم النسخ",
 howTitle:"كيف تتبرع",
 howSub:"يصل التبرع مباشرة إلى الحساب أو المحفظة المذكورة هنا، دون أي وسيط.",
 paypalTitle:"التبرع عبر PayPal",
 paypalEmailLabel:"بريد حساب PayPal",
 paypalLinkLabel:"رابط التبرع المباشر",
 payViaPaypal:"افتح PayPal",
 walletTitle:"التبرع بعملة رقمية",
 coinLabel:"العملة", netLabel:"الشبكة", addrLabel:"عنوان المحفظة",
 warn:"تأكد من اختيار شبكة BSC قبل الإرسال. الإرسال عبر شبكة أخرى قد يؤدي إلى ضياع المبلغ.",
 s1:"انسخ عنوان المحفظة أو بريد PayPal.",
 s2:"قم بالإرسال عبر تطبيق PayPal أو محفظة العملات الرقمية الخاصة بك.",
 s3:"أدخل المبلغ ثم أرسل.",
 contactTitle:"للاستفسار والمراجعة",
 contactText:"للأسئلة أو لتأكيد استلام التبرع أو لأي استفسار:",
 foot:"تذهب التبرعات مباشرة إلى الحساب أو المحفظة المذكورة في الصفحة. إذا وصلك الرابط من شخص لا تعرفه، فتحقق من بيانات الحملة مع القائمين عليها قبل التبرع."
 },
 en:{
 title:"Donation campaign for patients who cannot afford treatment",
 slogan:"No patient left behind",
 lead:"A donation campaign to help patients who cannot afford to pay for hospital treatment.",
 donateBtn:"Donate", share:"Share", copy:"Copy", copied:"Copied",
 howTitle:"How to donate",
 howSub:"Your donation goes straight to the account or wallet shown here, with no middleman.",
 paypalTitle:"Donate via PayPal",
 paypalEmailLabel:"PayPal Account Email",
 paypalLinkLabel:"Direct Donation Link",
 payViaPaypal:"Pay via PayPal",
 walletTitle:"Donate with crypto",
 coinLabel:"Coin", netLabel:"Network", addrLabel:"Wallet address",
 warn:"Make sure you select the BSC network before sending. Sending on a different network can lose your funds.",
 s1:"Copy the wallet address or PayPal email.",
 s2:"Send via your PayPal app or crypto wallet.",
 s3:"Enter the amount and send.",
 contactTitle:"Questions and inquiries",
 contactText:"For questions, donation confirmation or any inquiry:",
 foot:"Donations go directly to the account/wallet shown on this page. If you received this link from someone you don't know, verify the campaign details with the organizers before donating."
 }
};
const DIR = {he:"rtl", ar:"rtl", en:"ltr"};
const $ = s => document.querySelector(s);
let lang = "en";

function pick(){
 try { const s = localStorage.getItem("lang"); if (T[s]) return s; } catch(_){}
 const n = (navigator.language || "en").toLowerCase();
 if (n.startsWith("he") || n.startsWith("iw")) return "he";
 if (n.startsWith("ar")) return "ar";
 return "en";
}
function apply(l){
 lang = l;
 const d = document.documentElement;
 d.lang = l; d.dir = DIR[l];
 document.title = T[l].title;
 document.querySelectorAll("[data-i]").forEach(el => { el.textContent = T[l][el.dataset.i]; });
 document.querySelectorAll(".langs button").forEach(b => b.setAttribute("aria-pressed", b.dataset.lang === l));
 try { localStorage.setItem("lang", l); } catch(_){}
}
document.querySelectorAll(".langs button").forEach(b => b.onclick = () => apply(b.dataset.lang));
apply(pick());

$("#copy").onclick = async e => {
 const b = e.currentTarget, text = $("#addr").textContent;
 try { await navigator.clipboard.writeText(text); }
 catch(_){ const r = document.createRange(); r.selectNodeContents($("#addr")); const s = getSelection(); s.removeAllRanges(); s.addRange(r); }
 b.textContent = T[lang].copied; b.classList.add("done");
 setTimeout(() => { b.textContent = T[lang].copy; b.classList.remove("done"); }, 1600);
};

$("#copyPaypal").onclick = async e => {
 const b = e.currentTarget, text = $("#paypalEmail").textContent;
 try { await navigator.clipboard.writeText(text); }
 catch(_){ const r = document.createRange(); r.selectNodeContents($("#paypalEmail")); const s = getSelection(); s.removeAllRanges(); s.addRange(r); }
 b.textContent = T[lang].copied; b.classList.add("done");
 setTimeout(() => { b.textContent = T[lang].copy; b.classList.remove("done"); }, 1600);
};

$("#share").onclick = async e => {
 const b = e.currentTarget, url = location.href;
 try {
 if (navigator.share) { await navigator.share({ title: T[lang].title, text: T[lang].lead, url }); return; }
 await navigator.clipboard.writeText(url);
 b.textContent = T[lang].copied; setTimeout(() => { b.textContent = T[lang].share; }, 1600);
 } catch(_){}
};
</script>