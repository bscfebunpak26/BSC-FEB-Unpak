<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Absensi RFID — BSC FEB-Unpak</title>
<link href="https://fonts.googleapis.com/css2?family=Sora:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
:root{--o:#F97316;--od:#EA580C;--bk:#0A0A0A;--dk:#111827;--dk2:#1F2937;--dk3:#374151;--mu:#6B7280;--wh:#FFFFFF;--br:rgba(249,115,22,0.15);--ok:#10B981;--err:#EF4444;--warn:#F59E0B;--info:#3B82F6;--pu:#8B5CF6;}
*{margin:0;padding:0;box-sizing:border-box;}
body{font-family:'Sora',sans-serif;background:var(--bk);color:var(--wh);min-height:100vh;overflow-x:hidden;}
body::before{content:'';position:fixed;top:-200px;right:-200px;width:600px;height:600px;background:radial-gradient(circle,rgba(249,115,22,0.10) 0%,transparent 70%);pointer-events:none;z-index:0;}

/* ===SIDEBAR=== */
.sidebar{position:fixed;left:0;top:0;width:250px;height:100vh;background:var(--dk);border-right:1px solid var(--br);display:flex;flex-direction:column;z-index:100;overflow-y:auto;}
.sidebar-logo{padding:22px 20px 18px;border-bottom:1px solid var(--br);display:flex;align-items:center;gap:11px;flex-shrink:0;}
.logo-box{width:40px;height:40px;background:linear-gradient(135deg,#F97316,#EA580C);border-radius:10px;display:flex;align-items:center;justify-content:center;overflow:hidden;flex-shrink:0;cursor:pointer;position:relative;}
.logo-box:hover::after{content:'📷';position:absolute;inset:0;background:rgba(0,0,0,.55);display:flex;align-items:center;justify-content:center;font-size:16px;border-radius:10px;}
.logo-box img{width:100%;height:100%;object-fit:cover;border-radius:10px;display:block;}
.logo-t h1{font-size:12px;font-weight:700;color:var(--wh);letter-spacing:.4px;}
.logo-t p{font-size:9px;color:var(--mu);margin-top:1px;}
.sb-sec{padding:14px 14px 6px;}
.sb-lbl{font-size:9px;font-weight:600;color:var(--mu);letter-spacing:1.5px;text-transform:uppercase;padding:0 7px 7px;}
.nav{display:flex;align-items:center;gap:9px;padding:8px 10px;border-radius:7px;cursor:pointer;margin-bottom:2px;transition:all .15s;font-size:12px;font-weight:400;color:var(--mu);border:none;background:transparent;width:100%;text-align:left;}
.nav:hover{background:rgba(249,115,22,.08);color:var(--wh);}
.nav.active{background:rgba(249,115,22,.15);color:var(--o);font-weight:500;}
.nav-ic{font-size:14px;width:17px;text-align:center;}
.nav-badge{margin-left:auto;background:var(--o);color:#fff;font-size:9px;font-weight:700;padding:1px 6px;border-radius:20px;}
.sb-bot{margin-top:auto;padding:14px;border-top:1px solid var(--br);flex-shrink:0;}
.u-card{display:flex;align-items:center;gap:9px;padding:9px;border-radius:8px;background:rgba(249,115,22,.08);}
.u-av{width:34px;height:34px;border-radius:50%;background:linear-gradient(135deg,#F97316,#EA580C);display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:700;color:#fff;flex-shrink:0;}
.u-inf h4{font-size:11px;font-weight:600;color:var(--wh);}
.u-inf p{font-size:9px;color:var(--o);margin-top:1px;}

/* ===MAIN=== */
.main{margin-left:250px;min-height:100vh;position:relative;z-index:1;}
.topbar{display:flex;align-items:center;justify-content:space-between;padding:18px 28px;border-bottom:1px solid var(--br);background:rgba(10,10,10,.85);backdrop-filter:blur(10px);position:sticky;top:0;z-index:50;}
.tb-l h2{font-size:17px;font-weight:600;color:var(--wh);}
.tb-l p{font-size:11px;color:var(--mu);margin-top:2px;}
.tb-r{display:flex;align-items:center;gap:10px;}
.clock-chip{background:var(--dk2);border:1px solid var(--br);padding:5px 13px;border-radius:20px;font-size:11px;font-family:'JetBrains Mono',monospace;color:var(--o);}

/* ===PAGE SYSTEM=== */
.page{display:none;padding:24px 28px;}
.page.active{display:block;}

/* ===BUTTONS=== */
.btn{display:inline-flex;align-items:center;gap:6px;padding:8px 16px;border-radius:8px;font-family:'Sora',sans-serif;font-size:12px;font-weight:600;cursor:pointer;transition:all .15s;border:none;}
.btn-primary{background:var(--o);color:#fff;}
.btn-primary:hover{background:var(--od);}
.btn-ghost{background:transparent;color:var(--mu);border:1px solid var(--br);}
.btn-ghost:hover{border-color:var(--o);color:var(--o);}
.btn-danger{background:rgba(239,68,68,.15);color:#FC8181;border:1px solid rgba(239,68,68,.2);}
.btn-danger:hover{background:rgba(239,68,68,.25);}
.btn-sm{padding:5px 11px;font-size:11px;}

/* ===CARDS=== */
.card{background:var(--dk);border:1px solid var(--br);border-radius:14px;}
.card-p{padding:20px 22px;}
.card-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:16px;}
.card-title{font-size:13px;font-weight:600;color:var(--wh);}
.card-sub{font-size:11px;color:var(--mu);margin-top:2px;}

/* ===STATS=== */
.stats-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-bottom:22px;}
.stat{background:var(--dk);border:1px solid var(--br);border-radius:12px;padding:16px 18px;position:relative;overflow:hidden;}
.stat::after{content:attr(data-ico);position:absolute;right:12px;bottom:8px;font-size:26px;opacity:.1;}
.stat-lbl{font-size:9px;font-weight:600;color:var(--mu);letter-spacing:.5px;text-transform:uppercase;}
.stat-val{font-size:26px;font-weight:700;color:var(--wh);margin:5px 0 2px;font-family:'JetBrains Mono',monospace;}
.stat-note{font-size:10px;color:var(--mu);}

/* ===BADGES=== */
.badge{display:inline-flex;align-items:center;padding:2px 9px;border-radius:20px;font-size:10px;font-weight:600;}
.b-pi{background:rgba(139,92,246,.15);color:#A78BFA;}
.b-relasi{background:rgba(59,130,246,.15);color:#60A5FA;}
.b-kominfo{background:rgba(16,185,129,.15);color:#34D399;}
.b-pengurus{background:rgba(249,115,22,.15);color:var(--o);}
.b-hadir{background:rgba(16,185,129,.15);color:#34D399;}
.b-terlambat{background:rgba(245,158,11,.15);color:#FCD34D;}
.b-alpha{background:rgba(239,68,68,.15);color:#FC8181;}
.b-izin{background:rgba(107,114,128,.15);color:#9CA3AF;}

/* ===SCANNER=== */
.scanner-wrap{display:grid;grid-template-columns:1fr 360px;gap:18px;margin-bottom:22px;}
.rfid-card{background:var(--dk);border:1px solid var(--br);border-radius:16px;padding:28px;display:flex;flex-direction:column;align-items:center;text-align:center;position:relative;overflow:hidden;}
.rfid-card::before{content:'';position:absolute;top:0;left:50%;transform:translateX(-50%);width:200px;height:2px;background:linear-gradient(90deg,transparent,var(--o),transparent);}
.scan-lbl{font-size:10px;font-weight:600;letter-spacing:2px;color:var(--o);text-transform:uppercase;margin-bottom:20px;}
.ring{width:150px;height:150px;border-radius:50%;position:relative;display:flex;align-items:center;justify-content:center;margin-bottom:20px;}
.ring::before{content:'';position:absolute;inset:0;border-radius:50%;border:2px solid transparent;background:linear-gradient(135deg,var(--o),transparent,var(--o)) border-box;animation:spin 3s linear infinite;}
.ring::after{content:'';position:absolute;inset:8px;border-radius:50%;border:1px solid rgba(249,115,22,.2);animation:pr 2s ease-in-out infinite;}
@keyframes spin{to{transform:rotate(360deg)}}
@keyframes pr{0%,100%{opacity:.3;transform:scale(1)}50%{opacity:1;transform:scale(1.02)}}
.ring-ico{font-size:48px;position:relative;z-index:1;animation:fl 3s ease-in-out infinite;}
@keyframes fl{0%,100%{transform:translateY(0)}50%{transform:translateY(-5px)}}
.scan-status{font-size:14px;font-weight:500;color:var(--wh);margin-bottom:5px;}
.scan-sub2{font-size:11px;color:var(--mu);}
.scan-inp-row{margin-top:18px;width:100%;display:flex;gap:8px;}
.rfid-in{flex:1;background:var(--dk2);border:1px solid var(--br);border-radius:8px;padding:9px 13px;font-family:'JetBrains Mono',monospace;font-size:13px;color:var(--wh);outline:none;transition:border-color .15s;}
.rfid-in:focus{border-color:var(--o);}
.rfid-in::placeholder{color:var(--mu);}

/* ===RECENT LIST=== */
.recent-card{background:var(--dk);border:1px solid var(--br);border-radius:16px;padding:18px;display:flex;flex-direction:column;}
.scan-item{display:flex;align-items:center;gap:10px;padding:9px 0;border-bottom:1px solid rgba(249,115,22,.05);}
.scan-item:last-child{border-bottom:none;}
@keyframes si{from{opacity:0;transform:translateX(8px)}to{opacity:1;transform:translateX(0)}}
.scan-av{width:34px;height:34px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;color:#fff;flex-shrink:0;}
.scan-inf{flex:1;min-width:0;}
.scan-nm{font-size:11px;font-weight:500;color:var(--wh);white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
.scan-rl{font-size:10px;color:var(--mu);margin-top:1px;}
.scan-tm{font-family:'JetBrains Mono',monospace;font-size:10px;color:var(--o);}

/* ===TABLE=== */
.tbl-wrap{background:var(--dk);border:1px solid var(--br);border-radius:14px;overflow:hidden;}
.tbl-hdr{padding:16px 20px;border-bottom:1px solid var(--br);display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:10px;}
table{width:100%;border-collapse:collapse;}
thead tr{border-bottom:1px solid var(--br);}
th{padding:9px 20px;text-align:left;font-size:9px;font-weight:600;color:var(--mu);letter-spacing:.8px;text-transform:uppercase;}
td{padding:11px 20px;font-size:12px;color:var(--wh);}
tbody tr{border-bottom:1px solid rgba(249,115,22,.04);transition:background .1s;}
tbody tr:hover{background:rgba(249,115,22,.04);}
tbody tr:last-child{border-bottom:none;}
.mb-cell{display:flex;align-items:center;gap:9px;}
.mb-av{width:28px;height:28px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:9px;font-weight:700;color:#fff;}
.mb-nm{font-weight:500;font-size:11px;}
.mb-id{font-family:'JetBrains Mono',monospace;font-size:9px;color:var(--mu);}
.mono{font-family:'JetBrains Mono',monospace;font-size:11px;color:var(--mu);}
.filter-row{display:flex;gap:6px;}
.flt-btn{padding:5px 12px;border-radius:20px;font-size:10px;font-weight:500;cursor:pointer;border:1px solid var(--br);background:transparent;color:var(--mu);font-family:'Sora',sans-serif;transition:all .15s;}
.flt-btn.active,.flt-btn:hover{background:rgba(249,115,22,.15);border-color:var(--o);color:var(--o);}
.srch{background:var(--dk2);border:1px solid var(--br);border-radius:7px;padding:6px 11px;font-family:'Sora',sans-serif;font-size:11px;color:var(--wh);outline:none;width:180px;}
.srch:focus{border-color:var(--o);}
.srch::placeholder{color:var(--mu);}

/* ===FORM ELEMENTS=== */
.form-group{margin-bottom:14px;}
.form-label{display:block;font-size:11px;font-weight:600;color:var(--mu);margin-bottom:6px;letter-spacing:.3px;}
.form-input,.form-select{width:100%;background:var(--dk2);border:1px solid var(--br);border-radius:8px;padding:9px 13px;font-family:'Sora',sans-serif;font-size:12px;color:var(--wh);outline:none;transition:border-color .15s;}
.form-input:focus,.form-select:focus{border-color:var(--o);}
.form-input::placeholder{color:var(--mu);}
.form-select option{background:var(--dk2);color:var(--wh);}
.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:14px;}
textarea.form-input{resize:vertical;min-height:80px;}

/* ===UPLOAD ZONE=== */
.upload-zone{border:2px dashed var(--br);border-radius:12px;padding:28px;text-align:center;cursor:pointer;transition:all .2s;}
.upload-zone:hover,.upload-zone.drag{border-color:var(--o);background:rgba(249,115,22,.05);}
.upload-zone p{font-size:12px;color:var(--mu);margin-top:8px;}
.upload-zone strong{color:var(--o);}

/* ===EVENTS=== */
.events-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:14px;margin-bottom:22px;}
.event-card{background:var(--dk);border:1px solid var(--br);border-radius:12px;padding:16px;cursor:pointer;transition:all .15s;}
.event-card:hover{border-color:rgba(249,115,22,.4);transform:translateY(-1px);}
.event-card.selected{border-color:var(--o);background:rgba(249,115,22,.05);}
.ev-header{display:flex;align-items:flex-start;justify-content:space-between;margin-bottom:10px;}
.ev-title{font-size:13px;font-weight:600;color:var(--wh);}
.ev-date{font-size:10px;color:var(--mu);margin-top:3px;font-family:'JetBrains Mono',monospace;}
.ev-badge{font-size:9px;font-weight:700;padding:2px 8px;border-radius:20px;}
.ev-active{background:rgba(16,185,129,.15);color:#34D399;}
.ev-closed{background:rgba(107,114,128,.15);color:#9CA3AF;}
.ev-upcoming{background:rgba(59,130,246,.15);color:#60A5FA;}
.ev-stats{display:flex;gap:12px;margin-top:10px;padding-top:10px;border-top:1px solid var(--br);}
.ev-stat{font-size:10px;color:var(--mu);}
.ev-stat strong{color:var(--wh);display:block;font-size:14px;}

/* ===KPI=== */
.kpi-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(300px,1fr));gap:14px;}
.kpi-card{background:var(--dk);border:1px solid var(--br);border-radius:12px;padding:16px;}
.kpi-top{display:flex;align-items:center;gap:10px;margin-bottom:14px;}
.kpi-av{width:38px;height:38px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:13px;font-weight:700;color:#fff;flex-shrink:0;}
.kpi-nm{font-size:13px;font-weight:600;color:var(--wh);}
.kpi-role{font-size:10px;color:var(--mu);margin-top:1px;}
.kpi-score{font-size:22px;font-weight:700;font-family:'JetBrains Mono',monospace;margin-left:auto;}
.kpi-metrics{display:flex;flex-direction:column;gap:8px;}
.kpi-metric{display:flex;flex-direction:column;gap:4px;}
.kpi-metric-top{display:flex;justify-content:space-between;}
.kpi-metric-lbl{font-size:10px;color:var(--mu);}
.kpi-metric-val{font-size:10px;font-weight:600;color:var(--wh);}
.kpi-bar{height:5px;background:var(--dk2);border-radius:3px;overflow:hidden;}
.kpi-fill{height:100%;border-radius:3px;transition:width .6s ease;}
.kpi-grade{display:inline-block;padding:2px 8px;border-radius:20px;font-size:10px;font-weight:700;margin-top:8px;}
.grade-a{background:rgba(16,185,129,.15);color:#34D399;}
.grade-b{background:rgba(249,115,22,.15);color:var(--o);}
.grade-c{background:rgba(245,158,11,.15);color:#FCD34D;}
.grade-d{background:rgba(239,68,68,.15);color:#FC8181;}

/* ===MODAL=== */
.modal-bg{position:fixed;inset:0;background:rgba(0,0,0,.75);backdrop-filter:blur(4px);z-index:200;display:none;align-items:center;justify-content:center;padding:20px;}
.modal-bg.open{display:flex;}
.modal{background:var(--dk);border:1px solid var(--br);border-radius:18px;padding:28px;width:100%;max-width:480px;position:relative;animation:mi .25s ease;max-height:90vh;overflow-y:auto;}
.modal-lg{max-width:560px;}
@keyframes mi{from{opacity:0;transform:scale(.95)}to{opacity:1;transform:scale(1)}}
.modal-close{position:absolute;top:14px;right:14px;background:var(--dk2);border:1px solid var(--br);color:var(--mu);border-radius:50%;width:26px;height:26px;cursor:pointer;font-size:13px;display:flex;align-items:center;justify-content:center;}
.modal-ico{font-size:44px;text-align:center;margin-bottom:14px;}
.modal-ttl{font-size:17px;font-weight:700;text-align:center;margin-bottom:4px;}
.modal-sub{font-size:11px;color:var(--mu);text-align:center;margin-bottom:18px;}
.modal-detail{background:var(--dk2);border-radius:9px;padding:13px;margin-bottom:14px;}
.modal-row{display:flex;justify-content:space-between;padding:4px 0;font-size:11px;}
.modal-row span:first-child{color:var(--mu);}
.modal-row span:last-child{font-weight:500;color:var(--wh);}

/* ===TOAST=== */
.toast{position:fixed;top:18px;right:18px;z-index:999;background:var(--dk2);border:1px solid var(--br);border-radius:11px;padding:12px 16px;display:flex;align-items:center;gap:9px;font-size:12px;color:var(--wh);transform:translateX(120%);transition:transform .3s ease;max-width:300px;box-shadow:0 8px 24px rgba(0,0,0,.4);}
.toast.show{transform:translateX(0);}
.toast-ico{font-size:16px;}
.toast-ttl{font-weight:600;font-size:12px;}
.toast-sub{font-size:10px;color:var(--mu);margin-top:1px;}

/* ===EMPTY STATE=== */
.empty{text-align:center;padding:36px;color:var(--mu);font-size:12px;}
.empty-ico{font-size:32px;margin-bottom:10px;}

/* ===SECTION HEADER=== */
.sec-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:18px;}
.sec-ttl{font-size:16px;font-weight:600;color:var(--wh);}
.sec-sub{font-size:11px;color:var(--mu);margin-top:2px;}

/* ===STEP GUIDE=== */
.step-list{display:flex;flex-direction:column;gap:0;}
.step{display:flex;gap:16px;padding:16px 0;}
.step:not(:last-child){border-bottom:1px solid var(--br);}
.step-num{width:32px;height:32px;border-radius:50%;background:rgba(249,115,22,.15);border:1px solid rgba(249,115,22,.3);display:flex;align-items:center;justify-content:center;font-size:13px;font-weight:700;color:var(--o);flex-shrink:0;}
.step-content h4{font-size:13px;font-weight:600;color:var(--wh);margin-bottom:4px;}
.step-content p{font-size:11px;color:var(--mu);line-height:1.6;}
.step-content code{font-family:'JetBrains Mono',monospace;background:var(--dk2);padding:1px 6px;border-radius:4px;font-size:10px;color:var(--o);}
.tech-badge{display:inline-flex;align-items:center;gap:5px;background:var(--dk2);border:1px solid var(--br);padding:5px 12px;border-radius:20px;font-size:11px;color:var(--mu);margin:4px 4px 0 0;}
.tech-badge strong{color:var(--wh);}

/* ===DIVIDER=== */
.divider{height:1px;background:var(--br);margin:20px 0;}

/* scrollbar */
::-webkit-scrollbar{width:3px;}
::-webkit-scrollbar-track{background:transparent;}
::-webkit-scrollbar-thumb{background:var(--br);border-radius:2px;}

@media(max-width:1050px){.scanner-wrap{grid-template-columns:1fr;}.stats-grid{grid-template-columns:repeat(2,1fr);}}
@media(max-width:768px){.sidebar{display:none;}.main{margin-left:0;}.page{padding:16px;}.stats-grid{grid-template-columns:repeat(2,1fr);}.form-grid{grid-template-columns:1fr;}}
</style>
</head>
<body>

<!-- SIDEBAR -->
<div class="sidebar">
  <div class="sidebar-logo">
    <div class="logo-box" onclick="document.getElementById('logo-upload').click()" title="Klik untuk ganti logo"><img id="sidebar-logo" alt="BSC" style="display:none;"><span id="logo-fallback" style="font-size:14px;font-weight:700;color:#fff;">BSC</span></div><input type="file" id="logo-upload" accept="image/*" style="display:none" onchange="handleLogoUpload(this)">
    <div class="logo-t"><h1>BSC FEB-Unpak</h1><p>Business Simulation Club</p></div>
  </div>
  <div class="sb-sec">
    <div class="sb-lbl">Menu Utama</div>
    <button class="nav active" onclick="goPage('absensi',this)"><span class="nav-ic">📡</span>Absensi RFID<span class="nav-badge" id="badge-scan">0</span></button>
    <button class="nav" onclick="goPage('kegiatan',this)"><span class="nav-ic">📅</span>Kegiatan<span class="nav-badge" id="badge-event">0</span></button>
    <button class="nav" onclick="goPage('anggota',this)"><span class="nav-ic">👥</span>Data Anggota</button>
    <button class="nav" onclick="goPage('kpi',this)"><span class="nav-ic">📊</span>KPI Anggota</button>
  </div>
  <div class="sb-sec">
    <div class="sb-lbl">Divisi</div>
    <button class="nav" onclick="goPage('anggota',null);filterMember('PI')"><span class="nav-ic">🔧</span>Pengembangan Internal</button>
    <button class="nav" onclick="goPage('anggota',null);filterMember('Relasi')"><span class="nav-ic">🤝</span>Relasi</button>
    <button class="nav" onclick="goPage('anggota',null);filterMember('Kominfo')"><span class="nav-ic">💻</span>Kominfo</button>
  </div>
  <div class="sb-sec">
    <div class="sb-lbl">Sistem</div>
    <button class="nav" onclick="goPage('panduan',this)"><span class="nav-ic">📖</span>Panduan Penggunaan</button>
    <button class="nav" onclick="exportCSV()"><span class="nav-ic">📥</span>Export CSV</button>
  </div>
  <div class="sb-bot">
    <div class="u-card">
      <div class="u-av">MZ</div>
      <div class="u-inf"><h4>Muhamad Zikri</h4><p>Ketua Umum</p></div>
    </div>
  </div>
</div>

<!-- MAIN -->
<div class="main">
  <div class="topbar">
    <div class="tb-l">
      <h2 id="page-title">Absensi RFID</h2>
      <p id="page-sub">Business Simulation Club — FEB Universitas Pakuan</p>
    </div>
    <div class="tb-r">
      <div class="clock-chip" id="live-clock">--:--:--</div>
      <button class="btn btn-ghost" style="font-size:11px;" onclick="exportCSV()">📥 Export</button>
    </div>
  </div>

  <!-- ======= PAGE: ABSENSI ======= -->
  <div class="page active" id="page-absensi">
    <!-- Event selector -->
    <div style="margin-bottom:16px;background:var(--dk);border:1px solid var(--br);border-radius:12px;padding:14px 18px;display:flex;align-items:center;gap:12px;flex-wrap:wrap;">
      <span style="font-size:11px;font-weight:600;color:var(--mu);">KEGIATAN AKTIF</span>
      <select class="form-select" id="active-event-sel" style="flex:1;max-width:320px;" onchange="onEventSelect()">
        <option value="">— Pilih Kegiatan —</option>
      </select>
      <span id="ev-sel-info" style="font-size:11px;color:var(--mu);"></span>
      <button class="btn btn-primary btn-sm" onclick="goPage('kegiatan',null);openNewEvent()">+ Buat Kegiatan</button>
    </div>

    <!-- Stats -->
    <div class="stats-grid">
      <div class="stat" data-ico="✅"><div class="stat-lbl">Hadir</div><div class="stat-val" id="s-hadir">0</div><div class="stat-note">dari <span id="s-total">0</span> anggota</div></div>
      <div class="stat" data-ico="⏰"><div class="stat-lbl">Terlambat</div><div class="stat-val" id="s-terlambat">0</div><div class="stat-note" style="color:var(--warn)">setelah batas waktu</div></div>
      <div class="stat" data-ico="❌"><div class="stat-lbl">Alpha</div><div class="stat-val" id="s-alpha">0</div><div class="stat-note" style="color:var(--err)">belum absen</div></div>
      <div class="stat" data-ico="📡"><div class="stat-lbl">Total Scan</div><div class="stat-val" id="s-scan">0</div><div class="stat-note">scan RFID hari ini</div></div>
    </div>

    <!-- Scanner + Recent -->
    <div class="scanner-wrap">
      <div class="rfid-card">
        <div class="scan-lbl">📡 RFID Scanner</div>
        <div class="ring"><div class="ring-ico" id="ring-ico">📶</div></div>
        <div class="scan-status" id="scan-status">Menunggu Kartu RFID...</div>
        <div class="scan-sub2" id="scan-sub">Tempelkan kartu ke reader, atau ketik ID manual</div>
        <div class="scan-inp-row">
          <input type="text" class="rfid-in" id="rfid-input" placeholder="BSC-001" maxlength="20">
          <button class="btn btn-primary" onclick="processRFID()">Scan ↵</button>
        </div>
      </div>
      <div class="recent-card">
        <div class="card-hdr">
          <div><div class="card-title">Scan Terakhir</div><div class="card-sub" id="rc-date">—</div></div>
          <button class="btn btn-ghost btn-sm" onclick="clearFilter()">Semua</button>
        </div>
        <div id="recent-list"><div class="empty"><div class="empty-ico">📋</div>Belum ada scan</div></div>
      </div>
    </div>

    <!-- Table -->
    <div class="tbl-wrap">
      <div class="tbl-hdr">
        <div><div class="card-title">Daftar Hadir</div><div class="card-sub" id="tbl-ev-name">Pilih kegiatan untuk mulai absensi</div></div>
        <div style="display:flex;gap:8px;align-items:center;flex-wrap:wrap;">
          <div class="filter-row" id="filter-row">
            <button class="flt-btn active" onclick="setFilter('all',this)">Semua</button>
            <button class="flt-btn" onclick="setFilter('Hadir',this)">Hadir</button>
            <button class="flt-btn" onclick="setFilter('Terlambat',this)">Terlambat</button>
            <button class="flt-btn" onclick="setFilter('Alpha',this)">Alpha</button>
          </div>
          <input type="text" class="srch" placeholder="🔍 Cari..." oninput="searchTable(this.value)">
        </div>
      </div>
      <div style="overflow-x:auto;">
        <table>
          <thead><tr>
            <th>Anggota</th><th>RFID ID</th><th>Divisi</th><th>Waktu</th><th>Status</th>
          </tr></thead>
          <tbody id="att-tbody"></tbody>
        </table>
      </div>
    </div>
  </div>

  <!-- ======= PAGE: KEGIATAN ======= -->
  <div class="page" id="page-kegiatan">
    <div class="sec-hdr">
      <div><div class="sec-ttl">Manajemen Kegiatan</div><div class="sec-sub">Buat dan kelola kegiatan BSC</div></div>
      <button class="btn btn-primary" onclick="openNewEvent()">+ Tambah Kegiatan</button>
    </div>

    <!-- Filter -->
    <div style="display:flex;gap:8px;margin-bottom:16px;flex-wrap:wrap;">
      <button class="flt-btn active" onclick="filterEvents('all',this)">Semua</button>
      <button class="flt-btn" onclick="filterEvents('active',this)">Aktif</button>
      <button class="flt-btn" onclick="filterEvents('upcoming',this)">Mendatang</button>
      <button class="flt-btn" onclick="filterEvents('closed',this)">Selesai</button>
    </div>

    <div class="events-grid" id="events-grid">
      <div class="empty" style="grid-column:1/-1;"><div class="empty-ico">📅</div>Belum ada kegiatan. Buat kegiatan baru!</div>
    </div>
  </div>

  <!-- ======= PAGE: ANGGOTA ======= -->
  <div class="page" id="page-anggota">
    <div class="sec-hdr">
      <div><div class="sec-ttl">Data Anggota</div><div class="sec-sub" id="anggota-count">0 anggota terdaftar</div></div>
      <div style="display:flex;gap:8px;">
        <button class="btn btn-ghost" onclick="openUploadModal()">📤 Upload CSV</button>
        <button class="btn btn-primary" onclick="openAddMember()">+ Tambah Anggota</button>
      </div>
    </div>

    <!-- Filter divisi -->
    <div style="display:flex;gap:6px;margin-bottom:16px;flex-wrap:wrap;">
      <button class="flt-btn active" id="div-all" onclick="filterMember('all',this)">Semua</button>
      <button class="flt-btn" onclick="filterMember('Pengurus',this)">Pengurus</button>
      <button class="flt-btn" onclick="filterMember('PI',this)">Peng. Internal</button>
      <button class="flt-btn" onclick="filterMember('Relasi',this)">Relasi</button>
      <button class="flt-btn" onclick="filterMember('Kominfo',this)">Kominfo</button>
    </div>

    <div class="tbl-wrap">
      <div style="padding:12px 20px;border-bottom:1px solid var(--br);">
        <input type="text" class="srch" placeholder="🔍 Cari anggota..." oninput="searchMembers(this.value)" style="width:220px;">
      </div>
      <div style="overflow-x:auto;">
        <table>
          <thead><tr>
            <th>Anggota</th><th>RFID ID</th><th>Jabatan</th><th>Divisi</th><th>Total Kegiatan</th><th>Aksi</th>
          </tr></thead>
          <tbody id="member-tbody"></tbody>
        </table>
      </div>
    </div>
  </div>

  <!-- ======= PAGE: KPI ======= -->
  <div class="page" id="page-kpi">
    <div class="sec-hdr">
      <div><div class="sec-ttl">KPI Anggota</div><div class="sec-sub">Key Performance Indicator berdasarkan kehadiran & partisipasi</div></div>
      <div style="display:flex;gap:8px;align-items:center;">
        <select class="form-select" id="kpi-period" onchange="renderKPI()" style="width:160px;font-size:11px;">
          <option value="all">Semua Periode</option>
        </select>
        <select class="form-select" id="kpi-div" onchange="renderKPI()" style="width:140px;font-size:11px;">
          <option value="all">Semua Divisi</option>
          <option value="Pengurus">Pengurus</option>
          <option value="PI">Peng. Internal</option>
          <option value="Relasi">Relasi</option>
          <option value="Kominfo">Kominfo</option>
        </select>
      </div>
    </div>

    <!-- KPI Legend -->
    <div style="display:flex;gap:10px;margin-bottom:18px;flex-wrap:wrap;">
      <div style="display:flex;align-items:center;gap:5px;font-size:10px;color:var(--mu);">
        <span style="width:10px;height:10px;border-radius:50%;background:#34D399;display:inline-block;"></span>Grade A (≥85)
      </div>
      <div style="display:flex;align-items:center;gap:5px;font-size:10px;color:var(--mu);">
        <span style="width:10px;height:10px;border-radius:50%;background:var(--o);display:inline-block;"></span>Grade B (70–84)
      </div>
      <div style="display:flex;align-items:center;gap:5px;font-size:10px;color:var(--mu);">
        <span style="width:10px;height:10px;border-radius:50%;background:#FCD34D;display:inline-block;"></span>Grade C (55–69)
      </div>
      <div style="display:flex;align-items:center;gap:5px;font-size:10px;color:var(--mu);">
        <span style="width:10px;height:10px;border-radius:50%;background:#FC8181;display:inline-block;"></span>Grade D (&lt;55)
      </div>
    </div>

    <div class="kpi-grid" id="kpi-grid">
      <div class="empty" style="grid-column:1/-1;"><div class="empty-ico">📊</div>Tambah anggota dan buat kegiatan untuk melihat KPI</div>
    </div>
  </div>

  <!-- ======= PAGE: PANDUAN ======= -->
  <div class="page" id="page-panduan">
    <div class="sec-hdr">
      <div><div class="sec-ttl">Panduan Penggunaan</div><div class="sec-sub">Cara setup dan menggunakan sistem absensi BSC</div></div>
    </div>

    <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-bottom:20px;">
      <!-- Cara Pakai -->
      <div class="card card-p">
        <div class="card-hdr"><div><div class="card-title">🚀 Cara Menggunakan Web Ini</div><div class="card-sub">Langkah-langkah penggunaan harian</div></div></div>
        <div class="step-list">
          <div class="step"><div class="step-num">1</div><div class="step-content"><h4>Upload/Daftarkan Anggota</h4><p>Buka halaman <strong>Data Anggota</strong> → klik <strong>Upload CSV</strong> untuk import massal, atau <strong>Tambah Anggota</strong> untuk input manual. Setiap anggota perlu nama, RFID ID, jabatan, dan divisi.</p></div></div>
          <div class="step"><div class="step-num">2</div><div class="step-content"><h4>Buat Kegiatan</h4><p>Buka halaman <strong>Kegiatan</strong> → klik <strong>Tambah Kegiatan</strong>. Isi nama kegiatan, tanggal, dan batas waktu (untuk deteksi terlambat). Setiap rapat, seminar, atau event punya absensi terpisah.</p></div></div>
          <div class="step"><div class="step-num">3</div><div class="step-content"><h4>Pilih Kegiatan Aktif</h4><p>Di halaman <strong>Absensi RFID</strong>, pilih kegiatan yang sedang berlangsung dari dropdown di bagian atas.</p></div></div>
          <div class="step"><div class="step-num">4</div><div class="step-content"><h4>Scan / Input RFID</h4><p>Ketik atau scan RFID ID anggota (format: <code>BSC-001</code>) lalu tekan Enter atau klik Scan. Konfirmasi muncul otomatis.</p></div></div>
          <div class="step"><div class="step-num">5</div><div class="step-content"><h4>Monitor & Export</h4><p>Pantau statistik real-time. Export ke CSV untuk laporan ke Ketua/Pembina. KPI dihitung otomatis dari data absensi kegiatan.</p></div></div>
        </div>
      </div>

      <!-- Deploy Guide -->
      <div style="display:flex;flex-direction:column;gap:14px;">
        <div class="card card-p">
          <div class="card-hdr"><div><div class="card-title">🌐 Cara Deploy — Gratis</div><div class="card-sub">Biar bisa diakses semua pengurus</div></div></div>
          <div class="step-list">
            <div class="step"><div class="step-num">1</div><div class="step-content"><h4>GitHub Pages (Paling Mudah)</h4><p>Buat akun <code>github.com</code> → buat repository baru → upload file <code>bsc-absensi.html</code> → rename jadi <code>index.html</code> → masuk Settings → Pages → deploy. URL: <code>namakamu.github.io/bsc</code></p></div></div>
            <div class="step"><div class="step-num">2</div><div class="step-content"><h4>Netlify Drop (Tercepat)</h4><p>Buka <code>netlify.com/drop</code> → drag & drop file HTML → langsung online dalam 30 detik. Dapat URL seperti <code>bsc-absensi.netlify.app</code></p></div></div>
            <div class="step"><div class="step-num">3</div><div class="step-content"><h4>Google Drive (Internal)</h4><p>Upload ke Google Drive → klik kanan → Share → Anyone with link → buka di browser. Bisa diakses via link tanpa deploy.</p></div></div>
          </div>
        </div>

        <div class="card card-p">
          <div class="card-hdr"><div><div class="card-title">📡 Integrasi RFID Reader Fisik</div><div class="card-sub">Hubungkan ke hardware reader</div></div></div>
          <div class="step-list">
            <div class="step"><div class="step-num">1</div><div class="step-content"><h4>USB RFID Reader (Plug & Play)</h4><p>Sebagian besar USB RFID reader bekerja sebagai keyboard emulator. Cukup colok ke laptop, klik field input di web, tempel kartu → ID otomatis terketik dan langsung scan.</p></div></div>
            <div class="step"><div class="step-num">2</div><div class="step-content"><h4>Pastikan Auto-Enter</h4><p>Reader yang baik mengirim karakter Enter setelah ID. Kalau tidak, aktifkan setting di reader atau klik tombol Scan manual.</p></div></div>
          </div>
          <div style="margin-top:10px;">
            <div style="font-size:10px;color:var(--mu);margin-bottom:8px;">RFID Reader yang Direkomendasikan:</div>
            <span class="tech-badge"><strong>RFID USB 125KHz</strong> ~Rp 50rb</span>
            <span class="tech-badge"><strong>ACR122U NFC</strong> ~Rp 300rb</span>
            <span class="tech-badge"><strong>RDM6300</strong> Arduino ~Rp 30rb</span>
          </div>
        </div>

        <div class="card card-p">
          <div class="card-hdr"><div><div class="card-title">💾 Tentang Data</div></div></div>
          <p style="font-size:11px;color:var(--mu);line-height:1.7;">Data tersimpan di <strong style="color:var(--wh)">localStorage</strong> browser (permanen di perangkat itu). Selama tidak clear browsing data atau ganti browser, data aman. Untuk backup, gunakan <strong style="color:var(--wh)">Export CSV</strong> secara rutin. Kalau ingin data tersinkron antar perangkat, hubungi Zikri untuk upgrade ke versi dengan database.</p>
        </div>
      </div>
    </div>

    <!-- Format CSV -->
    <div class="card card-p">
      <div class="card-hdr"><div><div class="card-title">📋 Format Upload CSV Anggota</div><div class="card-sub">Format yang harus diikuti saat upload data anggota</div></div>
      <button class="btn btn-ghost btn-sm" onclick="downloadTemplate()">⬇ Download Template</button></div>
      <div style="background:var(--dk2);border-radius:8px;padding:14px;overflow-x:auto;">
        <code style="font-family:'JetBrains Mono',monospace;font-size:11px;color:var(--o);white-space:pre;">nama,rfid_id,jabatan,divisi
Muhamad Zikri,BSC-001,Ketua Umum,Pengurus
Wakil Ketua,BSC-002,Wakil Ketua,Pengurus
Budi Santoso,BSC-007,Kepala Divisi,PI
Sari Dewi,BSC-008,Staff,PI
Ahmad Fauzi,BSC-011,Kepala Divisi,Relasi</code>
      </div>
      <p style="font-size:10px;color:var(--mu);margin-top:10px;">Kolom wajib: <code style="font-family:'JetBrains Mono',monospace;background:var(--dk2);padding:1px 5px;border-radius:3px;color:var(--o);">nama, rfid_id, jabatan, divisi</code> — Nilai divisi: Pengurus / PI / Relasi / Kominfo</p>
    </div>
  </div>
</div><!-- end page panduan -->

</div><!-- end main -->

<!-- ===MODALS=== -->

<!-- Scan Result Modal -->
<div class="modal-bg" id="modal-scan" onclick="closeModalBg('modal-scan',event)">
  <div class="modal">
    <button class="modal-close" onclick="closeM('modal-scan')">✕</button>
    <div class="modal-ico" id="ms-ico">✅</div>
    <div class="modal-ttl" id="ms-ttl">Absensi Berhasil!</div>
    <div class="modal-sub" id="ms-sub">—</div>
    <div class="modal-detail" id="ms-detail"></div>
    <button class="btn btn-primary" style="width:100%;justify-content:center;padding:11px;" onclick="closeM('modal-scan')">Tutup</button>
  </div>
</div>

<!-- Add/Edit Member Modal -->
<div class="modal-bg" id="modal-member" onclick="closeModalBg('modal-member',event)">
  <div class="modal">
    <button class="modal-close" onclick="closeM('modal-member')">✕</button>
    <div style="font-size:17px;font-weight:700;margin-bottom:18px;" id="modal-member-title">Tambah Anggota</div>
    <input type="hidden" id="edit-member-idx" value="">
    <div class="form-group"><label class="form-label">Nama Lengkap *</label><input type="text" class="form-input" id="m-nama" placeholder="Nama anggota"></div>
    <div class="form-grid">
      <div class="form-group"><label class="form-label">RFID ID *</label><input type="text" class="form-input" id="m-rfid" placeholder="BSC-001" style="font-family:'JetBrains Mono',monospace;text-transform:uppercase;"></div>
      <div class="form-group"><label class="form-label">Divisi *</label>
        <select class="form-select" id="m-divisi">
          <option value="Pengurus">Pengurus</option>
          <option value="PI">Pengembangan Internal</option>
          <option value="Relasi">Relasi</option>
          <option value="Kominfo">Kominfo</option>
        </select>
      </div>
    </div>
    <div class="form-group"><label class="form-label">Jabatan *</label><input type="text" class="form-input" id="m-jabatan" placeholder="Ketua Umum / Staff / Kepala Divisi..."></div>
    <div style="display:flex;gap:8px;margin-top:6px;">
      <button class="btn btn-ghost" style="flex:1;justify-content:center;" onclick="closeM('modal-member')">Batal</button>
      <button class="btn btn-primary" style="flex:1;justify-content:center;" onclick="saveMember()">Simpan</button>
    </div>
  </div>
</div>

<!-- Upload CSV Modal -->
<div class="modal-bg" id="modal-upload" onclick="closeModalBg('modal-upload',event)">
  <div class="modal modal-lg">
    <button class="modal-close" onclick="closeM('modal-upload')">✕</button>
    <div style="font-size:17px;font-weight:700;margin-bottom:6px;">Upload Data Anggota</div>
    <div style="font-size:11px;color:var(--mu);margin-bottom:18px;">Upload file CSV dengan format yang sesuai. Data lama tidak akan terhapus kecuali RFID ID sama.</div>

    <div class="upload-zone" id="drop-zone" onclick="document.getElementById('csv-file').click()" ondragover="event.preventDefault();this.classList.add('drag')" ondragleave="this.classList.remove('drag')" ondrop="handleDrop(event)">
      <div style="font-size:32px;margin-bottom:8px;">📂</div>
      <p><strong>Klik untuk pilih file</strong> atau drag & drop di sini</p>
      <p style="font-size:10px;margin-top:4px;">Format: .csv — Maks 500 anggota</p>
    </div>
    <input type="file" id="csv-file" accept=".csv" style="display:none" onchange="handleCSV(this)">

    <div id="csv-preview" style="display:none;margin-top:14px;">
      <div style="font-size:11px;font-weight:600;color:var(--o);margin-bottom:8px;" id="csv-preview-info">—</div>
      <div style="overflow-x:auto;max-height:200px;overflow-y:auto;">
        <table><thead><tr><th>Nama</th><th>RFID ID</th><th>Jabatan</th><th>Divisi</th></tr></thead>
        <tbody id="csv-preview-body"></tbody></table>
      </div>
      <div style="display:flex;gap:8px;margin-top:14px;">
        <button class="btn btn-ghost" style="flex:1;justify-content:center;" onclick="document.getElementById('csv-preview').style.display='none'">Batal</button>
        <button class="btn btn-primary" style="flex:1;justify-content:center;" onclick="confirmImportCSV()">Import Sekarang</button>
      </div>
    </div>
  </div>
</div>

<!-- New Event Modal -->
<div class="modal-bg" id="modal-event" onclick="closeModalBg('modal-event',event)">
  <div class="modal">
    <button class="modal-close" onclick="closeM('modal-event')">✕</button>
    <div style="font-size:17px;font-weight:700;margin-bottom:18px;" id="modal-event-title">Tambah Kegiatan</div>
    <input type="hidden" id="edit-event-idx" value="">
    <div class="form-group"><label class="form-label">Nama Kegiatan *</label><input type="text" class="form-input" id="ev-nama" placeholder="Rapat Rutin Mingguan"></div>
    <div class="form-grid">
      <div class="form-group"><label class="form-label">Tanggal *</label><input type="date" class="form-input" id="ev-tgl"></div>
      <div class="form-group"><label class="form-label">Waktu Mulai</label><input type="time" class="form-input" id="ev-waktu" value="08:00"></div>
    </div>
    <div class="form-grid">
      <div class="form-group"><label class="form-label">Batas Waktu (Terlambat)</label><input type="time" class="form-input" id="ev-batas" value="08:15"></div>
      <div class="form-group"><label class="form-label">Lokasi</label><input type="text" class="form-input" id="ev-lokasi" placeholder="Ruang Rapat / Aula..."></div>
    </div>
    <div class="form-group"><label class="form-label">Jenis Kegiatan</label>
      <select class="form-select" id="ev-jenis">
        <option value="Rapat">Rapat Rutin</option>
        <option value="Seminar">Seminar / Workshop</option>
        <option value="Lomba">Lomba / Kompetisi</option>
        <option value="Sosial">Kegiatan Sosial</option>
        <option value="Lainnya">Lainnya</option>
      </select>
    </div>
    <div class="form-group"><label class="form-label">Keterangan</label><textarea class="form-input" id="ev-ket" placeholder="Deskripsi kegiatan..."></textarea></div>
    <div style="display:flex;gap:8px;">
      <button class="btn btn-ghost" style="flex:1;justify-content:center;" onclick="closeM('modal-event')">Batal</button>
      <button class="btn btn-primary" style="flex:1;justify-content:center;" onclick="saveEvent()">Simpan Kegiatan</button>
    </div>
  </div>
</div>

<!-- Toast -->
<div class="toast" id="toast">
  <div class="toast-ico" id="t-ico">✅</div>
  <div><div class="toast-ttl" id="t-ttl">—</div><div class="toast-sub" id="t-sub">—</div></div>
</div>

<script>
// ============================================================
// DATA & STATE
// ============================================================
let MEMBERS = [];
let EVENTS = [];
let attendance = {}; // { event_id: { rfid: { waktu, status } } }
let scanLog = [];
let activeEventId = null;
let filterMode = 'all';
let searchQ = '';
let memberFilter = 'all';
let memberSearch = '';
let csvPending = [];

const COLORS = ['#F97316','#EA580C','#8B5CF6','#7C3AED','#10B981','#059669','#3B82F6','#2563EB','#EC4899','#DB2777','#EF4444','#DC2626','#F59E0B','#D97706','#06B6D4','#0891B2'];

function getColor(idx){ return COLORS[idx % COLORS.length]; }
function initials(n){ return n.split(' ').map(w=>w[0]).join('').toUpperCase().slice(0,2); }
function fmtTime(d=new Date()){ return d.toLocaleTimeString('id-ID',{hour:'2-digit',minute:'2-digit',second:'2-digit'}); }
function fmtDate(d=new Date()){ return d.toLocaleDateString('id-ID',{weekday:'long',day:'numeric',month:'long',year:'numeric'}); }
function uid(){ return Date.now().toString(36)+Math.random().toString(36).slice(2,6); }

// ============================================================
// LOCALSTORAGE
// ============================================================
function saveData(){
  try{
    localStorage.setItem('bsc_members', JSON.stringify(MEMBERS));
    localStorage.setItem('bsc_events', JSON.stringify(EVENTS));
    localStorage.setItem('bsc_attendance', JSON.stringify(attendance));
  }catch(e){}
}
function loadData(){
  try{
    const m = localStorage.getItem('bsc_members');
    const e = localStorage.getItem('bsc_events');
    const a = localStorage.getItem('bsc_attendance');
    if(m) MEMBERS = JSON.parse(m);
    if(e) EVENTS = JSON.parse(e);
    if(a) attendance = JSON.parse(a);
    if(!MEMBERS.length) seedDefault();
  }catch(e){ seedDefault(); }
}
function seedDefault(){
  MEMBERS = [
    {id:'BSC-001',nama:'Muhamad Zikri',jabatan:'Ketua Umum',divisi:'Pengurus'},
    {id:'BSC-002',nama:'Wakil Ketua',jabatan:'Wakil Ketua Umum',divisi:'Pengurus'},
    {id:'BSC-003',nama:'Sekretaris I',jabatan:'Sekretaris I',divisi:'Pengurus'},
    {id:'BSC-004',nama:'Sekretaris II',jabatan:'Sekretaris II',divisi:'Pengurus'},
    {id:'BSC-005',nama:'Bendahara I',jabatan:'Bendahara I',divisi:'Pengurus'},
    {id:'BSC-006',nama:'Bendahara II',jabatan:'Bendahara II',divisi:'Pengurus'},
    {id:'BSC-007',nama:'Kadiv PI',jabatan:'Kepala Divisi',divisi:'PI'},
    {id:'BSC-008',nama:'Anggota PI 1',jabatan:'Staff',divisi:'PI'},
    {id:'BSC-009',nama:'Anggota PI 2',jabatan:'Staff',divisi:'PI'},
    {id:'BSC-010',nama:'Anggota PI 3',jabatan:'Staff',divisi:'PI'},
    {id:'BSC-011',nama:'Kadiv Relasi',jabatan:'Kepala Divisi',divisi:'Relasi'},
    {id:'BSC-012',nama:'Anggota Relasi 1',jabatan:'Staff',divisi:'Relasi'},
    {id:'BSC-013',nama:'Anggota Relasi 2',jabatan:'Staff',divisi:'Relasi'},
    {id:'BSC-014',nama:'Anggota Relasi 3',jabatan:'Staff',divisi:'Relasi'},
    {id:'BSC-015',nama:'Kadiv Kominfo',jabatan:'Kepala Divisi',divisi:'Kominfo'},
    {id:'BSC-016',nama:'Anggota Kominfo 1',jabatan:'Staff',divisi:'Kominfo'},
    {id:'BSC-017',nama:'Anggota Kominfo 2',jabatan:'Staff',divisi:'Kominfo'},
    {id:'BSC-018',nama:'Anggota Kominfo 3',jabatan:'Staff',divisi:'Kominfo'},
  ];
  saveData();
}

// ============================================================
// CLOCK
// ============================================================
function tick(){
  const now = new Date();
  document.getElementById('live-clock').textContent = fmtTime(now);
  document.getElementById('rc-date').textContent = fmtDate(now);
}
setInterval(tick,1000); tick();

// ============================================================
// PAGE NAVIGATION
// ============================================================
function goPage(id, btn){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.getElementById('page-'+id).classList.add('active');
  if(btn){ document.querySelectorAll('.nav').forEach(n=>n.classList.remove('active')); btn.classList.add('active'); }
  const titles = {absensi:'Absensi RFID',kegiatan:'Manajemen Kegiatan',anggota:'Data Anggota',kpi:'KPI Anggota',panduan:'Panduan Penggunaan'};
  document.getElementById('page-title').textContent = titles[id]||'';
  if(id==='absensi'){ refreshEventSel(); renderTable(); }
  if(id==='anggota'){ renderMemberTable(); }
  if(id==='kegiatan'){ renderEvents(); }
  if(id==='kpi'){ renderKPI(); }
}

// ============================================================
// RFID SCAN
// ============================================================
function processRFID(){
  const inp = document.getElementById('rfid-input');
  const rfid = inp.value.trim().toUpperCase();
  if(!rfid){ toast('⚠️','ID Kosong','Masukkan RFID ID','warn'); return; }
  if(!activeEventId){ toast('⚠️','Pilih Kegiatan','Pilih kegiatan aktif terlebih dahulu','warn'); inp.value=''; return; }
  const member = MEMBERS.find(m=>m.id===rfid);
  if(!member){ toast('❌','Tidak Dikenal',`ID "${rfid}" tidak terdaftar`,'err'); animScanner('err'); inp.value=''; return; }
  if(!attendance[activeEventId]) attendance[activeEventId]={};
  if(attendance[activeEventId][rfid]){
    const prev = attendance[activeEventId][rfid];
    showScanModal('⚠️','Sudah Absen',`${member.nama} sudah absen pukul ${prev.waktu}`,member,prev);
    inp.value=''; return;
  }
  const waktu = fmtTime();
  const ev = EVENTS.find(e=>e.id===activeEventId);
  let status = 'Hadir';
  if(ev && ev.batas){
    const [bh,bm] = ev.batas.split(':').map(Number);
    const now = new Date();
    if(now.getHours()>bh||(now.getHours()===bh&&now.getMinutes()>bm)) status='Terlambat';
  }
  attendance[activeEventId][rfid] = {waktu, status};
  scanLog.unshift({member, waktu, status});
  document.getElementById('badge-scan').textContent = Object.keys(attendance[activeEventId]).length;
  saveData(); updateStats(); renderRecentList(); renderTable();
  animScanner('ok'); showScanModal('✅','Absensi Berhasil!',`Selamat datang, ${member.nama}!`,member,{waktu,status});
  inp.value='';
}
document.getElementById('rfid-input').addEventListener('keydown',e=>{ if(e.key==='Enter') processRFID(); });

function animScanner(type){
  const ico=document.getElementById('ring-ico'),st=document.getElementById('scan-status'),sb=document.getElementById('scan-sub');
  if(type==='ok'){ico.textContent='✅';st.textContent='Absensi Tercatat!';}
  else{ico.textContent='❌';st.textContent='Kartu Tidak Dikenal!';}
  setTimeout(()=>{ico.textContent='📶';st.textContent='Menunggu Kartu RFID...';sb.textContent='Tempelkan kartu ke reader, atau ketik ID manual';},2500);
}

function updateStats(){
  const att = activeEventId && attendance[activeEventId] ? attendance[activeEventId] : {};
  const vals = Object.values(att);
  const hadir = vals.filter(a=>a.status==='Hadir').length;
  const terlambat = vals.filter(a=>a.status==='Terlambat').length;
  const total = MEMBERS.length;
  document.getElementById('s-hadir').textContent = hadir;
  document.getElementById('s-terlambat').textContent = terlambat;
  document.getElementById('s-alpha').textContent = total-hadir-terlambat;
  document.getElementById('s-total').textContent = total;
  document.getElementById('s-scan').textContent = vals.length;
}

function renderRecentList(){
  const list = document.getElementById('recent-list');
  if(!scanLog.length){ list.innerHTML='<div class="empty"><div class="empty-ico">📋</div>Belum ada scan</div>'; return; }
  list.innerHTML = scanLog.slice(0,7).map((s,i)=>`
    <div class="scan-item" style="animation:si .3s ease ${i*.05}s both">
      <div class="scan-av" style="background:${getColor(MEMBERS.findIndex(m=>m.id===s.member.id))}">${initials(s.member.nama)}</div>
      <div class="scan-inf">
        <div class="scan-nm">${s.member.nama}</div>
        <div class="scan-rl">${s.member.jabatan} · ${s.member.divisi}</div>
      </div>
      <div style="text-align:right">
        <div class="scan-tm">${s.waktu}</div>
        <span class="badge ${s.status==='Hadir'?'b-hadir':'b-terlambat'}" style="margin-top:3px">${s.status}</span>
      </div>
    </div>`).join('');
}

// ============================================================
// ATTENDANCE TABLE
// ============================================================
function renderTable(){
  const tbody = document.getElementById('att-tbody');
  const att = activeEventId && attendance[activeEventId] ? attendance[activeEventId] : {};
  let data = MEMBERS.map((m,i)=>{ const a=att[m.id]; return {...m,ci:i,waktu:a?a.waktu:'—',status:a?a.status:'Alpha'}; });
  if(filterMode!=='all') data = data.filter(d=>d.status===filterMode);
  if(searchQ) data = data.filter(d=>d.nama.toLowerCase().includes(searchQ)||d.divisi.toLowerCase().includes(searchQ));
  if(!data.length){ tbody.innerHTML='<tr><td colspan="5" class="empty">Tidak ada data</td></tr>'; return; }
  const divBadge=d=>d==='PI'?'b-pi':d==='Relasi'?'b-relasi':d==='Kominfo'?'b-kominfo':'b-pengurus';
  const stBadge=s=>s==='Hadir'?'b-hadir':s==='Terlambat'?'b-terlambat':s==='Alpha'?'b-alpha':'b-izin';
  tbody.innerHTML = data.map(m=>`
    <tr>
      <td><div class="mb-cell"><div class="mb-av" style="background:${getColor(m.ci)}">${initials(m.nama)}</div><div><div class="mb-nm">${m.nama}</div><div class="mb-id">${m.jabatan}</div></div></div></td>
      <td class="mono">${m.id}</td>
      <td><span class="badge ${divBadge(m.divisi)}">${m.divisi}</span></td>
      <td class="mono" style="color:var(--wh)">${m.waktu}</td>
      <td><span class="badge ${stBadge(m.status)}">${m.status}</span></td>
    </tr>`).join('');
}
function setFilter(f,btn){ filterMode=f; document.querySelectorAll('#filter-row .flt-btn').forEach(b=>b.classList.remove('active')); btn.classList.add('active'); renderTable(); }
function searchTable(q){ searchQ=q.toLowerCase(); renderTable(); }
function clearFilter(){ setFilter('all',document.querySelector('#filter-row .flt-btn')); }

// ============================================================
// EVENT MANAGEMENT
// ============================================================
function onEventSelect(){
  const sel = document.getElementById('active-event-sel').value;
  activeEventId = sel || null;
  if(activeEventId){ const ev=EVENTS.find(e=>e.id===activeEventId); document.getElementById('tbl-ev-name').textContent=ev?ev.nama:''; document.getElementById('ev-sel-info').textContent=ev?`${ev.tgl} • ${ev.waktu}`:''; }
  else{ document.getElementById('tbl-ev-name').textContent='Pilih kegiatan untuk mulai absensi'; document.getElementById('ev-sel-info').textContent=''; }
  if(!attendance[activeEventId]) attendance[activeEventId]={};
  scanLog=[];
  updateStats(); renderRecentList(); renderTable();
  document.getElementById('badge-scan').textContent = activeEventId&&attendance[activeEventId]?Object.keys(attendance[activeEventId]).length:0;
}
function refreshEventSel(){
  const sel=document.getElementById('active-event-sel');
  const cur=sel.value;
  sel.innerHTML='<option value="">— Pilih Kegiatan —</option>';
  EVENTS.forEach(ev=>{ const opt=document.createElement('option'); opt.value=ev.id; opt.textContent=`${ev.nama} (${ev.tgl})`; if(ev.id===cur) opt.selected=true; sel.appendChild(opt); });
  document.getElementById('badge-event').textContent=EVENTS.length;
}
function openNewEvent(){ document.getElementById('edit-event-idx').value=''; document.getElementById('modal-event-title').textContent='Tambah Kegiatan'; document.getElementById('ev-nama').value=''; document.getElementById('ev-tgl').value=new Date().toISOString().split('T')[0]; document.getElementById('ev-waktu').value='08:00'; document.getElementById('ev-batas').value='08:15'; document.getElementById('ev-lokasi').value=''; document.getElementById('ev-ket').value=''; openM('modal-event'); }
function saveEvent(){
  const nama=document.getElementById('ev-nama').value.trim();
  if(!nama){ toast('⚠️','Nama Kegiatan','Nama kegiatan wajib diisi','warn'); return; }
  const ev={id:uid(),nama,tgl:document.getElementById('ev-tgl').value,waktu:document.getElementById('ev-waktu').value,batas:document.getElementById('ev-batas').value,lokasi:document.getElementById('ev-lokasi').value.trim(),jenis:document.getElementById('ev-jenis').value,ket:document.getElementById('ev-ket').value.trim()};
  const idx=document.getElementById('edit-event-idx').value;
  if(idx!=='') EVENTS[parseInt(idx)]=ev; else EVENTS.push(ev);
  saveData(); refreshEventSel(); renderEvents(); closeM('modal-event');
  toast('✅','Kegiatan Tersimpan',ev.nama,'ok');
}
function deleteEvent(idx){ if(!confirm('Hapus kegiatan ini?')) return; const ev=EVENTS[idx]; delete attendance[ev.id]; EVENTS.splice(idx,1); saveData(); renderEvents(); refreshEventSel(); toast('🗑️','Kegiatan Dihapus','','ok'); }
function editEvent(idx){ const ev=EVENTS[idx]; document.getElementById('edit-event-idx').value=idx; document.getElementById('modal-event-title').textContent='Edit Kegiatan'; document.getElementById('ev-nama').value=ev.nama; document.getElementById('ev-tgl').value=ev.tgl; document.getElementById('ev-waktu').value=ev.waktu; document.getElementById('ev-batas').value=ev.batas||'08:15'; document.getElementById('ev-lokasi').value=ev.lokasi||''; document.getElementById('ev-jenis').value=ev.jenis||'Rapat'; document.getElementById('ev-ket').value=ev.ket||''; openM('modal-event'); }

let eventFilterMode='all';
function filterEvents(m,btn){ eventFilterMode=m; document.querySelectorAll('#page-kegiatan .flt-btn').forEach(b=>b.classList.remove('active')); btn.classList.add('active'); renderEvents(); }
function renderEvents(){
  const grid=document.getElementById('events-grid');
  const today=new Date().toISOString().split('T')[0];
  let data=[...EVENTS].reverse();
  if(eventFilterMode==='active') data=data.filter(e=>e.tgl===today);
  else if(eventFilterMode==='upcoming') data=data.filter(e=>e.tgl>today);
  else if(eventFilterMode==='closed') data=data.filter(e=>e.tgl<today);
  if(!data.length){ grid.innerHTML='<div class="empty" style="grid-column:1/-1"><div class="empty-ico">📅</div>Tidak ada kegiatan ditemukan</div>'; return; }
  grid.innerHTML = data.map((ev,revIdx)=>{
    const origIdx=EVENTS.indexOf(ev);
    const att=attendance[ev.id]||{};
    const hadir=Object.values(att).filter(a=>a.status==='Hadir').length;
    const terlambat=Object.values(att).filter(a=>a.status==='Terlambat').length;
    let badge,bclass;
    if(ev.tgl===today){badge='Aktif';bclass='ev-active';}
    else if(ev.tgl>today){badge='Mendatang';bclass='ev-upcoming';}
    else{badge='Selesai';bclass='ev-closed';}
    const jenisBadge={'Rapat':'🗣️','Seminar':'🎓','Lomba':'🏆','Sosial':'🤝','Lainnya':'📌'};
    return `<div class="event-card ${activeEventId===ev.id?'selected':''}">
      <div class="ev-header">
        <div>
          <div class="ev-title">${jenisBadge[ev.jenis]||'📌'} ${ev.nama}</div>
          <div class="ev-date">${ev.tgl} ${ev.waktu?'• '+ev.waktu:''} ${ev.lokasi?'• '+ev.lokasi:''}</div>
        </div>
        <span class="ev-badge ${bclass}">${badge}</span>
      </div>
      ${ev.ket?`<div style="font-size:10px;color:var(--mu);margin-bottom:8px;">${ev.ket}</div>`:''}
      <div class="ev-stats">
        <div class="ev-stat"><strong>${hadir}</strong>Hadir</div>
        <div class="ev-stat"><strong>${terlambat}</strong>Terlambat</div>
        <div class="ev-stat"><strong>${MEMBERS.length-hadir-terlambat}</strong>Alpha</div>
        <div class="ev-stat"><strong>${MEMBERS.length}</strong>Total</div>
      </div>
      <div style="display:flex;gap:6px;margin-top:12px;">
        <button class="btn btn-ghost btn-sm" style="flex:1;justify-content:center;" onclick="activeEventId='${ev.id}';refreshEventSel();document.getElementById('active-event-sel').value='${ev.id}';goPage('absensi',document.querySelector('.nav'))">📡 Absensi</button>
        <button class="btn btn-ghost btn-sm" onclick="editEvent(${origIdx})">✏️</button>
        <button class="btn btn-danger btn-sm" onclick="deleteEvent(${origIdx})">🗑️</button>
      </div>
    </div>`;
  }).join('');
}

// ============================================================
// MEMBER MANAGEMENT
// ============================================================
function openAddMember(){ document.getElementById('edit-member-idx').value=''; document.getElementById('modal-member-title').textContent='Tambah Anggota'; document.getElementById('m-nama').value=''; document.getElementById('m-rfid').value=''; document.getElementById('m-jabatan').value=''; document.getElementById('m-divisi').value='Pengurus'; openM('modal-member'); }
function editMember(idx){ const m=MEMBERS[idx]; document.getElementById('edit-member-idx').value=idx; document.getElementById('modal-member-title').textContent='Edit Anggota'; document.getElementById('m-nama').value=m.nama; document.getElementById('m-rfid').value=m.id; document.getElementById('m-jabatan').value=m.jabatan; document.getElementById('m-divisi').value=m.divisi; openM('modal-member'); }
function saveMember(){
  const nama=document.getElementById('m-nama').value.trim();
  const rfid=document.getElementById('m-rfid').value.trim().toUpperCase();
  const jabatan=document.getElementById('m-jabatan').value.trim();
  const divisi=document.getElementById('m-divisi').value;
  if(!nama||!rfid||!jabatan){ toast('⚠️','Data Tidak Lengkap','Isi semua field yang wajib','warn'); return; }
  const idx=document.getElementById('edit-member-idx').value;
  const existing=MEMBERS.findIndex(m=>m.id===rfid);
  if(existing>=0 && (idx===''||parseInt(idx)!==existing)){ toast('❌','RFID Duplikat',`ID ${rfid} sudah digunakan oleh ${MEMBERS[existing].nama}`,'err'); return; }
  const member={id:rfid,nama,jabatan,divisi};
  if(idx!=='') MEMBERS[parseInt(idx)]=member; else MEMBERS.push(member);
  saveData(); renderMemberTable(); closeM('modal-member'); updateStats();
  toast('✅','Anggota Tersimpan',nama,'ok');
  document.getElementById('anggota-count').textContent=MEMBERS.length+' anggota terdaftar';
}
function deleteMember(idx){ if(!confirm(`Hapus ${MEMBERS[idx].nama}?`)) return; MEMBERS.splice(idx,1); saveData(); renderMemberTable(); toast('🗑️','Anggota Dihapus','','ok'); }

function filterMember(div,btn){
  memberFilter=div;
  if(btn){ document.querySelectorAll('#page-anggota .flt-btn').forEach(b=>b.classList.remove('active')); btn.classList.add('active'); }
  renderMemberTable();
}
function searchMembers(q){ memberSearch=q.toLowerCase(); renderMemberTable(); }
function renderMemberTable(){
  const tbody=document.getElementById('member-tbody');
  let data=MEMBERS.map((m,i)=>({...m,_i:i}));
  if(memberFilter!=='all') data=data.filter(d=>d.divisi===memberFilter);
  if(memberSearch) data=data.filter(d=>d.nama.toLowerCase().includes(memberSearch)||d.id.toLowerCase().includes(memberSearch));
  document.getElementById('anggota-count').textContent=MEMBERS.length+' anggota terdaftar';
  if(!data.length){ tbody.innerHTML='<tr><td colspan="6" class="empty">Tidak ada anggota ditemukan</td></tr>'; return; }
  const divBadge=d=>d==='PI'?'b-pi':d==='Relasi'?'b-relasi':d==='Kominfo'?'b-kominfo':'b-pengurus';
  tbody.innerHTML=data.map(m=>{
    const totalKegiatan=EVENTS.filter(ev=>attendance[ev.id]&&attendance[ev.id][m.id]).length;
    return `<tr>
      <td><div class="mb-cell"><div class="mb-av" style="background:${getColor(m._i)}">${initials(m.nama)}</div><div><div class="mb-nm">${m.nama}</div></div></div></td>
      <td class="mono">${m.id}</td>
      <td style="font-size:11px">${m.jabatan}</td>
      <td><span class="badge ${divBadge(m.divisi)}">${m.divisi}</span></td>
      <td style="font-size:12px;font-family:'JetBrains Mono',monospace">${totalKegiatan}</td>
      <td><div style="display:flex;gap:6px;">
        <button class="btn btn-ghost btn-sm" onclick="editMember(${m._i})">✏️</button>
        <button class="btn btn-danger btn-sm" onclick="deleteMember(${m._i})">🗑️</button>
      </div></td>
    </tr>`;
  }).join('');
}

// ============================================================
// CSV UPLOAD
// ============================================================
function openUploadModal(){ document.getElementById('csv-preview').style.display='none'; openM('modal-upload'); }
function handleDrop(e){ e.preventDefault(); document.getElementById('drop-zone').classList.remove('drag'); const f=e.dataTransfer.files[0]; if(f) processCSVFile(f); }
function handleCSV(input){ if(input.files[0]) processCSVFile(input.files[0]); }
function processCSVFile(file){
  const reader=new FileReader();
  reader.onload=e=>{
    const lines=e.target.result.split('\n').map(l=>l.trim()).filter(Boolean);
    if(!lines.length) return;
    const headers=lines[0].toLowerCase().split(',').map(h=>h.trim());
    const ni=headers.indexOf('nama'),ri=headers.findIndex(h=>h.includes('rfid')),ji=headers.indexOf('jabatan'),di=headers.indexOf('divisi');
    if(ni<0||ri<0){ toast('❌','Format Salah','Kolom nama dan rfid_id wajib ada','err'); return; }
    csvPending=[];
    for(let i=1;i<lines.length;i++){
      const cols=lines[i].split(',').map(c=>c.trim());
      const nama=cols[ni]||'',rfid=(cols[ri]||'').toUpperCase(),jabatan=ji>=0?cols[ji]||'Staff':'Staff',divisi=di>=0?cols[di]||'Pengurus':'Pengurus';
      if(nama&&rfid) csvPending.push({id:rfid,nama,jabatan,divisi});
    }
    document.getElementById('csv-preview-info').textContent=`${csvPending.length} anggota siap diimport`;
    document.getElementById('csv-preview-body').innerHTML=csvPending.slice(0,10).map(m=>`<tr><td style="font-size:11px">${m.nama}</td><td class="mono">${m.id}</td><td style="font-size:11px">${m.jabatan}</td><td style="font-size:11px">${m.divisi}</td></tr>`).join('') + (csvPending.length>10?`<tr><td colspan="4" style="font-size:10px;color:var(--mu);text-align:center">...dan ${csvPending.length-10} lainnya</td></tr>`:'');
    document.getElementById('csv-preview').style.display='block';
  };
  reader.readAsText(file);
}
function confirmImportCSV(){
  let added=0,updated=0;
  csvPending.forEach(m=>{
    const idx=MEMBERS.findIndex(e=>e.id===m.id);
    if(idx>=0){MEMBERS[idx]=m;updated++;}else{MEMBERS.push(m);added++;}
  });
  saveData(); renderMemberTable(); closeM('modal-upload');
  toast('✅','Import Berhasil',`${added} ditambah, ${updated} diperbarui`,'ok');
}
function downloadTemplate(){
  const csv='nama,rfid_id,jabatan,divisi\nMuhamad Zikri,BSC-001,Ketua Umum,Pengurus\nWakil Ketua,BSC-002,Wakil Ketua,Pengurus\nBudi Santoso,BSC-007,Kepala Divisi,PI\nSari Dewi,BSC-008,Staff,PI';
  const blob=new Blob([csv],{type:'text/csv'});
  const a=document.createElement('a');a.href=URL.createObjectURL(blob);a.download='template-anggota-bsc.csv';a.click();
}

// ============================================================
// KPI
// ============================================================
function calcKPI(member){
  const totalEvents=EVENTS.length;
  if(!totalEvents) return {hadir:0,terlambat:0,alpha:0,total:0,pctHadir:0,pctTepat:0,score:0};
  let hadir=0,terlambat=0;
  EVENTS.forEach(ev=>{ const a=attendance[ev.id]; if(!a||!a[member.id]) return; if(a[member.id].status==='Hadir') hadir++; else terlambat++; });
  const alpha=totalEvents-hadir-terlambat;
  const pctHadir=Math.round(((hadir+terlambat)/totalEvents)*100);
  const pctTepat=hadir+terlambat>0?Math.round((hadir/(hadir+terlambat))*100):0;
  // KPI weights: kehadiran 60%, ketepatan waktu 30%, partisipasi aktif 10%
  const score=Math.min(100,Math.round(pctHadir*0.6 + pctTepat*0.3 + (hadir>0?10:0)));
  return {hadir,terlambat,alpha,total:totalEvents,pctHadir,pctTepat,score};
}
function grade(score){ if(score>=85)return{g:'A',cls:'grade-a'}; if(score>=70)return{g:'B',cls:'grade-b'}; if(score>=55)return{g:'C',cls:'grade-c'}; return{g:'D',cls:'grade-d'}; }
function kpiBar(val,color){ return `<div class="kpi-bar"><div class="kpi-fill" style="width:${val}%;background:${color}"></div></div>`; }

function renderKPI(){
  const grid=document.getElementById('kpi-grid');
  const kpiDiv=document.getElementById('kpi-div').value;
  if(!MEMBERS.length||!EVENTS.length){ grid.innerHTML='<div class="empty" style="grid-column:1/-1"><div class="empty-ico">📊</div>Tambah anggota dan kegiatan untuk melihat KPI</div>'; return; }
  let data=MEMBERS.map((m,i)=>({...m,_i:i,...calcKPI(m)}));
  if(kpiDiv!=='all') data=data.filter(d=>d.divisi===kpiDiv);
  data.sort((a,b)=>b.score-a.score);
  grid.innerHTML=data.map((m,rank)=>{
    const g=grade(m.score);
    const sc=m.score;
    const barColor=sc>=85?'#10B981':sc>=70?'#F97316':sc>=55?'#F59E0B':'#EF4444';
    return `<div class="kpi-card">
      <div class="kpi-top">
        <div class="kpi-av" style="background:${getColor(m._i)}">${initials(m.nama)}</div>
        <div>
          <div class="kpi-nm">${rank+1}. ${m.nama}</div>
          <div class="kpi-role">${m.jabatan} · ${m.divisi}</div>
          <span class="kpi-grade ${g.cls}">Grade ${g.g}</span>
        </div>
        <div class="kpi-score" style="color:${barColor}">${m.score}</div>
      </div>
      <div class="kpi-metrics">
        <div class="kpi-metric">
          <div class="kpi-metric-top"><span class="kpi-metric-lbl">Kehadiran (60%)</span><span class="kpi-metric-val">${m.hadir+m.terlambat}/${m.total} · ${m.pctHadir}%</span></div>
          ${kpiBar(m.pctHadir,'#3B82F6')}
        </div>
        <div class="kpi-metric">
          <div class="kpi-metric-top"><span class="kpi-metric-lbl">Ketepatan Waktu (30%)</span><span class="kpi-metric-val">${m.hadir}/${m.hadir+m.terlambat||1} · ${m.pctTepat}%</span></div>
          ${kpiBar(m.pctTepat,'#10B981')}
        </div>
        <div class="kpi-metric">
          <div class="kpi-metric-top"><span class="kpi-metric-lbl">Alpha</span><span class="kpi-metric-val" style="color:#FC8181">${m.alpha} kali</span></div>
          ${kpiBar(Math.max(0,100-m.alpha/m.total*100),'#8B5CF6')}
        </div>
      </div>
    </div>`;
  }).join('');
}

// ============================================================
// MODAL HELPERS
// ============================================================
function showScanModal(ico,ttl,sub,member,aData){
  document.getElementById('ms-ico').textContent=ico;
  document.getElementById('ms-ttl').textContent=ttl;
  document.getElementById('ms-sub').textContent=sub;
  document.getElementById('ms-detail').innerHTML=`
    <div class="modal-row"><span>Nama</span><span>${member.nama}</span></div>
    <div class="modal-row"><span>RFID ID</span><span style="font-family:'JetBrains Mono',monospace">${member.id}</span></div>
    <div class="modal-row"><span>Jabatan</span><span>${member.jabatan}</span></div>
    <div class="modal-row"><span>Divisi</span><span>${member.divisi}</span></div>
    <div class="modal-row"><span>Waktu</span><span style="color:var(--o)">${aData.waktu}</span></div>
    <div class="modal-row"><span>Status</span><span style="color:${aData.status==='Hadir'?'var(--ok)':aData.status==='Terlambat'?'var(--warn)':'var(--mu)'}">${aData.status}</span></div>`;
  openM('modal-scan');
}
function openM(id){ document.getElementById(id).classList.add('open'); }
function closeM(id){ document.getElementById(id).classList.remove('open'); }
function closeModalBg(id,e){ if(e.target===document.getElementById(id)) closeM(id); }

// ============================================================
// TOAST
// ============================================================
function toast(ico,ttl,sub,type){
  const el=document.getElementById('toast');
  document.getElementById('t-ico').textContent=ico;
  document.getElementById('t-ttl').textContent=ttl;
  document.getElementById('t-sub').textContent=sub;
  el.style.borderColor=type==='err'?'#EF4444':type==='warn'?'#F59E0B':'var(--br)';
  el.classList.add('show');
  setTimeout(()=>el.classList.remove('show'),3200);
}

// ============================================================
// EXPORT CSV
// ============================================================
function exportCSV(){
  const rows=[['Nama','RFID ID','Jabatan','Divisi','Kegiatan','Waktu','Status','Tanggal']];
  EVENTS.forEach(ev=>{
    MEMBERS.forEach(m=>{
      const a=attendance[ev.id]&&attendance[ev.id][m.id];
      rows.push([m.nama,m.id,m.jabatan,m.divisi,ev.nama,a?a.waktu:'-',a?a.status:'Alpha',ev.tgl]);
    });
  });
  const csv=rows.map(r=>r.map(c=>`"${c}"`).join(',')).join('\n');
  const blob=new Blob(['\ufeff'+csv],{type:'text/csv;charset=utf-8'});
  const a=document.createElement('a');a.href=URL.createObjectURL(blob);
  a.download=`absensi-bsc-${new Date().toISOString().split('T')[0]}.csv`;a.click();
  toast('📥','Export Berhasil','File CSV diunduh','ok');
}

// ============================================================
// LOGO UPLOAD
// ============================================================
function handleLogoUpload(input){
  const file=input.files[0]; if(!file) return;
  const reader=new FileReader();
  reader.onload=e=>{
    const dataUrl=e.target.result;
    const img=document.getElementById('sidebar-logo');
    const fallback=document.getElementById('logo-fallback');
    img.src=dataUrl; img.style.display='block';
    if(fallback) fallback.style.display='none';
    try{ localStorage.setItem('bsc_logo', dataUrl); }catch(err){}
    toast('✅','Logo Diperbarui','Logo BSC berhasil diunggah','ok');
  };
  reader.readAsDataURL(file);
}
function loadLogo(){
  try{
    const saved=localStorage.getItem('bsc_logo');
    if(saved){
      const img=document.getElementById('sidebar-logo');
      const fallback=document.getElementById('logo-fallback');
      img.src=saved; img.style.display='block';
      if(fallback) fallback.style.display='none';
    }
  }catch(e){}
}

// ============================================================
// INIT
// ============================================================
loadData();
loadLogo();
refreshEventSel();
renderTable();
updateStats();
document.getElementById('anggota-count').textContent=MEMBERS.length+' anggota terdaftar';
document.getElementById('badge-event').textContent=EVENTS.length;
</script>
</body>
</html>
