<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Performance KPI GraPARI Sibolga</title>
<style>
:root{--red:#e31b2f;--red2:#b90f21;--navy:#102a43;--ink:#1d2939;--muted:#667085;--bg:#f5f7fb;--card:#fff;--line:#e7ebf1;--green:#079455;--gold:#f4b740;--shadow:0 10px 30px rgba(16,42,67,.08)}
*{box-sizing:border-box}body{margin:0;font-family:Inter,Segoe UI,Arial,sans-serif;background:var(--bg);color:var(--ink)}
.header{background:linear-gradient(135deg,#9f0d1c,#e31b2f 58%,#ff4b58);color:#fff;padding:28px 4% 26px}.headIn{max-width:1500px;margin:auto;display:flex;justify-content:space-between;gap:20px;align-items:center}.brand{display:flex;gap:16px;align-items:center}.logo{width:62px;height:62px;border-radius:18px;background:#fff;color:var(--red);display:grid;place-items:center;font-weight:900;font-size:30px;box-shadow:0 8px 25px #0002}.brand h1{font-size:30px;margin:0}.brand p{margin:5px 0 0;opacity:.88}.topActions{display:flex;gap:10px;flex-wrap:wrap}.btn{border:0;border-radius:12px;padding:11px 16px;font-weight:800;cursor:pointer}.btn.white{background:#fff;color:var(--red)}.btn.dark{background:#162b44;color:#fff}.btn.red{background:var(--red);color:#fff}.btn.gray{background:#eef2f6;color:#334155}
.container{max-width:1500px;margin:auto;padding:28px 4% 60px}.toolbar{display:flex;justify-content:space-between;align-items:center;gap:12px;margin-bottom:24px;flex-wrap:wrap}.select{padding:12px 16px;border:1px solid var(--line);border-radius:12px;background:#fff;font-weight:800;color:var(--navy)}
.sectionTitle{display:flex;justify-content:space-between;align-items:end;margin:18px 0}.sectionTitle h2{font-size:30px;margin:0;color:var(--navy)}.sectionTitle p{margin:6px 0 0;color:var(--muted)}
.summary{display:grid;grid-template-columns:1fr 1fr 1.1fr;gap:18px}.summaryCard{background:#fff;border-radius:22px;padding:22px;box-shadow:var(--shadow);position:relative;overflow:hidden}.summaryCard:after{content:"";position:absolute;right:-30px;top:-40px;width:120px;height:120px;border-radius:50%;background:#f5f7fa}.summaryCard h3{margin:0;color:#6b7b8f;font-size:14px;letter-spacing:.7px}.summaryValue{font-size:36px;font-weight:900;color:var(--navy);margin:12px 0 4px}.summarySmall{color:var(--muted)}.mom{font-weight:900}.positive{color:var(--green)!important}.negative{color:var(--red)!important}.neutral{color:#667085!important}
.rankGrid{display:grid;grid-template-columns:1fr 1fr;gap:18px;margin-top:20px}.rankCard{background:#fff;border-radius:22px;padding:22px;box-shadow:var(--shadow);display:flex;gap:18px;align-items:center}.avatar{width:80px;height:80px;border-radius:50%;background:#eef2f6;object-fit:cover;border:4px solid #fff;box-shadow:0 3px 12px #0001}.medal{font-size:30px}.rankName{font-size:20px;font-weight:900;color:var(--navy)}.rankScore{font-size:28px;font-weight:900;margin-top:5px}.scoreLabel{font-size:12px;color:var(--muted)}
.kpiGrid{display:grid;grid-template-columns:repeat(5,1fr);gap:16px;margin-top:20px}.kpiCard{background:#fff;border-radius:20px;padding:19px;box-shadow:var(--shadow);min-height:145px}.kpiTitle{font-weight:900;color:#52657a;font-size:13px;text-transform:uppercase}.kpiScore{font-size:30px;font-weight:900;color:var(--navy);margin:12px 0}.highlow{font-size:13px;line-height:1.55}.highlow b{color:var(--navy)}
.panel{background:#fff;border-radius:22px;padding:22px;box-shadow:var(--shadow);margin-top:20px;overflow:auto}.panel h2{margin:0 0 15px;color:var(--navy)}table{border-collapse:collapse;width:100%;min-width:1050px}th,td{padding:12px 10px;border-bottom:1px solid #edf0f4;text-align:left}th{font-size:11px;text-transform:uppercase;color:#748399;background:#fafbfd}td{font-size:13px}.progress{height:8px;background:#edf0f4;border-radius:8px;overflow:hidden;margin-top:6px}.progress span{display:block;height:100%;background:var(--red);border-radius:8px}.adminPanel{display:none}.adminPanel.show{display:block}.notice{background:#fff7e8;border:1px solid #ffe1a8;padding:12px;border-radius:12px;color:#7a5a00;margin-bottom:15px}
.modal{display:none;position:fixed;inset:0;background:#07142699;z-index:20;align-items:center;justify-content:center;padding:20px}.modal.show{display:flex}.modalBox{background:#fff;border-radius:22px;padding:24px;width:min(980px,100%);max-height:92vh;overflow:auto}.small{width:min(400px,100%)}.formGrid{display:grid;grid-template-columns:1fr 1fr;gap:12px}.field{display:flex;flex-direction:column;gap:6px}.field label{font-weight:800;font-size:13px}.field input,.field select{padding:11px;border:1px solid #d9e0e8;border-radius:10px}.actions{display:flex;justify-content:flex-end;gap:10px;margin-top:18px}.photoGrid{display:grid;grid-template-columns:repeat(4,1fr);gap:12px}.photoBox{border:1px dashed #cbd5e1;border-radius:14px;padding:12px;text-align:center}.photoBox img{width:80px;height:80px;border-radius:50%;object-fit:cover;display:block;margin:8px auto}.photoBox input{max-width:100%;font-size:11px}
.parameterSummary{grid-template-columns:repeat(5,1fr)!important;gap:14px}.parameterCard{border-radius:50%;aspect-ratio:1/1;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;padding:18px;min-height:145px;box-shadow:0 8px 24px #07142614}.parameterCard h3{font-size:13px;margin:0 0 8px;color:var(--navy)}.parameterCard .summaryValue{font-size:26px;font-weight:900}.parameterCard .summarySmall{font-size:11px;font-weight:700;line-height:1.4}.parameterCard .summarySmall.positive{color:#138a45}.parameterCard .summarySmall.negative{color:#d71920}@media(max-width:1100px){.parameterSummary{grid-template-columns:repeat(3,1fr)!important}}@media(max-width:700px){.parameterSummary{grid-template-columns:repeat(2,1fr)!important}}@media(max-width:480px){.parameterSummary{grid-template-columns:1fr 1fr!important}}
@media(max-width:1100px){.kpiGrid{grid-template-columns:repeat(3,1fr)}.summary{grid-template-columns:1fr}.rankGrid{grid-template-columns:1fr}}
@media(max-width:700px){.kpiGrid{grid-template-columns:1fr 1fr}.formGrid{grid-template-columns:1fr}.photoGrid{grid-template-columns:1fr 1fr}.headIn{align-items:flex-start;flex-direction:column}.brand h1{font-size:24px}}
@media(max-width:480px){.kpiGrid{grid-template-columns:1fr}}
</style>
</head>
<body>
<header class="header">
 <div class="headIn">
  <div class="brand"><div class="logo">S</div><div><h1>Performance KPI GraPARI Sibolga</h1><p>Executive Dashboard • Monitoring Performance Team</p></div></div>
  <div class="topActions">
<button class="btn white" onclick="openLogin()">🔐 Admin</button>
<button class="btn dark" onclick="toggleEdit()">✏️ Menu Edit</button>
<button class="btn white" onclick="saveBackup()">💾 Save Data</button>
<button class="btn white" onclick="backupData()">⬇️ Backup</button>
<button class="btn white" onclick="document.getElementById('restoreFile').click()">⬆️ Restore</button>
<input id="restoreFile" type="file" accept=".json,application/json" style="display:none" onchange="restoreData(event)">
</div>
 </div>
</header>

<main class="container">
 <div class="toolbar">
  <div><b>Periode:</b> <select id="period" class="select" onchange="render()"></select></div>
  <div id="status" style="font-size:13px;color:#667085">View Dashboard</div>
 </div>

 <div id="saveStatus" style="background:#eefaf4;border:1px solid #b9ead1;color:#087443;border-radius:12px;padding:11px 14px;margin-bottom:18px;font-size:13px">💾 Data otomatis tersimpan di browser. Gunakan <b>Backup</b> untuk membuat file cadangan dan <b>Restore</b> untuk mengembalikannya.</div><div class="sectionTitle"><div><h2>Ringkasan Performansi</h2><p>Ranking berdasarkan rata-rata Achievement 5 KPI.</p></div><div id="updated" style="font-size:13px;color:#667085"></div></div>

 <section class="summary parameterSummary">
  <div class="summaryCard parameterCard"><h3>📱 HALO</h3><div class="summaryValue" id="sumHalo">0</div><div class="summarySmall" id="sumHaloSub">Ach: - • MoM: -</div></div>
  <div class="summaryCard parameterCard"><h3>🌐 INDIHOME</h3><div class="summaryValue" id="sumIndiHome">0</div><div class="summarySmall" id="sumIndiHomeSub">Ach: - • MoM: -</div></div>
  <div class="summaryCard parameterCard"><h3>📡 ORBIT</h3><div class="summaryValue" id="sumOrbit">0</div><div class="summarySmall" id="sumOrbitSub">Ach: - • MoM: -</div></div>
  <div class="summaryCard parameterCard"><h3>💰 REVENUE</h3><div class="summaryValue" id="sumRevenue">0</div><div class="summarySmall" id="sumRevenueSub">Ach: - • MoM: -</div></div>
  <div class="summaryCard parameterCard"><h3>⭐ tNPS</h3><div class="summaryValue" id="sumtNPS">0</div><div class="summarySmall" id="sumtNPSSub">Ach: - • MoM: -</div></div>
 </section>

 <section class="rankGrid" id="rankGrid"></section>

 <section class="kpiGrid" id="kpiGrid"></section>

 <section class="panel">
  <h2>📋 Detail Performance • Target • Realisasi • Achievement • N-1 • MoM</h2>
  <div id="detail"></div>
 </section>

 <section class="panel adminPanel" id="adminPanel">
  <h2>🛠️ Menu Edit Data</h2>
  <div class="notice">Menu ini terpisah dari View Utama. Hanya Admin yang dapat mengubah Target, Realisasi dan N-1. Achievement dan MoM dihitung otomatis.</div>
  <div id="adminTable"></div>
  <hr style="border:0;border-top:1px solid #eee;margin:25px 0">
  <h3>🖼️ Foto Petugas</h3><p style="color:#667085">Upload foto untuk kartu Ranking, Highest Score dan Lowest Score. Foto disimpan offline di browser ini.</p>
  <div class="photoGrid" id="photos"></div>
 </section>
</main>

<div class="modal" id="loginModal"><div class="modalBox small"><h2>🔐 Admin Login</h2><p>Login diperlukan untuk membuka menu Edit.</p><div class="field"><label>Password</label><input id="password" type="password" placeholder="Password Admin"></div><div id="loginError" style="color:#d71920;margin-top:8px"></div><div class="actions"><button class="btn gray" onclick="closeLogin()">Batal</button><button class="btn red" onclick="login()">Login</button></div></div></div>

<div class="modal" id="editModal"><div class="modalBox"><h2 id="editTitle">Edit KPI</h2><div class="field" style="margin-bottom:15px"><label>Petugas</label><select id="salesSelect" class="select"></select></div><div class="formGrid" id="editForm"></div><div class="actions"><button class="btn gray" onclick="closeEdit()">Batal</button><button class="btn red" onclick="save()">💾 Simpan</button></div></div></div>

<script>
const SALES=["Meli Mariana Sitinjak","Rafli Mido Ramansyah","Valentin Tania","Kiki Fatmawati Sihombing","Puput Andria Dewi Situmorang"];
const KPI=["Halo","IndiHome","Orbit","Revenue","tNPS"];
const PASS="admin123";
let db=JSON.parse(localStorage.getItem("gparisibolgaKPI")||"{}");
let photos=JSON.parse(localStorage.getItem("gparisibolaPhotos")||"{}");
let isAdmin=false, currentSales="";


function saveBackup(){
  saveDB();
  document.getElementById("saveStatus").innerHTML="✅ <b>Data berhasil disimpan.</b> Data KPI dan foto tersimpan di browser ini.";
  alert("Data berhasil disimpan.");
}
function backupData(){
  saveDB();
  const payload={app:"Performance KPI GraPARI Sibolga",version:2,exportedAt:new Date().toISOString(),db:db,photos:photos};
  const blob=new Blob([JSON.stringify(payload,null,2)],{type:"application/json"});
  const url=URL.createObjectURL(blob), a=document.createElement("a");
  a.href=url;
  a.download="Backup_Performance_KPI_GraPARI_Sibolga_"+new Date().toISOString().slice(0,10)+".json";
  document.body.appendChild(a); a.click(); a.remove(); URL.revokeObjectURL(url);
  document.getElementById("saveStatus").innerHTML="✅ <b>Backup berhasil dibuat.</b> Simpan file JSON tersebut di tempat yang aman.";
}
function restoreData(event){
  const file=event.target.files[0]; if(!file)return;
  const reader=new FileReader();
  reader.onload=function(){
    try{
      const payload=JSON.parse(reader.result);
      if(!payload || typeof payload.db!=="object" || typeof payload.photos!=="object") throw new Error();
      if(!confirm("Restore akan mengganti data yang sedang tersimpan dengan isi backup. Lanjutkan?")){event.target.value="";return;}
      db=payload.db||{}; photos=payload.photos||{}; saveDB(); render();
      document.getElementById("saveStatus").innerHTML="✅ <b>Restore berhasil.</b> Data backup sudah dimuat.";
      alert("Restore berhasil.");
    }catch(e){alert("Restore gagal: file backup tidak valid.");}
    event.target.value="";
  };
  reader.readAsText(file);
}

function months(){let a=[],d=new Date();for(let i=0;i<12;i++){let x=new Date(d.getFullYear(),d.getMonth()-i,1);a.push(x.toISOString().slice(0,7))}return a}
function monthName(p){let[y,m]=p.split("-");return new Date(y,m-1,1).toLocaleDateString("id-ID",{month:"long",year:"numeric"})}
function prev(p){let d=new Date(p+"-01");d.setMonth(d.getMonth()-1);return d.toISOString().slice(0,7)}
function get(p,n){let k=p+"|"+n;if(!db[k])db[k]={};KPI.forEach(k=>{if(!db[p+"|"+n][k])db[p+"|"+n][k]={target:0,actual:0,n1:0}});return db[k]}
function achievement(v){return v.target?100*v.actual/v.target:0}
function mom(v){return v.n1?100*(v.actual/v.n1-1):null}
function avg(p,n){return KPI.reduce((s,k)=>s+achievement(get(p,n)[k]),0)/KPI.length}
function fmt(x){return Number(x||0).toLocaleString("id-ID",{maximumFractionDigits:1})}
function pct(x){return fmt(x)+"%"}
function photo(n){return photos[n]||""}
function scoreRows(p){return SALES.map(n=>({name:n,score:avg(p,n),momTotal:(()=>{let a=KPI.reduce((s,k)=>s+get(p,n)[k].actual,0),b=KPI.reduce((s,k)=>s+get(p,n)[k].n1,0);return b?100*(a/b-1):null})()})).sort((a,b)=>b.score-a.score)}
function saveDB(){
  localStorage.setItem("gparisibolaKPI",JSON.stringify(db));
  localStorage.setItem("gparisibolaPhotos",JSON.stringify(photos));
  localStorage.setItem("gparisibolaLastSave",new Date().toISOString());
}
function render(){
 const p=period.value, rows=scoreRows(p), team=rows.reduce((s,r)=>s+r.score,0)/SALES.length;
 KPI.forEach(k=>{
   const key="sum"+k.replace(/[^A-Za-z0-9]/g,"");
   const total=SALES.reduce((s,n)=>s+(Number(get(p,n)[k].actual)||0),0);
   const target=SALES.reduce((s,n)=>s+(Number(get(p,n)[k].target)||0),0);
   const n1=SALES.reduce((s,n)=>s+(Number(get(p,n)[k].n1)||0),0);
   const ach=target?total/target*100:0;
   const mom=n1?((total-n1)/n1*100):0;
   const el=document.getElementById(key), sub=document.getElementById(key+"Sub");
   if(el) el.textContent=fmt(total);
   if(sub){sub.innerHTML=`Ach: <span class="${ach>=0?"positive":"negative"}">${ach.toFixed(1)}%</span> • MoM: <span class="${mom>=0?"positive":"negative"}">${mom>=0?"+":""}${mom.toFixed(1)}%</span>`;}
 });
 rankGrid.innerHTML=rows.slice(0,2).map((r,i)=>`<div class="rankCard"><img class="avatar" src="${photo(r.name)||'data:image/svg+xml,%3Csvg xmlns=%22http://www.w3.org/2000/svg%22 width=%2280%22 height=%2280%22%3E%3Crect width=%22100%25%22 height=%22100%25%22 rx=%2240%22 fill=%22%23eef2f6%22/%3E%3Ctext x=%2250%25%22 y=%2258%25%22 text-anchor=%22middle%22 font-size=%2232%22 fill=%22%23667785%22%3E%F0%9F%91%A4%3C/text%3E%3C/svg%3E'}"><div><div class="medal">${i===0?"🥇":"🥈"}</div><div class="rankName">${r.name}</div><div class="rankScore">${pct(r.score)}</div><div class="scoreLabel">Average Achievement</div></div></div>`).join("");
 kpiGrid.innerHTML=KPI.map(k=>{
   const vals=SALES.map(n=>({name:n,val:achievement(get(p,n)[k])}));
   const hi=vals.reduce((a,b)=>b.val>a.val?b:a),lo=vals.reduce((a,b)=>b.val<a.val?b:a);
   return `<div class="kpiCard"><div class="kpiTitle">${k}</div><div class="kpiScore">${pct(vals.reduce((s,x)=>s+x.val,0)/SALES.length)}</div><div class="highlow"><span class="positive">▲ Highest:</span> <b>${hi.name}</b><br>${pct(hi.val)}<br><span class="negative">▼ Lowest:</span> <b>${lo.name}</b><br>${pct(lo.val)}</div></div>`;
 }).join("");
 detail.innerHTML=`<table><thead><tr><th>Rank</th><th>Petugas</th>${KPI.map(k=>`<th>${k}<br>Target | Realisasi | Ach.</th>`).join("")}<th>AVG</th><th>MoM</th></tr></thead><tbody>`+
 rows.map((r,i)=>{let a=get(p,r.name);return `<tr><td><b>#${i+1}</b></td><td><b>${r.name}</b></td>`+KPI.map(k=>{let v=a[k],m=mom(v);return `<td>${fmt(v.target)} | ${fmt(v.actual)} | <b class="${achievement(v)<0?'negative':''}">${pct(achievement(v))}</b><br><small>N-1: ${fmt(v.n1)} • MoM: <span class="${m>0?'positive':m<0?'negative':'neutral'}">${m==null?"-":(m>=0?"+":"")+m.toFixed(1)+"%"}</span></small></td>`}).join("")+`<td><b>${pct(r.score)}</b><div class=progress><span style="width:${Math.min(r.score,100)}%"></span></div></td><td class="${r.momTotal>0?'positive':r.momTotal<0?'negative':''}">${r.momTotal==null?"-":(r.momTotal>=0?"+":"")+r.momTotal.toFixed(1)+"%"}</td></tr>`}).join("")+"</tbody></table>";
 renderAdmin(p);renderPhotos();
 updated.textContent="Last update: "+new Date().toLocaleString("id-ID",{day:"2-digit",month:"short",year:"numeric",hour:"2-digit",minute:"2-digit"})+" WIB";
}
function renderAdmin(p){
 adminTable.innerHTML=`<table><thead><tr><th>Petugas</th>${KPI.map(k=>`<th>${k}<br>Target / Realisasi / N-1</th>`).join("")}<th>Aksi</th></tr></thead><tbody>`+
 SALES.map(n=>{let a=get(p,n);return `<tr><td><b>${n}</b></td>`+KPI.map(k=>`<td>${fmt(a[k].target)} / ${fmt(a[k].actual)} / ${fmt(a[k].n1)}<br><small>Ach ${pct(achievement(a[k]))}</small></td>`).join("")+`<td><button class="btn dark" onclick='editSales(${JSON.stringify(n)})'>✏️ Edit</button></td></tr>`}).join("")+"</tbody></table>";
}
function renderPhotos(){
 photosDiv=document.getElementById("photos");
 photosDiv.innerHTML=SALES.map(n=>`<div class="photoBox"><b>${n}</b><img src="${photo(n)||'data:image/svg+xml,%3Csvg xmlns=%22http://www.w3.org/2000/svg%22 width=%2280%22 height=%2280%22%3E%3Crect width=%22100%25%22 height=%22100%25%22 rx=%2240%22 fill=%22%23eef2f6%22/%3E%3Ctext x=%2250%25%22 y=%2258%25%22 text-anchor=%22middle%22 font-size=%2232%22 fill=%22%23667785%22%3E%F0%9F%91%A4%3C/text%3E%3C/svg%3E'}"><input type="file" accept="image/*" onchange='uploadPhoto(this,${JSON.stringify(n)})'></div>`).join("");
}
function uploadPhoto(input,n){const f=input.files[0];if(!f)return;const r=new FileReader();r.onload=()=>{photos[n]=r.result;saveDB();render()};r.readAsDataURL(f)}
function openLogin(){loginModal.classList.add("show");password.focus()}
function closeLogin(){loginModal.classList.remove("show")}
function login(){if(password.value===PASS){isAdmin=true;closeLogin();document.getElementById("status").textContent="Admin aktif • Anda dapat mengedit data";document.getElementById("adminPanel").classList.add("show");}else loginError.textContent="Password salah."}
function toggleEdit(){if(!isAdmin){openLogin();return}document.getElementById("adminPanel").classList.toggle("show")}
function editSales(n){if(!isAdmin){openLogin();return}currentSales=n;editTitle.textContent="Edit KPI • "+n+" • "+monthName(period.value);salesSelect.innerHTML=`<option>${n}</option>`;fillForm(n);editModal.classList.add("show")}
function fillForm(n){let a=get(period.value,n);editForm.innerHTML=KPI.map((k,i)=>`<div class="field"><label>${k} — Target</label><input id="t${i}" type="number" value="${a[k].target}"></div><div class="field"><label>${k} — Realisasi</label><input id="a${i}" type="number" value="${a[k].actual}"></div><div class="field"><label>${k} — N-1 (Pencapaian bulan sebelumnya)</label><input id="n${i}" type="number" value="${a[k].n1}"></div>`).join("")}
function closeEdit(){editModal.classList.remove("show")}
function save(){let p=period.value,a=get(p,currentSales);KPI.forEach((k,i)=>{a[k].target=+document.getElementById("t"+i).value||0;a[k].actual=+document.getElementById("a"+i).value||0;a[k].n1=+document.getElementById("n"+i).value||0});db[p+"|"+currentSales]=a;saveDB();closeEdit();render();alert("Data berhasil disimpan.")}
months().forEach((p,i)=>{let o=document.createElement("option");o.value=p;o.textContent=monthName(p);if(i===0)o.selected=true;period.appendChild(o)});
render();
</script>
</body>
</html>
