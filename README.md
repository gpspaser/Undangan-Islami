<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no,viewport-fit=cover">
<meta name="theme-color" content="#0F5132">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="mobile-web-app-capable" content="yes">
<title>Undangan Digital Islami</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,sans-serif;-webkit-tap-highlight-color:transparent}
html,body{width:100%;background:#0F5132}
#app{min-height:100dvh;width:100vw;display:flex;flex-direction:column}
.header{background:#0F5132;padding:max(16px,env(safe-area-inset-top)) 12px 16px;text-align:center;color:#fff;border-bottom:2px solid #D4AF37;flex-shrink:0}
.bismillah{font-size:20px;color:#FFD700;margin-bottom:4px;font-weight:600}
.header h1{font-size:18px;font-weight:700;margin-bottom:2px}
.header p{font-size:11px;opacity:.8}
.scroll-area{flex:1;overflow-y:auto;overflow-x:hidden;-webkit-overflow-scrolling:touch}
.container{padding:12px 10px calc(60px + env(safe-area-inset-bottom));max-width:500px;margin:0 auto}
.judul-menu{text-align:center;font-size:14px;font-weight:700;color:#FFD700;margin-bottom:12px}
.grid{display:grid;grid-template-columns:repeat(2,1fr);gap:8px}
.menu-item{background:#FFD700;border:2px solid #D4AF37;border-radius:10px;padding:14px 6px;text-align:center;cursor:pointer;user-select:none}
.menu-item:active{background:#FFC107}
.menu-item i{font-size:24px;margin-bottom:4px;display:block}
.menu-item span{font-size:10px;font-weight:800;color:#0F5132;line-height:1.1;display:block}
.form-page{display:none;background:#0F5132;min-height:100dvh;flex-direction:column}
.form-page.active{display:flex}
.form-header{background:#0F5132;color:#fff;padding:10px 12px;padding-top:calc(10px + env(safe-area-inset-top));display:flex;align-items:center;gap:8px;flex-shrink:0;border-bottom:2px solid #D4AF37}
.form-header i{font-size:18px;cursor:pointer;padding:5px}
.form-header h2{font-size:14px}
.form-content{flex:1;overflow-y:auto;padding:10px;-webkit-overflow-scrolling:touch}
.card-form{background:#fff;border-radius:12px;padding:14px;border:2px solid #D4AF37;margin-bottom:calc(12px + env(safe-area-inset-bottom))}
label{font-size:10px;color:#555;margin:8px 0 3px;display:block;font-weight:700}
input,textarea{width:100%;padding:11px;border:2px solid #ddd;border-radius:6px;font-size:16px;background:#fff}
input:focus,textarea:focus{outline:none;border-color:#D4AF37;background:#FFFEF7}
textarea{resize:vertical;min-height:60px}
.btn-wa{background:#25D366;color:#fff;width:100%;padding:14px;border-radius:8px;font-size:14px;font-weight:800;border:none;margin-top:14px;cursor:pointer}
.btn-wa:active{transform:scale(.98)}
.btn-back{background:#757575;color:#fff;width:100%;padding:12px;border-radius:6px;font-size:12px;font-weight:600;border:none;margin-top:7px;cursor:pointer}
.donasi-box{background:#FFF9E6;border:2px dashed #D4AF37;border-radius:8px;padding:10px;margin:12px 0;text-align:center}
.donasi-box h3{color:#0F5132;font-size:12px;margin-bottom:6px}
.donasi-box p{font-size:9px;color:#666;margin-bottom:8px;line-height:1.3}
.donasi-item{display:flex;align-items:center;justify-content:space-between;background:#fff;padding:7px;border-radius:5px;margin-bottom:5px;border:1px solid #eee}
.donasi-item img{width:50px;height:auto}
.donasi-item span{font-weight:700;color:#0F5132;font-size:12px}
.btn-copy{background:#D4AF37;color:#0F5132;border:none;padding:4px 8px;border-radius:4px;font-size:9px;font-weight:700;cursor:pointer}
.btn-copy:active{transform:scale(.95)}
.hide{display:none!important}
hr{border:none;border-top:1px solid #eee;margin:12px 0}
</style>
</head>
<body>
<div id="app">

<div id="halamanMenu" class="scroll-area">
  <div class="header">
    <div class="bismillah">بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ</div>
    <h1>Undangan Digital Islami</h1>
    <p>Sebarkan Kebahagiaan Dengan Mudah</p>
  </div>
  <div class="container">
    <div class="judul-menu">Pilih Jenis Undangan</div>
    <div class="grid">
      <div class="menu-item" onclick="bukaForm('nikah')"><i>💍</i><span>Pernikahan</span></div>
      <div class="menu-item" onclick="bukaForm('haji')"><i>🕋</i><span>Haji & Umroh</span></div>
      <div class="menu-item" onclick="bukaForm('khitan')"><i>✂️</i><span>Khitanan</span></div>
      <div class="menu-item" onclick="bukaForm('tasmiyah')"><i>👶</i><span>Tasmiyah</span></div>
      <div class="menu-item" onclick="bukaForm('isra')"><i>🌙</i><span>Isra Mi'raj</span></div>
      <div class="menu-item" onclick="bukaForm('maulid')"><i>🌟</i><span>Maulid Nabi</span></div>
      <div class="menu-item" onclick="bukaForm('ultah')"><i>🎂</i><span>Ulang Tahun</span></div>
      <div class="menu-item" onclick="bukaForm('syukuran')"><i>🕌</i><span>Syukuran</span></div>
    </div>
  </div>
</div>

<div id="templateDonasi" class="hide">
  <div class="donasi-box">
    <h3>💝 Donasi Suka Rela</h3>
    <p>Jika berkenan berbagi kebahagiaan, bisa melalui:</p>
    <div class="donasi-item"><img src="https://i.imgur.com/2RsM8zD.png" alt="DANA"><span>081254693504</span><button class="btn-copy" onclick="copyNo('081254693504')">Salin</button></div>
    <div class="donasi-item"><img src="https://i.imgur.com/sQqZt2k.png" alt="ShopeePay"><span>081254693504</span><button class="btn-copy" onclick="copyNo('081254693504')">Salin</button></div>
    <p style="font-size:8px;margin-top:5px">Jazakumullah Khairan Katsiran 🤲</p>
  </div>
</div>

<div class="form-page" id="form-nikah">
  <div class="form-header"><i onclick="tutupForm()">←</i><h2>Undangan Pernikahan</h2></div>
  <div class="form-content"><div class="card-form">
    <label>Nama Mempelai Pria</label><input id="pria" placeholder="Ahmad Fauzi">
    <label>Nama Mempelai Wanita</label><input id="wanita" placeholder="Siti Aisyah">
    <label>Hari & Tanggal Akad</label><input id="tglNikah" placeholder="Minggu, 25 Mei 2026">
    <label>Jam Akad</label><input id="jamNikah" placeholder="09.00 WIB">
    <label>Tempat Akad & Resepsi</label><textarea id="tempatNikah" rows="2" placeholder="Kediaman Mempelai Wanita, Jl. Merdeka No.123"></textarea>
    <div id="donasi-nikah"></div><hr>
    <label>Nama Tamu Undangan</label><input id="tamuNikah" placeholder="Yth. Bapak/Ibu/Saudara/i">
    <label>No. WhatsApp Tamu</label><input id="waNikah" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('nikah')">KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div></div>
</div>

<div class="form-page" id="form-haji">
  <div class="form-header"><i onclick="tutupForm()">←</i><h2>Undangan Syukuran Haji</h2></div>
  <div class="form-content"><div class="card-form">
    <label>Nama Haji/Hajjah</label><input id="namaHaji" placeholder="H. Ahmad Suparman">
    <label>Jenis Acara</label><input id="jenisHaji" placeholder="Walimatus Safar / Syukuran Haji">
    <label>Hari & Tanggal</label><input id="tglHaji" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamHaji" placeholder="10.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatHaji" rows="2" placeholder="Kediaman Bpk. Ahmad, Jl. Merdeka No.123"></textarea>
    <label>Atas Nama Keluarga</label><input id="keluargaHaji" placeholder="Keluarga Besar H. Ahmad">
    <div id="donasi-haji"></div><hr>
    <label>Nama Tamu Undangan</label><input id="tamuHaji" placeholder="Yth. Bapak H. Hasan">
    <label>No. WhatsApp Tamu</label><input id="waHaji" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('haji')">KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div></div>
</div>

<div class="form-page" id="form-isra">
  <div class="form-header"><i onclick="tutupForm()">←</i><h2>Undangan Isra Mi'raj</h2></div>
  <div class="form-content"><div class="card-form">
    <label>Tema Acara</label><input id="temaIsra" placeholder="Memperingati Isra Mi'raj Nabi Muhammad SAW">
    <label>Penceramah/Ustadz</label><input id="ustadzIsra" placeholder="Ustadz Dr. H. Abdullah, Lc., MA">
    <label>Hari & Tanggal</label><input id="tglIsra" placeholder="Kamis Malam Jumat, 26 Rajab 1447 H">
    <label>Jam</label><input id="jamIsra" placeholder="19.30 WIB - Selesai">
    <label>Tempat / Masjid</label><textarea id="alamatIsra" rows="2" placeholder="Masjid Agung Al-Ikhlas, Jl. Sudirman No. 1"></textarea>
    <label>Penyelenggara</label><input id="panitiaIsra" placeholder="Remaja Masjid Al-Ikhlas / PHBI">
    <div id="donasi-isra"></div><hr>
    <label>Nama Tamu Undangan</label><input id="tamuIsra" placeholder="Kaum Muslimin & Muslimat">
    <label>No. WhatsApp Tamu</label><input id="waIsra" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('isra')">KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div></div>
</div>

<div class="form-page" id="form-maulid">
  <div class="form-header"><i onclick="tutupForm()">←</i><h2>Undangan Maulid Nabi</h2></div>
  <div class="form-content"><div class="card-form">
    <label>Tema Maulid</label><input id="temaMaulid" placeholder="Meneladani Akhlak Rasulullah SAW">
    <label>Penceramah/Ustadz</label><input id="ustadzMaulid" placeholder="KH. Ahmad Musthofa Bisri">
    <label>Hari & Tanggal</label><input id="tglMaulid" placeholder="Senin, 12 Rabiul Awal 1447 H">
    <label>Jam</label><input id="jamMaulid" placeholder="19.30 WIB - Selesai">
    <label>Tempat / Masjid</label><textarea id="alamatMaulid" rows="2" placeholder="Masjid Jami' Baiturrahman"></textarea>
    <label>Penyelenggara</label><input id="panitiaMaulid" placeholder="Takmir Masjid Baiturrahman">
    <div id="donasi-maulid"></div><hr>
    <label>Nama Tamu Undangan</label><input id="tamuMaulid" placeholder="Kaum Muslimin & Muslimat">
    <label>No. WhatsApp Tamu</label><input id="waMaulid" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('maulid')">KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div></div>
</div>

<div class="form-page" id="form-khitan">
  <div class="form-header"><i onclick="tutupForm()">←</i><h2>Undangan Khitanan</h2></div>
  <div class="form-content"><div class="card-form">
    <label>Nama Anak</label><input id="namaKhitan" placeholder="Ananda Muhammad Rizki">
    <label>Putra Dari</label><input id="ortuKhitan" placeholder="Bpk. Ahmad & Ibu Siti">
    <label>Hari & Tanggal</label><input id="tglKhitan" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamKhitan" placeholder="10.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatKhitan" rows="2"></textarea>
    <div id="donasi-khitan"></div><hr>
    <label>Nama Tamu Undangan</label><input id="tamuKhitan" placeholder="Yth. Bapak/Ibu">
    <label>No. WhatsApp Tamu</label><input id="waKhitan" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('khitan')">KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div></div>
</div>

<div class="form-page" id="form-tasmiyah">
  <div class="form-header"><i onclick="tutupForm()">←</i><h2>Undangan Tasmiyah</h2></div>
  <div class="form-content"><div class="card-form">
    <label>Nama Bayi</label><input id="namaBayi" placeholder="Aisyah Nur Ramadhani">
    <label>Putri/Putra Dari</label><input id="ortuBayi" placeholder="Bpk. Ahmad & Ibu Siti">
    <label>Hari & Tanggal</label><input id="tglTasmiyah" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamTasmiyah" placeholder="10.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatTasmiyah" rows="2"></textarea>
    <div id="donasi-tasmiyah"></div><hr>
    <label>Nama Tamu Undangan</label><input id="tamuTasmiyah" placeholder="Yth. Bapak/Ibu">
    <label>No. WhatsApp Tamu</label><input id="waTasmiyah" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('tasmiyah')">KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div></div>
</div>

<div class="form-page" id="form-ultah">
  <div class="form-header"><i onclick="tutupForm()">←</i><h2>Undangan Ulang Tahun</h2></div>
  <div class="form-content"><div class="card-form">
    <label>Nama Yang Ultah</label><input id="namaUltah" placeholder="Muhammad Rizki">
    <label>Ultah Yang Ke-</label><input id="umurUltah" placeholder="5" type="number">
    <label>Hari & Tanggal</label><input id="tglUltah" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamUltah" placeholder="16.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatUltah" rows="2"></textarea>
    <div id="donasi-ultah"></div><hr>
    <label>Nama Tamu Undangan</label><input id="tamuUltah" placeholder="Teman-teman Rizki">
    <label>No. WhatsApp Tamu</label><input id="waUltah" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('ultah')">KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div></div>
</div>

<div class="form-page" id="form-syukuran">
  <div class="form-header"><i onclick="tutupForm()">←</i><h2>Undangan Syukuran</h2></div>
  <div class="form-content"><div class="card-form">
    <label>Acara Syukuran Apa</label><input id="acaraSyukuran" placeholder="Rumah Baru / Kelahiran / dll">
    <label>Atas Nama</label><input id="namaSyukuran" placeholder="Keluarga Bpk. Ahmad">
    <label>Hari & Tanggal</label><input id="tglSyukuran" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamSyukuran" placeholder="10.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatSyukuran" rows="2"></textarea>
    <div id="donasi-syukuran"></div><hr>
    <label>Nama Tamu Undangan</label><input id="tamuSyukuran" placeholder="Yth. Bapak/Ibu">
    <label>No. WhatsApp Tamu</label><input id="waSyukuran" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('syukuran')">KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div></div>
</div>

</div>
<script>
function copyNo(no){
  navigator.clipboard.writeText(no);
  alert('Nomor '+no+' berhasil disalin! 🙏');
}
function bukaForm(jenis){
  document.getElementById('halamanMenu').style.display='none';
  document.getElementById('form-'+jenis).classList.add('active');
  document.getElementById('donasi-'+jenis).innerHTML = document.getElementById('templateDonasi').innerHTML;
}
function tutupForm(){
  document.querySelectorAll('.form-page').forEach(el=>el.classList.remove('active'));
  document.getElementById('halamanMenu').style.display='block';
}
function formatWA(no){
  let nomor = no.replace(/[^0-9]/g,'');
  if(nomor.startsWith('08')) return '62'+nomor.substring(1);
  if(nomor.startsWith('8')) return '62'+nomor;
  if(!nomor.startsWith('62')) return '62'+nomor;
  return nomor;
}
function kirimWA(jenis){
  let pesan = '';
  let wa = '';
  const donasiText = `\n\n💚 *Donasi Suka Rela:*\nDANA/ShopeePay: 081254693504\nJazakumullah Khairan Katsiran 🤲`;
  
  if(jenis==='nikah'){
    const pria = document.getElementById('pria').value;
    const wanita = document.getElementById('wanita').value;
    const tgl = document.getElementById('tglNikah').value;
    const jam = document.getElementById('jamNikah').value;
    const tempat = document.getElementById('tempatNikah').value;
    const tamu = document.getElementById('tamuNikah').value;
    wa = document.getElementById('waNikah').value;
    if(!pria||!wanita||!tgl||!jam||!tempat||!tamu||!wa) return alert('Lengkapi semua data!');
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ\n\nAssalamu'alaikum Warahmatullahi Wabarakatuh\n\nDengan memohon rahmat & ridho Allah SWT, kami bermaksud menyelenggarakan pernikahan:\n\n*${pria}*\n& \n*${wanita}*\n\nYang Insya Allah dilaksanakan:\n📅 ${tgl}\n⏰ ${jam}\n📍 ${tempat}\n\nMerupakan kehormatan bagi kami apabila *${tamu}* berkenan hadir & memberikan doa restu.\n\nWassalamu'alaikum Wr. Wb.\n*Keluarga Kedua Mempelai*${donasiText}`;
  }
  else if(jenis==='haji'){
    const nama = document.getElementById('namaHaji').value;
    const jenisAcara = document.getElementById('jenisHaji').value;
    const tgl = document.getElementById('tglHaji').value;
    const jam = document.getElementById('jamHaji').value;
    const alamat = document.getElementById('alamatHaji').value;
    const keluarga = document.getElementById('keluargaHaji').value;
    const tamu = document.getElementById('tamuHaji').value;
    wa = document.getElementById('waHaji').value;
    if(!nama||!tgl||!jam||!alamat||!tamu||!wa) return alert('Lengkapi semua data!');
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ\n\nAssalamu'alaikum Warahmatullahi Wabarakatuh\n\nAlhamdulillah, dengan memohon rahmat Allah SWT, kami mengundang:\n*${tamu}*\n\nUntuk hadir dalam acara:\n*${jenisAcara || 'SYUKURAN HAJI'}*\n*${nama}*\n\nYang telah selesai menunaikan ibadah haji ke Baitullah.\n\nInsya Allah dilaksanakan:\n📅 ${tgl}\n⏰ ${jam}\n📍 ${alamat}\n📖 Acara: Doa Bersama & Ramah Tamah\n\nKehadiran Bapak/Ibu adalah doa untuk kami. Semoga menjadi haji mabrur. Aamiin.\n\nWassalamu'alaikum Wr. Wb.\n*${keluarga}*${donasiText}`;
  }
  else if(jenis==='isra'){
    const tema = document.getElementById('temaIsra').value;
    const ustadz = document.getElementById('ustadzIsra').value;
    const tgl = document.getElementById('tglIsra').value;
    const jam = document.getElementById('jamIsra').value;
    const alamat = document.getElementById('alamatIsra').value;
    const panitia = document.getElementById('panitiaIsra').value;
    const tamu = document.getElementById('tamuIsra').value;
    wa = document.getElementById('waIsra').value;
    if(!tema||!tgl||!jam||!alamat||!tamu||!wa) return alert('Lengkapi semua data!');
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ\n\nAssalamu'alaikum Warahmatullahi Wabarakatuh\n\nDengan memohon rahmat Allah SWT, kami mengundang:\n*${tamu}*\n\nUntuk menghadiri:\n*PERINGATAN ISRA MI'RAJ NABI MUHAMMAD SAW*\n*${tema}*\n\nBersama: *${ustadz}*\n\nInsya Allah dilaksanakan:\n📅 ${tgl}\n⏰ ${jam}\n📍 ${alamat}\n\nMari kita ambil hikmah dari perjalanan agung Rasulullah SAW. Kehadiran Bapak/Ibu sangat kami harapkan.\n\nWassalamu'alaikum Wr. Wb.\n*${panitia}*${donasiText}`;
  }
  else if(jenis==='maulid'){
    const tema = document.getElementById('temaMaulid').value;
    const ustadz = document.getElementById('ustadzMaulid').value;
    const tgl = document.getElementById('tglMaulid').value;
    const jam = document.getElementById('jamMaulid').value;
    const alamat = document.getElementById('alamatMaulid').value;
    const panitia = document.getElementById('panitiaMaulid').value;
    const tamu = document.getElementById('tamuMaulid').value;
    wa = document.getElementById('waMaulid').value;
    if(!tema||!tgl||!jam||!alamat||!tamu||!wa) return alert('Lengkapi semua data!');
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ\n\nAssalamu'alaikum Warahmatullahi Wabarakatuh\n\nاللهم صل على سيدنا محمد\n\nDengan penuh cinta kepada Rasulullah SAW, kami mengundang:\n*${tamu}*\n\nUntuk menghadiri:\n*PERINGATAN MAULID NABI MUHAMMAD SAW*\n*${tema}*\n\nBersama: *${ustadz}*\n\nInsya Allah dilaksanakan:\n📅 ${tgl}\n⏰ ${jam}\n📍 ${alamat}\n\nMari kita bersholawat & meneladani akhlak Rasulullah SAW. Kehadiran Bapak/Ibu adalah keberkahan bagi kami.\n\nWassalamu'alaikum Wr. Wb.\n*${panitia}*${donasiText}`;
  }
  else if(jenis==='khitan'){
    const nama = document.getElementById('namaKhitan').value;
    const ortu = document.getElementById('ortuKhitan').value;
    const tgl = document.getElementById('tglKhitan').value;
    const jam = document.getElementById('jamKhitan').value;
    const alamat = document.getElementById('alamatKhitan').value;
    const tamu = document.getElementById('tamuKhitan').value;
    wa = document.getElementById('waKhitan').value;
    if(!nama||!ortu||!tgl||!jam||!alamat||!tamu||!wa) return alert('Lengkapi semua data!');
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ\n\nAssalamu'alaikum Wr. Wb.\n\nKami mengundang *${tamu}* untuk hadir di acara:\n*WALIMATUL KHITAN*\n*${nama}*\nPutra dari ${ortu}\n\nInsya Allah:\n📅 ${tgl}\n⏰ ${jam}\n📍 ${alamat}\n\nMohon doa agar menjadi anak sholeh. Kehadiran Bapak/Ibu sangat kami harapkan.\n\nWassalamu'alaikum Wr. Wb.\n*Keluarga ${ortu}*${donasiText}`;
  }
  else if(jenis==='tasmiyah'){
    const nama = document.getElementById('namaBayi').value;
    const ortu = document.getElementById('ortuBayi').value;
    const tgl = document.getElementById('tglTasmiyah').value;
    const jam = document.getElementById('jamTasmiyah').value;
    const alamat = document.getElementById('alamatTasmiyah').value;
    const tamu = document.getElementById('tamuTasmiyah').value;
    wa = document.getElementById('waTasmiyah').value;
    if(!nama||!ortu||!tgl||!jam||!alamat||!tamu||!wa) return alert('Lengkapi semua data!');
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ\n\nAssalamu'alaikum Wr. Wb.\n\nAlhamdulillah telah lahir putra/putri kami:\n*${nama}*\nPutra/Putri dari ${ortu}\n\nKami mengundang *${tamu}* dalam acara:\n*TASMIYAH & AQIQAH*\n\n📅 ${tgl}\n⏰ ${jam}\n📍 ${alamat}\n\nMohon doa agar menjadi anak sholeh/sholehah, berbakti & berguna bagi agama.\n\nWassalamu'alaikum Wr. Wb.\n*Keluarga ${ortu}*${donasiText}`;
  }
  else if(jenis==='ultah'){
    const nama = document.getElementById('namaUltah').value;
    const umur = document.getElementById('umurUltah').value;
    const tgl = document.getElementById('tglUltah').value;
    const jam = document.getElementById('jamUltah').value;
    const alamat = document.getElementById('alamatUltah').value;
    const tamu = document.getElementById('tamuUltah').value;
    wa = document.getElementById('waUltah').value;
    if(!nama||!umur||!tgl||!jam||!alamat||!tamu||!wa) return alert('Lengkapi semua data!');
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ\n\nAssalamu'alaikum Wr. Wb.\n\nAlhamdulillah *${nama}* genap berusia *${umur} Tahun* 🎂\n\nMengundang *${tamu}* untuk hadir di acara:\n*SYUKURAN ULANG TAHUN*\n\n📅 ${tgl}\n⏰ ${jam}\n📍 ${alamat}\n\nMohon doanya agar selalu diberi kesehatan, panjang umur & jadi anak sholeh/sholehah. Aamiin.\n\nWassalamu'alaikum Wr. Wb.\n*Keluarga ${nama}*${donasiText}`;
  }
  else if(jenis==='syukuran'){
    const acara = document.getElementById('acaraSyukuran').value;
    const nama = document.getElementById('namaSyukuran').value;
    const tgl = document.getElementById('tglSyukuran').value;
    const jam = document.getElementById('jamSyukuran').value;
    const alamat = document.getElementById('alamatSyukuran').value;
    const tamu = document.getElementById('tamuSyukuran').value;
    wa = document.getElementById('waSyukuran').value;
    if(!acara||!nama||!tgl||!jam||!alamat||!tamu||!wa) return alert('Lengkapi semua data!');
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ\n\nAssalamu'alaikum Wr. Wb.\n\nDengan rasa syukur, kami *${nama}* mengundang *${tamu}* dalam acara:\n*SYUKURAN ${acara.toUpperCase()}*\n\nInsya Allah:\n📅 ${tgl}\n⏰ ${jam}\n📍 ${alamat}\n\nKehadiran Bapak/Ibu adalah kebahagiaan bagi kami. Mohon doanya.\n\nWassalamu'alaikum Wr. Wb.\n*${nama}*${donasiText}`;
  }
  
  window.open('https://wa.me/'+formatWA(wa)+'?text='+encodeURIComponent(pesan));
}
</script>
</body>
</html>
