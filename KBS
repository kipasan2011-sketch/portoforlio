<!DOCTYPE html>
<html lang="ms" class="h-full bg-slate-50">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portal Tempahan Kemudahan KBS - Kementerian Belia & Sukan</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons CDN -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Font (Inter) -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
</head>
<body class="h-full flex flex-col font-sans text-slate-800 antialiased bg-slate-50">

    <!-- Toast Notification Container -->
    <div id="toast-container" class="fixed bottom-5 right-5 z-50 flex flex-col gap-2 pointer-events-none"></div>

    <!-- Navigation Header -->
    <header class="sticky top-0 z-40 bg-slate-950/90 backdrop-blur-md border-b border-slate-800 shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <!-- Logo & Title -->
                <div class="flex items-center gap-3 cursor-pointer" onclick="switchTab('explore')">
                    <img src="Gemini_Generated_Image_4ifews4ifews4ife.jpg" alt="Logo KBS" class="w-12 h-12 object-contain" onerror="this.src='https://placehold.co/100x100/F39200/fff?text=KBS'">
                    <div>
                        <div class="flex items-center gap-2">
                            <span class="text-white font-extrabold text-lg tracking-tight">KBS<span class="text-amber-500">Tempahan</span></span>
                            <span class="bg-amber-500/20 text-amber-400 text-[10px] font-bold px-2 py-0.5 rounded-full border border-amber-500/30 uppercase">Rasmi</span>
                        </div>
                        <p class="text-[11px] text-slate-400">Portal Tempahan Kemudahan Sukan Paroi</p>
                    </div>
                </div>

                <!-- Navigation Links & User Action -->
                <div class="flex items-center gap-4">
                    <div class="flex items-center bg-slate-900/90 rounded-2xl p-1 border border-slate-800">
                        <button id="nav-explore-btn" onclick="switchTab('explore')" class="px-3 sm:px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold transition-all text-amber-500 bg-slate-800 shadow-sm">
                            <i class="fa-solid fa-magnifying-glass mr-1.5"></i> Terokai Kemudahan
                        </button>
                        <button id="nav-bookings-btn" onclick="switchTab('bookings')" class="px-3 sm:px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold transition-all text-slate-400 hover:text-white relative">
                            <i class="fa-solid fa-calendar-check mr-1.5"></i> Tempahan Saya
                            <span id="booking-badge" class="hidden absolute -top-1 -right-1 bg-amber-500 text-slate-950 text-[10px] font-black w-5 h-5 rounded-full flex items-center justify-center border-2 border-slate-950">0</span>
                        </button>
                    </div>

                    <!-- Auth State Buttons -->
                    <div id="nav-logged-out">
                        <button onclick="openAuthModal('login')" class="px-4 py-2.5 rounded-xl bg-amber-600 hover:bg-amber-500 text-white font-bold text-xs shadow-lg shadow-amber-600/20 transition-all flex items-center gap-2">
                            <i class="fa-solid fa-right-to-bracket"></i> Log Masuk / Daftar
                        </button>
                    </div>

                    <div id="nav-logged-in" class="hidden flex items-center gap-3">
                        <div class="flex items-center gap-2.5 bg-slate-900 border border-slate-800 px-3 py-1.5 rounded-xl">
                            <div id="user-avatar-initials" class="w-8 h-8 rounded-lg bg-amber-500 text-slate-950 font-black flex items-center justify-center text-xs">
                                KBS
                            </div>
                            <div class="text-left hidden sm:block">
                                <span id="user-display-name" class="block text-xs font-bold text-white leading-none">Nama Pengguna</span>
                                <span id="user-display-role" class="text-[10px] text-amber-400">Ahli KBS</span>
                            </div>
                        </div>
                        <button onclick="handleLogout()" title="Log Keluar" class="w-9 h-9 rounded-xl bg-slate-900 border border-slate-800 text-slate-400 hover:text-red-400 flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-power-off"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- Main Content Body -->
    <main class="flex-grow">
        
        <!-- ================= EXPLORE / SEARCH TAB CONTENT ================= -->
        <section id="explore-tab" class="space-y-8 pb-16">
            
            <!-- Hero Banner Section -->
            <div class="relative bg-slate-950 text-white overflow-hidden py-16 border-b border-slate-800">
                <div class="absolute inset-0 opacity-20 bg-[radial-gradient(#f59e0b_1px,transparent_1px)] [background-size:16px_16px]"></div>
                
                <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
                    <div class="flex flex-col lg:flex-row lg:items-center justify-between gap-8">
                        <div class="max-w-2xl">
                            <div class="inline-flex items-center gap-2 px-3 py-1 bg-amber-500/10 border border-amber-500/30 rounded-full text-amber-400 text-xs font-bold mb-4">
                                <i class="fa-solid fa-building-columns"></i> Kompleks Sukan Paroi, Negeri Sembilan
                            </div>
                            <h1 class="text-3xl sm:text-5xl font-black tracking-tight leading-tight">
                                Tempah Kemudahan Sukan <span class="text-amber-500">KBS Paroi</span> Dengan Mudah
                            </h1>
                            <p class="text-slate-400 text-sm sm:text-base mt-4 leading-relaxed">
                                Portal rasmi tempahan sewaan Centre Court, Stadium, Kolam Renang, dan Gelanggang Futsal bertaraf antarabangsa untuk kejohanan, latihan, dan aktiviti belia.
                            </p>
                        </div>
                        <div class="hidden lg:block bg-slate-900/90 p-6 rounded-3xl border border-amber-500/30 backdrop-blur-md max-w-xs text-center shadow-2xl">
                            <i class="fa-solid fa-trophy text-4xl text-amber-400 mb-3"></i>
                            <h3 class="text-lg font-bold text-white">Sokongan Belia & Kelab</h3>
                            <p class="text-xs text-slate-400 mt-2">Kadar permohonan khas tersedia untuk persatuan belia berdaftar, kelab sukan tempatan, dan program komuniti.</p>
                        </div>
                    </div>

                    <!-- Category Quick Filter Chips -->
                    <div class="mt-8 flex flex-wrap gap-2.5" id="quick-category-chips">
                        <!-- Generated by JS -->
                    </div>
                </div>
            </div>

            <!-- Main Filter & Search Section -->
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 -mt-6 relative z-20">
                <div class="bg-white rounded-2xl shadow-xl p-5 md:p-6 border border-slate-200">
                    <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
                        
                        <!-- Search Keyword -->
                        <div>
                            <label class="block text-xs font-bold text-slate-500 uppercase tracking-wider mb-1.5">Carian Kemudahan</label>
                            <div class="relative">
                                <i class="fa-solid fa-magnifying-glass absolute left-3.5 top-1/2 -translate-y-1/2 text-slate-400"></i>
                                <input type="text" id="filter-keyword" placeholder="Nama kemudahan / lokasi..." class="w-full pl-10 pr-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500 transition-all">
                            </div>
                        </div>

                        <!-- Space Category -->
                        <div>
                            <label class="block text-xs font-bold text-slate-500 uppercase tracking-wider mb-1.5">Kategori Kemudahan</label>
                            <div class="relative">
                                <i class="fa-solid fa-layer-group absolute left-3.5 top-1/2 -translate-y-1/2 text-slate-400"></i>
                                <select id="filter-category" class="w-full pl-10 pr-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500 transition-all appearance-none cursor-pointer">
                                    <option value="all">Semua Kemudahan Sukan</option>
                                    <option value="Centre Court">Centre Court (Gelanggang Pusat)</option>
                                    <option value="Stadium">Stadium Utama & Mini</option>
                                    <option value="Kolam Renang">Kolam Renang / Akuatik</option>
                                    <option value="Futsal">Gelanggang Futsal</option>
                                </select>
                                <i class="fa-solid fa-chevron-down absolute right-3.5 top-1/2 -translate-y-1/2 text-slate-400 pointer-events-none text-xs"></i>
                            </div>
                        </div>

                        <!-- Capacity Slider -->
                        <div>
                            <div class="flex justify-between items-center mb-1.5">
                                <label class="block text-xs font-bold text-slate-500 uppercase tracking-wider">Kapasiti Min (Orang)</label>
                                <span id="capacity-value" class="text-xs font-bold text-amber-600 bg-amber-50 px-2 py-0.5 rounded">1 Orang</span>
                            </div>
                            <input type="range" id="filter-capacity" min="1" max="500" value="1" class="w-full h-2 bg-slate-200 rounded-lg appearance-none cursor-pointer accent-amber-600 mt-2">
                        </div>

                        <!-- Price Slider -->
                        <div>
                            <div class="flex justify-between items-center mb-1.5">
                                <label class="block text-xs font-bold text-slate-500 uppercase tracking-wider">Kadar Maksimum</label>
                                <span id="price-value" class="text-xs font-bold text-amber-600 bg-amber-50 px-2 py-0.5 rounded">RM 800/jam</span>
                            </div>
                            <input type="range" id="filter-price" min="20" max="800" step="10" value="800" class="w-full h-2 bg-slate-200 rounded-lg appearance-none cursor-pointer accent-amber-600 mt-2">
                        </div>

                    </div>

                    <!-- Filter Action Buttons -->
                    <div class="mt-4 pt-4 border-t border-slate-100 flex items-center justify-between">
                        <span id="results-count" class="text-xs font-medium text-slate-500">Menampilkan kemudahan sukan...</span>
                        <button onclick="resetFilters()" class="text-xs font-bold text-slate-500 hover:text-amber-600 transition-colors flex items-center gap-1">
                            <i class="fa-solid fa-rotate-left"></i> Set Semula Penapis
                        </button>
                    </div>
                </div>
            </div>

            <!-- Space Listings Grid -->
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
                <div id="spaces-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Dynamic Space Cards Generated by JS -->
                </div>
                
                <!-- Empty State -->
                <div id="empty-results" class="hidden text-center py-16 bg-white rounded-2xl border border-slate-200 shadow-sm">
                    <div class="w-16 h-16 bg-amber-50 text-amber-600 rounded-full flex items-center justify-center mx-auto mb-4 text-2xl">
                        <i class="fa-solid fa-person-running"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-800">Tiada kemudahan sukan ditemui</h3>
                    <p class="text-sm text-slate-500 mt-1">Cuba ubah carian perkataan atau nilai penapis kadar sewaan.</p>
                    <button onclick="resetFilters()" class="mt-4 px-4 py-2 bg-amber-600 text-white rounded-xl text-xs font-bold hover:bg-amber-700 transition-all">
                        Tunjukkan Semua Kemudahan
                    </button>
                </div>
            </div>
        </section>


        <!-- ================= MY BOOKINGS TAB CONTENT ================= -->
        <section id="bookings-tab" class="hidden max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-10">
            <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-4 mb-8">
                <div>
                    <h2 class="text-2xl sm:text-3xl font-extrabold text-slate-900">Rekod Tempahan Saya</h2>
                    <p class="text-sm text-slate-500 mt-1">Senarai semua rekod tempahan kemudahan sukan KBS anda.</p>
                </div>
                <div class="flex items-center gap-3">
                    <button onclick="switchTab('explore')" class="px-4 py-2.5 bg-amber-600 text-white font-bold rounded-xl text-xs hover:bg-amber-700 transition-all flex items-center gap-2">
                        <i class="fa-solid fa-plus"></i> Tempah Kemudahan Baharu
                    </button>
                </div>
            </div>

            <!-- Bookings List Container -->
            <div id="bookings-list" class="space-y-4">
                <!-- Rendered dynamically by JS -->
            </div>

            <!-- Empty Bookings State -->
            <div id="empty-bookings" class="hidden text-center py-20 bg-white rounded-2xl border border-slate-200 shadow-sm">
                <div class="w-20 h-20 bg-slate-100 text-slate-400 rounded-full flex items-center justify-center mx-auto mb-4 text-3xl">
                    <i class="fa-solid fa-calendar-xmark"></i>
                </div>
                <h3 class="text-xl font-bold text-slate-800">Tiada Tempahan Aktif</h3>
                <p class="text-sm text-slate-500 mt-2 max-w-md mx-auto">Anda belum membuat sebarang tempahan gelanggang atau stadium sukan KBS lagi.</p>
                <button onclick="switchTab('explore')" class="mt-6 px-6 py-3 bg-amber-600 text-white font-bold rounded-xl text-sm hover:bg-amber-700 transition-all shadow-md">
                    Terokai Kemudahan Sukan Sekarang
                </button>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-slate-950 text-slate-400 text-xs border-t border-slate-800 mt-auto">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-10">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-8">
                <div class="space-y-3">
                    <div class="flex items-center gap-2">
                        <img src="Gemini_Generated_Image_4ifews4ifews4ife.jpg" alt="Logo KBS" class="w-8 h-8 object-contain" onerror="this.src='https://placehold.co/100x100/F39200/fff?text=KBS'">
                        <span class="text-white font-bold text-sm">KBS Tempahan Sukan</span>
                    </div>
                    <p class="text-slate-400 text-xs leading-relaxed">
                        Sistem tempahan rasmi untuk fasiliti belia, stadium, dan arena sukan di bawah Kementerian Belia & Sukan Malaysia.
                    </p>
                </div>
                <div>
                    <h4 class="text-white font-bold mb-3">Kategori Kemudahan</h4>
                    <ul class="space-y-2">
                        <li><a href="#" onclick="filterByCategory('Centre Court')" class="hover:text-amber-400 transition-colors">Centre Court (Gelanggang Pusat)</a></li>
                        <li><a href="#" onclick="filterByCategory('Stadium')" class="hover:text-amber-400 transition-colors">Stadium Utama & Mini</a></li>
                        <li><a href="#" onclick="filterByCategory('Kolam Renang')" class="hover:text-amber-400 transition-colors">Kolam Renang / Akuatik</a></li>
                        <li><a href="#" onclick="filterByCategory('Futsal')" class="hover:text-amber-400 transition-colors">Gelanggang Futsal</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-white font-bold mb-3">Pautan Penting</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="hover:text-amber-400 transition-colors">Syarat & Peraturan Penggunaan</a></li>
                        <li><a href="#" class="hover:text-amber-400 transition-colors">Kadar Diskaun Persatuan Belia</a></li>
                        <li><a href="#" class="hover:text-amber-400 transition-colors">Pusat Bantuan & Soalan Lazim</a></li>
                        <li><a href="#" class="hover:text-amber-400 transition-colors">Hubungi Pegawai Kompleks Sukan</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-white font-bold mb-3">Hubungi Kami</h4>
                    <p class="text-slate-400 leading-relaxed mb-2">
                        Kementerian Belia dan Sukan,<br>Menara KBS, Presint 4, Putrajaya.
                    </p>
                    <p class="text-amber-400 font-medium"><i class="fa-solid fa-phone mr-1"></i> 03-8871 3000</p>
                </div>
            </div>
            <div class="pt-6 border-t border-slate-900 flex flex-col sm:flex-row justify-between items-center gap-4 text-slate-500">
                <p>© 2026 Kementerian Belia & Sukan (KBS) Malaysia. Hak Cipta Terpelihara.</p>
                <div class="flex gap-4">
                    <a href="#" class="hover:text-white"><i class="fa-brands fa-facebook"></i></a>
                    <a href="#" class="hover:text-white"><i class="fa-brands fa-x-twitter"></i></a>
                    <a href="#" class="hover:text-white"><i class="fa-brands fa-instagram"></i></a>
                </div>
            </div>
        </div>
    </footer>


    <!-- ================= BOOKING DRAWER MODAL ================= -->
    <div id="booking-drawer" class="fixed inset-0 z-50 hidden">
        <div class="modal-backdrop fixed inset-0 bg-slate-950/60 backdrop-blur-sm" onclick="closeBookingDrawer()"></div>
        <div class="fixed inset-y-0 right-0 max-w-full flex pl-10">
            <div class="w-screen max-w-xl bg-white shadow-2xl flex flex-col relative z-10">
                
                <!-- Drawer Header -->
                <div class="p-6 bg-slate-900 text-white flex items-center justify-between border-b border-amber-500/30">
                    <div>
                        <span class="text-xs font-bold uppercase tracking-wider text-amber-400" id="drawer-space-category">Category</span>
                        <h2 class="text-xl font-extrabold text-white" id="drawer-space-title">Nama Kemudahan</h2>
                        <p class="text-xs text-slate-400 mt-0.5" id="drawer-space-location"><i class="fa-solid fa-location-dot text-amber-500 mr-1"></i> Lokasi</p>
                    </div>
                    <button onclick="closeBookingDrawer()" class="w-9 h-9 rounded-full bg-slate-800 hover:bg-slate-700 text-slate-400 hover:text-white flex items-center justify-center transition-colors">
                        <i class="fa-solid fa-xmark"></i>
                    </button>
                </div>

                <!-- Drawer Content Scrollable -->
                <div class="flex-grow overflow-y-auto p-6 space-y-6">
                    
                    <!-- Main Image Preview -->
                    <div class="rounded-2xl overflow-hidden h-48 bg-slate-100 relative shadow-inner">
                        <img id="drawer-space-img" src="" alt="Kemudahan Preview" class="w-full h-full object-cover">
                        <div class="absolute bottom-3 right-3 bg-slate-900/80 backdrop-blur-md text-white text-xs px-3 py-1.5 rounded-xl font-bold" id="drawer-space-price">
                            RM 0/jam
                        </div>
                    </div>

                    <!-- Facility Description & Features -->
                    <div>
                        <h4 class="text-xs font-bold uppercase text-slate-400 tracking-wider mb-2">Penerangan Kemudahan</h4>
                        <p id="drawer-space-desc" class="text-sm text-slate-600 leading-relaxed">Penerangan lengkap kemudahan sukan.</p>
                    </div>

                    <!-- Specifications Grid -->
                    <div class="grid grid-cols-2 gap-3 bg-slate-50 p-4 rounded-xl border border-slate-200 text-xs">
                        <div>
                            <span class="text-slate-400 block">Kapasiti Maksimum:</span>
                            <span id="drawer-space-capacity" class="font-bold text-slate-800">0 Orang</span>
                        </div>
                        <div>
                            <span class="text-slate-400 block">Jenis Permukaan/Fasiliti:</span>
                            <span id="drawer-space-surface" class="font-bold text-slate-800">Standard KBS</span>
                        </div>
                    </div>

                    <!-- Included Amenities Checkbox -->
                    <div>
                        <h4 class="text-xs font-bold uppercase text-slate-400 tracking-wider mb-3">Kemudahan Termasuk</h4>
                        <div id="drawer-amenities-list" class="flex flex-wrap gap-2">
                            <!-- Rendered by JS -->
                        </div>
                    </div>

                    <!-- Form Inputs for Booking -->
                    <form id="booking-form" onsubmit="handleConfirmBooking(event)" class="space-y-4 pt-4 border-t border-slate-200">
                        <h4 class="text-sm font-bold text-slate-900 flex items-center gap-2">
                            <i class="fa-solid fa-clock text-amber-600"></i> Pilih Tarikh & Slot Masa
                        </h4>

                        <!-- Date Picker -->
                        <div>
                            <label class="block text-xs font-bold text-slate-600 mb-1">Tarikh Tempahan</label>
                            <input type="date" id="book-date" required class="w-full px-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500 font-medium">
                        </div>

                        <!-- Time Slot Selectors -->
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-xs font-bold text-slate-600 mb-1">Masa Mula</label>
                                <select id="book-start-time" required onchange="calculateBookingTotal()" class="w-full px-3 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500">
                                    <option value="08:00">08:00 Pagi</option>
                                    <option value="09:00">09:00 Pagi</option>
                                    <option value="10:00">10:00 Pagi</option>
                                    <option value="11:00">11:00 Pagi</option>
                                    <option value="14:00">02:00 Petang</option>
                                    <option value="15:00">03:00 Petang</option>
                                    <option value="16:00">04:00 Petang</option>
                                    <option value="17:00">05:00 Petang</option>
                                    <option value="20:00">08:00 Malam</option>
                                    <option value="21:00">09:00 Malam</option>
                                </select>
                            </div>
                            <div>
                                <label class="block text-xs font-bold text-slate-600 mb-1">Masa Tamat</label>
                                <select id="book-end-time" required onchange="calculateBookingTotal()" class="w-full px-3 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500">
                                    <option value="10:00">10:00 Pagi</option>
                                    <option value="11:00">11:00 Pagi</option>
                                    <option value="12:00">12:00 Tengah Hari</option>
                                    <option value="16:00">04:00 Petang</option>
                                    <option value="18:00">06:00 Petang</option>
                                    <option value="22:00">10:00 Malam</option>
                                    <option value="23:00">11:00 Malam</option>
                                </select>
                            </div>
                        </div>

                        <!-- Attendees Count -->
                        <div>
                            <label class="block text-xs font-bold text-slate-600 mb-1">Anggaran Bilangan Pemain / Pengunjung</label>
                            <input type="number" id="book-guests" min="1" value="10" required class="w-full px-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500">
                        </div>

                        <!-- Optional Addons -->
                        <div>
                            <label class="block text-xs font-bold text-slate-600 mb-2">Servis Tambahan (Pilihan)</label>
                            <div class="space-y-2">
                                <label class="flex items-center gap-3 p-3 bg-slate-50 rounded-xl border border-slate-200 cursor-pointer hover:bg-slate-100 transition-colors">
                                    <input type="checkbox" id="addon-lighting" onchange="calculateBookingTotal()" class="w-4 h-4 text-amber-600 rounded focus:ring-amber-500">
                                    <div class="flex-grow text-xs">
                                        <span class="font-bold text-slate-800">Lampu Limpah (Floodlights / Malam)</span>
                                        <span class="block text-slate-500">+RM 30 / jam</span>
                                    </div>
                                </label>
                                <label class="flex items-center gap-3 p-3 bg-slate-50 rounded-xl border border-slate-200 cursor-pointer hover:bg-slate-100 transition-colors">
                                    <input type="checkbox" id="addon-scoreboard" onchange="calculateBookingTotal()" class="w-4 h-4 text-amber-600 rounded focus:ring-amber-500">
                                    <div class="flex-grow text-xs">
                                        <span class="font-bold text-slate-800">Papan Skor Digital & Sistem PA</span>
                                        <span class="block text-slate-500">+RM 50 satu sesi</span>
                                    </div>
                                </label>
                            </div>
                        </div>
                        
                        <button type="submit" id="submit-booking-btn" class="hidden"></button>
                    </form>
                </div>

                <!-- Drawer Footer with Total Calculation -->
                <div class="p-6 bg-slate-50 border-t border-slate-200 flex items-center justify-between">
                    <div>
                        <span class="text-xs text-slate-500 block">Jumlah Keseluruhan Bayaran</span>
                        <div class="text-2xl font-black text-amber-600" id="summary-total-price">RM 0.00</div>
                        <span class="text-[10px] text-slate-400" id="summary-hours-count">0 jam dipilih</span>
                    </div>
                    <button onclick="document.getElementById('submit-booking-btn').click()" class="px-6 py-3.5 bg-amber-600 hover:bg-amber-700 text-white font-bold rounded-xl text-sm shadow-lg shadow-amber-600/30 transition-all flex items-center gap-2">
                        <i class="fa-solid fa-check-circle"></i> Sahkan Tempahan
                    </button>
                </div>

            </div>
        </div>
    </div>


    <!-- ================= AUTH MODAL (LOG MASUK / DAFTAR) ================= -->
    <div id="auth-modal" class="fixed inset-0 z-50 hidden flex items-center justify-center p-4">
        <div class="modal-backdrop fixed inset-0 bg-slate-950/60 backdrop-blur-sm" onclick="closeAuthModal()"></div>
        <div class="bg-white rounded-3xl shadow-2xl max-w-md w-full overflow-hidden relative z-10 border border-slate-100">
            
            <!-- Auth Header -->
            <div class="bg-slate-950 p-6 text-white text-center relative border-b border-amber-500/30">
                <button onclick="closeAuthModal()" class="absolute top-4 right-4 w-8 h-8 rounded-full bg-slate-800 text-slate-400 hover:text-white flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
                <img src="Gemini_Generated_Image_4ifews4ifews4ife.jpg" alt="KBS Logo" class="w-12 h-12 object-contain mx-auto mb-2" onerror="this.src='https://placehold.co/100x100/F39200/fff?text=KBS'">
                <h3 class="text-lg font-extrabold text-white">Portal Keahlian Sukan KBS</h3>
                <p class="text-xs text-slate-400 mt-1">Satu akaun untuk semua tempahan stadium & gelanggang</p>
            </div>

            <!-- Auth Tabs Switcher -->
            <div class="flex border-b border-slate-200 bg-slate-50">
                <button id="tab-btn-login" onclick="switchAuthTab('login')" class="flex-1 py-3 text-xs font-bold text-amber-600 border-b-2 border-amber-600 transition-all">
                    Log Masuk
                </button>
                <button id="tab-btn-signup" onclick="switchAuthTab('signup')" class="flex-1 py-3 text-xs font-bold text-slate-500 hover:text-slate-800 border-b-2 border-transparent transition-all">
                    Daftar Akaun Baharu
                </button>
            </div>

            <div class="p-6">
                <!-- FORM LOG MASUK -->
                <form id="form-login" onsubmit="handleLoginSubmit(event)" class="space-y-4">
                    <div>
                        <label class="block text-xs font-bold text-slate-700 mb-1">Alamat E-mel</label>
                        <input type="email" id="login-email" required placeholder="contoh@gmail.com / user@kbs.gov.my" class="w-full px-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500">
                    </div>
                    <div>
                        <label class="block text-xs font-bold text-slate-700 mb-1">Kata Laluan</label>
                        <input type="password" id="login-password" required placeholder="••••••••" class="w-full px-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500">
                    </div>
                    <div class="flex items-center justify-between text-xs">
                        <label class="flex items-center gap-2 cursor-pointer">
                            <input type="checkbox" checked class="w-3.5 h-3.5 text-amber-600 rounded">
                            <span class="text-slate-600">Ingat Saya</span>
                        </label>
                        <a href="#" onclick="showToast('Sila hubungi pentadbir KBS untuk penetapan semula kata laluan.', 'info')" class="text-amber-600 font-bold hover:underline">Lupa kata laluan?</a>
                    </div>
                    <button type="submit" class="w-full py-3 bg-slate-900 hover:bg-amber-600 text-white font-bold rounded-xl text-sm shadow-md transition-all">
                        Log Masuk Sekarang
                    </button>
                </form>

                <!-- FORM DAFTAR AKAUN -->
                <form id="form-signup" onsubmit="handleSignupSubmit(event)" class="space-y-4 hidden">
                    <div>
                        <label class="block text-xs font-bold text-slate-700 mb-1">Nama Penuh (Mengikut MyKad)</label>
                        <input type="text" id="signup-name" required placeholder="Ahmad Harith Bin Razali" class="w-full px-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500">
                    </div>
                    <div>
                        <label class="block text-xs font-bold text-slate-700 mb-1">Alamat E-mel</label>
                        <input type="email" id="signup-email" required placeholder="ahmad@gmail.com" class="w-full px-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500">
                    </div>
                    <div>
                        <label class="block text-xs font-bold text-slate-700 mb-1">Kategori Pengguna / Peranan</label>
                        <select id="signup-role" class="w-full px-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500">
                            <option value="Orang Awam">Orang Awam / Individu</option>
                            <option value="Persatuan Belia">Persatuan / Kelab Belia Berdaftar</option>
                            <option value="Kelab Sukan">Kelab Sukan Tempatan</option>
                            <option value="Pegawai Kerajaan">Pegawai Kerajaan / Agensi</option>
                        </select>
                    </div>
                    <div>
                        <label class="block text-xs font-bold text-slate-700 mb-1">Cipta Kata Laluan</label>
                        <input type="password" id="signup-password" minlength="6" required placeholder="••••••••" class="w-full px-4 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-amber-500">
                    </div>
                    <button type="submit" class="w-full py-3 bg-amber-600 hover:bg-amber-700 text-white font-bold rounded-xl text-sm shadow-md transition-all">
                        Daftar Akaun KBS
                    </button>
                </form>

            </div>
        </div>
    </div>


    <!-- JavaScript Data & Logic -->
    <script>
        // DATA KEMUDAHAN SUKAN KBS (Centre Court, Stadium, Kolam Renang, Futsal - Paroi)
        const SPACES_DATA = [
            {
                id: 'kbs-1',
                title: 'Centre Court Utama Paroi',
                category: 'Centre Court',
                location: 'Kompleks Sukan Paroi, Negeri Sembilan',
                pricePerHour: 150,
                capacity: 500,
                surface: 'Lantai Parquet Kayu Antarabangsa',
                description: 'Gelanggang pusat berhawa dingin serbaguna bertaraf antarabangsa yang sesuai untuk perlawanan bola keranjang, bola tampar, dan badminton.',
                imageUrl: 'https://images.unsplash.com/photo-1546519638-68e109498ffc?auto=format&fit=crop&w=800&q=80',
                amenities: ['Penghawa Dingin', 'Bilik Persalinan Pemain', 'Papan Skor LED Digital', 'Tempat Duduk Penonton', 'Sistem Bunyi PA'],
                badge: 'Pilihan Utama'
            },
            {
                id: 'kbs-2',
                title: 'Stadium Mini Paroi',
                category: 'Stadium',
                location: 'Kompleks Sukan Paroi, Negeri Sembilan',
                pricePerHour: 350,
                capacity: 3500,
                surface: 'Rumput Sintetik & Balapan Tartan',
                description: 'Stadium mini rumput tiruan gred FIFA lengkap dengan balapan olahraga 8 lorong dan lampu limpah kejohanan.',
                imageUrl: 'https://images.unsplash.com/photo-1508098682722-e99c43a406b2?auto=format&fit=crop&w=800&q=80',
                amenities: ['Lampu Limpah (Lampu Malam)', 'Balapan Olahraga', 'Pentas Utama VIP', 'Bilik Pertolongan Cemas', 'Kawasan Parkir Luas'],
                badge: 'Popular'
            },
            {
                id: 'kbs-3',
                title: 'Pusat Akuatik & Kolam Renang Paroi',
                category: 'Kolam Renang',
                location: 'Kompleks Akuatik Paroi, Negeri Sembilan',
                pricePerHour: 120,
                capacity: 200,
                surface: 'Kolam 10 Lorong Olimpik (50m)',
                description: 'Kolam renang bersaiz Olimpik (50m) 10 lorong lengkap dengan sistem kawalan suhu dan sistem keselamatan penyelamat bertauliah.',
                imageUrl: 'https://images.unsplash.com/photo-1576013551627-0cc20b96c2a7?auto=format&fit=crop&w=800&q=80',
                amenities: ['Penyelamat Bertugas (Lifeguard)', 'Bilik Mandi Warm-up', 'Papan Terjun 3m & 10m', 'Loker Keselamatan'],
                badge: 'Gred Olimpik'
            },
            {
                id: 'kbs-4',
                title: 'Gelanggang Futsal Sintetik VIP Paroi',
                category: 'Futsal',
                location: 'Pusat Futsal Belia Paroi, Negeri Sembilan',
                pricePerHour: 80,
                capacity: 25,
                surface: 'Rumput Artificial Turf High-Density',
                description: 'Gelanggang futsal bertutup dengan rumput tiruan berkualiti tinggi gred kejohanan dan pencahayaan LED malam penuh.',
                imageUrl: 'https://images.unsplash.com/photo-1574629810360-7efbbe195018?auto=format&fit=crop&w=800&q=80',
                amenities: ['Lampu Limpah LED', 'Jaring Keselamatan Perimeter', 'Kantin / Vending Machine', 'Bilik Persalinan'],
                badge: 'Hot Slot'
            },
            {
                id: 'kbs-5',
                title: 'Centre Court Arena Tertutup Paroi',
                category: 'Centre Court',
                location: 'Kompleks Sukan Belia Paroi, Negeri Sembilan',
                pricePerHour: 130,
                capacity: 300,
                surface: 'Mat Sukan Flexi-Rubber',
                description: 'Gelanggang dewan tertutup serbaguna berkualiti tinggi bersesuaian untuk sebarang kejohanan sepak takraw, badminton & futsal dewan.',
                imageUrl: 'https://images.unsplash.com/photo-1626248801379-51a0748a5f96?auto=format&fit=crop&w=800&q=80',
                amenities: ['Penghawa Dingin', 'Sistem Garisan Pelbagai Sukan', 'Papan Skor'],
                badge: null
            },
            {
                id: 'kbs-6',
                title: 'Stadium Utama Kompleks Sukan Paroi',
                category: 'Stadium',
                location: 'Presint Sukan Paroi, Negeri Sembilan',
                pricePerHour: 450,
                capacity: 8000,
                surface: 'Rumput Natural Bermuda',
                description: 'Stadium terbuka gred kebangsaan berskala besar sesuai untuk sukan tahunan, kejohanan bola sepak dan konsert belia kebangsaan.',
                imageUrl: 'https://images.unsplash.com/photo-1577223625816-7546f13df25d?auto=format&fit=crop&w=800&q=80',
                amenities: ['Grandstand Berbumbung', 'Bilik Persidangan Media', 'Lampu Kejohanan 1500 Lux', 'Surau & Tandas Awam'],
                badge: 'Prestij'
            },
            {
                id: 'kbs-7',
                title: 'Kolam Latihan & Rekreasi Paroi',
                category: 'Kolam Renang',
                location: 'Pusat Akuatik Paroi, Negeri Sembilan',
                pricePerHour: 70,
                capacity: 100,
                surface: 'Kolam Kedalaman Boleh Laras (1.2m - 2.0m)',
                description: 'Kolam renang berukuran 25m berserta kawasan kolam cetek rekreasi sesuai untuk sesi latihan kelab dan pengajaran asas renang.',
                imageUrl: 'https://images.unsplash.com/photo-1519315901367-f34ff9154487?auto=format&fit=crop&w=800&q=80',
                amenities: ['Kolam Kanak-Kanak asing', 'Jaket Keselamatan Ditawarkan', 'Kantin'],
                badge: null
            },
            {
                id: 'kbs-8',
                title: 'Gelanggang Futsal Terbuka Polimer Paroi',
                category: 'Futsal',
                location: 'Kompleks Sukan Komuniti Paroi, Negeri Sembilan',
                pricePerHour: 50,
                capacity: 20,
                surface: 'Lantai Hardcourt Polimer Anti-Slip',
                description: 'Gelanggang futsal lantai gelanggang serbaguna polimer berturap sesuai untuk latihan harian dan perlawanan persahabatan belia.',
                imageUrl: 'https://images.unsplash.com/photo-1529900748604-07564a03e7a6?auto=format&fit=crop&w=800&q=80',
                amenities: ['Pencahayaan Asas', 'Tiang Gol Rasmi Futsal'],
                badge: 'Ekonomi'
            }
        ];

        // GLOBAL APP STATE
        let currentUser = null;
        let userBookings = [];
        let selectedSpaceForBooking = null;

        // INITIALIZATION ON LOAD
        window.onload = function() {
            loadUserSession();
            renderCategoryChips();
            renderSpaces();
            setupFilterListeners();
            updateBookingBadge();
            
            // Set min date for booking to today
            const today = new Date().toISOString().split('T')[0];
            document.getElementById('book-date').min = today;
            document.getElementById('book-date').value = today;
        };

        // USER SESSION MANAGEMENT
        function loadUserSession() {
            const savedUser = localStorage.getItem('kbs_user');
            if (savedUser) {
                currentUser = JSON.parse(savedUser);
                updateAuthUI();
            }
            loadUserBookings();
        }

        function updateAuthUI() {
            const loggedOutView = document.getElementById('nav-logged-out');
            const loggedInView = document.getElementById('nav-logged-in');
            
            if (currentUser) {
                loggedOutView.classList.add('hidden');
                loggedInView.classList.remove('hidden');
                
                document.getElementById('user-display-name').innerText = currentUser.name;
                document.getElementById('user-display-role').innerText = currentUser.role || 'Pengguna KBS';
                
                // Get initials
                const initials = currentUser.name.split(' ').map(n => n[0]).join('').substring(0, 2).toUpperCase();
                document.getElementById('user-avatar-initials').innerText = initials || 'KBS';
            } else {
                loggedOutView.classList.remove('hidden');
                loggedInView.classList.add('hidden');
            }
        }

        function handleLogout() {
            currentUser = null;
            localStorage.removeItem('kbs_user');
            updateAuthUI();
            loadUserBookings();
            showToast('Anda telah berjaya log keluar.', 'info');
        }

        // AUTH MODAL LOGIC
        function openAuthModal(tab = 'login') {
            document.getElementById('auth-modal').classList.remove('hidden');
            switchAuthTab(tab);
        }

        function closeAuthModal() {
            document.getElementById('auth-modal').classList.add('hidden');
        }

        function switchAuthTab(tab) {
            const loginForm = document.getElementById('form-login');
            const signupForm = document.getElementById('form-signup');
            const loginBtn = document.getElementById('tab-btn-login');
            const signupBtn = document.getElementById('tab-btn-signup');

            if (tab === 'login') {
                loginForm.classList.remove('hidden');
                signupForm.classList.add('hidden');
                loginBtn.className = "flex-1 py-3 text-xs font-bold text-amber-600 border-b-2 border-amber-600 transition-all";
                signupBtn.className = "flex-1 py-3 text-xs font-bold text-slate-500 hover:text-slate-800 border-b-2 border-transparent transition-all";
            } else {
                loginForm.classList.add('hidden');
                signupForm.classList.remove('hidden');
                signupBtn.className = "flex-1 py-3 text-xs font-bold text-amber-600 border-b-2 border-amber-600 transition-all";
                loginBtn.className = "flex-1 py-3 text-xs font-bold text-slate-500 hover:text-slate-800 border-b-2 border-transparent transition-all";
            }
        }

        function handleLoginSubmit(e) {
            e.preventDefault();
            const email = document.getElementById('login-email').value;
            const name = email.split('@')[0].replace('.', ' ');

            currentUser = {
                email: email,
                name: name.charAt(0).toUpperCase() + name.slice(1),
                role: 'Ahli Berdaftar'
            };

            localStorage.setItem('kbs_user', JSON.stringify(currentUser));
            updateAuthUI();
            closeAuthModal();
            loadUserBookings();
            showToast(`Selamat kembali, ${currentUser.name}!`, 'success');
        }

        function handleSignupSubmit(e) {
            e.preventDefault();
            const name = document.getElementById('signup-name').value;
            const email = document.getElementById('signup-email').value;
            const role = document.getElementById('signup-role').value;

            currentUser = {
                name: name,
                email: email,
                role: role
            };

            localStorage.setItem('kbs_user', JSON.stringify(currentUser));
            updateAuthUI();
            closeAuthModal();
            loadUserBookings();
            showToast(`Akaun ${role} berjaya didaftarkan! Selamat datang, ${name}.`, 'success');
        }

        // NAVIGATION TABS
        function switchTab(tabId) {
            const exploreTab = document.getElementById('explore-tab');
            const bookingsTab = document.getElementById('bookings-tab');
            const navExploreBtn = document.getElementById('nav-explore-btn');
            const navBookingsBtn = document.getElementById('nav-bookings-btn');

            if (tabId === 'explore') {
                exploreTab.classList.remove('hidden');
                bookingsTab.classList.add('hidden');
                navExploreBtn.className = "px-3 sm:px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold transition-all text-amber-500 bg-slate-800 shadow-sm";
                navBookingsBtn.className = "px-3 sm:px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold transition-all text-slate-400 hover:text-white relative";
            } else if (tabId === 'bookings') {
                exploreTab.classList.add('hidden');
                bookingsTab.classList.remove('hidden');
                navBookingsBtn.className = "px-3 sm:px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold transition-all text-amber-500 bg-slate-800 shadow-sm relative";
                navExploreBtn.className = "px-3 sm:px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold transition-all text-slate-400 hover:text-white";
                renderBookings();
            }
        }

        // RENDER CATEGORY CHIPS
        function renderCategoryChips() {
            const categories = [
                { id: 'all', label: 'Semua Kemudahan', icon: 'fa-cubes' },
                { id: 'Centre Court', label: 'Centre Court', icon: 'fa-basketball' },
                { id: 'Stadium', label: 'Stadium', icon: 'fa-building-columns' },
                { id: 'Kolam Renang', label: 'Kolam Renang', icon: 'fa-person-swimming' },
                { id: 'Futsal', label: 'Futsal', icon: 'fa-futbol' }
            ];

            const container = document.getElementById('quick-category-chips');
            container.innerHTML = categories.map(c => `
                <button onclick="filterByCategory('${c.id}')" class="px-4 py-2 rounded-full text-xs font-bold transition-all flex items-center gap-2 bg-slate-900/80 hover:bg-amber-600 border border-slate-700 text-white shadow-sm">
                    <i class="fa-solid ${c.icon} text-amber-400"></i> ${c.label}
                </button>
            `).join('');
        }

        function filterByCategory(catId) {
            document.getElementById('filter-category').value = catId;
            renderSpaces();
        }

        // FILTER & RENDER SPACES
        function setupFilterListeners() {
            document.getElementById('filter-keyword').addEventListener('input', renderSpaces);
            document.getElementById('filter-category').addEventListener('change', renderSpaces);
            
            const capInput = document.getElementById('filter-capacity');
            capInput.addEventListener('input', (e) => {
                document.getElementById('capacity-value').innerText = `${e.target.value} Orang`;
                renderSpaces();
            });

            const priceInput = document.getElementById('filter-price');
            priceInput.addEventListener('input', (e) => {
                document.getElementById('price-value').innerText = `RM ${e.target.value}/jam`;
                renderSpaces();
            });
        }

        function resetFilters() {
            document.getElementById('filter-keyword').value = '';
            document.getElementById('filter-category').value = 'all';
            document.getElementById('filter-capacity').value = 1;
            document.getElementById('capacity-value').innerText = '1 Orang';
            document.getElementById('filter-price').value = 800;
            document.getElementById('price-value').innerText = 'RM 800/jam';
            renderSpaces();
            showToast('Penapis telah diset semula', 'info');
        }

        function renderSpaces() {
            const keyword = document.getElementById('filter-keyword').value.toLowerCase();
            const category = document.getElementById('filter-category').value;
            const minCap = parseInt(document.getElementById('filter-capacity').value) || 0;
            const maxPrice = parseInt(document.getElementById('filter-price').value) || 1000;

            const filtered = SPACES_DATA.filter(space => {
                const matchKeyword = space.title.toLowerCase().includes(keyword) || space.location.toLowerCase().includes(keyword);
                const matchCategory = category === 'all' || space.category === category;
                const matchCapacity = space.capacity >= minCap;
                const matchPrice = space.pricePerHour <= maxPrice;
                return matchKeyword && matchCategory && matchCapacity && matchPrice;
            });

            const grid = document.getElementById('spaces-grid');
            const emptyState = document.getElementById('empty-results');
            document.getElementById('results-count').innerText = `Menampilkan ${filtered.length} kemudahan sukan KBS`;

            if (filtered.length === 0) {
                grid.innerHTML = '';
                emptyState.classList.remove('hidden');
                return;
            }

            emptyState.classList.add('hidden');
            grid.innerHTML = filtered.map(space => `
                <div class="bg-white rounded-2xl overflow-hidden border border-slate-200 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col group">
                    
                    <!-- Card Media -->
                    <div class="relative h-52 overflow-hidden bg-slate-100">
                        <img src="${space.imageUrl}" alt="${space.title}" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" onerror="this.src='https://placehold.co/600x400/1e293b/fff?text=Kemudahan+KBS'">
                        
                        <span class="absolute top-3 left-3 bg-slate-900/80 backdrop-blur-md text-amber-400 font-bold text-[10px] px-3 py-1 rounded-full uppercase tracking-wider border border-amber-500/30">
                            ${space.category}
                        </span>

                        ${space.badge ? `
                            <span class="absolute top-3 right-3 bg-amber-600 text-white font-extrabold text-[10px] px-2.5 py-1 rounded-md shadow-md">
                                ${space.badge}
                            </span>
                        ` : ''}

                        <div class="absolute bottom-3 left-3 bg-slate-950/80 backdrop-blur-md px-3 py-1 rounded-xl text-white font-black text-sm">
                            RM ${space.pricePerHour} <span class="text-[10px] font-normal text-slate-300">/ jam</span>
                        </div>
                    </div>

                    <!-- Card Body -->
                    <div class="p-5 flex-grow flex flex-col justify-between">
                        <div>
                            <h3 class="text-base font-bold text-slate-900 group-hover:text-amber-600 transition-colors line-clamp-1">
                                ${space.title}
                            </h3>
                            <p class="text-xs text-slate-500 mt-1 flex items-center gap-1">
                                <i class="fa-solid fa-location-dot text-amber-500"></i> ${space.location}
                            </p>
                            <p class="text-xs text-slate-600 mt-3 line-clamp-2 leading-relaxed">
                                ${space.description}
                            </p>
                        </div>

                        <div class="mt-4 pt-4 border-t border-slate-100">
                            <div class="flex items-center justify-between text-xs text-slate-500 mb-4">
                                <span class="flex items-center gap-1 font-medium"><i class="fa-solid fa-users text-slate-400"></i> Kapasiti: <strong>${space.capacity} pax</strong></span>
                                <span class="flex items-center gap-1 font-medium"><i class="fa-solid fa-shield text-slate-400"></i> <strong>KBS Verified</strong></span>
                            </div>

                            <button onclick="openBookingDrawer('${space.id}')" class="w-full py-2.5 bg-slate-900 hover:bg-amber-600 text-white font-bold rounded-xl text-xs shadow-md transition-all flex items-center justify-center gap-2">
                                <i class="fa-solid fa-calendar-plus"></i> Semak & Tempah
                            </button>
                        </div>
                    </div>

                </div>
            `).join('');
        }

        // BOOKING DRAWER LOGIC
        function openBookingDrawer(spaceId) {
            selectedSpaceForBooking = SPACES_DATA.find(s => s.id === spaceId);
            if (!selectedSpaceForBooking) return;

            document.getElementById('drawer-space-title').innerText = selectedSpaceForBooking.title;
            document.getElementById('drawer-space-category').innerText = selectedSpaceForBooking.category;
            document.getElementById('drawer-space-location').innerHTML = `<i class="fa-solid fa-location-dot text-amber-500 mr-1"></i> ${selectedSpaceForBooking.location}`;
            document.getElementById('drawer-space-price').innerText = `RM ${selectedSpaceForBooking.pricePerHour} / jam`;
            document.getElementById('drawer-space-desc').innerText = selectedSpaceForBooking.description;
            document.getElementById('drawer-space-capacity').innerText = `${selectedSpaceForBooking.capacity} Pemain / Pengunjung`;
            document.getElementById('drawer-space-surface').innerText = selectedSpaceForBooking.surface;
            document.getElementById('drawer-space-img').src = selectedSpaceForBooking.imageUrl;

            // Render Amenities
            const amenitiesContainer = document.getElementById('drawer-amenities-list');
            amenitiesContainer.innerHTML = selectedSpaceForBooking.amenities.map(a => `
                <span class="px-3 py-1 bg-slate-100 text-slate-700 rounded-lg text-xs font-semibold flex items-center gap-1.5 border border-slate-200">
                    <i class="fa-solid fa-check text-amber-600"></i> ${a}
                </span>
            `).join('');

            calculateBookingTotal();
            document.getElementById('booking-drawer').classList.remove('hidden');
        }

        function closeBookingDrawer() {
            document.getElementById('booking-drawer').classList.add('hidden');
            selectedSpaceForBooking = null;
        }

        function calculateBookingTotal() {
            if (!selectedSpaceForBooking) return;

            const startTime = document.getElementById('book-start-time').value;
            const endTime = document.getElementById('book-end-time').value;

            const startHour = parseInt(startTime.split(':')[0]);
            const endHour = parseInt(endTime.split(':')[0]);

            let hours = endHour - startHour;
            if (hours <= 0) hours = 1; // Default min 1 hour fallback calculation

            let total = hours * selectedSpaceForBooking.pricePerHour;

            // Check Addons
            if (document.getElementById('addon-lighting').checked) {
                total += (30 * hours);
            }
            if (document.getElementById('addon-scoreboard').checked) {
                total += 50;
            }

            document.getElementById('summary-total-price').innerText = `RM ${total.toFixed(2)}`;
            document.getElementById('summary-hours-count').innerText = `${hours} jam masa sewaan dipilih`;
        }

        function handleConfirmBooking(e) {
            e.preventDefault();

            if (!currentUser) {
                showToast('Sila log masuk atau daftar akaun untuk membuat tempahan.', 'warning');
                openAuthModal('login');
                return;
            }

            const date = document.getElementById('book-date').value;
            const startTime = document.getElementById('book-start-time').value;
            const endTime = document.getElementById('book-end-time').value;
            const guests = document.getElementById('book-guests').value;
            const totalPrice = document.getElementById('summary-total-price').innerText;

            const newBooking = {
                id: 'KBS-REF-' + Math.floor(100000 + Math.random() * 900000),
                userEmail: currentUser.email,
                userName: currentUser.name,
                spaceTitle: selectedSpaceForBooking.title,
                spaceCategory: selectedSpaceForBooking.category,
                spaceLocation: selectedSpaceForBooking.location,
                date: date,
                startTime: startTime,
                endTime: endTime,
                guests: guests,
                totalPrice: totalPrice,
                status: 'Disahkan',
                createdAt: new Date().toLocaleDateString('ms-MY')
            };

            // Save booking
            userBookings.unshift(newBooking);
            saveUserBookings();

            closeBookingDrawer();
            showToast(`Tempahan Berjaya! No Rujukan: ${newBooking.id}`, 'success');
            switchTab('bookings');
        }

        // BOOKINGS STORAGE & RENDER
        function saveUserBookings() {
            localStorage.setItem('kbs_bookings', JSON.stringify(userBookings));
            updateBookingBadge();
        }

        function loadUserBookings() {
            const saved = localStorage.getItem('kbs_bookings');
            if (saved) {
                const allBookings = JSON.parse(saved);
                // Filter by logged-in user if logged in
                if (currentUser) {
                    userBookings = allBookings.filter(b => b.userEmail === currentUser.email);
                } else {
                    userBookings = [];
                }
            } else {
                userBookings = [];
            }
            updateBookingBadge();
        }

        function updateBookingBadge() {
            const badge = document.getElementById('booking-badge');
            if (userBookings.length > 0) {
                badge.innerText = userBookings.length;
                badge.classList.remove('hidden');
            } else {
                badge.classList.add('hidden');
            }
        }

        function renderBookings() {
            const container = document.getElementById('bookings-list');
            const emptyState = document.getElementById('empty-bookings');

            if (userBookings.length === 0) {
                container.innerHTML = '';
                emptyState.classList.remove('hidden');
                return;
            }

            emptyState.classList.add('hidden');
            container.innerHTML = userBookings.map(b => `
                <div class="bg-white rounded-2xl p-6 border border-slate-200 shadow-sm flex flex-col md:flex-row items-start md:items-center justify-between gap-6 hover:border-amber-400 transition-all">
                    <div class="space-y-2 flex-grow">
                        <div class="flex items-center gap-3">
                            <span class="px-3 py-1 bg-amber-50 text-amber-700 font-bold text-xs rounded-full border border-amber-200">
                                ${b.spaceCategory}
                            </span>
                            <span class="text-xs font-mono font-bold text-slate-400">${b.id}</span>
                            <span class="px-2.5 py-0.5 bg-emerald-100 text-emerald-700 text-[10px] font-extrabold rounded-md">
                                <i class="fa-solid fa-circle-check mr-1"></i> ${b.status}
                            </span>
                        </div>
                        <h3 class="text-lg font-bold text-slate-900">${b.spaceTitle}</h3>
                        <p class="text-xs text-slate-500"><i class="fa-solid fa-location-dot text-amber-500 mr-1"></i> ${b.spaceLocation}</p>
                        
                        <div class="flex flex-wrap gap-4 pt-2 text-xs font-medium text-slate-600">
                            <span><i class="fa-solid fa-calendar text-slate-400 mr-1"></i> ${b.date}</span>
                            <span><i class="fa-solid fa-clock text-slate-400 mr-1"></i> ${b.startTime} - ${b.endTime}</span>
                            <span><i class="fa-solid fa-user-group text-slate-400 mr-1"></i> ${b.guests} Pemain</span>
                        </div>
                    </div>

                    <div class="flex md:flex-col items-end justify-between w-full md:w-auto border-t md:border-t-0 pt-4 md:pt-0 border-slate-100">
                        <div class="text-left md:text-right">
                            <span class="text-[10px] uppercase font-bold text-slate-400 block">Jumlah Bayaran</span>
                            <span class="text-xl font-black text-amber-600">${b.totalPrice}</span>
                        </div>
                        <button onclick="cancelBooking('${b.id}')" class="mt-2 text-xs text-red-600 font-bold hover:text-red-800 transition-colors flex items-center gap-1">
                            <i class="fa-solid fa-trash"></i> Batalkan Tempahan
                        </button>
                    </div>
                </div>
            `).join('');
        }

        function cancelBooking(bookingId) {
            if (confirm('Adakah anda pasti mahu membatalkan tempahan kemudahan sukan ini?')) {
                userBookings = userBookings.filter(b => b.id !== bookingId);
                // Save updated array back
                const saved = JSON.parse(localStorage.getItem('kbs_bookings') || '[]');
                const updatedAll = saved.filter(b => b.id !== bookingId);
                localStorage.setItem('kbs_bookings', JSON.stringify(updatedAll));
                
                updateBookingBadge();
                renderBookings();
                showToast('Tempahan telah berjaya dibatalkan.', 'info');
            }
        }

        // TOAST NOTIFICATIONS SYSTEM
        function showToast(message, type = 'info') {
            const container = document.getElementById('toast-container');
            const toast = document.createElement('div');
            
            const bgColors = {
                success: 'bg-emerald-900 border-emerald-500 text-white',
                warning: 'bg-amber-900 border-amber-500 text-white',
                info: 'bg-slate-900 border-slate-700 text-white'
            };

            const icons = {
                success: 'fa-circle-check text-emerald-400',
                warning: 'fa-triangle-exclamation text-amber-400',
                info: 'fa-circle-info text-amber-400'
            };

            toast.className = `pointer-events-auto flex items-center gap-3 px-4 py-3 rounded-2xl border shadow-xl text-xs font-semibold transform transition-all duration-300 translate-y-2 opacity-0 ${bgColors[type] || bgColors.info}`;
            toast.innerHTML = `
                <i class="fa-solid ${icons[type]} text-sm"></i>
                <span>${message}</span>
            `;

            container.appendChild(toast);

            setTimeout(() => {
                toast.classList.remove('translate-y-2', 'opacity-0');
            }, 10);

            setTimeout(() => {
                toast.classList.add('opacity-0', 'translate-y-2');
                setTimeout(() => toast.remove(), 300);
            }, 3500);
        }
    </script>
</body>
</html>
