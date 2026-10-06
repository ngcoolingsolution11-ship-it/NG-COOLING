<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<meta name="theme-color" content="#0b1f3a">
<meta name="description" content="N.G Cooling Solution - Home Appliances Service & Repair">

<title>N.G Cooling Solution | V1.5</title>

<style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
    font-family:Arial,"Noto Sans Bengali",sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#f4f7fb;
    color:#172033;
    line-height:1.5;
}

button,
input,
textarea,
select{
    font-family:inherit;
}

/* ================= COLORS ================= */

:root{
    --navy:#0b1f3a;
    --navy2:#102f55;
    --blue:#075985;
    --sky:#0284c7;
    --green:#16a34a;
    --white:#ffffff;
    --text:#172033;
    --muted:#64748b;
    --border:#e2e8f0;
    --light:#eff6ff;
}

/* ================= HEADER ================= */

header{
    position:sticky;
    top:0;
    z-index:1000;
    background:rgba(255,255,255,.95);
    backdrop-filter:blur(16px);
    border-bottom:1px solid var(--border);
    box-shadow:0 4px 20px rgba(11,31,58,.09);
}

.header-inner{
    max-width:1200px;
    min-height:72px;
    margin:auto;
    padding:10px 16px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:12px;
}

.logo-area{
    display:flex;
    align-items:center;
    gap:10px;
    min-width:0;
}

.logo-icon{
    width:48px;
    height:48px;
    border-radius:15px;
    background:linear-gradient(135deg,var(--navy),var(--blue));
    color:white;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:24px;
    flex-shrink:0;
    box-shadow:0 7px 18px rgba(11,31,58,.25);
}

.logo-text{
    min-width:0;
}

.logo-text h1{
    color:var(--navy);
    font-size:18px;
    font-weight:900;
    white-space:nowrap;
}

.logo-text p{
    color:var(--muted);
    font-size:10px;
    font-weight:700;
}

.version{
    display:inline-block;
    margin-left:5px;
    padding:3px 7px;
    border-radius:8px;
    background:#dbeafe;
    color:var(--navy);
    font-size:9px;
    vertical-align:middle;
}

.whatsapp-btn{
    min-height:44px;
    padding:10px 16px;
    border-radius:13px;
    background:var(--green);
    color:white;
    text-decoration:none;
    font-size:13px;
    font-weight:900;
    display:inline-flex;
    align-items:center;
    justify-content:center;
    gap:7px;
    box-shadow:0 6px 18px rgba(22,163,74,.25);
    transition:.2s;
    white-space:nowrap;
}

.whatsapp-btn:hover{
    transform:translateY(-2px);
}

.whatsapp-btn:active{
    transform:scale(.96);
}

/* ================= HERO ================= */

.hero{
    position:relative;
    overflow:hidden;
    background:
        radial-gradient(circle at 90% 10%,rgba(56,189,248,.24),transparent 30%),
        radial-gradient(circle at 5% 90%,rgba(59,130,246,.18),transparent 30%),
        linear-gradient(135deg,#06172c,#0b1f3a 52%,#123c69);
    color:white;
    padding:52px 16px 64px;
}

.hero:before{
    content:"";
    position:absolute;
    width:300px;
    height:300px;
    right:-120px;
    top:-120px;
    border:1px solid rgba(255,255,255,.12);
    border-radius:50%;
}

.hero:after{
    content:"";
    position:absolute;
    width:180px;
    height:180px;
    left:-90px;
    bottom:-90px;
    border:1px solid rgba(255,255,255,.10);
    border-radius:50%;
}

.hero-inner{
    max-width:1200px;
    margin:auto;
    position:relative;
    z-index:2;
}

.hero-content{
    max-width:800px;
}

.hero-badge{
    display:inline-flex;
    align-items:center;
    gap:7px;
    background:rgba(255,255,255,.11);
    border:1px solid rgba(255,255,255,.20);
    padding:8px 14px;
    border-radius:30px;
    font-size:12px;
    font-weight:800;
    margin-bottom:18px;
}

.hero h2{
    font-size:clamp(34px,6vw,58px);
    line-height:1.04;
    font-weight:900;
    margin-bottom:17px;
}

.hero h2 span{
    display:block;
    color:#bae6fd;
}

.hero-description{
    max-width:710px;
    color:#dbeafe;
    font-size:15px;
    margin-bottom:28px;
}

.hero-buttons{
    display:flex;
    flex-wrap:wrap;
    gap:12px;
}

.primary-btn,
.secondary-btn{
    min-height:53px;
    padding:14px 25px;
    border:none;
    border-radius:14px;
    font-size:15px;
    font-weight:900;
    text-decoration:none;
    display:inline-flex;
    align-items:center;
    justify-content:center;
    gap:8px;
    cursor:pointer;
    transition:.2s;
}

.primary-btn{
    background:white;
    color:var(--navy);
    box-shadow:0 8px 22px rgba(0,0,0,.16);
}

.secondary-btn{
    background:var(--green);
    color:white;
    box-shadow:0 8px 22px rgba(22,163,74,.25);
}

.primary-btn:hover,
.secondary-btn:hover{
    transform:translateY(-2px);
}

.primary-btn:active,
.secondary-btn:active{
    transform:scale(.96);
}

/* ================= CONTAINER ================= */

.container{
    max-width:1200px;
    margin:auto;
    padding:0 16px;
}

.section{
    padding:40px 0;
}

.section-title{
    text-align:center;
    margin-bottom:23px;
}

.section-title h2{
    color:var(--navy);
    font-size:27px;
    font-weight:900;
}

.section-title p{
    color:var(--muted);
    font-size:13px;
    margin-top:5px;
}

/* ================= WARRANTY ================= */

.warranty{
    margin-top:-25px;
    position:relative;
    z-index:5;
}

.warranty-box{
    max-width:920px;
    margin:auto;
    background:white;
    border:1px solid var(--border);
    border-radius:21px;
    padding:19px;
    display:flex;
    align-items:center;
    justify-content:center;
    gap:13px;
    box-shadow:0 13px 38px rgba(11,31,58,.12);
}

.warranty-icon{
    width:48px;
    height:48px;
    border-radius:50%;
    background:#dcfce7;
    color:#15803d;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:23px;
}

.warranty-text strong{
    display:block;
    color:#15803d;
    font-size:17px;
}

.warranty-text span{
    color:var(--muted);
    font-size:12px;
}

/* ================= QUICK STATS ================= */

.quick-stats{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:13px;
}

.stat{
    background:white;
    border:1px solid var(--border);
    border-radius:18px;
    padding:18px 10px;
    text-align:center;
    box-shadow:0 6px 20px rgba(11,31,58,.05);
}

.stat-icon{
    font-size:25px;
    margin-bottom:4px;
}

.stat strong{
    display:block;
    color:var(--navy);
    font-size:14px;
}

.stat span{
    color:var(--muted);
    font-size:10px;
}

/* ================= SEARCH ================= */

.search-box{
    max-width:670px;
    margin:0 auto 22px;
}

.search-box input{
    width:100%;
    height:53px;
    border:1px solid #d5deea;
    border-radius:16px;
    padding:0 18px;
    outline:none;
    font-size:14px;
    background:white;
    box-shadow:0 6px 20px rgba(11,31,58,.06);
}

.search-box input:focus{
    border-color:var(--navy);
    box-shadow:0 0 0 3px rgba(11,31,58,.08);
}

/* ================= SERVICE CARDS ================= */

.service-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:15px;
}

.service-card{
    position:relative;
    overflow:hidden;
    background:white;
    border:1px solid var(--border);
    border-radius:19px;
    padding:18px;
    box-shadow:0 7px 21px rgba(11,31,58,.06);
    transition:.2s;
}

.service-card:before{
    content:"";
    position:absolute;
    left:0;
    top:0;
    width:100%;
    height:4px;
    background:linear-gradient(90deg,var(--navy),var(--blue));
}

.service-card:hover{
    transform:translateY(-4px);
    box-shadow:0 15px 32px rgba(11,31,58,.12);
}

.service-icon{
    width:48px;
    height:48px;
    border-radius:14px;
    background:#e8f1fb;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:23px;
    margin-bottom:11px;
}

.service-card h3{
    color:var(--navy);
    font-size:15px;
    line-height:1.35;
    margin-bottom:7px;
}

.price{
    color:#000;
    font-size:19px;
    font-weight:900;
    margin-bottom:12px;
}

/* NAVY BOOKING BUTTON */

.book-btn{
    width:100%;
    min-height:45px;
    border:none;
    border-radius:12px;
    background:var(--navy);
    color:white;
    cursor:pointer;
    font-size:13px;
    font-weight:900;
    transition:.2s;
    box-shadow:0 5px 13px rgba(11,31,58,.20);
}

.book-btn:hover{
    background:#123c69;
    transform:translateY(-1px);
}

.book-btn:active{
    transform:scale(.97);
}

/* ================= INFO ================= */

.info-strip{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:13px;
}

.info-box{
    background:white;
    border:1px solid var(--border);
    border-radius:18px;
    padding:18px;
    text-align:center;
    box-shadow:0 6px 18px rgba(11,31,58,.05);
}

.info-box .icon{
    font-size:25px;
    margin-bottom:5px;
}

.info-box strong{
    display:block;
    font-size:14px;
    color:var(--navy);
}

.info-box span{
    color:var(--muted);
    font-size:11px;
}

/* ================= LOCATION ================= */

.location-box{
    background:linear-gradient(135deg,#edf5ff,#f8fafc);
    border:1px solid #d8e7f8;
    border-radius:22px;
    padding:24px;
}

.location-list{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:9px;
}

.location-tag{
    background:white;
    border:1px solid #d5e4f5;
    color:var(--navy);
    border-radius:30px;
    padding:9px 14px;
    font-size:12px;
    font-weight:800;
}

/* ================= WHY ================= */

.why-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:14px;
}

.why-card{
    background:white;
    border-radius:18px;
    padding:21px 14px;
    text-align:center;
    border:1px solid var(--border);
    box-shadow:0 6px 18px rgba(11,31,58,.05);
}

.why-icon{
    font-size:29px;
    margin-bottom:8px;
}

.why-card h3{
    color:var(--navy);
    font-size:14px;
    margin-bottom:4px;
}

.why-card p{
    color:var(--muted);
    font-size:11px;
}

/* ================= FOOTER ================= */

footer{
    background:var(--navy);
    color:white;
    padding:33px 16px 98px;
    margin-top:20px;
}

.footer-inner{
    max-width:1200px;
    margin:auto;
    text-align:center;
}

.footer-logo{
    font-size:22px;
    font-weight:900;
}

.footer-text{
    color:#bfdbfe;
    font-size:12px;
    margin:7px 0 16px;
}

.footer-wa{
    display:inline-flex;
    min-height:47px;
    padding:12px 21px;
    border-radius:13px;
    background:var(--green);
    color:white;
    text-decoration:none;
    font-weight:900;
    font-size:13px;
}

.copyright{
    margin-top:19px;
    color:#94a3b8;
    font-size:10px;
}

/* ================= FLOATING WHATSAPP ================= */

.floating-wa{
    position:fixed;
    right:16px;
    bottom:18px;
    width:59px;
    height:59px;
    border-radius:50%;
    background:var(--green);
    color:white;
    display:flex;
    align-items:center;
    justify-content:center;
    text-decoration:none;
    font-size:27px;
    box-shadow:0 9px 28px rgba(22,163,74,.40);
    z-index:1100;
    animation:pulse 2s infinite;
}

@keyframes pulse{
    0%,100%{
        box-shadow:0 9px 28px rgba(22,163,74,.40);
    }
    50%{
        box-shadow:0 9px 35px rgba(22,163,74,.68);
    }
}

/* ================= MODAL ================= */

.modal{
    position:fixed;
    inset:0;
    background:rgba(2,6,23,.74);
    display:none;
    align-items:center;
    justify-content:center;
    padding:15px;
    z-index:2000;
}

.modal.show{
    display:flex;
}

.modal-box{
    width:min(620px,100%);
    max-height:93vh;
    overflow:auto;
    background:white;
    border-radius:24px;
    padding:23px;
    position:relative;
    box-shadow:0 25px 75px rgba(0,0,0,.34);
}

.modal-header{
    padding-right:42px;
    margin-bottom:16px;
}

.modal-header h2{
    color:var(--navy);
    font-size:22px;
}

.modal-header p{
    color:var(--muted);
    font-size:12px;
    margin-top:3px;
}

.close-btn{
    position:absolute;
    right:15px;
    top:13px;
    width:39px;
    height:39px;
    border:none;
    border-radius:50%;
    background:#f1f5f9;
    color:#475569;
    cursor:pointer;
    font-size:22px;
}

.selected-service{
    background:#edf5ff;
    border:1px solid #c9ddf2;
    border-radius:14px;
    padding:13px;
    margin-bottom:15px;
}

.selected-service strong{
    display:block;
    color:var(--navy);
    font-size:14px;
}

.selected-service span{
    color:#000;
    font-weight:900;
    font-size:17px;
}

.form-group{
    margin-bottom:12px;
}

.form-group label{
    display:block;
    margin-bottom:5px;
    font-size:12px;
    font-weight:900;
    color:#334155;
}

.form-group input,
.form-group textarea,
.form-group select{
    width:100%;
    border:1px solid #dbe3ec;
    border-radius:12px;
    min-height:46px;
    padding:10px 12px;
    outline:none;
    font-size:13px;
    background:white;
}

.form-group textarea{
    min-height:78px;
    resize:vertical;
}

.form-group input:focus,
.form-group textarea:focus,
.form-group select:focus{
    border-color:var(--navy);
    box-shadow:0 0 0 3px rgba(11,31,58,.08);
}

.gps-row{
    display:flex;
    gap:8px;
}

.gps-row input{
    flex:1;
}

.gps-btn{
    min-width:112px;
    border:none;
    border-radius:12px;
    background:var(--navy);
    color:white;
    cursor:pointer;
    font-size:12px;
    font-weight:900;
}

/* NAVY CONFIRM BOOKING */

.submit-btn{
    width:100%;
    min-height:52px;
    border:none;
    border-radius:14px;
    background:var(--navy);
    color:white;
    cursor:pointer;
    font-size:15px;
    font-weight:900;
    margin-top:5px;
    box-shadow:0 7px 17px rgba(11,31,58,.22);
    transition:.2s;
}

.submit-btn:hover{
    background:#123c69;
}

.submit-btn:active{
    transform:scale(.98);
}

.modal-note{
    text-align:center;
    color:var(--muted);
    font-size:10px;
    margin-top:9px;
}

/* ================= TOAST ================= */

.toast{
    position:fixed;
    left:50%;
    bottom:91px;
    transform:translateX(-50%) translateY(20px);
    background:var(--navy);
    color:white;
    padding:11px 17px;
    border-radius:12px;
    font-size:12px;
    opacity:0;
    pointer-events:none;
    transition:.25s;
    z-index:3000;
    max-width:90%;
    text-align:center;
}

.toast.show{
    opacity:1;
    transform:translateX(-50%) translateY(0);
}

.no-result{
    display:none;
    text-align:center;
    padding:20px;
    color:var(--muted);
    font-size:13px;
}

/* ================= MOBILE ================= */

@media(max-width:900px){

    .service-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .why-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .quick-stats{
        grid-template-columns:repeat(2,1fr);
    }
}

@media(max-width:600px){

    .header-inner{
        min-height:62px;
        padding:8px 11px;
    }

    .logo-icon{
        width:40px;
        height:40px;
        font-size:21px;
        border-radius:12px;
    }

    .logo-text h1{
        font-size:13px;
    }

    .logo-text p{
        font-size:8px;
    }

    .version{
        font-size:8px;
        padding:2px 5px;
    }

    .whatsapp-btn{
        min-height:40px;
        padding:9px 10px;
        font-size:10px;
    }

    .hero{
        padding:38px 14px 47px;
    }

    .hero h2{
        font-size:31px;
    }

    .hero-description{
        font-size:13px;
    }

    .hero-buttons{
        display:grid;
        grid-template-columns:1fr 1fr;
        gap:10px;
    }

    .primary-btn,
    .secondary-btn{
        min-height:54px;
        padding:13px 8px;
        font-size:13px;
    }

    .container{
        padding:0 12px;
    }

    .section{
        padding:29px 0;
    }

    .section-title h2{
        font-size:22px;
    }

    .quick-stats{
        grid-template-columns:1fr 1fr;
        gap:9px;
    }

    .stat{
        padding:14px 7px;
    }

    .stat strong{
        font-size:12px;
    }

    .service-grid{
        grid-template-columns:1fr 1fr;
        gap:9px;
    }

    .service-card{
        padding:13px;
        border-radius:15px;
    }

    .service-icon{
        width:39px;
        height:39px;
        font-size:19px;
        border-radius:11px;
    }

    .service-card h3{
        font-size:12px;
    }

    .price{
        font-size:16px;
    }

    .book-btn{
        min-height:42px;
        font-size:11px;
    }

    .info-strip{
        grid-template-columns:1fr;
    }

    .warranty{
        margin-top:-17px;
    }

    .warranty-box{
        margin:0 5px;
        padding:14px;
    }

    .warranty-text strong{
        font-size:15px;
    }

    .location-box{
        padding:16px;
    }

    .location-tag{
        padding:8px 11px;
        font-size:10px;
    }

    .modal-box{
        padding:17px;
        border-radius:19px;
    }

    .gps-row{
        flex-direction:column;
    }

    .gps-btn{
        min-height:43px;
    }

    .floating-wa{
        width:54px;
        height:54px;
        right:13px;
        bottom:14px;
    }
}

@media(max-width:380px){

    .logo-text h1{
        font-size:11px;
    }

    .whatsapp-btn{
        padding:8px;
    }

    .hero h2{
        font-size:27px;
    }

    .service-grid{
        gap:7px;
    }

    .service-card{
        padding:10px;
    }
}
</style>
</head>

<body>

<!-- ================= HEADER ================= -->

<header>
<div class="header-inner">

    <div class="logo-area">

        <div class="logo-icon">❄️</div>

        <div class="logo-text">

            <h1>
                N.G Cooling Solution
                <span class="version">V1.5</span>
            </h1>

            <p>
                Home Appliances Service & Repair
            </p>

        </div>

    </div>

    <a
        class="whatsapp-btn"
        href="https://wa.me/918420063054"
        target="_blank"
    >
        💬 WhatsApp
    </a>

</div>
</header>


<!-- ================= HERO ================= -->

<section class="hero">

<div class="hero-inner">

<div class="hero-content">

    <div class="hero-badge">
        🚀 Advanced 2026 Model • V1.5
    </div>

    <h2>
        Home Appliances
        <span>Service & Repair</span>
    </h2>

    <p class="hero-description">
        AC, Fridge, Washing Machine, Microwave, Geyser ও
        Water Purifier-এর জন্য দ্রুত ও নির্ভরযোগ্য
        Home Service & Repair।
    </p>

    <div class="hero-buttons">

        <button
            class="primary-btn"
            onclick="viewServices()"
        >
            🛠️ View Services
        </button>

        <a
            class="secondary-btn"
            href="https://wa.me/918420063054"
            target="_blank"
        >
            💬 WhatsApp
        </a>

    </div>

</div>

</div>
</section>


<!-- ================= WARRANTY ================= -->

<section class="warranty">

<div class="warranty-box">

    <div class="warranty-icon">
        🛡️
    </div>

    <div class="warranty-text">
        <strong>90 Days Warranty</strong>

        <span>
            Selected repair / parts replacement work-এর ক্ষেত্রে প্রযোজ্য
        </span>
    </div>

</div>
</section>


<!-- ================= QUICK STATS ================= -->

<section class="section">

<div class="container">

<div class="quick-stats">

    <div class="stat">
        <div class="stat-icon">👨‍🔧</div>
        <strong>Professional</strong>
        <span>Technician Team</span>
    </div>

    <div class="stat">
        <div class="stat-icon">⚡</div>
        <strong>Quick Service</strong>
        <span>Fast Booking</span>
    </div>

    <div class="stat">
        <div class="stat-icon">🧾</div>
        <strong>Service Bill</strong>
        <span>Bill Provided</span>
    </div>

    <div class="stat">
        <div class="stat-icon">💬</div>
        <strong>WhatsApp</strong>
        <span>Easy Booking</span>
    </div>

</div>

</div>
</section>


<!-- ================= POPULAR SERVICES ================= -->

<section class="section">

<div class="container">

<div class="section-title">

    <h2>⭐ Popular Services</h2>

    <p>
        দ্রুত Booking-এর জন্য জনপ্রিয় Service
    </p>

</div>

<div class="search-box">

    <input
        type="text"
        id="serviceSearch"
        placeholder="🔍 Service Search করুন..."
        oninput="searchServices()"
    >

</div>


<div
    class="service-grid"
    id="popularServices"
>

    <div class="service-card"
         data-service="AC General Service">

        <div class="service-icon">❄️</div>

        <h3>
            AC General Service
        </h3>

        <div class="price">
            ₹399
        </div>

        <button
            class="book-btn"
            onclick="openBooking('AC General Service','399')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="Foam Jet AC Service">

        <div class="service-icon">💦</div>

        <h3>
            Foam-Jet AC Service
        </h3>

        <div class="price">
            ₹499
        </div>

        <button
            class="book-btn"
            onclick="openBooking('Foam-Jet AC Service','499')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="Lite AC Service">

        <div class="service-icon">🧹</div>

        <h3>
            Lite AC Service
        </h3>

        <div class="price">
            ₹399
        </div>

        <button
            class="book-btn"
            onclick="openBooking('Lite AC Service','399')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="AC Water Leakage Repair">

        <div class="service-icon">💧</div>

        <h3>
            AC Water Leakage Repair
        </h3>

        <div class="price">
            ₹499
        </div>

        <button
            class="book-btn"
            onclick="openBooking('AC Water Leakage Repair','499')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="AC Cooling Problem">

        <div class="service-icon">🌬️</div>

        <h3>
            AC Cooling Problem
        </h3>

        <div class="price">
            ₹199
        </div>

        <button
            class="book-btn"
            onclick="openBooking('AC Cooling Problem','199')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="AC No Cooling Issue">

        <div class="service-icon">🥶</div>

        <h3>
            AC No Cooling Issue
        </h3>

        <div class="price">
            ₹199
        </div>

        <button
            class="book-btn"
            onclick="openBooking('AC No Cooling Issue','199')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="Fridge Cooling Problem">

        <div class="service-icon">🧊</div>

        <h3>
            Fridge Cooling Problem
        </h3>

        <div class="price">
            ₹199
        </div>

        <button
            class="book-btn"
            onclick="openBooking('Fridge Cooling Problem','199')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="Washing Machine Not Working">

        <div class="service-icon">🧺</div>

        <h3>
            Washing Machine Not Working
        </h3>

        <div class="price">
            ₹199
        </div>

        <button
            class="book-btn"
            onclick="openBooking('Washing Machine Not Working','199')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="Microwave Repair">

        <div class="service-icon">🍽️</div>

        <h3>
            Microwave Repair
        </h3>

        <div class="price">
            ₹199
        </div>

        <button
            class="book-btn"
            onclick="openBooking('Microwave Repair','199')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="Geyser Heating Problem">

        <div class="service-icon">🚿</div>

        <h3>
            Geyser Heating Problem
        </h3>

        <div class="price">
            ₹199
        </div>

        <button
            class="book-btn"
            onclick="openBooking('Geyser Heating Problem','199')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="Water Purifier Repair">

        <div class="service-icon">💧</div>

        <h3>
            Water Purifier Repair
        </h3>

        <div class="price">
            ₹199
        </div>

        <button
            class="book-btn"
            onclick="openBooking('Water Purifier Repair','199')"
        >
            Book Now
        </button>

    </div>


    <div class="service-card"
         data-service="AC Repair">

        <div class="service-icon">🔧</div>

        <h3>
            AC Repair
        </h3>

        <div class="price">
            ₹199
        </div>

        <button
            class="book-btn"
            onclick="openBooking('AC Repair','199')"
        >
            Book Now
        </button>

    </div>

</div>


<div
    id="noResult"
    class="no-result"
>
    কোনো Service পাওয়া যায়নি।
</div>

</div>
</section>


<!-- ================= INFO STRIP ================= -->

<section
    class="section"
    style="padding-top:0;"
>

<div class="container">

<div class="info-strip">

    <div class="info-box">

        <div class="icon">👨‍🔧</div>

        <strong>
            Professional Technician
        </strong>

        <span>
            Experienced Service Team
        </span>

    </div>


    <div class="info-box">

        <div class="icon">🧾</div>

        <strong>
            Service Bill
        </strong>

        <span>
            Service-এর পর Bill প্রদান
        </span>

    </div>


    <div class="info-box">

        <div class="icon">💬</div>

        <strong>
            WhatsApp Booking
        </strong>

        <span>
            সহজে Booking Confirmation
        </span>

    </div>

</div>

</div>
</section>


<!-- ================= ALL SERVICES ================= -->

<section
    class="section"
    id="allServicesSection"
>

<div class="container">

<div class="section-title">

    <h2>
        🛠️ All Services
    </h2>

    <p>
        Home Appliances Service & Repair
    </p>

</div>


<div class="service-grid">

    <div class="service-card">
        <div class="service-icon">❄️</div>
        <h3>AC Service</h3>
        <div class="price">₹399</div>
        <button class="book-btn"
            onclick="openBooking('AC Service','399')">
            Book Now
        </button>
    </div>


    <div class="service-card">
        <div class="service-icon">🔧</div>
        <h3>AC Repair</h3>
        <div class="price">₹199</div>
        <button class="book-btn"
            onclick="openBooking('AC Repair','199')">
            Book Now
        </button>
    </div>


    <div class="service-card">
        <div class="service-icon">🏠</div>
        <h3>AC Installation</h3>
        <div class="price">₹1499</div>
        <button class="book-btn"
            onclick="openBooking('AC Installation','1499')">
            Book Now
        </button>
    </div>


    <div class="service-card">
        <div class="service-icon">⛽</div>
        <h3>AC Gas Charging</h3>
        <div class="price">₹2499</div>
        <button class="book-btn"
            onclick="openBooking('AC Gas Charging','2499')">
            Book Now
        </button>
    </div>


    <div class="service-card">
        <div class="service-icon">📦</div>
        <h3>AC Uninstallation</h3>
        <div class="price">₹599</div>
        <button class="book-btn"
            onclick="openBooking('AC Uninstallation','599')">
            Book Now
        </button>
    </div>


    <div class="service-card">
        <div class="service-icon">🧊</div>
        <h3>Fridge Repair</h3>
        <div class="price">₹199</div>
        <button class="book-btn"
            onclick="openBooking('Fridge Repair','199')">
            Book Now
        </button>
    </div>


    <div class="service-card">
        <div class="service-icon">🧺</div>
        <h3>Washing Machine Repair</h3>
        <div class="price">₹199</div>
        <button class="book-btn"
            onclick="openBooking('Washing Machine Repair','199')">
            Book Now
        </button>
    </div>


    <div class="service-card">
        <div class="service-icon">🍽️</div>
        <h3>Microwave Repair</h3>
        <div class="price">₹199</div>
        <button class="book-btn"
            onclick="openBooking('Microwave Repair','199')">
            Book Now
        </button>
    </div>


    <div class="service-card">
        <div class="service-icon">🚿</div>
        <h3>Geyser Repair</h3>
        <div class="price">₹199</div>
        <button class="book-btn"
            onclick="openBooking('Geyser Repair','199')">
            Book Now
        </button>
    </div>


    <div class="service-card">
        <div class="service-icon">💧</div>
        <h3>Water Purifier Service</h3>
        <div class="price">₹199</div>
        <button class="book-btn"
            onclick="openBooking('Water Purifier Service','199')">
            Book Now
        </button>
    </div>

</div>

</div>
</section>


<!-- ================= LOCATION ================= -->

<section class="section">

<div class="container">

<div class="section-title">

    <h2>
        📍 Service Location
    </h2>

    <p>
        Dum Dum ও আশেপাশের এলাকায় Service
    </p>

</div>


<div class="location-box">

<div class="location-list">

    <div class="location-tag">📍 Dum Dum</div>
    <div class="location-tag">📍 Dakshineswar</div>
    <div class="location-tag">📍 Belghoria</div>
    <div class="location-tag">📍 Belgachia</div>
    <div class="location-tag">📍 Shyambazar</div>
    <div class="location-tag">📍 Lake Town</div>
    <div class="location-tag">📍 Barasat</div>
    <div class="location-tag">📍 New Town</div>
    <div class="location-tag">📍 Rajarhat</div>
    <div class="location-tag">📍 Dum Dum & Nearby</div>

</div>

</div>

</div>
</section>


<!-- ================= WHY CHOOSE US ================= -->

<section class="section">

<div class="container">

<div class="section-title">

    <h2>
        ⭐ Why Choose Us
    </h2>

    <p>
        Service-এর সময় আমাদের সুবিধাগুলি
    </p>

</div>


<div class="why-grid">

    <div class="why-card">
        <div class="why-icon">👨‍🔧</div>
        <h3>Experienced Team</h3>
        <p>অভিজ্ঞ Technician দ্বারা Service</p>
    </div>

    <div class="why-card">
        <div class="why-icon">⚡</div>
        <h3>Quick Service</h3>
        <p>দ্রুত Booking ও Service Support</p>
    </div>

    <div class="why-card">
        <div class="why-icon">🧾</div>
        <h3>Bill Provided</h3>
        <p>Service-এর পর Bill প্রদান</p>
    </div>

    <div class="why-card">
        <div class="why-icon">🛡️</div>
        <h3>90 Days Warranty</h3>
        <p>Selected repair work-এর ক্ষেত্রে</p>
    </div>

</div>

</div>
</section>


<!-- ================= FOOTER ================= -->

<footer>

<div class="footer-inner">

    <div class="footer-logo">
        ❄️ N.G Cooling Solution
    </div>

    <div class="footer-text">
        Home Appliances Service & Repair • V1.5 • 2026
    </div>

    <a
        class="footer-wa"
        href="https://wa.me/918420063054"
        target="_blank"
    >
        💬 WhatsApp: 8420063054
    </a>

    <div class="copyright">
        © 2026 N.G Cooling Solution. All Rights Reserved.
    </div>

</div>
</footer>


<!-- ================= FLOATING WHATSAPP ================= -->

<a
    class="floating-wa"
    href="https://wa.me/918420063054"
    target="_blank"
    aria-label="WhatsApp"
>
    💬
</a>


<!-- ================= BOOKING MODAL ================= -->

<div
    class="modal"
    id="bookingModal"
>

<div class="modal-box">

<button
    class="close-btn"
    onclick="closeModal()"
    aria-label="Close"
>
    ×
</button>


<div class="modal-header">

    <h2>
        📋 Service Booking
    </h2>

    <p>
        তথ্য পূরণ করে WhatsApp-এ Booking পাঠান।
    </p>

</div>


<div class="selected-service">

    <strong id="selectedService">
        Service
    </strong>

    <span id="selectedPrice">
        ₹0
    </span>

</div>


<form id="bookingForm">


<div class="form-group">

    <label>
        Customer Name *
    </label>

    <input
        type="text"
        id="customerName"
        placeholder="আপনার নাম"
        required
    >

</div>


<div class="form-group">

    <label>
        Mobile Number *
    </label>

    <input
        type="tel"
        id="customerMobile"
        placeholder="10 Digit Mobile Number"
        maxlength="10"
        inputmode="numeric"
        required
    >

</div>


<div class="form-group">

    <label>
        Service Address *
    </label>

    <textarea
        id="serviceAddress"
        placeholder="সম্পূর্ণ Service Address লিখুন"
        required
    ></textarea>

</div>


<div class="form-group">

    <label>
        GPS Location
    </label>

    <div class="gps-row">

        <input
            type="text"
            id="gpsLocation"
            placeholder="GPS Location নেওয়া হয়নি"
            readonly
        >

        <button
            type="button"
            class="gps-btn"
            onclick="getGPS()"
        >
            📍 GPS Location
        </button>

    </div>

</div>


<div class="form-group">

    <label>
        Booking Date *
    </label>

    <input
        type="date"
        id="bookingDate"
        required
    >

</div>


<div class="form-group">

    <label>
        Booking Time *
    </label>

    <select
        id="bookingTime"
        required
    >

        <option value="">
            Select Time
        </option>

        <option>8 AM - 9 AM</option>
        <option>9 AM - 10 AM</option>
        <option>10 AM - 11 AM</option>
        <option>11 AM - 12 PM</option>
        <option>12 PM - 1 PM</option>
        <option>1 PM - 2 PM</option>
        <option>2 PM - 3 PM</option>
        <option>3 PM - 4 PM</option>
        <option>4 PM - 5 PM</option>
        <option>5 PM - 6 PM</option>
        <option>6 PM - 7 PM</option>
        <option>7 PM - 8 PM</option>
        <option>8 PM - 9 PM</option>
        <option>9 PM - 10 PM</option>

    </select>

</div>


<div class="form-group">

    <label>
        Problem / Details
    </label>

    <textarea
        id="problemDetails"
        placeholder="AC / Appliance-এর Problem লিখুন"
    ></textarea>

</div>


<button
    type="submit"
    class="submit-btn"
>
    💬 Confirm Booking on WhatsApp
</button>


<div class="modal-note">
    Booking submit করলে WhatsApp confirmation message তৈরি হবে।
</div>

</form>

</div>
</div>


<!-- ================= TOAST ================= -->

<div
    class="toast"
    id="toast"
></div>


<script>

/* ================= SETTINGS ================= */

const WHATSAPP_NUMBER = "918420063054";

let selectedServiceName = "";
let selectedServicePrice = "";


/* ================= VIEW SERVICES ================= */

function viewServices(){

    const section =
        document.getElementById("allServicesSection");

    if(section){

        section.scrollIntoView({
            behavior:"smooth",
            block:"start"
        });

    }
}


/* ================= OPEN BOOKING ================= */

function openBooking(service,price){

    selectedServiceName = service;

    selectedServicePrice = price;

    document.getElementById("selectedService")
        .textContent = service;

    document.getElementById("selectedPrice")
        .textContent = "₹" + price;

    document.getElementById("bookingModal")
        .classList.add("show");

    document.body.style.overflow = "hidden";
}


/* ================= CLOSE MODAL ================= */

function closeModal(){

    document.getElementById("bookingModal")
        .classList.remove("show");

    document.body.style.overflow = "";
}


/* ================= GPS ================= */

function getGPS(){

    const gpsInput =
        document.getElementById("gpsLocation");

    if(!navigator.geolocation){

        showToast(
            "আপনার Browser GPS Support করে না।"
        );

        return;
    }

    gpsInput.value =
        "Location নেওয়া হচ্ছে...";

    navigator.geolocation.getCurrentPosition(

        function(position){

            const lat =
                position.coords.latitude;

            const lng =
                position.coords.longitude;

            const mapLink =
                "https://www.google.com/maps?q="
                + lat + "," + lng;

            gpsInput.value =
                lat.toFixed(6)
                + ", "
                + lng.toFixed(6);

            gpsInput.dataset.link =
                mapLink;

            showToast(
                "📍 GPS Location নেওয়া হয়েছে"
            );
        },

        function(error){

            gpsInput.value = "";

            let message =
                "GPS Location নেওয়া যায়নি।";

            if(error.code === 1){

                message =
                    "Location Permission Allow করুন।";
            }

            showToast(message);
        },

        {
            enableHighAccuracy:true,
            timeout:10000,
            maximumAge:0
        }
    );
}


/* ================= BOOKING SUBMIT ================= */

document.getElementById("bookingForm")
.addEventListener("submit",function(event){

    event.preventDefault();

    const name =
        document.getElementById("customerName")
        .value.trim();

    const mobile =
        document.getElementById("customerMobile")
        .value.trim();

    const address =
        document.getElementById("serviceAddress")
        .value.trim();

    const date =
        document.getElementById("bookingDate")
        .value;

    const time =
        document.getElementById("bookingTime")
        .value;

    const problem =
        document.getElementById("problemDetails")
        .value.trim();

    const gpsInput =
        document.getElementById("gpsLocation");

    const gps =
        gpsInput.value.trim();

    const gpsLink =
        gpsInput.dataset.link || "";


    /* MOBILE VALIDATION */

    if(!/^[0-9]{10}$/.test(mobile)){

        showToast(
            "সঠিক 10 Digit Mobile Number দিন।"
        );

        return;
    }


    /* DATE VALIDATION */

    if(!date){

        showToast(
            "Booking Date নির্বাচন করুন।"
        );

        return;
    }


    /* CREATE BOOKING ID */

    const bookingId =
        "NG"
        + Date.now()
        .toString()
        .slice(-8);


    /* SAVE BOOKING */

    const booking = {

        bookingId:bookingId,

        service:selectedServiceName,

        price:selectedServicePrice,

        customerName:name,

        mobile:mobile,

        address:address,

        gps:gps,

        gpsLink:gpsLink,

        date:date,

        time:time,

        problem:problem,

        warranty:"90 Days Warranty",

        version:"V1.5",

        createdAt:new Date().toISOString()

    };


    let bookings = [];

    try{

        bookings =
            JSON.parse(
                localStorage.getItem(
                    "ngcs_bookings"
                )
            ) || [];

    }catch(error){

        bookings = [];

    }


    bookings.push(booking);


    localStorage.setItem(
        "ngcs_bookings",
        JSON.stringify(bookings)
    );


    /* WHATSAPP MESSAGE */

    const message =
`🛠️ *N.G COOLING SOLUTION*

📋 *SERVICE BOOKING*

🆔 *Booking ID:* ${bookingId}

📌 *Service:* ${selectedServiceName}
💰 *Starting Price:* ₹${selectedServicePrice}

👤 *Customer:* ${name}
📱 *Mobile:* ${mobile}

📍 *Service Address:*
${address}

📅 *Booking Date:* ${date}
⏰ *Booking Time:* ${time}

🔧 *Problem / Details:*
${problem || "Not Provided"}

🛡️ *Warranty:* 90 Days Warranty

📍 *GPS Location:*
${
    gpsLink
    ? gpsLink
    : (gps || "Not Provided")
}

🌐 *Website:* V1.5
📅 *Model:* Advanced 2026

Please confirm my service booking.`;


    const whatsappURL =
        "https://wa.me/"
        + WHATSAPP_NUMBER
        + "?text="
        + encodeURIComponent(message);


    closeModal();


    showToast(
        "✅ Booking Created • WhatsApp Opening..."
    );


    setTimeout(function(){

        window.open(
            whatsappURL,
            "_blank"
        );

    },700);


    document.getElementById("bookingForm")
        .reset();

    gpsInput.dataset.link = "";

});


/* ================= SEARCH ================= */

function searchServices(){

    const input =
        document.getElementById("serviceSearch")
        .value
        .toLowerCase()
        .trim();

    const cards =
        document.querySelectorAll(
            "#popularServices .service-card"
        );

    let visible = 0;


    cards.forEach(function(card){

        const service =
            card.dataset.service
            .toLowerCase();

        if(service.includes(input)){

            card.style.display = "";

            visible++;

        }else{

            card.style.display = "none";
        }

    });


    document.getElementById("noResult")
        .style.display =
            visible === 0
            ? "block"
            : "none";
}


/* ================= TOAST ================= */

let toastTimer;

function showToast(message){

    const toast =
        document.getElementById("toast");

    toast.textContent = message;

    toast.classList.add("show");

    clearTimeout(toastTimer);

    toastTimer =
        setTimeout(function(){

            toast.classList.remove("show");

        },3000);
}


/* ================= OUTSIDE MODAL ================= */

document.getElementById("bookingModal")
.addEventListener("click",function(event){

    if(event.target === this){

        closeModal();
    }

});


/* ================= ESCAPE ================= */

document.addEventListener(
    "keydown",
    function(event){

        if(event.key === "Escape"){

            closeModal();
        }

    }
);


/* ================= MIN BOOKING DATE ================= */

(function(){

    const dateInput =
        document.getElementById("bookingDate");

    const today =
        new Date();

    const year =
        today.getFullYear();

    const month =
        String(today.getMonth()+1)
        .padStart(2,"0");

    const day =
        String(today.getDate())
        .padStart(2,"0");

    dateInput.min =
        year + "-" + month + "-" + day;

})();

</script>

</body>
</html>
