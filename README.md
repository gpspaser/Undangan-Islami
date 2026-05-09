<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Undangan Digital Islami</title>
<link href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css' rel='stylesheet'/>
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,sans-serif}
body{
  background:linear-gradient(rgba(15,81,50,0.9),rgba(15,81,50,0.9)),url('https://i.imgur.com/8QfGjKL.jpg');
  background-size:cover;background-position:center;background-attachment:fixed;
}
.header{
  background:linear-gradient(135deg,rgba(15,81,50,0.95) 0%,rgba(26,122,76,0.95) 100%);
  padding:30px 20px 25px;text-align:center;color:#fff;backdrop-filter:blur(10px);
  border-bottom:3px solid #D4AF37;
}
.bismillah{font-size:26px;color:#FFD700;margin-bottom:8px;font-weight:600;text-shadow:0 2px 10px rgba(0,0,0,.3)}
.header h1{font-size:24px;font-weight:700;margin-bottom:5px}
.header p{font-size:13px;opacity:.9;border-top:1px solid rgba(255,215,0,.3);padding-top:8px;margin-top:8px;display:inline-block}
.container{padding:20px 15px 80px;max-width:500px;margin:0 auto}
.judul-menu{text-align:center;font-size:18px;font-weight:700;color:#fff;margin-bottom:20px;text-shadow:0 2px 5px rgba(0,0,0,.5)}
.grid{display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
.menu-item{
  background:rgba(255,255,255,0.95);border:3px solid #D4AF37;border-radius:16px;padding:20px 10px;
  text-align:center;cursor:pointer;transition:.3s;backdrop-filter:blur(5px);
  box-shadow:0 5px 20px rgba(0,0,0,.2);
}
.menu-item:active{transform:scale(.95);background:#FFFEF7}
.menu-item i{font-size:36px;margin-bottom:8px;display:block}
.menu-item span{font-size:12px;font-weight:700;color:#0F5132;line-height:1.3}
.form-page{display:none;background:linear-gradient(rgba(248,246,240,0.98),rgba(248,246,240,0.98)),url('https://i.imgur.com/8QfGjKL.jpg');background-size:cover;min-height:100vh;padding:15px}
.form-page.active{display:block}
.form-header{background:#0F5132;color:#fff;padding:15px;margin:-15px -15px 20px;display:flex;align-items:center;gap:12px}
.form-header i{font-size:20px}
.form-header h2{font-size:16px}
.card-form{background:rgba(255,255,255,0.98);border-radius:16px;padding:20px;border:2px solid #D4AF37;box-shadow:0 5px 20px rgba(0,0,0,.1)}
label{font-size:12px;color:#555;margin:12px 0 5px;display:block;font-weight:700}
input,textarea{width:100%;padding:13px;border:2px solid #eee;border-radius:10px;font-size:14px;background:#fff}
input:focus,textarea:focus{outline:none;border-color:#D4AF37;background:#FFFEF7}
textarea{resize:vertical;min-height:80px}
.btn-wa{background:linear-gradient(135deg,#25D366 0%,#128C7E 100%);color:#fff;width:100%;padding:16px;border-radius:12px;font-size:16px;font-weight:800;border:none;margin-top:20px;box-shadow:0 4px 15px rgba(37,211,102,.3)}
.btn-back{background:#757575;color:#fff;width:100%;padding:14px;border-radius:10px;font-size:14px;font-weight:600;border:none;margin-top:10px}
.hide{display:none!important}
.audio-control{
  position:fixed;bottom:20px;right:20px;z-index:999;
  background:rgba(212,175,55,0.95);width:55px;height:55px;border-radius:50%;
  display:flex;align-items:center;justify-content:center;cursor:pointer;
  box-shadow:0 5px 20px rgba(0,0,0,.3);border:3px solid #fff;
}
.audio-control i{color:#0F5132;font-size:22px}
.audio-control.playing{animation:pulse 2s infinite}
@keyframes pulse{0%,100%{transform:scale(1)}50%{transform:scale(1.1)}}
  .donasi-box{
  background:linear-gradient(135deg,#FFF9E6 0%,#FFFEF7 100%);border:2px dashed #D4AF37;
  border-radius:12px;padding:15px;margin:18px 0;text-align:center;
}
.donasi-box h3{color:#0F5132;font-size:14px;margin-bottom:10px}
.donasi-box p{font-size:11px;color:#666;margin-bottom:12px;line-height:1.5}
.donasi-item{display:flex;align-items:center;justify-content:space-between;background:#fff;padding:10px;border-radius:8px;margin-bottom:8px;border:1px solid #eee}
.donasi-item img{width:70px;height:auto}
.donasi-item span{font-weight:700;color:#0F5132;font-size:14px}
.btn-copy{background:#D4AF37;color:#0F5132;border:none;padding:6px 12px;border-radius:6px;font-size:11px;font-weight:700;cursor:pointer}
.btn-copy:active{transform:scale(.95)}
</style>
</head>
<body>

<!-- AUDIO SHOLAWAT GURU SEKUMPUL -->
<audio id="sholawat" loop>
  <source src="https://ia801504.us.archive.org/10/items/SholawatGuruSekumpul/Sholawat%20Guru%20Sekumpul.mp3" type="audio/mpeg">
</audio>
<div class="audio-control" onclick="toggleAudio()" id="btnAudio">
  <i class="fa-solid fa-play"></i>
</div>

<!-- HALAMAN MENU UTAMA -->
<div id="halamanMenu">
  <div class="header">
    <div class="bismillah">بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ</div>
    <h1>Undangan Digital Islami</h1>
    <p>Sebarkan Kebahagiaan Dengan Mudah</p>
  </div>
  
  <div class="container">
    <div class="judul-menu">Pilih Jenis Undangan</div>
    <div class="grid">
      <div class="menu-item" onclick="bukaForm('nikah')">
        <i class="fa-solid fa-ring" style="color:#4FC3F7"></i>
        <span>Pernikahan</span>
      </div>
      <div class="menu-item" onclick="bukaForm('haji')">
        <i class="fa-solid fa-kaaba" style="color:#424242"></i>
        <span>Haji & Umroh</span>
      </div>
      <div class="menu-item" onclick="bukaForm('khitan')">
        <i class="fa-solid fa-scissors" style="color:#424242"></i>
        <span>Khitanan</span>
      </div>
      <div class="menu-item" onclick="bukaForm('tasmiyah')">
        <i class="fa-solid fa-baby" style="color:#FFD54F"></i>
        <span>Tasmiyah</span>
      </div>
      <div class="menu-item" onclick="bukaForm('isra')">
        <i class="fa-solid fa-moon" style="color:#5C6BC0"></i>
        <span>Isra Mi'raj</span>
      </div>
      <div class="menu-item" onclick="bukaForm('maulid')">
        <i class="fa-solid fa-star-and-crescent" style="color:#66BB6A"></i>
        <span>Maulid Nabi</span>
      </div>
      <div class="menu-item" onclick="bukaForm('ultah')">
        <i class="fa-solid fa-cake-candles" style="color:#FF7043"></i>
        <span>Ulang Tahun</span>
      </div>
      <div class="menu-item" onclick="bukaForm('syukuran')">
        <i class="fa-solid fa-mosque" style="color:#FFD54F"></i>
        <span>Syukuran</span>
      </div>
    </div>
  </div>
</div>

<!-- FORM PERNIKAHAN -->
<div class="form-page" id="form-nikah">
  <div class="form-header"><i class="fa-solid fa-arrow-left" onclick="tutupForm()"></i><h2>Undangan Pernikahan</h2></div>
  <div class="card-form">
    <label>Nama Mempelai Pria</label><input id="pria" placeholder="Ahmad Fauzi">
    <label>Nama Mempelai Wanita</label><input id="wanita" placeholder="Siti Aisyah">
    <label>Hari & Tanggal Akad</label><input id="tglNikah" placeholder="Minggu, 25 Mei 2026">
    <label>Jam Akad</label><input id="jamNikah" placeholder="09.00 WIB">
    <label>Tempat Akad & Resepsi</label><textarea id="tempatNikah" rows="2" placeholder="Kediaman Mempelai Wanita, Jl. Merdeka No.123"></textarea>
    <hr style="margin:18px 0;border:1px solid #eee">
    <label>Nama Tamu Undangan</label><input id="tamuNikah" placeholder="Yth. Bapak/Ibu/Saudara/i">
    <label>No. WhatsApp Tamu</label><input id="waNikah" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('nikah')"><i class="fa-brands fa-whatsapp"></i>KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div>
</div>

<!-- FORM HAJI -->
<div class="form-page" id="form-haji">
  <div class="form-header"><i class="fa-solid fa-arrow-left" onclick="tutupForm()"></i><h2>Undangan Syukuran Haji</h2></div>
  <div class="card-form">
    <label>Nama Haji/Hajjah</label><input id="namaHaji" placeholder="H. Ahmad Suparman">
    <label>Jenis Acara</label><input id="jenisHaji" placeholder="Walimatus Safar / Syukuran Haji">
    <label>Hari & Tanggal</label><input id="tglHaji" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamHaji" placeholder="10.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatHaji" rows="2" placeholder="Kediaman Bpk. Ahmad, Jl. Merdeka No.123"></textarea>
    <label>Atas Nama Keluarga</label><input id="keluargaHaji" placeholder="Keluarga Besar H. Ahmad">
    <div class="donasi-box">
  <h3><i class="fa-solid fa-hand-holding-heart"></i> Donasi Suka Rela</h3>
  <p>Jika berkenan berbagi kebahagiaan, bisa melalui:</p>
  <div class="donasi-item">
    <img src="https://i.imgur.com/2RsM8zD.png" alt="DANA">
    <span>081254693504</span>
    <button class="btn-copy" onclick="copyNo('081254693504')">Salin</button>
  </div>
  <div class="donasi-item">
    <img src="https://i.imgur.com/sQqZt2k.png" alt="ShopeePay">
    <span>081254693504</span>
    <button class="btn-copy" onclick="copyNo('081254693504')">Salin</button>
  </div>
  <p style="font-size:10px;margin-top:8px">Jazakumullah Khairan Katsiran 🤲</p>
</div>
    <hr style="margin:18px 0;border:1px solid #eee">
    <label>Nama Tamu Undangan</label><input id="tamuHaji" placeholder="Yth. Bapak H. Hasan">
    <label>No. WhatsApp Tamu</label><input id="waHaji" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('haji')"><i class="fa-brands fa-whatsapp"></i>KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div>
</div>

<!-- FORM ISRA MI'RAJ -->
<div class="form-page" id="form-isra">
  <div class="form-header"><i class="fa-solid fa-arrow-left" onclick="tutupForm()"></i><h2>Undangan Isra Mi'raj</h2></div>
  <div class="card-form">
    <label>Tema Acara</label><input id="temaIsra" placeholder="Memperingati Isra Mi'raj Nabi Muhammad SAW">
    <label>Penceramah/Ustadz</label><input id="ustadzIsra" placeholder="Ustadz Dr. H. Abdullah, Lc., MA">
    <label>Hari & Tanggal</label><input id="tglIsra" placeholder="Kamis Malam Jumat, 26 Rajab 1447 H">
    <label>Jam</label><input id="jamIsra" placeholder="19.30 WIB - Selesai">
    <label>Tempat / Masjid</label><textarea id="alamatIsra" rows="2" placeholder="Masjid Agung Al-Ikhlas, Jl. Sudirman No. 1"></textarea>
    <label>Penyelenggara</label><input id="panitiaIsra" placeholder="Remaja Masjid Al-Ikhlas / PHBI">
    <hr style="margin:18px 0;border:1px solid #eee">
    <label>Nama Tamu Undangan</label><input id="tamuIsra" placeholder="Kaum Muslimin & Muslimat">
    <label>No. WhatsApp Tamu</label><input id="waIsra" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('isra')"><i class="fa-brands fa-whatsapp"></i>KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div>
</div>

<!-- FORM MAULID NABI -->
<div class="form-page" id="form-maulid">
  <div class="form-header"><i class="fa-solid fa-arrow-left" onclick="tutupForm()"></i><h2>Undangan Maulid Nabi</h2></div>
  <div class="card-form">
    <label>Tema Maulid</label><input id="temaMaulid" placeholder="Meneladani Akhlak Rasulullah SAW">
    <label>Penceramah/Ustadz</label><input id="ustadzMaulid" placeholder="KH. Ahmad Musthofa Bisri">
    <label>Hari & Tanggal</label><input id="tglMaulid" placeholder="Senin, 12 Rabiul Awal 1447 H">
    <label>Jam</label><input id="jamMaulid" placeholder="19.30 WIB - Selesai">
    <label>Tempat / Masjid</label><textarea id="alamatMaulid" rows="2" placeholder="Masjid Jami' Baiturrahman"></textarea>
    <label>Penyelenggara</label><input id="panitiaMaulid" placeholder="Takmir Masjid Baiturrahman">
    <hr style="margin:18px 0;border:1px solid #eee">
    <label>Nama Tamu Undangan</label><input id="tamuMaulid" placeholder="Kaum Muslimin & Muslimat">
    <label>No. WhatsApp Tamu</label><input id="waMaulid" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('maulid')"><i class="fa-brands fa-whatsapp"></i>KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div>
</div>

<!-- FORM KHITANAN -->
<div class="form-page" id="form-khitan">
  <div class="form-header"><i class="fa-solid fa-arrow-left" onclick="tutupForm()"></i><h2>Undangan Khitanan</h2></div>
  <div class="card-form">
    <label>Nama Anak</label><input id="namaKhitan" placeholder="Ananda Muhammad Rizki">
    <label>Putra Dari</label><input id="ortuKhitan" placeholder="Bpk. Ahmad & Ibu Siti">
    <label>Hari & Tanggal</label><input id="tglKhitan" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamKhitan" placeholder="10.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatKhitan" rows="2"></textarea>
    <hr style="margin:18px 0;border:1px solid #eee">
    <label>Nama Tamu Undangan</label><input id="tamuKhitan" placeholder="Yth. Bapak/Ibu">
    <label>No. WhatsApp Tamu</label><input id="waKhitan" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('khitan')"><i class="fa-brands fa-whatsapp"></i>KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div>
</div>

<!-- FORM TASMIYAH -->
<div class="form-page" id="form-tasmiyah">
  <div class="form-header"><i class="fa-solid fa-arrow-left" onclick="tutupForm()"></i><h2>Undangan Tasmiyah</h2></div>
  <div class="card-form">
    <label>Nama Bayi</label><input id="namaBayi" placeholder="Aisyah Nur Ramadhani">
    <label>Putri/Putra Dari</label><input id="ortuBayi" placeholder="Bpk. Ahmad & Ibu Siti">
    <label>Hari & Tanggal</label><input id="tglTasmiyah" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamTasmiyah" placeholder="10.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatTasmiyah" rows="2"></textarea>
    <hr style="margin:18px 0;border:1px solid #eee">
    <label>Nama Tamu Undangan</label><input id="tamuTasmiyah" placeholder="Yth. Bapak/Ibu">
    <label>No. WhatsApp Tamu</label><input id="waTasmiyah" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('tasmiyah')"><i class="fa-brands fa-whatsapp"></i>KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div>
</div>

<!-- FORM ULTAH -->
<div class="form-page" id="form-ultah">
  <div class="form-header"><i class="fa-solid fa-arrow-left" onclick="tutupForm()"></i><h2>Undangan Ulang Tahun</h2></div>
  <div class="card-form">
    <label>Nama Yang Ultah</label><input id="namaUltah" placeholder="Muhammad Rizki">
    <label>Ultah Yang Ke-</label><input id="umurUltah" placeholder="5" type="number">
    <label>Hari & Tanggal</label><input id="tglUltah" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamUltah" placeholder="16.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatUltah" rows="2"></textarea>
    <hr style="margin:18px 0;border:1px solid #eee">
    <label>Nama Tamu Undangan</label><input id="tamuUltah" placeholder="Teman-teman Rizki">
    <label>No. WhatsApp Tamu</label><input id="waUltah" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('ultah')"><i class="fa-brands fa-whatsapp"></i>KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div>
</div>

<!-- FORM SYUKURAN -->
<div class="form-page" id="form-syukuran">
  <div class="form-header"><i class="fa-solid fa-arrow-left" onclick="tutupForm()"></i><h2>Undangan Syukuran</h2></div>
  <div class="card-form">
    <label>Acara Syukuran Apa</label><input id="acaraSyukuran" placeholder="Rumah Baru / Kelahiran / dll">
    <label>Atas Nama</label><input id="namaSyukuran" placeholder="Keluarga Bpk. Ahmad">
    <label>Hari & Tanggal</label><input id="tglSyukuran" placeholder="Minggu, 18 Mei 2026">
    <label>Jam</label><input id="jamSyukuran" placeholder="10.00 WITA">
    <label>Tempat / Alamat</label><textarea id="alamatSyukuran" rows="2"></textarea>
    <hr style="margin:18px 0;border:1px solid #eee">
    <label>Nama Tamu Undangan</label><input id="tamuSyukuran" placeholder="Yth. Bapak/Ibu">
    <label>No. WhatsApp Tamu</label><input id="waSyukuran" placeholder="08123456789" type="tel">
    <button class="btn-wa" onclick="kirimWA('syukuran')"><i class="fa-brands fa-whatsapp"></i>KIRIM VIA WHATSAPP</button>
    <button class="btn-back" onclick="tutupForm()">Kembali ke Menu</button>
  </div>
</div>

<script>
const audio = document.getElementById('sholawat');
const btnAudio = document.getElementById('btnAudio');
let isPlaying = false;

function toggleAudio(){
  if(isPlaying){
    audio.pause();
    btnAudio.innerHTML = '<i class="fa-solid fa-play"></i>';
    btnAudio.classList.remove('playing');
  } else {
    audio.play();
    btnAudio.innerHTML = '<i class="fa-solid fa-pause"></i>';
    btnAudio.classList.add('playing');
  }
  isPlaying = !isPlaying;
}

function bukaForm(jenis){
  document.getElementById('halamanMenu').style.display='none';
  document.getElementById('form-'+jenis).classList.add('active');
  window.scrollTo(0,0);
}

function tutupForm(){
  document.querySelectorAll('.form-page').forEach(el=>el.classList.remove('active'));
  document.getElementById('halamanMenu').style.display='block';
  window.scrollTo(0,0);
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
  
  if(jenis==='nikah'){
    const pria = document.getElementById('pria').value;
    const wanita = document.getElementById('wanita').value;
    const tgl = document.getElementById('tglNikah').value;
    const jam = document.getElementById('jamNikah').value;
    const tempat = document.getElementById('tempatNikah').value;
    const tamu = document.getElementById('tamuNikah').value;
    wa = document.getElementById('waNikah').value;
    if(!pria||!wanita||!tgl||!jam||!tempat||!tamu||!wa) return alert('Lengkapi semua data!');
    
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ

Assalamu'alaikum Warahmatullahi Wabarakatuh

Dengan memohon rahmat & ridho Allah SWT, kami bermaksud menyelenggarakan pernikahan:

*${pria}*
& 
*${wanita}*

Yang Insya Allah dilaksanakan:
📅 ${tgl}
⏰ ${jam}
📍 ${tempat}

Merupakan kehormatan bagi kami apabila *${tamu}* berkenan hadir & memberikan doa restu.

Wassalamu'alaikum Wr. Wb.
*Keluarga Kedua Mempelai*${donasiText}`;
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
    
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ

Assalamu'alaikum Warahmatullahi Wabarakatuh

Alhamdulillah, dengan memohon rahmat Allah SWT, kami mengundang:
*${tamu}*

Untuk hadir dalam acara:
*${jenisAcara || 'SYUKURAN HAJI'}*
*${nama}*

Yang telah selesai menunaikan ibadah haji ke Baitullah.

Insya Allah dilaksanakan:
📅 ${tgl}
⏰ ${jam}
📍 ${alamat}
📖 Acara: Doa Bersama & Ramah Tamah

Kehadiran Bapak/Ibu adalah doa untuk kami. Semoga menjadi haji mabrur. Aamiin.

Wassalamu'alaikum Wr. Wb.
*${keluarga}*`;
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
    
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ

Assalamu'alaikum Warahmatullahi Wabarakatuh

Dengan memohon rahmat Allah SWT, kami mengundang:
*${tamu}*

Untuk menghadiri:
*PERINGATAN ISRA MI'RAJ NABI MUHAMMAD SAW*
*${tema}*

Bersama: *${ustadz}*

Insya Allah dilaksanakan:
📅 ${tgl}
⏰ ${jam}
📍 ${alamat}

Mari kita ambil hikmah dari perjalanan agung Rasulullah SAW. Kehadiran Bapak/Ibu sangat kami harapkan.

Wassalamu'alaikum Wr. Wb.
*${panitia}*`;
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
    
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ

Assalamu'alaikum Warahmatullahi Wabarakatuh

اللهم صل على سيدنا محمد

Dengan penuh cinta kepada Rasulullah SAW, kami mengundang:
*${tamu}*

Untuk menghadiri:
*PERINGATAN MAULID NABI MUHAMMAD SAW*
*${tema}*

Bersama: *${ustadz}*

Insya Allah dilaksanakan:
📅 ${tgl}
⏰ ${jam}
📍 ${alamat}

Mari kita bersholawat & meneladani akhlak Rasulullah SAW. Kehadiran Bapak/Ibu adalah keberkahan bagi kami.

Wassalamu'alaikum Wr. Wb.
*${panitia}*`;
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
    
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ

Assalamu'alaikum Wr. Wb.

Kami mengundang *${tamu}* untuk hadir di acara:
*WALIMATUL KHITAN*
*${nama}*
Putra dari ${ortu}

Insya Allah:
📅 ${tgl}
⏰ ${jam}
📍 ${alamat}

Mohon doa agar menjadi anak sholeh. Kehadiran Bapak/Ibu sangat kami harapkan.

Wassalamu'alaikum Wr. Wb.
*Keluarga ${ortu}*`;
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
    
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ

Assalamu'alaikum Wr. Wb.

Alhamdulillah telah lahir putra/putri kami:
*${nama}*
Putra/Putri dari ${ortu}

Kami mengundang *${tamu}* dalam acara:
*TASMIYAH & AQIQAH*

📅 ${tgl}
⏰ ${jam}
📍 ${alamat}

Mohon doa agar menjadi anak sholeh/sholehah, berbakti & berguna bagi agama.

Wassalamu'alaikum Wr. Wb.
*Keluarga ${ortu}*`;
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
    
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ

Assalamu'alaikum Wr. Wb.

Alhamdulillah *${nama}* genap berusia *${umur} Tahun* 🎂

Mengundang *${tamu}* untuk hadir di acara:
*SYUKURAN ULANG TAHUN*

📅 ${tgl}
⏰ ${jam}
📍 ${alamat}

Mohon doanya agar selalu diberi kesehatan, panjang umur & jadi anak sholeh/sholehah. Aamiin.

Wassalamu'alaikum Wr. Wb.
*Keluarga ${nama}*`;
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
    
    pesan = `بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيمِ

Assalamu'alaikum Wr. Wb.

Dengan rasa syukur, kami *${nama}* mengundang *${tamu}* dalam acara:
*SYUKURAN ${acara.toUpperCase()}*

Insya Allah:
📅 ${tgl}
⏰ ${jam}
📍 ${alamat}

Kehadiran Bapak/Ibu adalah kebahagiaan bagi kami. Mohon doanya.

Wassalamu'alaikum Wr. Wb.
*${nama}*`;
  }
  
  window.open('https://wa.me/'+formatWA(wa)+'?text='+encodeURIComponent(pesan));
}
  function copyNo(no){
  navigator.clipboard.writeText(no);
  alert('Nomor '+no+' berhasil disalin! 🙏');
}
</script>
</body>
</html>
