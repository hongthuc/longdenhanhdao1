<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lồng Đèn Hạnh Đào - Xưởng Sản Xuất Đèn Lồng Hội An | longdenhanhdao.com</title>
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
  <!-- Google Fonts: Inter & Playfair Display (Chuẩn phong cách truyền thống kết hợp hiện đại dễ dùng trên Flatsome) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet">

  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: {
              red: '#9E1B1B',      // Đỏ trầm truyền thống Hội An
              darkRed: '#7A1212',  // Đỏ đậm
              gold: '#D4AF37',     // Vàng đồng ấm
              lightGold: '#FDF8E7',// Nền kem vàng nhạt
              bg: '#FAF7F2'        // Nền trang kem sáng nhẹ chuẩn Flatsome
            }
          },
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
            serif: ['Playfair Display', 'serif']
          }
        }
      }
    }
  </script>

  <style>
    body {
      font-family: 'Inter', sans-serif;
      background-color: #FAF7F2;
      color: #262626;
      overflow-x: hidden;
    }

    /* Chuẩn khung Container 1200px của Flatsome */
    .flatsome-container {
      max-width: 1200px;
      margin-left: auto;
      margin-right: auto;
      padding-left: 15px;
      padding-right: 15px;
    }

    /* Tiêu đề Section kiểu Flatsome [title style="center"] */
    .section-title-container {
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 1.5rem;
    }
    .section-title-line {
      flex: 1;
      height: 2px;
      background-color: #e5dcd0;
    }
    .section-title-text {
      padding: 0 1.25rem;
      font-weight: 700;
      text-transform: uppercase;
      color: #9E1B1B;
      letter-spacing: 0.04em;
      text-align: center;
    }

    /* Hiệu ứng mượt cho ảnh sản phẩm chuẩn Flatsome image-zoom */
    .box-image {
      overflow: hidden;
      position: relative;
    }
    .box-image img {
      transition: transform 0.45s cubic-bezier(0.25, 0.46, 0.45, 0.94);
    }
    .product-box:hover .box-image img,
    .cat-box:hover .box-image img {
      transform: scale(1.06);
    }

    /* Hiệu ứng sóng lan tỏa cho nút liên hệ nổi */
    @keyframes pulse-ring {
      0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(220, 38, 38, 0.7); }
      70% { transform: scale(1); box-shadow: 0 0 0 12px rgba(220, 38, 38, 0); }
      100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(220, 38, 38, 0); }
    }
    @keyframes pulse-zalo {
      0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(0, 104, 255, 0.7); }
      70% { transform: scale(1); box-shadow: 0 0 0 12px rgba(0, 104, 255, 0); }
      100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(0, 104, 255, 0); }
    }
    .animate-pulse-red {
      animation: pulse-ring 2s infinite;
    }
    .animate-pulse-blue {
      animation: pulse-zalo 2s infinite;
    }

    /* Ẩn thanh cuộn ngang nhưng vẫn vuốt được */
    .no-scrollbar::-webkit-scrollbar {
      display: none;
    }
    .no-scrollbar {
      -ms-overflow-style: none;
      scrollbar-width: none;
    }

    /* Giới hạn 2 dòng tên sản phẩm để cột điện thoại luôn bằng nhau */
    .line-clamp-2 {
      display: -webkit-box;
      -webkit-line-clamp: 2;
      -webkit-box-orient: vertical;
      overflow: hidden;
    }
  </style>
</head>
<body class="antialiased selection:bg-brand-red selection:text-white">

  <!-- =========================================================
       1. FLATSOME TOP BAR (Chỉ hiển thị thông tin cửa hàng, không có thanh chỉnh sửa)
  ========================================================== -->
  <div class="bg-brand-darkRed text-amber-100 text-xs py-2 border-b border-red-900/60">
    <div class="flatsome-container flex flex-col sm:flex-row items-center justify-between gap-1.5">
      <div class="flex items-center gap-2 text-center sm:text-left">
        <i class="fa-solid fa-lantern text-brand-gold"></i>
        <span><strong>LỒNG ĐÈN HẠNH ĐÀO</strong> – Xưởng sản xuất đèn lồng Hội An sỉ & lẻ giá gốc | <strong>longdenhanhdao.com</strong></span>
      </div>
      <div class="flex flex-wrap items-center justify-center gap-4 text-xs">
        <a href="#ban-do-trang-chu" class="hover:text-white transition flex items-center gap-1">
          <i class="fa-solid fa-location-dot text-brand-gold"></i>
          <span>92 Nguyễn Du, Hội An, Đà Nẵng</span>
        </a>
        <span class="hidden md:inline text-red-400">|</span>
        <a href="tel:0796693304" class="hover:text-white transition flex items-center gap-1 font-semibold text-amber-200">
          <i class="fa-solid fa-phone-volume text-brand-gold"></i>
          <span>0796.693.304</span>
        </a>
      </div>
    </div>
  </div>

  <!-- =========================================================
       2. FLATSOME HEADER MAIN (Logo Fanpage + Tìm kiếm + Hotline)
  ========================================================== -->
  <header class="bg-white sticky top-0 z-40 shadow-sm border-b border-stone-200">
    <div class="flatsome-container py-3 md:py-4">
      <div class="flex items-center justify-between gap-3 md:gap-6">
        
        <!-- Nút mở Menu trên Điện thoại -->
        <button onclick="toggleMobileMenu()" aria-label="Mở danh mục" class="lg:hidden p-2.5 rounded-lg border border-stone-200 text-brand-red hover:bg-red-50 transition">
          <i class="fa-solid fa-bars text-xl"></i>
        </button>

        <!-- Logo Lồng Đèn Hạnh Đào (Lấy từ Fanpage ID 61577469388669 - Chuẩn mẫu Logo tròn nền đen chữ vàng Hạnh Đào) -->
        <a href="#" onclick="filterByCategory('all'); return false;" class="flex items-center gap-3 group shrink-0">
          <div class="relative w-14 h-14 md:w-16 md:h-16 rounded-full border-2 border-brand-gold overflow-hidden bg-[#0c0a09] flex items-center justify-center shadow-md shrink-0">
            <img 
              src="https://graph.facebook.com/v19.0/61577469388669/picture?type=large&width=500&height=500" 
              alt="Logo Cơ Sở Sản Xuất Lồng Đèn Hạnh Đào Hội An" 
              class="w-full h-full object-cover"
              onerror="this.style.display='none'; document.getElementById('fallback-logo-svg').style.display='flex';"
            >
            <!-- Logo chuẩn nguyên bản Fanpage Lồng Đèn Hạnh Đào (Nền đen viền vàng, đèn lồng & Chùa Cầu, chữ vàng nghệ thuật) -->
            <div id="fallback-logo-svg" style="display:none;" class="w-full h-full items-center justify-center bg-[#0c0a09]">
              <svg class="w-full h-full" viewBox="0 0 200 200" fill="none" xmlns="http://www.w3.org/2000/svg">
                <circle cx="100" cy="100" r="96" fill="#0F0C0A" stroke="#D4AF37" stroke-width="4"/>
                <circle cx="100" cy="100" r="91" stroke="#D4AF37" stroke-width="1" stroke-opacity="0.5"/>
                <!-- Biểu tượng đèn lồng đỉnh logo -->
                <ellipse cx="100" cy="27" rx="14" ry="12" stroke="#D4AF37" stroke-width="1.8"/>
                <ellipse cx="100" cy="27" rx="7" ry="12" stroke="#D4AF37" stroke-width="1.2"/>
                <line x1="86" y1="27" x2="114" y2="27" stroke="#D4AF37" stroke-width="1.2"/>
                <rect x="95" y="13" width="10" height="3" fill="#D4AF37"/>
                <rect x="95" y="39" width="10" height="3" fill="#D4AF37"/>
                <!-- Dòng chữ thương hiệu giống hệt Logo Fanpage -->
                <text x="100" y="56" text-anchor="middle" fill="#FFFFFF" font-size="10.5" font-family="Inter, sans-serif" font-weight="600" letter-spacing="0.8">CƠ SỞ SẢN XUẤT</text>
                <text x="96" y="84" text-anchor="middle" fill="#F3C65F" font-size="27" font-family="Playfair Display, serif" font-weight="700" font-style="italic">Lồng Đèn</text>
                <text x="94" y="112" text-anchor="middle" fill="#E5A93C" font-size="27" font-family="Playfair Display, serif" font-weight="700" font-style="italic">Hạnh Đào</text>
                <!-- Dấu đỏ Hội An -->
                <rect x="160" y="78" width="24" height="30" rx="4" fill="#9E1B1B" stroke="#D4AF37" stroke-width="1"/>
                <text x="172" y="91" text-anchor="middle" fill="#FFFFFF" font-size="8" font-family="Playfair Display, serif" font-style="italic">Hội</text>
                <text x="172" y="102" text-anchor="middle" fill="#FFFFFF" font-size="8" font-family="Playfair Display, serif" font-style="italic">An</text>
                <!-- Nền đỏ LỒNG ĐÈN TRE HỘI AN -->
                <rect x="38" y="120" width="124" height="15" rx="3" fill="#8B1515"/>
                <text x="100" y="131" text-anchor="middle" fill="#FDE68A" font-size="9.5" font-family="Inter, sans-serif" font-weight="700" letter-spacing="0.6">LỒNG ĐÈN TRE HỘI AN</text>
                <!-- Khung vàng SĐT Zalo -->
                <rect x="36" y="142" width="128" height="20" rx="10" fill="#E5B869"/>
                <text x="100" y="156" text-anchor="middle" fill="#5A0C0C" font-size="12" font-family="Inter, sans-serif" font-weight="800">0796 693 304</text>
                <!-- Địa chỉ -->
                <rect x="44" y="166" width="112" height="15" rx="7" fill="#4A1212" stroke="#D4AF37" stroke-width="0.7"/>
                <text x="100" y="176" text-anchor="middle" fill="#FDE68A" font-size="8" font-family="Inter, sans-serif" font-weight="600">92 Nguyễn Du, Hội An</text>
              </svg>
            </div>
          </div>
          <div>
            <span class="block font-serif font-bold text-lg md:text-2xl text-brand-red tracking-tight leading-none">
              LỒNG ĐÈN HẠNH ĐÀO
            </span>
            <span class="block text-[11px] md:text-xs text-stone-500 font-medium mt-1">
              Lồng đèn tre & lụa Hội An • longdenhanhdao.com
            </span>
          </div>
        </a>

        <!-- Thanh tìm kiếm sản phẩm (Chuẩn Flatsome Search Box) -->
        <div class="hidden md:flex flex-1 max-w-md mx-auto">
          <div class="relative w-full">
            <input 
              id="desktop-search" 
              type="text" 
              oninput="handleSearch(this.value)"
              placeholder="Tìm đèn lồng lụa, phi hoa 3D, đèn gỗ, đèn vẽ..." 
              class="w-full pl-4 pr-11 py-2.5 text-sm rounded-full border border-stone-300 focus:outline-none focus:border-brand-red bg-stone-50 focus:bg-white transition"
            >
            <button onclick="handleSearch(document.getElementById('desktop-search').value)" aria-label="Tìm kiếm" class="absolute right-1.5 top-1.5 bottom-1.5 px-3.5 bg-brand-red text-white rounded-full hover:bg-brand-darkRed transition">
              <i class="fa-solid fa-magnifying-glass text-xs"></i>
            </button>
          </div>
        </div>

        <!-- Cụm nút Hotline & Fanpage bên phải Header -->
        <div class="flex items-center gap-2.5 md:gap-3">
          <a href="tel:0796693304" class="hidden sm:flex items-center gap-2.5 px-3.5 py-2 rounded-xl bg-amber-50 border border-amber-200 hover:bg-amber-100 transition">
            <div class="w-8 h-8 rounded-full bg-brand-red text-white flex items-center justify-center shrink-0">
              <i class="fa-solid fa-phone text-xs"></i>
            </div>
            <div class="leading-tight">
              <span class="block text-[10px] uppercase tracking-wider text-stone-500 font-semibold">Hotline / Zalo Sỉ & Lẻ</span>
              <span class="block text-sm font-bold text-brand-red">0796.693.304</span>
            </div>
          </a>

          <a href="https://www.facebook.com/profile.php?id=61577469388669" target="_blank" rel="noopener noreferrer" class="px-3.5 py-2.5 rounded-xl bg-brand-red hover:bg-brand-darkRed text-white text-xs md:text-sm font-semibold flex items-center gap-2 shadow-sm transition">
            <i class="fa-brands fa-facebook-f"></i>
            <span class="hidden md:inline">Fanpage Hạnh Đào</span>
          </a>
        </div>

      </div>

      <!-- Thanh tìm kiếm trên Điện thoại -->
      <div class="mt-2.5 md:hidden">
        <div class="relative w-full">
          <input 
            id="mobile-search" 
            type="text" 
            oninput="handleSearch(this.value)"
            placeholder="Tìm mẫu đèn lồng Hội An..." 
            class="w-full pl-3.5 pr-10 py-2 text-sm rounded-lg border border-stone-300 bg-stone-50 focus:bg-white focus:outline-none focus:border-brand-red"
          >
          <button onclick="handleSearch(document.getElementById('mobile-search').value)" aria-label="Tìm kiếm" class="absolute right-2 top-1/2 -translate-y-1/2 text-brand-red p-1">
            <i class="fa-solid fa-magnifying-glass"></i>
          </button>
        </div>
      </div>
    </div>

    <!-- =========================================================
         3. THANH ĐIỀU HƯỚNG & MENU DANH MỤC TRÊN MÁY TÍNH (Tối ưu chuẩn Flatsome)
    ========================================================== -->
    <nav class="hidden lg:block bg-brand-red text-white border-t border-red-800">
      <div class="flatsome-container flex items-center justify-between">
        
        <!-- Nút Dropdown Danh Mục Sản Phẩm kiểu Flatsome Mega Menu -->
        <div class="relative group">
          <button class="bg-brand-darkRed px-5 py-3.5 font-bold text-xs uppercase tracking-wider flex items-center gap-3 min-w-[250px] justify-between border-x border-red-900/60">
            <span class="flex items-center gap-2.5">
              <i class="fa-solid fa-list-ul text-brand-gold"></i>
              <span>DANH MỤC SẢN PHẨM</span>
            </span>
            <i class="fa-solid fa-chevron-down text-[10px] text-amber-200 group-hover:rotate-180 transition-transform"></i>
          </button>

          <!-- Danh sách xổ xuống lấy từ denlongvn.com -->
          <div class="absolute left-0 top-full w-[270px] bg-white text-stone-800 shadow-xl rounded-b-xl border border-stone-200 py-2 hidden group-hover:block z-50">
            <a href="#san-pham" onclick="filterByCategory('all')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red font-medium border-b border-stone-100 transition">
              <span><i class="fa-solid fa-border-all w-5 text-brand-red"></i> Tất cả sản phẩm</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('den-long-hoi-an')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng Hội An (Lụa tơ tằm)</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('phi-hoa-3d')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng phi hoa 3D</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('vai-hoa-gam-truc')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng vải hoa & Gấm trúc</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('xo-voan-tho-cam')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng Xô Voan & Thổ cẩm</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('theu-tay-ve-hoa-tiet')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng thêu tay & Vẽ họa tiết</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('in-logo-su-kien')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng in Logo & Sự kiện</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('den-go-hoa-sen')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn gỗ lục giác & Đèn hoa sen</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('den-long-nhat')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng kiểu Nhật</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
          </div>
        </div>

        <!-- Menu ngang trên máy tính -->
        <ul class="flex items-center gap-1 text-xs font-semibold uppercase tracking-wide">
          <li><a href="#" onclick="filterByCategory('all'); return false;" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Trang chủ</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('den-long-hoi-an')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Đèn lồng Hội An</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('phi-hoa-3d')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Phi hoa 3D</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('vai-hoa-gam-truc')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Vải hoa & Gấm</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('xo-voan-tho-cam')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Xô Voan & Thổ Cẩm</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('theu-tay-ve-hoa-tiet')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Đèn vẽ & Thêu tay</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('den-go-hoa-sen')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Đèn Gỗ & Hoa Sen</a></li>
          <li><a href="#ban-do-trang-chu" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition text-amber-200"><i class="fa-solid fa-map-location-dot mr-1"></i>Bản đồ & Liên hệ</a></li>
        </ul>

      </div>
    </nav>
  </header>

  <!-- =========================================================
       MENU TRƯỢT MOBILE (Off-Canvas Menu chuẩn Flatsome)
  ========================================================== -->
  <div id="mobile-menu-backdrop" onclick="toggleMobileMenu()" class="fixed inset-0 bg-black/60 z-50 hidden transition-opacity"></div>
  <aside id="mobile-menu-drawer" class="fixed top-0 left-0 bottom-0 w-[290px] bg-white z-50 -translate-x-full transition-transform duration-300 flex flex-col shadow-2xl">
    <div class="p-4 bg-brand-red text-white flex items-center justify-between">
      <div>
        <div class="font-serif font-bold text-base">LỒNG ĐÈN HẠNH ĐÀO</div>
        <div class="text-xs text-amber-200">longdenhanhdao.com</div>
      </div>
      <button onclick="toggleMobileMenu()" aria-label="Đóng menu" class="w-8 h-8 rounded-full bg-white/10 flex items-center justify-center text-white">
        <i class="fa-solid fa-xmark"></i>
      </button>
    </div>
    <div class="p-3 bg-amber-50 border-b border-amber-200 text-xs text-stone-700">
      <div class="font-semibold text-brand-red">Danh mục sản phẩm (Chuẩn mẫu)</div>
    </div>
    <div class="flex-1 overflow-y-auto divide-y divide-stone-100 text-sm">
      <a href="#san-pham" onclick="filterByCategory('all'); toggleMobileMenu();" class="block px-4 py-3 font-semibold text-brand-red hover:bg-red-50">Tất cả sản phẩm</a>
      <a href="#san-pham" onclick="filterByCategory('den-long-hoi-an'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">1. Đèn lồng Hội An (Lụa tơ tằm)</a>
      <a href="#san-pham" onclick="filterByCategory('phi-hoa-3d'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">2. Đèn lồng phi hoa 3D</a>
      <a href="#san-pham" onclick="filterByCategory('vai-hoa-gam-truc'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">3. Đèn lồng vải hoa & Gấm trúc</a>
      <a href="#san-pham" onclick="filterByCategory('xo-voan-tho-cam'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">4. Đèn lồng Xô Voan & Thổ cẩm</a>
      <a href="#san-pham" onclick="filterByCategory('theu-tay-ve-hoa-tiet'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">5. Đèn lồng thêu tay & Vẽ họa tiết</a>
      <a href="#san-pham" onclick="filterByCategory('in-logo-su-kien'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">6. Đèn lồng in Logo & Sự kiện</a>
      <a href="#san-pham" onclick="filterByCategory('den-go-hoa-sen'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">7. Đèn gỗ lục giác & Đèn hoa sen</a>
      <a href="#san-pham" onclick="filterByCategory('den-long-nhat'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">8. Đèn lồng kiểu Nhật</a>
      <a href="#ban-do-trang-chu" onclick="toggleMobileMenu();" class="block px-4 py-3 font-semibold text-stone-800 hover:bg-red-50">
        <i class="fa-solid fa-location-dot text-brand-red mr-1.5"></i> Bản đồ: 92 Nguyễn Du, Hội An
      </a>
    </div>
    <div class="p-4 bg-stone-50 border-t border-stone-200 text-xs space-y-1.5">
      <div><strong>Địa chỉ:</strong> 92 Nguyễn Du, Hội An, Đà Nẵng</div>
      <div><strong>Hotline/Zalo:</strong> <a href="tel:0796693304" class="text-brand-red font-bold">0796.693.304</a></div>
    </div>
  </aside>

  <!-- =========================================================
       4. SLIDER 2 ẢNH BANNER TỰ TRƯỢT (Flatsome [ux_slider] + [ux_banner])
  ========================================================== -->
  <section class="py-3 md:py-5">
    <div class="flatsome-container">
      <div class="relative rounded-2xl overflow-hidden shadow-md bg-stone-900 h-[270px] sm:h-[360px] md:h-[440px]" id="hero-slider">
        
        <!-- SLIDE 1: Xưởng Sản Xuất Lồng Đèn Hạnh Đào -->
        <div class="hero-slide absolute inset-0 transition-opacity duration-700 opacity-100 z-10">
          <img 
            src="https://images.pexels.com/photos/31476945/pexels-photo-31476945.jpeg?auto=compress&cs=tinysrgb&w=1600" 
            alt="Xưởng Lồng Đèn Hạnh Đào Hội An" 
            class="w-full h-full object-cover object-center"
            onerror="this.src='https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An,_Vietnam_(25708206924).jpg?width=1200'"
          >
          <div class="absolute inset-0 bg-gradient-to-r from-black/80 via-black/55 to-black/25 flex items-center">
            <div class="px-6 sm:px-12 md:px-16 max-w-2xl text-white space-y-2.5 md:space-y-4">
              <p class="text-amber-300 text-xs md:text-sm font-semibold uppercase tracking-widest">
                Cơ Sở Sản Xuất Lồng Đèn Tre & Lụa Hội An • longdenhanhdao.com
              </p>
              <h1 class="font-serif text-2xl sm:text-4xl md:text-5xl font-bold leading-tight text-white">
                Lồng Đèn Hạnh Đào <br><span class="text-amber-300">Sản Xuất Trực Tiếp Tại Xưởng</span>
              </h1>
              <p class="text-xs sm:text-sm md:text-base text-stone-200 leading-relaxed">
                Chuyên sỉ & lẻ đèn lồng tre đan tự nhiên, đèn lồng lụa Hội An, phi hoa 3D, đèn vẽ tay & in logo theo yêu cầu. Thắp sáng không gian Việt.
              </p>
              <div class="pt-1 flex flex-wrap items-center gap-3">
                <a href="#san-pham" class="px-5 py-2.5 rounded-full bg-brand-red hover:bg-brand-darkRed text-white font-semibold text-xs md:text-sm border border-amber-300/40 transition shadow">
                  Xem mẫu đèn lồng
                </a>
                <a href="tel:0796693304" class="px-5 py-2.5 rounded-full bg-amber-400 hover:bg-amber-300 text-stone-900 font-bold text-xs md:text-sm transition shadow">
                  <i class="fa-solid fa-phone mr-1.5"></i> 0796.693.304
                </a>
              </div>
            </div>
          </div>
        </div>

        <!-- SLIDE 2: Đa dạng chất liệu Tre tự nhiên, Lụa tơ tằm, Phi hoa 3D & Vẽ tay -->
        <div class="hero-slide absolute inset-0 transition-opacity duration-700 opacity-0 z-0">
          <img 
            src="https://images.pexels.com/photos/38914416/pexels-photo-38914416.jpeg?auto=compress&cs=tinysrgb&w=1600" 
            alt="Đèn lồng lụa tơ tằm, đèn lồng tre và phi hoa 3D Hội An" 
            class="w-full h-full object-cover object-center"
            onerror="this.src='https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_1.jpg?width=1200'"
          >
          <div class="absolute inset-0 bg-gradient-to-r from-red-950/85 via-stone-900/60 to-transparent flex items-center">
            <div class="px-6 sm:px-12 md:px-16 max-w-2xl text-white space-y-2.5 md:space-y-4">
              <p class="text-amber-300 text-xs md:text-sm font-semibold uppercase tracking-widest">
                92 Nguyễn Du, Hội An, Đà Nẵng
              </p>
              <h2 class="font-serif text-2xl sm:text-4xl md:text-5xl font-bold leading-tight text-white">
                Lồng Đèn Tre Tự Nhiên <br><span class="text-amber-300">& Đèn Lồng Lụa Hội An</span>
              </h2>
              <p class="text-xs sm:text-sm md:text-base text-stone-200 leading-relaxed">
                Chất liệu tre tự nhiên xử lý tỉ mỉ, bền đẹp thân thiện – Nhận gia công sỉ & lẻ toàn quốc giá tốt nhất tại xưởng.
              </p>
              <div class="pt-1 flex flex-wrap items-center gap-3">
                <a href="https://zalo.me/0796693304" target="_blank" rel="noopener noreferrer" class="px-5 py-2.5 rounded-full bg-amber-400 hover:bg-amber-300 text-stone-900 font-bold text-xs md:text-sm transition shadow">
                  Nhận báo giá sỉ qua Zalo
                </a>
                <a href="#ban-do-trang-chu" class="px-5 py-2.5 rounded-full bg-white/15 hover:bg-white/25 backdrop-blur text-white font-semibold text-xs md:text-sm border border-white/30 transition">
                  Chỉ đường đến xưởng
                </a>
              </div>
            </div>
          </div>
        </div>

        <!-- Nút điều hướng Trái / Phải của Banner -->
        <button onclick="changeSlide(-1)" aria-label="Banner trước" class="absolute left-3 top-1/2 -translate-y-1/2 z-20 w-9 h-9 md:w-10 md:h-10 rounded-full bg-black/40 hover:bg-brand-red text-white flex items-center justify-center transition">
          <i class="fa-solid fa-chevron-left text-sm"></i>
        </button>
        <button onclick="changeSlide(1)" aria-label="Banner tiếp" class="absolute right-3 top-1/2 -translate-y-1/2 z-20 w-9 h-9 md:w-10 md:h-10 rounded-full bg-black/40 hover:bg-brand-red text-white flex items-center justify-center transition">
          <i class="fa-solid fa-chevron-right text-sm"></i>
        </button>

        <!-- Dấu chấm chuyển Slide -->
        <div class="absolute bottom-3.5 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
          <button onclick="goToSlide(0)" id="dot-0" aria-label="Banner 1" class="w-7 h-2 rounded-full bg-amber-400 transition-all"></button>
          <button onclick="goToSlide(1)" id="dot-1" aria-label="Banner 2" class="w-2.5 h-2 rounded-full bg-white/60 transition-all"></button>
        </div>

      </div>
    </div>
  </section>

  <!-- =========================================================
       5. DANH MỤC SẢN PHẨM (Tối ưu hiển thị đẹp trên cả Máy tính & Điện thoại)
          Lấy từ danh mục web mẫu denlongvn.com
  ========================================================== -->
  <section class="py-5 md:py-8">
    <div class="flatsome-container">
      
      <div class="section-title-container">
        <div class="section-title-line"></div>
        <h2 class="section-title-text text-base md:text-xl font-serif">DANH MỤC ĐÈN LỒNG HỘI AN</h2>
        <div class="section-title-line"></div>
      </div>

      <!-- Bố cục: 4 cột gọn đẹp trên điện thoại (2 hàng x 4) và 8 cột sang trọng trên máy tính -->
      <div class="grid grid-cols-4 lg:grid-cols-8 gap-2.5 sm:gap-4" id="category-visual-grid">
        <!-- Render động từ danh sách danh mục chuẩn denlongvn.com -->
      </div>

      <!-- Thanh nút lọc nhanh hỗ trợ UX Builder -->
      <div class="mt-5 flex items-center justify-start md:justify-center gap-2 overflow-x-auto no-scrollbar pb-1" id="category-pills">
        <!-- Render động các pill danh mục -->
      </div>

    </div>
  </section>

  <!-- =========================================================
       6. DANH SÁCH SẢN PHẨM THEO DANH MỤC (Chuẩn Flatsome Section, 2 cột trên Điện thoại, 4 cột trên Máy tính)
          LƯU Ý: KHÔNG ĐỂ CÁC NHÃN DÁN (SALE/HOT/NEW) Ở TRANG CHỦ
  ========================================================== -->
  <main id="san-pham" class="py-4 md:py-6 space-y-10">
    <div class="flatsome-container" id="product-sections-wrapper">
      <!-- Render các Section sản phẩm theo đúng cấu trúc Row/Col của Flatsome -->
    </div>
  </main>

  <!-- =========================================================
       7. ĐẶC ĐIỂM XƯỞNG LỒNG ĐÈN HẠNH ĐÀO (Flatsome 4-Col Featured Box)
  ========================================================== -->
  <section class="py-8 bg-white border-y border-stone-200">
    <div class="flatsome-container">
      <div class="grid grid-cols-2 lg:grid-cols-4 gap-4 md:gap-6">
        <div class="p-4 rounded-xl bg-brand-bg border border-stone-200/80 text-center space-y-1.5">
          <div class="w-11 h-11 mx-auto rounded-full bg-red-50 text-brand-red flex items-center justify-center text-lg">
            <i class="fa-solid fa-hammer"></i>
          </div>
          <h3 class="font-bold text-sm md:text-base text-stone-800">Giá Gốc Tại Xưởng</h3>
          <p class="text-xs text-stone-600">Sản xuất trực tiếp tại 92 Nguyễn Du, Hội An không qua trung gian.</p>
        </div>

        <div class="p-4 rounded-xl bg-brand-bg border border-stone-200/80 text-center space-y-1.5">
          <div class="w-11 h-11 mx-auto rounded-full bg-red-50 text-brand-red flex items-center justify-center text-lg">
            <i class="fa-solid fa-palette"></i>
          </div>
          <h3 class="font-bold text-sm md:text-base text-stone-800">Nhận Làm Theo Yêu Cầu</h3>
          <p class="text-xs text-stone-600">Đặt kích thước riêng, vẽ tay, thêu hoa văn và in logo thương hiệu.</p>
        </div>

        <div class="p-4 rounded-xl bg-brand-bg border border-stone-200/80 text-center space-y-1.5">
          <div class="w-11 h-11 mx-auto rounded-full bg-red-50 text-brand-red flex items-center justify-center text-lg">
            <i class="fa-solid fa-medal"></i>
          </div>
          <h3 class="font-bold text-sm md:text-base text-stone-800">Tre Xử Lý & Lụa Cao Cấp</h3>
          <p class="text-xs text-stone-600">Khung tre già xử lý chống mối mọt, bọc lụa tơ tằm, gấm, phi hoa 3D bền màu.</p>
        </div>

        <div class="p-4 rounded-xl bg-brand-bg border border-stone-200/80 text-center space-y-1.5">
          <div class="w-11 h-11 mx-auto rounded-full bg-red-50 text-brand-red flex items-center justify-center text-lg">
            <i class="fa-solid fa-truck-fast"></i>
          </div>
          <h3 class="font-bold text-sm md:text-base text-stone-800">Giao Hàng Toàn Quốc</h3>
          <p class="text-xs text-stone-600">Đóng gói xếp gọn an toàn, vận chuyển nhanh chóng khắp 63 tỉnh thành.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- =========================================================
       8. BẢN ĐỒ GOOGLE MAPS NGOÀI TRANG CHỦ & THÔNG TIN LIÊN HỆ
          Địa chỉ: 92 Nguyễn Du, Hội An, Đà Nẵng | SĐT: 0796.693.304
  ========================================================== -->
  <section id="ban-do-trang-chu" class="py-8 md:py-12">
    <div class="flatsome-container">
      
      <div class="section-title-container">
        <div class="section-title-line"></div>
        <h2 class="section-title-text text-base md:text-xl font-serif">BẢN ĐỒ ĐẾN XƯỞNG LỒNG ĐÈN HẠNH ĐÀO</h2>
        <div class="section-title-line"></div>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 bg-white p-4 sm:p-6 rounded-2xl shadow-sm border border-stone-200">
        
        <!-- Cột trái: Thông tin xưởng & Đặt hàng nhanh (5 cột) -->
        <div class="lg:col-span-5 flex flex-col justify-between space-y-5">
          <div class="space-y-4">
            <div>
              <h3 class="font-serif font-bold text-xl text-brand-red">Cơ Sở Sản Xuất Lồng Đèn Hạnh Đào</h3>
              <p class="text-xs text-stone-500 mt-0.5">Website chính thức: <strong>longdenhanhdao.com</strong></p>
            </div>

            <div class="space-y-3 text-sm text-stone-700">
              <div class="flex items-start gap-3">
                <div class="w-8 h-8 rounded-lg bg-red-50 text-brand-red flex items-center justify-center shrink-0 mt-0.5">
                  <i class="fa-solid fa-location-dot"></i>
                </div>
                <div>
                  <span class="font-semibold text-stone-900 block">Địa chỉ xưởng & cửa hàng:</span>
                  <span>92 Nguyễn Du, Hội An, Đà Nẵng</span>
                </div>
              </div>

              <div class="flex items-start gap-3">
                <div class="w-8 h-8 rounded-lg bg-red-50 text-brand-red flex items-center justify-center shrink-0 mt-0.5">
                  <i class="fa-solid fa-phone-volume"></i>
                </div>
                <div>
                  <span class="font-semibold text-stone-900 block">Điện thoại / Zalo tư vấn sỉ & lẻ:</span>
                  <a href="tel:0796693304" class="text-brand-red font-bold text-base hover:underline">0796.693.304</a>
                </div>
              </div>

              <div class="flex items-start gap-3">
                <div class="w-8 h-8 rounded-lg bg-red-50 text-brand-red flex items-center justify-center shrink-0 mt-0.5">
                  <i class="fa-brands fa-facebook"></i>
                </div>
                <div>
                  <span class="font-semibold text-stone-900 block">Fanpage Facebook:</span>
                  <a href="https://www.facebook.com/profile.php?id=61577469388669" target="_blank" rel="noopener noreferrer" class="text-blue-600 hover:underline break-all">
                    facebook.com/profile.php?id=61577469388669
                  </a>
                </div>
              </div>
            </div>
          </div>

          <!-- Form gửi yêu cầu báo giá sỉ/lẻ nhanh -->
          <form onsubmit="submitQuickQuote(event)" class="p-4 rounded-xl bg-stone-50 border border-stone-200 space-y-3">
            <div class="font-bold text-sm text-stone-800">Nhận báo giá sỉ / Đặt đèn theo yêu cầu</div>
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-2.5">
              <input type="text" id="quote-name" required placeholder="Tên của bạn *" class="w-full px-3 py-2 text-xs rounded-lg border border-stone-300 bg-white focus:outline-none focus:border-brand-red">
              <input type="tel" id="quote-phone" required placeholder="Số điện thoại / Zalo *" class="w-full px-3 py-2 text-xs rounded-lg border border-stone-300 bg-white focus:outline-none focus:border-brand-red">
            </div>
            <input type="text" id="quote-note" placeholder="Loại đèn & số lượng cần báo giá (VD: 50 đèn lụa 30cm)..." class="w-full px-3 py-2 text-xs rounded-lg border border-stone-300 bg-white focus:outline-none focus:border-brand-red">
            <button type="submit" class="w-full py-2.5 rounded-lg bg-brand-red hover:bg-brand-darkRed text-white font-semibold text-xs uppercase tracking-wider transition">
              Gửi yêu cầu báo giá
            </button>
            <p id="quote-success" class="hidden text-xs text-emerald-700 font-medium text-center pt-1"></p>
          </form>
        </div>

        <!-- Cột phải: Bản đồ Google Maps hiển thị trực tiếp ngoài trang chủ (7 cột) -->
        <div class="lg:col-span-7 flex flex-col space-y-2.5">
          <div class="relative w-full h-[320px] sm:h-[380px] rounded-xl overflow-hidden border border-stone-300 bg-stone-100 shadow-inner">
            <iframe 
              title="Bản đồ Google Map Lồng Đèn Hạnh Đào 92 Nguyễn Du, Hội An"
              src="https://maps.google.com/maps?q=92%20Nguy%E1%BB%85n%20Du,%20H%E1%BB%99i%20An&t=&z=16&ie=UTF8&iwloc=&output=embed" 
              class="w-full h-full border-0" 
              allowfullscreen="" 
              loading="lazy" 
              referrerpolicy="no-referrer-when-downgrade">
            </iframe>
          </div>
          <div class="flex flex-wrap items-center justify-between gap-2 text-xs text-stone-600 px-1">
            <span><i class="fa-solid fa-map-pin text-brand-red mr-1"></i> <strong>Vị trí trên bản đồ:</strong> 92 Nguyễn Du, Hội An, Đà Nẵng</span>
            <a 
              href="https://www.google.com/maps/search/?api=1&query=92+Nguyen+Du+Hoi+An" 
              target="_blank" 
              rel="noopener noreferrer" 
              class="inline-flex items-center gap-1.5 font-semibold text-brand-red hover:underline"
            >
              <span>Mở trên ứng dụng Google Maps</span>
              <i class="fa-solid fa-arrow-up-right-from-square text-[10px]"></i>
            </a>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- =========================================================
       9. FOOTER CHUẨN FLATSOME (4 Cột đơn giản, dễ chỉnh sửa trên UX Builder)
  ========================================================== -->
  <footer class="bg-stone-900 text-stone-300 pt-10 pb-6 border-t-4 border-brand-red">
    <div class="flatsome-container">
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 pb-8 border-b border-stone-800 text-sm">
        
        <!-- Cột 1 -->
        <div class="space-y-3">
          <div class="font-serif font-bold text-lg text-amber-400">LỒNG ĐÈN HẠNH ĐÀO</div>
          <p class="text-xs text-stone-400 leading-relaxed">
            Xưởng chuyên sản xuất và cung cấp sỉ & lẻ các loại đèn lồng Hội An truyền thống, đèn lồng lụa tơ tằm, phi hoa 3D, gấm trúc, đèn gỗ lục giác, đèn hoa sen trang trí phòng, quán cafe, nhà hàng và sự kiện.
          </p>
          <div class="text-xs text-amber-300 font-medium">Website: longdenhanhdao.com</div>
        </div>

        <!-- Cột 2 -->
        <div class="space-y-3">
          <div class="font-bold text-white uppercase tracking-wider text-xs">Danh Mục Sản Phẩm</div>
          <ul class="space-y-2 text-xs text-stone-400">
            <li><a href="#san-pham" onclick="filterByCategory('den-long-hoi-an')" class="hover:text-amber-300 transition">• Đèn lồng Hội An lụa tơ tằm</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('phi-hoa-3d')" class="hover:text-amber-300 transition">• Đèn lồng phi hoa 3D</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('vai-hoa-gam-truc')" class="hover:text-amber-300 transition">• Đèn lồng vải hoa & Gấm trúc</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('xo-voan-tho-cam')" class="hover:text-amber-300 transition">• Đèn lồng Xô Voan & Thổ cẩm</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('theu-tay-ve-hoa-tiet')" class="hover:text-amber-300 transition">• Đèn lồng thêu tay & Vẽ họa tiết</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('den-go-hoa-sen')" class="hover:text-amber-300 transition">• Đèn gỗ & Đèn hoa sen</a></li>
          </ul>
        </div>

        <!-- Cột 3 -->
        <div class="space-y-3">
          <div class="font-bold text-white uppercase tracking-wider text-xs">Hỗ Trợ Khách Hàng</div>
          <ul class="space-y-2 text-xs text-stone-400">
            <li>• Tư vấn chọn kích thước đèn (20cm - 80cm)</li>
            <li>• Chính sách chiết khấu đơn hàng sỉ & dự án</li>
            <li>• Hướng dẫn bung mở và bảo quản đèn lồng</li>
            <li>• Ship COD toàn quốc & gửi xe đi các tỉnh</li>
          </ul>
        </div>

        <!-- Cột 4 -->
        <div class="space-y-3">
          <div class="font-bold text-white uppercase tracking-wider text-xs">Thông Tin Liên Hệ</div>
          <ul class="space-y-2 text-xs text-stone-300">
            <li><i class="fa-solid fa-location-dot text-amber-400 w-4"></i> 92 Nguyễn Du, Hội An, Đà Nẵng</li>
            <li><i class="fa-solid fa-phone text-amber-400 w-4"></i> Hotline/Zalo: <a href="tel:0796693304" class="font-bold text-amber-300">0796.693.304</a></li>
            <li><i class="fa-solid fa-globe text-amber-400 w-4"></i> Website: longdenhanhdao.com</li>
            <li>
              <a href="https://www.facebook.com/profile.php?id=61577469388669" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-1.5 mt-1 px-3 py-1.5 rounded bg-blue-600 hover:bg-blue-500 text-white text-xs font-medium transition">
                <i class="fa-brands fa-facebook-f"></i> Kết nối Fanpage Hạnh Đào
              </a>
            </li>
          </ul>
        </div>

      </div>

      <div class="pt-5 flex flex-col sm:flex-row items-center justify-between gap-2 text-xs text-stone-500">
        <div>© Bản quyền thuộc về <strong>Lồng Đèn Hạnh Đào (longdenhanhdao.com)</strong> – 92 Nguyễn Du, Hội An, Đà Nẵng.</div>
        <div>Thiết kế giao diện chuẩn Flatsome</div>
      </div>
    </div>
  </footer>

  <!-- =========================================================
       10. CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE)
  ========================================================== -->
  <div class="fixed bottom-4 left-4 z-50 flex flex-col gap-3">
    
    <!-- Nút Facebook Fanpage nổi bật -->
    <a 
      href="https://www.facebook.com/profile.php?id=61577469388669" 
      target="_blank" 
      rel="noopener noreferrer"
      title="Nhắn tin Facebook Lồng Đèn Hạnh Đào"
      class="flex items-center gap-2.5 bg-[#1877F2] hover:bg-[#1464cc] text-white px-3.5 py-2.5 rounded-full shadow-lg transition transform hover:-translate-y-0.5"
    >
      <span class="w-7 h-7 rounded-full bg-white text-[#1877F2] flex items-center justify-center font-bold text-base shrink-0">
        <i class="fa-brands fa-facebook-f"></i>
      </span>
      <span class="text-xs font-bold pr-1">Facebook</span>
    </a>

    <!-- Nút Chat Zalo nổi bật -->
    <a 
      href="https://zalo.me/0796693304" 
      target="_blank" 
      rel="noopener noreferrer"
      title="Chat Zalo 0796.693.304"
      class="flex items-center gap-2.5 bg-[#0068FF] hover:bg-[#0056d6] text-white px-3.5 py-2.5 rounded-full shadow-lg animate-pulse-blue transition transform hover:-translate-y-0.5"
    >
      <span class="w-7 h-7 rounded-full bg-white text-[#0068FF] flex items-center justify-center font-extrabold text-[11px] tracking-tighter shrink-0">
        Zalo
      </span>
      <span class="text-xs font-bold pr-1">Zalo: 0796.693.304</span>
    </a>

    <!-- Nút Gọi Hotline nổi bật -->
    <a 
      href="tel:0796693304" 
      title="Gọi ngay 0796.693.304"
      class="flex items-center gap-2.5 bg-red-600 hover:bg-red-700 text-white px-3.5 py-2.5 rounded-full shadow-lg animate-pulse-red transition transform hover:-translate-y-0.5"
    >
      <span class="w-7 h-7 rounded-full bg-white text-red-600 flex items-center justify-center text-sm shrink-0">
        <i class="fa-solid fa-phone-volume"></i>
      </span>
      <span class="text-xs font-bold pr-1">0796.693.304</span>
    </a>

  </div>

  <!-- =========================================================
       MODAL CHI TIẾT SẢN PHẨM & ĐẶT HÀNG NHANH
  ========================================================== -->
  <div id="product-modal" class="fixed inset-0 bg-black/60 z-50 hidden items-center justify-center p-4">
    <div class="bg-white rounded-2xl max-w-lg w-full overflow-hidden shadow-2xl border border-stone-200 relative">
      <button onclick="closeProductModal()" aria-label="Đóng" class="absolute top-3 right-3 w-8 h-8 rounded-full bg-stone-100 hover:bg-stone-200 text-stone-700 flex items-center justify-center z-10">
        <i class="fa-solid fa-xmark"></i>
      </button>
      <div class="grid grid-cols-1 sm:grid-cols-12">
        <div class="sm:col-span-5 bg-stone-100">
          <img id="modal-img" src="" alt="" class="w-full h-56 sm:h-full object-cover">
        </div>
        <div class="sm:col-span-7 p-5 space-y-3">
          <div id="modal-cat" class="text-xs text-stone-500 font-medium"></div>
          <h3 id="modal-title" class="font-serif font-bold text-lg text-stone-900"></h3>
          <div id="modal-price" class="text-base font-bold text-brand-red"></div>
          <p id="modal-desc" class="text-xs text-stone-600 leading-relaxed"></p>
          <div class="text-xs text-stone-700 space-y-1 pt-1 border-t border-stone-100">
            <div><strong>Kích thước phổ biến:</strong> 20cm, 30cm, 35cm, 40cm, 45cm, 60cm</div>
            <div><strong>Kiểu dáng:</strong> Tròn, Tỏi, Na, Dù, Kim cương, Bánh ú, Trụ</div>
          </div>
          <div class="pt-2 flex flex-col gap-2">
            <a href="https://zalo.me/0796693304" target="_blank" rel="noopener noreferrer" class="w-full py-2.5 rounded-lg bg-[#0068FF] hover:bg-blue-700 text-white font-semibold text-xs text-center transition">
              Nhắn Zalo đặt mẫu này (0796.693.304)
            </a>
            <a href="tel:0796693304" class="w-full py-2.5 rounded-lg bg-brand-red hover:bg-brand-darkRed text-white font-semibold text-xs text-center transition">
              Gọi trực tiếp: 0796.693.304
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- =========================================================
       JAVASCRIPT: DỮ LIỆU DANH MỤC & SẢN PHẨM + SLIDER TỰ TRƯỢT
  ========================================================== -->
  <script>
    // 1. Danh mục sản phẩm lấy từ trang mẫu denlongvn.com & Fanpage Lồng Đèn Hạnh Đào (Hình ảnh đèn lồng thực tế)
    const categories = [
      {
        id: 'den-long-hoi-an',
        name: 'Đèn lồng Hội An',
        shortName: 'Đèn Hội An',
        image: 'https://images.pexels.com/photos/31476945/pexels-photo-31476945.jpeg?auto=compress&cs=tinysrgb&w=500'
      },
      {
        id: 'phi-hoa-3d',
        name: 'Đèn lồng phi hoa 3D',
        shortName: 'Phi hoa 3D',
        image: 'https://images.pexels.com/photos/38914416/pexels-photo-38914416.jpeg?auto=compress&cs=tinysrgb&w=500'
      },
      {
        id: 'vai-hoa-gam-truc',
        name: 'Vải hoa & Gấm trúc',
        shortName: 'Vải hoa & Gấm',
        image: 'https://images.pexels.com/photos/33186289/pexels-photo-33186289.jpeg?auto=compress&cs=tinysrgb&w=500'
      },
      {
        id: 'xo-voan-tho-cam',
        name: 'Xô Voan & Thổ cẩm',
        shortName: 'Xô Voan & Thổ cẩm',
        image: 'https://images.pexels.com/photos/39128604/pexels-photo-39128604.jpeg?auto=compress&cs=tinysrgb&w=500'
      },
      {
        id: 'theu-tay-ve-hoa-tiet',
        name: 'Thêu tay & Vẽ họa tiết',
        shortName: 'Thêu & Vẽ tay',
        image: 'https://images.pexels.com/photos/29670758/pexels-photo-29670758.jpeg?auto=compress&cs=tinysrgb&w=500'
      },
      {
        id: 'in-logo-su-kien',
        name: 'Đèn lồng in Logo',
        shortName: 'In Logo & Sự kiện',
        image: 'https://images.pexels.com/photos/39018006/pexels-photo-39018006.jpeg?auto=compress&cs=tinysrgb&w=500'
      },
      {
        id: 'den-go-hoa-sen',
        name: 'Đèn tre, Gỗ & Hoa sen',
        shortName: 'Đèn tre, Gỗ & Sen',
        image: 'https://images.pexels.com/photos/33743381/pexels-photo-33743381.jpeg?auto=compress&cs=tinysrgb&w=500'
      },
      {
        id: 'den-long-nhat',
        name: 'Đèn lồng kiểu Nhật',
        shortName: 'Đèn kiểu Nhật',
        image: 'https://images.pexels.com/photos/38757705/pexels-photo-38757705.jpeg?auto=compress&cs=tinysrgb&w=500'
      }
    ];

    // 2. Danh sách sản phẩm thực tế theo các danh mục của denlongvn.com & Fanpage Lồng Đèn Hạnh Đào
    // Mỗi sản phẩm sử dụng ảnh chụp đèn lồng thực tế riêng biệt, không trùng lặp, không gắn nhãn dán ở trang chủ
    const products = [
      // Danh mục 1: Đèn lồng Hội An (Lụa tơ tằm)
      {
        id: 101,
        catId: 'den-long-hoi-an',
        catName: 'Đèn lồng Hội An',
        name: 'Đèn lồng Hội An lụa tơ tằm kiểu tròn truyền thống',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/31476945/pexels-photo-31476945.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Đèn lồng Hội An khung tre già xử lý chống mối mọt, bọc vải lụa tơ tằm trơn đủ màu sắc (đỏ, vàng, cam, xanh, tím, hồng).'
      },
      {
        id: 102,
        catId: 'den-long-hoi-an',
        catName: 'Đèn lồng Hội An',
        name: 'Đèn lồng Hội An kiểu củ tỏi lụa Hà Đông cao cấp',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Hoi_An_lantern_lampion_(38834258624).jpg?width=600',
        desc: 'Mẫu đèn lồng kiểu củ tỏi đặc trưng của phố cổ Hội An, thích hợp phối treo nhà hàng, quán cà phê, hiên nhà và không gian lễ hội.'
      },
      {
        id: 103,
        catId: 'den-long-hoi-an',
        catName: 'Đèn lồng Hội An',
        name: 'Đèn lồng Hội An kiểu quả Na thon dài dễ bung mở',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An,_Vietnam_(25708206924).jpg?width=600',
        desc: 'Thiết kế dáng quả Na thanh thoát, kết hợp hài hòa với đèn kiểu tròn và kiểu tỏi để tạo điểm nhấn ánh sáng ấm áp.'
      },
      {
        id: 104,
        catId: 'den-long-hoi-an',
        catName: 'Đèn lồng Hội An',
        name: 'Đèn lồng Hội An kiểu Dù & Kim Cương trang trí',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_(26652147368).jpg?width=600',
        desc: 'Kiểu dáng chiếc ô kết hợp kim cương độc đáo, tạo hiệu ứng ánh sáng sang trọng cho sảnh khách sạn, resort và homestay.'
      },

      // Danh mục 2: Đèn lồng phi hoa 3D
      {
        id: 201,
        catId: 'phi-hoa-3d',
        catName: 'Đèn lồng phi hoa 3D',
        name: 'Đèn lồng phi hoa 3D họa tiết hoa đào nổi bật',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/38914416/pexels-photo-38914416.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Chất liệu vải phi hoa 3D bóng đẹp, họa tiết sắc nét khi thắp sáng cả ban ngày lẫn ban đêm.'
      },
      {
        id: 202,
        catId: 'phi-hoa-3d',
        catName: 'Đèn lồng phi hoa 3D',
        name: 'Bộ đèn lồng phi hoa 3D Hội An phối đủ màu sắc',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_1.jpg?width=600',
        desc: 'Bộ sưu tập đèn phi hoa 3D nhiều dáng (tròn, tỏi, kim cương, bánh ú) chuyên dùng decor phố đi bộ, sự kiện và quán ăn.'
      },
      {
        id: 203,
        catId: 'phi-hoa-3d',
        catName: 'Đèn lồng phi hoa 3D',
        name: 'Đèn lồng phi hoa 3D kiểu bánh ú treo hiên nhà',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/32045721/pexels-photo-32045721.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Dáng bánh ú truyền thống bọc vải phi hoa 3D bền màu, chịu được thời tiết ngoài trời có mái che.'
      },
      {
        id: 204,
        catId: 'phi-hoa-3d',
        catName: 'Đèn lồng phi hoa 3D',
        name: 'Đèn lồng phi hoa 3D kiểu tỏi ngược nghệ thuật',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/26805261/pexels-photo-26805261.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Thiết kế tỏi ngược phá cách bọc vải phi hoa 3D rực rỡ.'
      },

      // Danh mục 3: Vải hoa & Gấm trúc
      {
        id: 301,
        catId: 'vai-hoa-gam-truc',
        catName: 'Vải hoa & Gấm trúc',
        name: 'Đèn lồng vải gấm trúc Hội An sang trọng',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/33186289/pexels-photo-33186289.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Chất liệu vải gấm dệt họa tiết tùng trúc, hoa mẫu đơn cổ điển, mang đậm nét Á Đông.'
      },
      {
        id: 302,
        catId: 'vai-hoa-gam-truc',
        catName: 'Vải hoa & Gấm trúc',
        name: 'Đèn lồng vải hoa nhí trang trí quán cafe & homestay',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/14360805/pexels-photo-14360805.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Đèn lồng bọc vải hoa trang nhã, tạo không gian nhẹ nhàng, hoài cổ tại Hội An.'
      },

      // Danh mục 4: Xô Voan & Thổ cẩm
      {
        id: 401,
        catId: 'xo-voan-tho-cam',
        catName: 'Xô Voan & Thổ cẩm',
        name: 'Đèn lồng Xô Voan xuyên sáng dịu nhẹ decor phòng',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/39128604/pexels-photo-39128604.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Chất liệu vải xô voan mềm mại, tán sáng êm dịu thích hợp decor phòng ngủ, spa và studio.'
      },
      {
        id: 402,
        catId: 'xo-voan-tho-cam',
        catName: 'Xô Voan & Thổ cẩm',
        name: 'Đèn lồng thổ cẩm vải lanh họa tiết truyền thống',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/39388830/pexels-photo-39388830.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Hoa văn thổ cẩm độc đáo kết hợp khung tre thủ công bền chắc.'
      },

      // Danh mục 5: Đèn lồng thêu tay & Vẽ họa tiết
      {
        id: 501,
        catId: 'theu-tay-ve-hoa-tiet',
        catName: 'Thêu tay & Vẽ họa tiết',
        name: 'Đèn lồng vẽ tay họa tiết hoa đào & phố cổ Hội An',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/29670758/pexels-photo-29670758.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Nghệ nhân Hội An vẽ tay trực tiếp lên nền lụa tơ tằm: Hoa đào, hoa sen, cá chép, Chùa Cầu, phố cổ.'
      },
      {
        id: 502,
        catId: 'theu-tay-ve-hoa-tiet',
        catName: 'Thêu tay & Vẽ họa tiết',
        name: 'Đèn lồng thêu tay hoa sen & chim hạc tinh xảo',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/29594627/pexels-photo-29594627.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Đèn lồng thêu nổi thủ công tỉ mỉ từng đường kim mũi chỉ, thích hợp làm quà tặng và trang trí cao cấp.'
      },

      // Danh mục 6: Đèn lồng in Logo & Sự kiện
      {
        id: 601,
        catId: 'in-logo-su-kien',
        catName: 'Đèn lồng in Logo',
        name: 'Đèn lồng in Logo thương hiệu nhà hàng, quán cafe',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/30700751/pexels-photo-30700751.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Nhận in logo, tên quán, slogan lên đèn lồng Hội An sắc nét, gia công nhanh số lượng sỉ & lẻ.'
      },
      {
        id: 602,
        catId: 'in-logo-su-kien',
        catName: 'Đèn lồng in Logo',
        name: 'Đèn lồng đỏ trang trí sự kiện, lễ hội Tết & Trung Thu',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/39018006/pexels-photo-39018006.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Cung cấp số lượng lớn đèn lồng trang trí đường phố, trung tâm thương mại, lễ hội và sự kiện.'
      },

      // Danh mục 7: Đèn tre đan Hạnh Đào, Đèn gỗ & Đèn hoa sen
      {
        id: 701,
        catId: 'den-go-hoa-sen',
        catName: 'Đèn tre, Gỗ & Hoa sen',
        name: 'Lồng đèn tre đan tự nhiên Hạnh Đào Hội An thủ công tỉ mỉ',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/33743381/pexels-photo-33743381.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Mẫu lồng đèn tre tự nhiên đan thủ công đặc trưng trên Fanpage Cơ Sở Sản Xuất Lồng Đèn Hạnh Đào Hội An, bền đẹp và thân thiện môi trường.'
      },
      {
        id: 702,
        catId: 'den-go-hoa-sen',
        catName: 'Đèn tre, Gỗ & Hoa sen',
        name: 'Đèn hoa sen Hội An trang trí chùa, phòng thờ & lễ Phật Đản',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/15207187/pexels-photo-15207187.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Đèn hoa sen cánh xếp tỉ mỉ kết hợp khung gỗ chạm khắc sang trọng.'
      },

      // Danh mục 8: Đèn lồng kiểu Nhật
      {
        id: 801,
        catId: 'den-long-nhat',
        catName: 'Đèn lồng kiểu Nhật',
        name: 'Đèn lồng kiểu Nhật dáng trụ dài trang trí quán Izakaya',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/38757705/pexels-photo-38757705.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Đèn lồng kiểu Nhật chống thấm nước, nhận viết chữ Kanji / in logo nhà hàng Nhật Bản.'
      },
      {
        id: 802,
        catId: 'den-long-nhat',
        catName: 'Đèn lồng kiểu Nhật',
        name: 'Lồng đèn mây tre thả trần phong cách Nhật & Hội An',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://images.pexels.com/photos/34311868/pexels-photo-34311868.jpeg?auto=compress&cs=tinysrgb&w=600',
        desc: 'Lồng đèn tre đan thả trần trang trí nhà hàng Nhật, quán cafe, resort và không gian sân vườn.'
      }
    ];

    let activeCategory = 'all';
// ... existing code ... -->
