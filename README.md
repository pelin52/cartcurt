[index.html](https://github.com/user-attachments/files/27307527/index.html)
<!DOCTYPE html>
<html lang="tr" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SKYBEE | Prestige Drone Media</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="icon" type="image/x-icon" href="logo1.png">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;900&display=swap" rel="stylesheet">
    
    <style>
        body { font-family: 'Outfit', sans-serif; background-color: #000; }
        
        .panorama-bg {
            position: fixed; top: 0; left: 0; width: 100vw; height: 100vh;
            z-index: -1; opacity: 0.20;
            background: url('https://c8.alamy.com/comp/2F5K398/panoramic-aerial-view-of-historic-harbour-in-kyrenia-girne-north-cyprus-in-a-beautiful-summer-day-2F5K398.jpg') repeat-x;
            background-size: cover;
            animation: moveBg 140s linear infinite;
        }
        
        @keyframes moveBg { 
            from { background-position: 0 0; } 
            to { background-position: -3840px 0; } 
        }

        .logo-text {
            text-shadow: 0 4px 12px rgba(0, 0, 0, 1), 0 0 20px rgba(234, 179, 8, 0.4);
            -webkit-box-reflect: below -6px linear-gradient(transparent, rgba(255, 255, 255, 0.15));
        }

        .social-icon {
            -webkit-box-reflect: below 2px linear-gradient(transparent, rgba(255, 255, 255, 0.1));
            transition: transform 0.3s ease;
        }
        .social-icon:hover { transform: scale(1.15); }

        .content-layer { position: relative; z-index: 10; }
        
        .map-container {
            border-radius: 30px;
            overflow: hidden;
        }

        .gallery-card {
            position: relative;
            overflow: hidden;
            border-radius: 25px;
            aspect-ratio: 16/9;
            border: 1px solid rgba(255, 255, 255, 0.1);
            background: rgba(255, 255, 255, 0.05);
        }
        .gallery-card img, .gallery-card video {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.8s cubic-bezier(0.2, 0, 0.2, 1);
        }
        .gallery-card:hover img, .gallery-card:hover video {
            transform: scale(1.1);
        }
    </style>
</head>
<body class="text-white overflow-x-hidden">

    <div class="panorama-bg"></div>

    <!-- WhatsApp Button -->
    <a href="https://wa.me/905391100777" target="_blank" class="fixed bottom-8 right-8 bg-[#25d366] w-16 h-16 rounded-full flex items-center justify-center text-3xl shadow-lg z-[1500] hover:scale-110 transition-transform">
        <i class="fa-brands fa-whatsapp text-white"></i>
    </a>

    <!-- Navbar -->
    <nav class="fixed top-0 w-full h-24 bg-black/90 backdrop-blur-xl border-b border-yellow-600/30 z-[1000]">
        <div class="max-w-screen-2xl mx-auto w-full h-full flex items-center justify-between px-6 md:px-12">
            <div class="flex items-center gap-2">
                <img src="logo1.png" alt="SKYBEE Logo" class="w-20 md:w-28 h-auto drop-shadow-[0_0_15px_rgba(234,179,8,0.5)]">
                <div class="logo-text font-black italic uppercase tracking-tighter leading-none text-3xl md:text-5xl">
                    SKY<span class="text-yellow-500">BEE</span>
                </div>
            </div>

            <div class="hidden lg:flex items-center gap-8">
                <button onclick="openAbout()" class="text-xs font-bold uppercase tracking-widest hover:text-yellow-500 transition-colors">Hakkımızda</button>
                <a href="#hizmetler" class="text-xs font-bold uppercase tracking-widest hover:text-yellow-500 transition-colors">Hizmetlerimiz</a>
                <a href="#galeri" class="text-xs font-bold uppercase tracking-widest hover:text-yellow-500 transition-colors">Galeri</a>
                <a href="#iletisim" class="text-xs font-bold uppercase tracking-widest hover:text-yellow-500 transition-colors">İletişim</a>
                
                <div class="flex gap-6 ml-4 text-2xl">
                    <a href="https://instagram.com/skybeemedya" target="_blank" class="social-icon" style="color: #E4405F;"><i class="fa-brands fa-instagram"></i></a>
                    <a href="https://youtube.com/@skybeemedya" target="_blank" class="social-icon" style="color: #FF0000;"><i class="fa-brands fa-youtube"></i></a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Header Video -->
    <header class="mt-32 mb-4 w-11/12 max-w-7xl mx-auto h-auto rounded-[40px] overflow-hidden border border-yellow-600/20 shadow-2xl relative content-layer">
        <video autoplay muted loop playsinline class="w-full h-auto block">
            <source src="tanitim/tanitim_videosu.mp4" type="video/mp4">
        </video>
    </header>

    <!-- Hizmetler Section -->
    <section id="hizmetler" class="pt-8 pb-24 w-full max-w-7xl mx-auto px-6 content-layer">
        <h2 class="text-4xl md:text-5xl font-black italic uppercase text-center mb-16">Hizmet <span class="text-yellow-500">Alanlarımız</span></h2>
        <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 gap-6">
            <div class="bg-white/5 backdrop-blur-md p-8 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group">
                <i class="fa-solid fa-futbol text-3xl text-yellow-500 mb-4 group-hover:scale-110 transition-transform"></i>
                <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest">Futbol Kulüpleri & Maçlar</h3>
            </div>
            <div class="bg-white/5 backdrop-blur-md p-8 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group">
                <i class="fa-solid fa-landmark text-3xl text-yellow-500 mb-4 group-hover:scale-110 transition-transform"></i>
                <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest">Siyasi Partiler & Toplantılar</h3>
            </div>
            <div class="bg-white/5 backdrop-blur-md p-0 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group overflow-hidden relative min-h-[140px] flex items-center justify-center">
                <video autoplay muted loop playsinline class="absolute inset-0 w-full h-full object-cover opacity-40 group-hover:opacity-70 transition-opacity">
                    <source src="senaryolu_araba_cekimleri/yapay_zeka.mp4" type="video/mp4">
                </video>
                <div class="relative z-10 p-4">
                    <i class="fa-solid fa-car-side text-3xl text-yellow-500 mb-2 group-hover:scale-110 transition-transform shadow-black"></i>
                    <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest text-white drop-shadow-md">Senaryolu Araba Çekimleri</h3>
                </div>
            </div>
            <div class="bg-white/5 backdrop-blur-md p-8 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group">
                <i class="fa-solid fa-motorcycle text-3xl text-yellow-500 mb-4 group-hover:scale-110 transition-transform"></i>
                <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest">Motor Kulübü Çekimleri</h3>
            </div>
            <div class="bg-white/5 backdrop-blur-md p-0 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group overflow-hidden relative min-h-[140px] flex items-center justify-center">
                <video autoplay muted loop playsinline class="absolute inset-0 w-full h-full object-cover opacity-40 group-hover:opacity-70 transition-opacity">
                    <source src="universite_tanitimlari/okul_yatay.mp4" type="video/mp4">
                </video>
                <div class="relative z-10 p-4">
                    <i class="fa-solid fa-graduation-cap text-3xl text-yellow-500 mb-2 group-hover:scale-110 transition-transform shadow-black"></i>
                    <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest text-white drop-shadow-md">Üniversite Tanıtımları</h3>
                </div>
            </div>
            <div class="bg-white/5 backdrop-blur-md p-8 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group">
                <i class="fa-solid fa-city text-3xl text-yellow-500 mb-4 group-hover:scale-110 transition-transform"></i>
                <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest">Belediye Projeleri</h3>
            </div>
            <div class="bg-white/5 backdrop-blur-md p-0 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group overflow-hidden relative min-h-[140px] flex items-center justify-center">
                <video autoplay muted loop playsinline class="absolute inset-0 w-full h-full object-cover opacity-40 group-hover:opacity-70 transition-opacity">
                    <source src="senaryolu_dugun_cekimleri/dugun.mp4" type="video/mp4">
                </video>
                <div class="relative z-10 p-4">
                    <i class="fa-solid fa-camera-retro text-3xl text-yellow-500 mb-2 group-hover:scale-110 transition-transform shadow-black"></i>
                    <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest text-white drop-shadow-md">Senaryolu Düğün Çekimleri</h3>
                </div>
            </div>
            <div class="bg-white/5 backdrop-blur-md p-8 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group">
                <i class="fa-solid fa-ring text-3xl text-yellow-500 mb-4 group-hover:scale-110 transition-transform"></i>
                <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest">Evlenme Teklifi Çekimleri</h3>
            </div>
            <div class="bg-white/5 backdrop-blur-md p-0 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group overflow-hidden relative min-h-[140px] flex items-center justify-center">
                <video autoplay muted loop playsinline class="absolute inset-0 w-full h-full object-cover opacity-40 group-hover:opacity-70 transition-opacity">
                  <source src="oteller_insaat/insaat.mp4" type="video/mp4"> 
                </video>
                <div class="relative z-10 p-4">
                    <i class="fa-solid fa-hotel text-3xl text-yellow-500 mb-2 group-hover:scale-110 transition-transform shadow-black"></i>
                    <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest text-white drop-shadow-md">Oteller & İnşaat</h3>
                </div>
            </div>
            <div class="bg-white/5 backdrop-blur-md p-8 rounded-[35px] border border-white/10 text-center hover:border-yellow-500 transition-all hover:-translate-y-2 group">
                <i class="fa-solid fa-house-chimney text-3xl text-yellow-500 mb-4 group-hover:scale-110 transition-transform"></i>
                <h3 class="text-[10px] md:text-xs font-bold uppercase tracking-widest">Emlak Şirketleri</h3>
            </div>
        </div>
    </section>

    <!-- Galeri Section -->
    <section id="galeri" class="py-24 w-full max-w-7xl mx-auto px-6 content-layer">
        <h2 class="text-4xl md:text-5xl font-black italic uppercase text-center mb-16"><span class="text-yellow-500">Galeri</span></h2>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
            <div class="gallery-card"><img src="galeri/foto_1.jpg" alt="Foto 1"></div>
            <div class="gallery-card"><img src="galeri/foto_2.jpg" alt="Foto 2"></div>
            <div class="gallery-card"><img src="galeri/foto_3.jpg" alt="Foto 3"></div>
            <div class="gallery-card"><video autoplay muted loop playsinline><source src="galeri/bisiklet_hoverair.mp4" type="video/mp4"></video></div>
            <div class="gallery-card"><video autoplay muted loop playsinline><source src="galeri/hover_kayak.mp4" type="video/mp4"></video></div>
            <div class="gallery-card"><video autoplay muted loop playsinline><source src="galeri/girne_liman.mp4" type="video/mp4"></video></div>
            <div class="gallery-card"><video autoplay muted loop playsinline><source src="galeri/kibris.mp4" type="video/mp4"></video></div>
            <div class="gallery-card"><video autoplay muted loop playsinline><source src="galeri/manzara.mp4" type="video/mp4"></video></div>
        </div>
    </section>

    <!-- İletişim Section -->
    <section id="iletisim" class="py-24 w-full max-w-7xl mx-auto px-6 content-layer">
        <h2 class="text-4xl md:text-5xl font-black italic uppercase text-center mb-16">İletişim <span class="text-yellow-500">Bilgileri</span></h2>
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
            <div class="space-y-8 order-2 lg:order-1">
                <div class="flex items-start gap-6 group">
                    <div class="w-14 h-14 rounded-2xl bg-yellow-500/10 border border-yellow-500/20 flex items-center justify-center shrink-0 group-hover:bg-yellow-500 transition-colors">
                        <i class="fa-solid fa-phone text-2xl text-yellow-500 group-hover:text-black"></i>
                    </div>
                    <div>
                        <h4 class="text-xs font-bold uppercase text-gray-500 tracking-widest mb-1">Telefon</h4>
                        <a href="tel:+905391100777" class="text-xl md:text-2xl font-bold hover:text-yellow-500 transition-colors">+90 539 110 07 77</a>
                    </div>
                </div>
                <div class="flex items-start gap-6 group">
                    <div class="w-14 h-14 rounded-2xl bg-yellow-500/10 border border-yellow-500/20 flex items-center justify-center shrink-0 group-hover:bg-yellow-500 transition-colors">
                        <i class="fa-solid fa-envelope text-2xl text-yellow-500 group-hover:text-black"></i>
                    </div>
                    <div>
                        <h4 class="text-xs font-bold uppercase text-gray-500 tracking-widest mb-1">E-Posta</h4>
                        <a href="mailto:Skybeecyprus@gmail.com" class="text-xl md:text-2xl font-bold hover:text-yellow-500 transition-colors">Skybeecyprus@gmail.com</a>
                    </div>
                </div>
                <div class="flex items-start gap-6 group">
                    <div class="w-14 h-14 rounded-2xl bg-yellow-500/10 border border-yellow-500/20 flex items-center justify-center shrink-0 group-hover:bg-yellow-500 transition-colors">
                        <i class="fa-solid fa-location-dot text-2xl text-yellow-500 group-hover:text-black"></i>
                    </div>
                    <div>
                        <h4 class="text-xs font-bold uppercase text-gray-500 tracking-widest mb-1">Adres</h4>
                        <p class="text-lg text-gray-300 leading-relaxed uppercase italic font-medium">Ecevit Caddesi, Yukarı Girne Eski Türk Mahallesi, Vakıflar Çarşısı 2C Blok Kat 2 No:5 Girne</p>
                    </div>
                </div>
            </div>
            <div class="order-1 lg:order-2">
                <div class="map-container h-[400px] border border-white/10 shadow-2xl">
                    <iframe 
                        width="100%" 
                        height="100%" 
                        style="border:0;" 
                        allowfullscreen="" 
                        loading="lazy" 
                        referrerpolicy="no-referrer-when-downgrade"
                        src="https://www.google.com/maps?q=35.334863,33.318356&hl=tr&z=17&output=embed">
                    </iframe>
                </div>
            </div>
        </div>
    </section>

    <!-- Hakkımızda Modal -->
    <div id="about-modal" class="fixed inset-0 bg-black/98 backdrop-blur-3xl z-[2000] hidden overflow-y-auto p-6">
        <div class="max-w-4xl mx-auto my-12 bg-zinc-900 rounded-[60px] border-t-8 border-yellow-500 p-10 md:p-16 relative shadow-2xl">
            <button onclick="closeAbout()" class="absolute top-8 right-10 text-5xl text-yellow-500 hover:rotate-90 transition-transform">×</button>
            <h2 class="text-4xl font-black italic uppercase text-yellow-500 mb-8">Hakkımızda - Skybee</h2>
            <div class="text-gray-300 text-lg leading-relaxed space-y-6">
                <p><strong>Skybee</strong>, üst segment drone teknolojileri ve yaratıcı prodüksiyon gücünü bir araya getirerek, markalara ve bireylere yüksek standartlarda görsel deneyimler sunan seçkin bir medya üretim markasıdır. Her projede yalnızca bir çekim değil; algı, prestij ve etki inşa etmeyi hedefleriz.</p>
                <p>Hizmet verdiğimiz alanlar geniştir ancak yaklaşımımız nettir: sıradan olanı değil, fark yaratanı üretmek. Futbol kulüplerinin profesyonel maç çekimleri, siyasi organizasyonların üst düzey toplantıları, üniversite ve belediyelerin kurumsal tanıtım projeleri, otel, inşaat ve emlak sektörüne yönelik prestij odaklı içerikler; Skybee’nin kurumsal çözümlerinden yalnızca bir kısmıdır.</p>
                <p>Bununla birlikte; kişiye özel senaryolu araç çekimleri, motor kulübü prodüksiyonları, düğün ve evlenme teklifi gibi özel anları sinematik bir dille yeniden kurguladığımız projelerle, bireysel müşterilerimize de ayrıcalıklı bir deneyim sunarız. Tüm süreçlerde alanında uzman ekipler ve iş birlikleriyle çalışarak, kusursuz bir sonuç hedefleriz.</p>
                <p>Skybee, standart paketler sunan bir yapıdan ziyade; her müşterisine özel, sınırlı ve nitelikli projeler üretmeyi tercih eder. Bu yaklaşım, hem kaliteyi hem de ortaya çıkan işin değerini korumamızı sağlar.</p>
                <p>Eğer siz de sıradanın ötesine geçen, markanızı veya hikâyenizi üst seviyeye taşıyacak bir prodüksiyon arıyorsanız, detayları konuşmak için bizimle iletişime geçin.</p>
            </div>
        </div>
    </div>

    <footer class="py-12 border-t border-white/5 text-center content-layer">
        <p class="text-gray-500 text-sm font-bold tracking-widest uppercase">© 2024 SKYBEE MEDIA | PRESTIGE DRONE SOLUTIONS</p>
    </footer>

    <script>
        function openAbout() { document.getElementById('about-modal').classList.remove('hidden'); document.body.style.overflow = 'hidden'; }
        function closeAbout() { document.getElementById('about-modal').classList.add('hidden'); document.body.style.overflow = 'auto'; }
    </script>
</body>
</html>
