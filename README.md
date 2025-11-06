<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tính Giá Khung Ảnh NGOCTHUANART</title>
    <!-- Load Tailwind CSS via CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- LOAD FONT POPPINS (Đã xóa liên kết tải font Poppins) -->

    <style>
        /* Sử dụng font mặc định của Tailwind (Inter/Sans-serif) */
        body {
            /* Đã hoàn nguyên về mặc định (Inter/Sans-serif) */
            font-family: ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
            background-color: #f3f4f6;
        }
        input[type="number"]::-webkit-inner-spin-button, 
        input[type="number"]::-webkit-outer-spin-button { 
            -webkit-appearance: none; 
            margin: 0; 
        }
        input[type="number"] {
            -moz-appearance: textfield;
        }
    </style>
</head>
<body>

<div id="app" class="min-h-screen flex justify-center p-4">
    <div class="w-full max-w-md bg-white rounded-2xl shadow-2xl overflow-hidden md:my-8">
        
        <!-- Header -->
        <div class="bg-indigo-600 p-5 shadow-lg flex justify-between items-center">
            <h1 class="text-xl font-bold text-white flex items-center">
                <!-- DollarSign Icon -->
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6 mr-2"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
                Tính Giá NGOCTHUANART
            </h1>
            <button id="resetButton" class="text-white p-2 rounded-full hover:bg-indigo-700 transition-colors" title="Đặt lại các giá trị">
                <!-- RefreshCcw Icon -->
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5"><path d="M21 12a9 9 0 0 0-9-9 9.75 9.75 0 0 0-6.76 2.76L3 7"></path><path d="M3 3v4h4"></path><path d="M3 12a9 9 0 0 0 9 9 9.75 9.75 0 0 0 6.76-2.76L21 17"></path><path d="M21 21v-4h-4"></path></svg>
            </button>
        </div>

        <!-- Thân ứng dụng - Kéo xuống được -->
        <div class="p-4 space-y-6">

            <!-- NHẬP KÍCH THƯỚC -->
            <div class="space-y-3">
                <h2 class="text-lg font-bold text-gray-800 border-b pb-2 flex items-center">
                    <!-- Ruler Icon -->
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4 mr-2 text-blue-500"><path d="M1 10h4v14H1z"></path><path d="M19 10h4v14h-4z"></path><path d="M12 1h-2v4h-2v-4h-2v4h-2v-4h-2v4h-2v-4H0v4h2v20h20v-20h2v-4h-2v4h-2v-4h-2v4h-2v-4h-2v4h-2v-4h-2v4h-2v-4H6z"></path></svg>
                    1. Kích Thước 2 Cạnh (CM)
                </h2>
                <div class="grid grid-cols-2 gap-3">
                    <!-- Dài (cm) -->
                    <div class="bg-white/90 p-4 rounded-xl shadow-md transition-all duration-300 hover:shadow-lg">
                        <div class="flex items-center text-blue-600 mb-2">
                            <!-- Ruler Icon -->
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2"><path d="M21.3 15.3l-5.6-5.6"></path><path d="M15.3 21.3l-5.6-5.6"></path><path d="M7 10h3v4h-3z"></path><path d="M14 10h3v4h-3z"></path><path d="M12 21a9 9 0 0 1-9-9c0-4.97 4.03-9 9-9s9 4.03 9 9-4.03 9-9 9z"></path></svg>
                            <label class="text-sm font-semibold text-gray-700">Dài (cm)</label>
                        </div>
                        <div class="flex items-center border border-gray-300 rounded-lg overflow-hidden">
                            <input type="number" id="lengthCm" class="flex-grow p-2 text-base font-medium text-gray-800 focus:outline-none bg-transparent" min="0" placeholder="60 (Mặc định)" value="60">
                            <span class="p-2 bg-gray-100 text-sm text-gray-500 border-l border-gray-300">cm</span>
                        </div>
                    </div>
                    <!-- Rộng (cm) -->
                    <div class="bg-white/90 p-4 rounded-xl shadow-md transition-all duration-300 hover:shadow-lg">
                        <div class="flex items-center text-blue-600 mb-2">
                            <!-- Ruler Icon -->
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2"><path d="M21.3 15.3l-5.6-5.6"></path><path d="M15.3 21.3l-5.6-5.6"></path><path d="M7 10h3v4h-3z"></path><path d="M14 10h3v4h-3z"></path><path d="M12 21a9 9 0 0 1-9-9c0-4.97 4.03-9 9-9s9 4.03 9 9-4.03 9-9 9z"></path></svg>
                            <label class="text-sm font-semibold text-gray-700">Rộng (cm)</label>
                        </div>
                        <div class="flex items-center border border-gray-300 rounded-lg overflow-hidden">
                            <input type="number" id="widthCm" class="flex-grow p-2 text-base font-medium text-gray-800 focus:outline-none bg-transparent" min="0" placeholder="90 (Mặc định)" value="90">
                            <span class="p-2 bg-gray-100 text-sm text-gray-500 border-l border-gray-300">cm</span>
                        </div>
                    </div>
                </div>
                <!-- Cộng Cạnh (Waste Factor - M) -->
                <div class="bg-white/90 p-4 rounded-xl shadow-md transition-all duration-300 hover:shadow-lg">
                    <div class="flex items-center text-blue-600 mb-2">
                        <!-- Package Icon (used for Waste Factor) -->
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2"><path d="M21 10V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v2"></path><path d="M3 14v-4h18v4"></path><path d="M18.88 12.56L12 16.51L5.12 12.56"></path><path d="M12 22.08V16.51"></path><path d="M21 14v-4"></path><path d="M3 14v-4"></path><path d="M3 10v6a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4a2 2 0 0 0 1-1.73v-6"></path></svg>
                        <label class="text-sm font-semibold text-gray-700">Cộng Cạnh (Waste Factor - M)</label>
                    </div>
                    <div class="flex items-center border border-gray-300 rounded-lg overflow-hidden">
                        <input type="number" step="0.01" id="wasteFactor" class="flex-grow p-2 text-base font-medium text-gray-800 focus:outline-none bg-transparent" min="0" placeholder="0.5 (Mặc định)" value="0.5">
                        <span class="p-2 bg-gray-100 text-sm text-gray-500 border-l border-gray-300">m</span>
                    </div>
                </div>
            </div>

            <!-- CẤU HÌNH VẬT TƯ -->
            <div class="space-y-4">
                <h2 class="text-lg font-bold text-gray-800 border-b pb-2 flex items-center">
                    <!-- Package Icon -->
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4 mr-2 text-blue-500"><rect width="20" height="15" x="2" y="7" rx="2" ry="2"></rect><path d="M17 2h3a2 2 0 0 1 2 2v2"></path><path d="M2 4a2 2 0 0 1 2-2h3"></path><path d="M22 17v3a2 2 0 0 1-2 2h-3"></path><path d="M7 22H4a2 2 0 0 1-2-2v-3"></path></svg>
                    2. Giá Vật Tư
                </h2>

                <!-- Giá Khung -->
                <div class="bg-white/90 p-4 rounded-xl shadow-md transition-all duration-300 hover:shadow-lg">
                    <div class="flex items-center text-blue-600 mb-2">
                        <!-- DollarSign Icon -->
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
                        <label class="text-sm font-semibold text-gray-700">Giá Khung/m</label>
                    </div>
                    <div class="flex items-center border border-gray-300 rounded-lg overflow-hidden">
                        <input type="number" id="framePricePerM" class="flex-grow p-2 text-base font-medium text-gray-800 focus:outline-none bg-transparent" min="0" placeholder="20000 (Mặc định)" value="20000">
                        <span class="p-2 bg-gray-100 text-sm text-gray-500 border-l border-gray-300">VNĐ</span>
                    </div>
                </div>
                
                <!-- Loại Ruột và Giá M2 -->
                <div class="space-y-3">
                    <div class="flex space-x-2">
                        <button id="infillGlassBtn" data-type="glass" class="flex-1 p-3 text-center rounded-lg font-semibold transition-all button-infill bg-green-500 text-white shadow-md">
                        KÍNH + VÁN
                        </button>
                        <button id="infillMicaBtn" data-type="mica" class="flex-1 p-3 text-center rounded-lg font-semibold transition-all button-infill bg-gray-200 text-gray-700 hover:bg-gray-300">
                        MICA + VÁN
                        </button>
                    </div>
                    
                    <div id="infillPriceInputContainer">
                        <!-- Input cho Giá Kính + Ván / m² (Mặc định hiển thị) -->
                        <div id="glassInput" class="bg-white/90 p-4 rounded-xl shadow-md transition-all duration-300 hover:shadow-lg">
                            <div class="flex items-center text-blue-600 mb-2">
                                <!-- DollarSign Icon -->
                                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
                                <label class="text-sm font-semibold text-gray-700">Giá Kính + Ván / m²</label>
                            </div>
                            <div class="flex items-center border border-gray-300 rounded-lg overflow-hidden">
                                <input type="number" id="glassM2Price" class="flex-grow p-2 text-base font-medium text-gray-800 focus:outline-none bg-transparent" min="0" placeholder="290000 (Mặc định)" value="290000">
                                <span class="p-2 bg-gray-100 text-sm text-gray-500 border-l border-gray-300">VNĐ</span>
                            </div>
                        </div>

                        <!-- Input cho Giá Mica + Ván / m² (Ẩn) -->
                        <div id="micaInput" class="bg-white/90 p-4 rounded-xl shadow-md transition-all duration-300 hover:shadow-lg hidden">
                            <div class="flex items-center text-blue-600 mb-2">
                                <!-- DollarSign Icon -->
                                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
                                <label class="text-sm font-semibold text-gray-700">Giá Mica + Ván / m²</label>
                            </div>
                            <div class="flex items-center border border-gray-300 rounded-lg overflow-hidden">
                                <input type="number" id="micaM2Price" class="flex-grow p-2 text-base font-medium text-gray-800 focus:outline-none bg-transparent" min="0" placeholder="350000 (Mặc định)" value="350000">
                                <span class="p-2 bg-gray-100 text-sm text-gray-500 border-l border-gray-300">VNĐ</span>
                            </div>
                        </div>

                    </div>
                </div>

                <!-- Kênh Bán -->
                <div class="space-y-2">
                    <h3 class="text-sm font-semibold text-gray-700 flex items-center">
                        <!-- ShoppingBag Icon -->
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4 mr-1 text-red-500"><path d="M6 2L3 6v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V6l-3-4z"></path><line x1="3" y1="6" x2="21" y2="6"></line><path d="M16 10a4 4 0 0 1-8 0"></path></svg>
                        Kênh Bán Hàng
                    </h3>
                    <div class="flex space-x-2">
                        <button id="channelStoreBtn" data-channel="store" class="flex-1 p-3 text-center rounded-lg font-semibold transition-all button-channel bg-red-500 text-white shadow-md">
                        CỬA HÀNG
                        </button>
                        <button id="channelTmdtBtn" data-channel="tmđt" class="flex-1 p-3 text-center rounded-lg font-semibold transition-all button-channel bg-gray-200 text-gray-700 hover:bg-gray-300">
                        TMDT (25%)
                        </button>
                    </div>
                    <div id="tmđtInfo" class="text-xs text-red-600 flex items-center bg-red-50 p-2 rounded-lg hidden">
                        <!-- Info Icon -->
                        <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-3 h-3 mr-1"><circle cx="12" cy="12" r="10"></circle><line x1="12" y1="16" x2="12" y2="12"></line><line x1="12" y1="8" x2="12.01" y2="8"></line></svg>
                        Giá TMDT được tính thêm Markup 25%
                    </div>
                </div>
            </div>

            <!-- KẾT QUẢ -->
            <div class="space-y-4 pt-4 border-t border-gray-200">
                <h2 class="text-lg font-bold text-gray-800 flex items-center">
                    <!-- TrendingUp Icon -->
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4 mr-2 text-indigo-600"><polyline points="22 7 13.5 15.5 8.5 10.5 2 17"></polyline><polyline points="18 7 22 7 22 11"></polyline></svg>
                    3. Kết Quả Tính Toán
                </h2>
                
                <!-- Giá Khung và Ruột -->
                <div class="grid grid-cols-2 gap-3">
                    <!-- Giá Khung -->
                    <div id="resultFrameCost" class="p-4 rounded-xl shadow-inner bg-gray-100/80 text-gray-800">
                        <div class="flex items-center mb-1">
                            <!-- DollarSign Icon -->
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2 text-indigo-500"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
                            <h3 class="text-sm font-medium text-gray-600">Giá Khung</h3>
                        </div>
                        <p class="text-2xl font-bold transition-transform duration-300 text-gray-900">
                            0 VNĐ
                        </p>
                    </div>
                    <!-- Giá Ruột -->
                    <div id="resultInfillCost" class="p-4 rounded-xl shadow-inner bg-gray-100/80 text-gray-800">
                        <div class="flex items-center mb-1">
                            <!-- DollarSign Icon -->
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2 text-indigo-500"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
                            <h3 id="infillCostTitle" class="text-sm font-medium text-gray-600">Giá Kính + Ván</h3>
                        </div>
                        <p class="text-2xl font-bold transition-transform duration-300 text-gray-900">
                            0 VNĐ
                        </p>
                    </div>
                </div>
                
                <!-- Giá Gốc và Markup -->
                <div class="grid grid-cols-2 gap-3">
                    <!-- GIÁ GỐC -->
                    <div id="resultBasePrice" class="p-4 rounded-xl shadow-inner bg-gray-100/80 text-gray-800">
                        <div class="flex items-center mb-1">
                            <!-- DollarSign Icon -->
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2 text-indigo-500"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
                            <h3 class="text-sm font-medium text-gray-600">GIÁ GỐC (Chưa Markup)</h3>
                        </div>
                        <p class="text-2xl font-bold transition-transform duration-300 text-gray-900">
                            0 VNĐ
                        </p>
                    </div>
                    <!-- Markup -->
                    <div id="resultMarkup" class="p-4 rounded-xl shadow-inner bg-gray-100/80 text-gray-800">
                        <div class="flex items-center mb-1">
                            <!-- TrendingUp Icon -->
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2 text-indigo-500"><polyline points="22 7 13.5 15.5 8.5 10.5 2 17"></polyline><polyline points="18 7 22 7 22 11"></polyline></svg>
                            <h3 id="markupTitle" class="text-sm font-medium text-gray-600">Markup (0%)</h3>
                        </div>
                        <p class="text-2xl font-bold transition-transform duration-300 text-gray-900">
                            0 VNĐ
                        </p>
                    </div>
                </div>

                <!-- GIÁ CUỐI CÙNG -->
                <div id="resultFinalPrice" class="p-4 rounded-xl shadow-inner bg-indigo-600 text-white shadow-indigo-800/50">
                    <div class="flex items-center mb-1">
                        <!-- DollarSign Icon -->
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 mr-2 text-white"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
                        <h3 id="finalPriceTitle" class="text-sm font-medium text-indigo-200">GIÁ BÁN CUỐI CÙNG (CỬA HÀNG)</h3>
                    </div>
                    <p class="text-3xl font-extrabold transition-transform duration-300 text-white">
                        0 VNĐ
                    </p>
                </div>
                
                <!-- Thông số kỹ thuật -->
                <div class="bg-white p-3 rounded-xl border border-gray-200 text-sm text-gray-600 space-y-1">
                    <p>• Chiều Dài Khung (m): <span id="techFrameLength" class="font-mono text-gray-800">0.00 m</span></p>
                    <p>• Diện Tích Ruột (m²): <span id="techAreaM2" class="font-mono text-gray-800">0.0000 m²</span></p>
                </div>
            </div>
        </div>

        <!-- Footer -->
        <div class="p-4 text-center text-xs text-gray-400 border-t mt-4">
            <p>Được phát triên bởi NGOCTHUANART.COM</p>
        </div>
    </div>
</div>

<script>
    // Constants and Default Values
    const DEFAULT_PRICES = {
        FRAME_PRICE_PER_M: 20000,
        GLASS_M2_PRICE: 290000,
        MICA_M2_PRICE: 350000,
        WASTE_FACTOR: 0.5, // Cộng Cạnh
        TMDT_MARKUP_PERCENT: 25, // Markup 25%
    };

    // Global State
    let state = {
        lengthCm: 60,
        widthCm: 90,
        infillType: 'glass',
        wasteFactor: DEFAULT_PRICES.WASTE_FACTOR,
        framePricePerM: DEFAULT_PRICES.FRAME_PRICE_PER_M,
        salesChannel: 'store',
        glassM2Price: DEFAULT_PRICES.GLASS_M2_PRICE,
        micaM2Price: DEFAULT_PRICES.MICA_M2_PRICE,
    };

    // DOM Elements Map
    const DOMElements = {
        lengthCm: document.getElementById('lengthCm'),
        widthCm: document.getElementById('widthCm'),
        wasteFactor: document.getElementById('wasteFactor'),
        framePricePerM: document.getElementById('framePricePerM'),
        glassM2Price: document.getElementById('glassM2Price'),
        micaM2Price: document.getElementById('micaM2Price'),
        glassInput: document.getElementById('glassInput'),
        micaInput: document.getElementById('micaInput'),
        infillGlassBtn: document.getElementById('infillGlassBtn'),
        infillMicaBtn: document.getElementById('infillMicaBtn'),
        channelStoreBtn: document.getElementById('channelStoreBtn'),
        channelTmdtBtn: document.getElementById('channelTmdtBtn'),
        tmđtInfo: document.getElementById('tmđtInfo'),
        resetButton: document.getElementById('resetButton'),
        
        // Results
        resultFrameCost: document.querySelector('#resultFrameCost p'),
        resultInfillCost: document.querySelector('#resultInfillCost p'),
        infillCostTitle: document.getElementById('infillCostTitle'),
        resultBasePrice: document.querySelector('#resultBasePrice p'),
        resultMarkup: document.querySelector('#resultMarkup p'),
        markupTitle: document.getElementById('markupTitle'),
        resultFinalPrice: document.querySelector('#resultFinalPrice p'),
        finalPriceTitle: document.getElementById('finalPriceTitle'),
        techFrameLength: document.getElementById('techFrameLength'),
        techAreaM2: document.getElementById('techAreaM2'),
    };

    // Hàm định dạng tiền tệ Việt Nam Đồng
    function formatCurrency(amount) {
        if (isNaN(amount) || amount === null) return '0 VNĐ';
        return new Intl.NumberFormat('vi-VN', {
            style: 'currency',
            currency: 'VND',
            minimumFractionDigits: 0,
            maximumFractionDigits: 0,
        }).format(amount);
    }

    // Hàm tính toán logic (tương đương useMemo)
    function calculatePrices(s) {
        // Chuyển đổi và xử lý lỗi input
        const lengthM = parseFloat(s.lengthCm) / 100 || 0;
        const widthM = parseFloat(s.widthCm) / 100 || 0;
        const wasteFactorVal = parseFloat(s.wasteFactor) || 0;
        const framePricePerMVal = parseInt(s.framePricePerM) || 0;
        const glassM2PriceVal = parseInt(s.glassM2Price) || 0;
        const micaM2PriceVal = parseInt(s.micaM2Price) || 0;

        // 2. Tính Chiều dài Khung (m)
        // Formula: (Dài_m + Rộng_m) * 2 + WasteFactor
        const frameLength = (lengthM + widthM) * 2 + wasteFactorVal;

        // 3. Tính Giá Khung
        const frameCost = frameLength * framePricePerMVal;

        // 4. Chọn Giá Ruột
        const infillPricePerM2 = s.infillType === 'glass' ? glassM2PriceVal : micaM2PriceVal;

        // 5. Tính Diện tích (m2)
        const areaM2 = lengthM * widthM;

        // 6. Tính Giá Ruột
        const infillCost = areaM2 * infillPricePerM2;

        // 7. Giá Gốc (Giá Khung + Giá Ruột)
        const baseTotalPrice = frameCost + infillCost;

        // 8. Giá Bán Cuối Cùng (Áp dụng Markup)
        let finalPrice = baseTotalPrice;
        let markup = 0;

        if (s.salesChannel === 'tmđt') {
            markup = baseTotalPrice * (DEFAULT_PRICES.TMDT_MARKUP_PERCENT / 100);
            finalPrice = baseTotalPrice + markup;
        }

        // Làm tròn giá bán cuối cùng (lên 1000 VNĐ gần nhất)
        finalPrice = Math.ceil(finalPrice / 1000) * 1000;

        return {
            frameLength: frameLength.toFixed(2),
            areaM2: areaM2 > 0 ? areaM2.toFixed(4) : "0.0000",
            frameCost: Math.round(frameCost),
            infillCost: Math.round(infillCost),
            baseTotalPrice: Math.round(baseTotalPrice),
            markup: Math.round(markup),
            finalPrice: Math.round(finalPrice),
        };
    }

    // Hàm cập nhật DOM dựa trên trạng thái hiện tại
    function renderApp() {
        const results = calculatePrices(state);

        // Cập nhật giao diện nhập liệu
        DOMElements.lengthCm.value = state.lengthCm;
        DOMElements.widthCm.value = state.widthCm;
        DOMElements.wasteFactor.value = state.wasteFactor;
        DOMElements.framePricePerM.value = state.framePricePerM;
        DOMElements.glassM2Price.value = state.glassM2Price;
        DOMElements.micaM2Price.value = state.micaM2Price;

        // Cập nhật giao diện Ruột (Infill Type)
        const isGlass = state.infillType === 'glass';
        DOMElements.glassInput.classList.toggle('hidden', !isGlass);
        DOMElements.micaInput.classList.toggle('hidden', isGlass);

        DOMElements.infillGlassBtn.className = isGlass
            ? 'flex-1 p-3 text-center rounded-lg font-semibold transition-all button-infill bg-green-500 text-white shadow-md'
            : 'flex-1 p-3 text-center rounded-lg font-semibold transition-all button-infill bg-gray-200 text-gray-700 hover:bg-gray-300';
        
        DOMElements.infillMicaBtn.className = !isGlass
            ? 'flex-1 p-3 text-center rounded-lg font-semibold transition-all button-infill bg-green-500 text-white shadow-md'
            : 'flex-1 p-3 text-center rounded-lg font-semibold transition-all button-infill bg-gray-200 text-gray-700 hover:bg-gray-300';

        // Cập nhật giao diện Kênh Bán (Sales Channel)
        const isTMDT = state.salesChannel === 'tmđt';
        DOMElements.tmđtInfo.classList.toggle('hidden', !isTMDT);

        DOMElements.channelStoreBtn.className = isTMDT
            ? 'flex-1 p-3 text-center rounded-lg font-semibold transition-all button-channel bg-gray-200 text-gray-700 hover:bg-gray-300'
            : 'flex-1 p-3 text-center rounded-lg font-semibold transition-all button-channel bg-red-500 text-white shadow-md';
        
        DOMElements.channelTmdtBtn.className = !isTMDT
            ? 'flex-1 p-3 text-center rounded-lg font-semibold transition-all button-channel bg-gray-200 text-gray-700 hover:bg-gray-300'
            : 'flex-1 p-3 text-center rounded-lg font-semibold transition-all button-channel bg-red-500 text-white shadow-md';


        // Cập nhật Kết quả
        DOMElements.resultFrameCost.innerHTML = formatCurrency(results.frameCost);
        DOMElements.infillCostTitle.textContent = isGlass ? 'Giá Kính + Ván' : 'Giá Mica + Ván';
        DOMElements.resultInfillCost.innerHTML = formatCurrency(results.infillCost);
        DOMElements.resultBasePrice.innerHTML = formatCurrency(results.baseTotalPrice);
        
        const markupPercent = isTMDT ? `${DEFAULT_PRICES.TMDT_MARKUP_PERCENT}%` : '0%';
        DOMElements.markupTitle.textContent = `Markup (${markupPercent})`;
        DOMElements.resultMarkup.innerHTML = formatCurrency(results.markup);
        
        const channelName = isTMDT ? 'TMDT' : 'CỬA HÀNG';
        DOMElements.finalPriceTitle.textContent = `GIÁ BÁN CUỐI CÙNG (${channelName})`;
        DOMElements.resultFinalPrice.innerHTML = `<p class="text-3xl font-extrabold transition-transform duration-300 text-white">${formatCurrency(results.finalPrice)}</p>`;
        
        // Cập nhật thông số kỹ thuật
        DOMElements.techFrameLength.textContent = `${results.frameLength} m`;
        DOMElements.techAreaM2.textContent = `${results.areaM2} m²`;
    }

    // Hàm chung để cập nhật trạng thái
    function updateState(key, value) {
        state[key] = value;
        renderApp();
    }

    // Thiết lập Listeners
    function setupListeners() {
        // Input handlers (chỉ cần nghe sự kiện 'input' để cập nhật real-time)
        DOMElements.lengthCm.addEventListener('input', (e) => updateState('lengthCm', e.target.value));
        DOMElements.widthCm.addEventListener('input', (e) => updateState('widthCm', e.target.value));
        DOMElements.wasteFactor.addEventListener('input', (e) => updateState('wasteFactor', e.target.value));
        DOMElements.framePricePerM.addEventListener('input', (e) => updateState('framePricePerM', e.target.value));
        DOMElements.glassM2Price.addEventListener('input', (e) => updateState('glassM2Price', e.target.value));
        DOMElements.micaM2Price.addEventListener('input', (e) => updateState('micaM2Price', e.target.value));

        // Infill Type buttons
        DOMElements.infillGlassBtn.addEventListener('click', () => updateState('infillType', 'glass'));
        DOMElements.infillMicaBtn.addEventListener('click', () => updateState('infillType', 'mica'));

        // Sales Channel buttons
        DOMElements.channelStoreBtn.addEventListener('click', () => updateState('salesChannel', 'store'));
        DOMElements.channelTmdtBtn.addEventListener('click', () => updateState('salesChannel', 'tmđt'));

        // Reset button
        DOMElements.resetButton.addEventListener('click', handleReset);
    }

    // Hàm reset
    function handleReset() {
        state.lengthCm = 60;
        state.widthCm = 90;
        state.infillType = 'glass';
        state.wasteFactor = DEFAULT_PRICES.WASTE_FACTOR;
        state.framePricePerM = DEFAULT_PRICES.FRAME_PRICE_PER_M;
        state.glassM2Price = DEFAULT_PRICES.GLASS_M2_PRICE;
        state.micaM2Price = DEFAULT_PRICES.MICA_M2_PRICE;
        state.salesChannel = 'store';
        renderApp();
    }

    // Khởi tạo ứng dụng khi DOM đã sẵn sàng
    window.onload = function() {
        setupListeners();
        // Render lần đầu tiên để hiển thị giá trị mặc định (60cm x 90cm)
        renderApp(); 
    };
</script>

</body>
</html>
