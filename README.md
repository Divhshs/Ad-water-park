```html
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AD Water Park - Instant Ticket Booking | ₹900 All-Day Pass</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        aqua: {
                            50: '#f0fdfa',
                            100: '#ccfbf1',
                            200: '#99f6e4',
                            400: '#2dd4bf',
                            500: '#14b8a6',
                            600: '#0d9488',
                            700: '#0f766e',
                            800: '#115e59',
                            900: '#134e4a',
                        },
                        splash: {
                            blue: '#0284c7',
                            cyan: '#06b6d4',
                            amber: '#f59e0b',
                            coral: '#f43f5e'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- QR Code Generator Library -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap');
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
        }
        .water-wave-bg {
            background: linear-gradient(135deg, #0284c7 0%, #06b6d4 50%, #14b8a6 100%);
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.92);
            backdrop-filter: blur(14px);
        }
        .ticket-cutout-left, .ticket-cutout-right {
            position: absolute;
            width: 28px;
            height: 28px;
            border-radius: 50%;
            background-color: #f8fafc;
            top: 68%;
            transform: translateY(-50%);
            z-index: 10;
        }
        .ticket-cutout-left { left: -14px; }
        .ticket-cutout-right { right: -14px; }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 antialiased selection:bg-cyan-500 selection:text-white">

    <!-- Top Announcement Bar -->
    <header class="bg-gradient-to-r from-cyan-600 via-sky-600 to-teal-600 text-white text-xs sm:text-sm py-2 px-4 text-center font-medium shadow-sm">
        <span class="inline-flex items-center gap-2">
            <span class="bg-amber-400 text-slate-900 text-xs px-2 py-0.5 rounded-full font-bold uppercase tracking-wider animate-pulse">Special Offer</span>
            Flat Summer Special: All-Day Unlimited Access Pass at just <strong>₹900 / Person</strong>!
        </span>
    </header>

    <!-- Navigation Bar -->
    <nav class="sticky top-0 z-40 bg-white/95 backdrop-blur-md border-b border-slate-200/80 shadow-sm transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <div class="flex items-center gap-3">
                <div class="w-12 h-12 rounded-2xl bg-gradient-to-tr from-cyan-500 to-blue-600 flex items-center justify-center text-white text-2xl shadow-lg shadow-cyan-500/25">
                    <i class="fa-solid fa-water"></i>
                </div>
                <div>
                    <span class="text-2xl font-black tracking-tight text-slate-900 flex items-center gap-1.5">
                        AD <span class="text-cyan-600">WATER</span> PARK
                    </span>
                    <p class="text-xs font-semibold text-slate-500 tracking-wider uppercase -mt-1">Splash & Joy World</p>
                </div>
            </div>

            <div class="hidden md:flex items-center space-x-8 text-sm font-semibold text-slate-600">
                <a href="#attractions" class="hover:text-cyan-600 transition">Attractions</a>
                <a href="#pricing" class="hover:text-cyan-600 transition">Pricing & Inclusions</a>
                <a href="#booking-section" class="hover:text-cyan-600 transition">Book Tickets</a>
                <a href="#faqs" class="hover:text-cyan-600 transition">FAQs</a>
            </div>

            <div class="flex items-center gap-3">
                <a href="#booking-section" class="inline-flex items-center gap-2 bg-gradient-to-r from-cyan-500 to-blue-600 text-white font-bold px-5 py-2.5 rounded-xl shadow-md hover:shadow-cyan-500/40 hover:-translate-y-0.5 transition-all duration-200 text-sm">
                    <i class="fa-solid fa-ticket"></i>
                    <span>Book Pass (₹900)</span>
                </a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative overflow-hidden pt-12 pb-20 lg:pt-20 lg:pb-28 bg-gradient-to-b from-sky-50 via-cyan-50/40 to-slate-50">
        <!-- Floating decorative bubbles -->
        <div class="absolute top-10 left-10 w-44 h-44 bg-cyan-300/30 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute bottom-10 right-10 w-72 h-72 bg-blue-400/20 rounded-full blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid lg:grid-cols-12 gap-12 items-center">
                
                <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                    <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-cyan-100 text-cyan-800 text-xs sm:text-sm font-bold border border-cyan-200">
                        <i class="fa-solid fa-sparkles text-amber-500"></i> The Ultimate Splash Adventure
                    </div>
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold text-slate-900 leading-tight">
                        Beat the Heat with Non-Stop Water Thrills at <span class="bg-gradient-to-r from-cyan-600 to-blue-600 bg-clip-text text-transparent">AD Water Park</span>
                    </h1>
                    <p class="text-base sm:text-lg text-slate-600 max-w-2xl mx-auto lg:mx-0 leading-relaxed">
                        Experience 25+ exhilarating slides, massive wave pool tides, musical rain dance, and calm lazy river lagoons. Premium summer fun for family & friends!
                    </p>

                    <!-- Highlights Badge Row -->
                    <div class="grid grid-cols-2 sm:grid-cols-4 gap-3 pt-2 max-w-xl mx-auto lg:mx-0">
                        <div class="p-3 bg-white rounded-xl shadow-sm border border-slate-200 text-center">
                            <span class="text-2xl font-black text-cyan-600">25+</span>
                            <p class="text-xs text-slate-500 font-medium">Mega Slides</p>
                        </div>
                        <div class="p-3 bg-white rounded-xl shadow-sm border border-slate-200 text-center">
                            <span class="text-2xl font-black text-cyan-600">50K+</span>
                            <p class="text-xs text-slate-500 font-medium">Happy Visitors</p>
                        </div>
                        <div class="p-3 bg-white rounded-xl shadow-sm border border-slate-200 text-center">
                            <span class="text-2xl font-black text-cyan-600">100%</span>
                            <p class="text-xs text-slate-500 font-medium">Treated Clean Water</p>
                        </div>
                        <div class="p-3 bg-white rounded-xl shadow-sm border border-slate-200 text-center">
                            <span class="text-2xl font-black text-cyan-600">₹900</span>
                            <p class="text-xs text-slate-500 font-medium">Flat Price/Person</p>
                        </div>
                    </div>

                    <div class="pt-4 flex flex-wrap items-center justify-center lg:justify-start gap-4">
                        <a href="#booking-section" class="px-8 py-4 bg-gradient-to-r from-cyan-500 via-sky-600 to-blue-600 text-white rounded-2xl font-bold text-lg shadow-xl shadow-cyan-500/30 hover:scale-[1.02] active:scale-95 transition-all inline-flex items-center gap-3">
                            <i class="fa-solid fa-bolt"></i>
                            <span>Book Now for ₹900</span>
                        </a>
                        <a href="#attractions" class="px-7 py-4 bg-white text-slate-700 hover:text-cyan-600 rounded-2xl font-bold text-base border border-slate-200 shadow-sm hover:shadow transition-all inline-flex items-center gap-2">
                            <i class="fa-regular fa-compass"></i>
                            <span>Explore Rides</span>
                        </a>
                    </div>
                </div>

                <!-- Hero Graphic / Pass Highlight -->
                <div class="lg:col-span-5 relative">
                    <div class="relative mx-auto max-w-sm rounded-3xl p-6 bg-gradient-to-br from-cyan-600 to-blue-800 text-white shadow-2xl shadow-cyan-900/40 border border-white/20">
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs uppercase tracking-widest text-cyan-200 font-semibold">AD Water Park Official Pass</span>
                                <h3 class="text-2xl font-black mt-1">ALL-ACCESS TICKET</h3>
                            </div>
                            <span class="px-3 py-1 bg-amber-400 text-slate-900 text-xs font-black rounded-lg">INSTANT E-PASS</span>
                        </div>

                        <div class="my-6 py-4 border-y border-white/20 space-y-2 text-sm text-cyan-100">
                            <div class="flex justify-between">
                                <span><i class="fa-solid fa-check text-cyan-300 mr-2"></i>Mega Wave Pool</span>
                                <span class="font-bold text-white">Included</span>
                            </div>
                            <div class="flex justify-between">
                                <span><i class="fa-solid fa-check text-cyan-300 mr-2"></i>Multi-lane Water Coasters</span>
                                <span class="font-bold text-white">Included</span>
                            </div>
                            <div class="flex justify-between">
                                <span><i class="fa-solid fa-check text-cyan-300 mr-2"></i>DJ & Rain Dance Arena</span>
                                <span class="font-bold text-white">Included</span>
                            </div>
                            <div class="flex justify-between">
                                <span><i class="fa-solid fa-check text-cyan-300 mr-2"></i>Lazy River Relax Zone</span>
                                <span class="font-bold text-white">Included</span>
                            </div>
                            <div class="flex justify-between">
                                <span><i class="fa-solid fa-check text-cyan-300 mr-2"></i>Locker & Changing Rooms</span>
                                <span class="font-bold text-white">Free Access</span>
                            </div>
                        </div>

                        <div class="flex items-end justify-between">
                            <div>
                                <p class="text-xs text-cyan-200 uppercase font-semibold">Admission Rate</p>
                                <p class="text-3xl font-extrabold text-white">₹900 <span class="text-sm font-normal text-cyan-200">/ Person</span></p>
                            </div>
                            <a href="#booking-section" class="px-4 py-2.5 bg-white text-blue-900 rounded-xl font-bold text-sm shadow hover:bg-cyan-50 transition">
                                Grab Tickets
                            </a>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Attractions Showcase -->
    <section id="attractions" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-cyan-600 font-bold tracking-widest text-xs uppercase bg-cyan-50 px-3 py-1 rounded-full border border-cyan-100">World-Class Entertainment</span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 mt-3">Rides & Fun For Everyone</h2>
                <p class="text-slate-600 mt-3 text-base">Your ₹900 ticket grants you unrestricted, unlimited access to each of these high-octane water zones throughout the day!</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Attraction 1 -->
                <div class="group bg-slate-50 border border-slate-200/80 rounded-2xl p-6 hover:shadow-xl hover:border-cyan-400 hover:-translate-y-1 transition-all duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-cyan-500/10 text-cyan-600 flex items-center justify-center text-2xl mb-5 group-hover:bg-cyan-500 group-hover:text-white transition duration-300">
                        <i class="fa-solid fa-water-ladder"></i>
                    </div>
                    <h3 class="text-xl font-bold text-slate-800">Tsunami Wave Pool</h3>
                    <p class="text-slate-600 text-sm mt-2 leading-relaxed">Experience artificial ocean tides rising up to 4 feet with family-safe shallow zones & rhythmic surges.</p>
                    <span class="inline-block mt-4 text-xs font-semibold text-cyan-700 bg-cyan-100 px-2.5 py-1 rounded-lg">High Energy</span>
                </div>

                <!-- Attraction 2 -->
                <div class="group bg-slate-50 border border-slate-200/80 rounded-2xl p-6 hover:shadow-xl hover:border-cyan-400 hover:-translate-y-1 transition-all duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-blue-500/10 text-blue-600 flex items-center justify-center text-2xl mb-5 group-hover:bg-blue-600 group-hover:text-white transition duration-300">
                        <i class="fa-solid fa-meteor"></i>
                    </div>
                    <h3 class="text-xl font-bold text-slate-800">Kamikaze Slide</h3>
                    <p class="text-slate-600 text-sm mt-2 leading-relaxed">A breathtaking 45-foot near-vertical drop slide designed for adrenaline junkies craving sheer velocity.</p>
                    <span class="inline-block mt-4 text-xs font-semibold text-rose-700 bg-rose-100 px-2.5 py-1 rounded-lg">Thrilling Drop</span>
                </div>

                <!-- Attraction 3 -->
                <div class="group bg-slate-50 border border-slate-200/80 rounded-2xl p-6 hover:shadow-xl hover:border-cyan-400 hover:-translate-y-1 transition-all duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-teal-500/10 text-teal-600 flex items-center justify-center text-2xl mb-5 group-hover:bg-teal-600 group-hover:text-white transition duration-300">
                        <i class="fa-solid fa-music"></i>
                    </div>
                    <h3 class="text-xl font-bold text-slate-800">Rain Dance & Live DJ</h3>
                    <p class="text-slate-600 text-sm mt-2 leading-relaxed">Groove to high-energy party tracks while overhead misty rain jets keep you cool under the sun.</p>
                    <span class="inline-block mt-4 text-xs font-semibold text-amber-700 bg-amber-100 px-2.5 py-1 rounded-lg">Party Favorite</span>
                </div>

                <!-- Attraction 4 -->
                <div class="group bg-slate-50 border border-slate-200/80 rounded-2xl p-6 hover:shadow-xl hover:border-cyan-400 hover:-translate-y-1 transition-all duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-sky-500/10 text-sky-600 flex items-center justify-center text-2xl mb-5 group-hover:bg-sky-600 group-hover:text-white transition duration-300">
                        <i class="fa-solid fa-ferry"></i>
                    </div>
                    <h3 class="text-xl font-bold text-slate-800">Serene Lazy River</h3>
                    <p class="text-slate-600 text-sm mt-2 leading-relaxed">Grab a float tube and drift effortlessly through peaceful waterways surrounded by tropical palm scapes.</p>
                    <span class="inline-block mt-4 text-xs font-semibold text-emerald-700 bg-emerald-100 px-2.5 py-1 rounded-lg">Relaxation</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Pricing Summary Section -->
    <section id="pricing" class="py-14 bg-gradient-to-r from-cyan-900 to-slate-900 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="bg-gradient-to-r from-cyan-600/20 to-blue-600/20 rounded-3xl p-8 sm:p-12 border border-white/10 flex flex-col lg:flex-row items-center justify-between gap-8">
                <div>
                    <span class="text-amber-400 font-bold uppercase tracking-wider text-xs">Standard All-Day Ticket</span>
                    <h2 class="text-3xl sm:text-4xl font-black mt-2">One Pass, Unlimited Fun. Only ₹900.</h2>
                    <p class="text-cyan-100/90 mt-2 max-w-xl text-sm sm:text-base">
                        No hidden charges. Your entry ticket covers all waterslides, wave pools, safety life jackets, shower facilities, and live DJ dance floors.
                    </p>
                    <div class="flex flex-wrap gap-4 mt-4 text-xs font-semibold text-cyan-200">
                        <span class="flex items-center gap-1.5"><i class="fa-solid fa-circle-check text-cyan-400"></i> Free Parking</span>
                        <span class="flex items-center gap-1.5"><i class="fa-solid fa-circle-check text-cyan-400"></i> Children below 3ft: FREE</span>
                        <span class="flex items-center gap-1.5"><i class="fa-solid fa-circle-check text-cyan-400"></i> Instant QR Validation</span>
                    </div>
                </div>

                <div class="bg-white/10 backdrop-blur-md p-6 rounded-2xl border border-white/20 text-center min-w-[280px]">
                    <span class="text-xs text-cyan-200 uppercase font-semibold">Fixed Rate Per Ticket</span>
                    <div class="text-5xl font-black text-amber-400 my-2">₹900</div>
                    <span class="text-xs text-white/80 block mb-4">GST and Tax Inclusive</span>
                    <a href="#booking-section" class="w-full inline-block py-3 px-6 bg-amber-400 hover:bg-amber-300 text-slate-950 font-bold rounded-xl transition shadow-lg">
                        Select Tickets Now
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Interactive Booking & Live Pass Preview Section -->
    <section id="booking-section" class="py-20 bg-slate-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            
            <div class="text-center max-w-2xl mx-auto mb-14">
                <span class="text-cyan-700 font-bold text-xs uppercase bg-cyan-100 px-3 py-1 rounded-full">Fast & Secure Booking</span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 mt-3">Book Your AD Water Park Tickets</h2>
                <p class="text-slate-600 mt-2 text-sm sm:text-base">Fill your details below. Real-time ticket calculation and immediate digital pass preview!</p>
            </div>

            <div class="grid lg:grid-cols-12 gap-8 items-start">
                
                <!-- Left: Booking Form -->
                <div class="lg:col-span-7 bg-white rounded-3xl p-6 sm:p-8 shadow-xl shadow-slate-200/80 border border-slate-200">
                    <form id="bookingForm" onsubmit="handleProceedToPay(event)" class="space-y-6">
                        
                        <!-- Step 1: Select Quantity & Date -->
                        <div class="border-b border-slate-200 pb-6">
                            <h3 class="text-lg font-bold text-slate-900 flex items-center gap-2 mb-4">
                                <span class="w-7 h-7 rounded-full bg-cyan-600 text-white flex items-center justify-center text-xs">1</span>
                                Select Date & Visitors
                            </h3>

                            <div class="grid sm:grid-cols-2 gap-4">
                                <!-- Date Picker -->
                                <div>
                                    <label class="block text-xs font-bold uppercase tracking-wider text-slate-700 mb-2">Visit Date</label>
                                    <input 
                                        type="date" 
                                        id="visitDate" 
                                        required 
                                        class="w-full px-4 py-3 rounded-xl border border-slate-300 focus:ring-2 focus:ring-cyan-500 focus:border-cyan-500 outline-none text-slate-800 font-medium text-sm transition"
                                    />
                                    <span class="text-xs text-slate-500 mt-1 block">Valid only on selected date</span>
                                </div>

                                <!-- Visitors Counter -->
                                <div>
                                    <label class="block text-xs font-bold uppercase tracking-wider text-slate-700 mb-2">Number of Visitors</label>
                                    <div class="flex items-center border border-slate-300 rounded-xl overflow-hidden bg-slate-50">
                                        <button 
                                            type="button" 
                                            onclick="updateTicketCount(-1)" 
                                            class="w-12 h-11 flex items-center justify-center bg-slate-200 hover:bg-slate-300 text-slate-800 font-bold text-lg active:scale-95 transition"
                                        >
                                            <i class="fa-solid fa-minus text-xs"></i>
                                        </button>
                                        <input 
                                            type="number" 
                                            id="ticketCount" 
                                            min="1" 
                                            max="50" 
                                            value="1" 
                                            readonly 
                                            class="w-full text-center bg-transparent font-extrabold text-slate-900 text-lg outline-none"
                                        />
                                        <button 
                                            type="button" 
                                            onclick="updateTicketCount(1)" 
                                            class="w-12 h-11 flex items-center justify-center bg-cyan-600 hover:bg-cyan-700 text-white font-bold text-lg active:scale-95 transition"
                                        >
                                            <i class="fa-solid fa-plus text-xs"></i>
                                        </button>
                                    </div>
                                    <span class="text-xs text-slate-500 mt-1 block">₹900 per visitor</span>
                                </div>
                            </div>
                        </div>

                        <!-- Step 2: Primary Visitor Contact -->
                        <div class="border-b border-slate-200 pb-6">
                            <h3 class="text-lg font-bold text-slate-900 flex items-center gap-2 mb-4">
                                <span class="w-7 h-7 rounded-full bg-cyan-600 text-white flex items-center justify-center text-xs">2</span>
                                Primary Visitor Details
                            </h3>

                            <div class="space-y-4">
                                <div>
                                    <label class="block text-xs font-bold uppercase tracking-wider text-slate-700 mb-1">Full Name</label>
                                    <div class="relative">
                                        <span class="absolute inset-y-0 left-0 pl-3.5 flex items-center pointer-events-none text-slate-400">
                                            <i class="fa-regular fa-user"></i>
                                        </span>
                                        <input 
                                            type="text" 
                                            id="visitorName" 
                                            required 
                                            placeholder="e.g. Rahul Sharma" 
                                            oninput="updatePreview()" 
                                            class="w-full pl-10 pr-4 py-3 rounded-xl border border-slate-300 focus:ring-2 focus:ring-cyan-500 focus:border-cyan-500 outline-none text-slate-800 text-sm font-medium transition"
                                        />
                                    </div>
                                </div>

                                <div class="grid sm:grid-cols-2 gap-4">
                                    <div>
                                        <label class="block text-xs font-bold uppercase tracking-wider text-slate-700 mb-1">Email Address</label>
                                        <div class="relative">
                                            <span class="absolute inset-y-0 left-0 pl-3.5 flex items-center pointer-events-none text-slate-400">
                                                <i class="fa-regular fa-envelope"></i>
                                            </span>
                                            <input 
                                                type="email" 
                                                id="visitorEmail" 
                                                required 
                                                placeholder="rahul@example.com" 
                                                class="w-full pl-10 pr-4 py-3 rounded-xl border border-slate-300 focus:ring-2 focus:ring-cyan-500 focus:border-cyan-500 outline-none text-slate-800 text-sm font-medium transition"
                                            />
                                        </div>
                                    </div>
                                    <div>
                                        <label class="block text-xs font-bold uppercase tracking-wider text-slate-700 mb-1">Mobile Number</label>
                                        <div class="relative">
                                            <span class="absolute inset-y-0 left-0 pl-3.5 flex items-center pointer-events-none text-slate-400">
                                                <i class="fa-solid fa-phone"></i>
                                            </span>
                                            <input 
                                                type="tel" 
                                                id="visitorPhone" 
                                                required 
                                                pattern="[0-9]{10}"
                                                placeholder="10-digit mobile" 
                                                oninput="updatePreview()" 
                                                class="w-full pl-10 pr-4 py-3 rounded-xl border border-slate-300 focus:ring-2 focus:ring-cyan-500 focus:border-cyan-500 outline-none text-slate-800 text-sm font-medium transition"
                                            />
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- Step 3: Bill Calculation Breakdown -->
                        <div class="bg-slate-50 p-5 rounded-2xl border border-slate-200">
                            <div class="space-y-2 text-sm">
                                <div class="flex justify-between text-slate-600">
                                    <span>Ticket Base Fare (<span id="calcTicketCount">1</span> × ₹900):</span>
                                    <span class="font-bold text-slate-800" id="calcSubtotal">₹900</span>
                                </div>
                                <div class="flex justify-between text-slate-600">
                                    <span>Park Maintenance & Pool Tax:</span>
                                    <span class="text-emerald-600 font-semibold">Included (₹0)</span>
                                </div>
                                <div class="flex justify-between text-slate-600">
                                    <span>Lockers & Tube Float:</span>
                                    <span class="text-emerald-600 font-semibold">Free Complimentary</span>
                                </div>
                                <div class="border-t border-slate-300 pt-3 mt-3 flex justify-between items-center text-base">
                                    <span class="font-extrabold text-slate-900">Total Payable Amount:</span>
                                    <span class="text-2xl font-black text-cyan-600" id="calcTotal">₹900</span>
                                </div>
                            </div>
                        </div>

                        <!-- Submit Button -->
                        <button 
                            type="submit" 
                            class="w-full py-4 bg-gradient-to-r from-cyan-600 via-sky-600 to-blue-600 hover:from-cyan-700 hover:to-blue-700 text-white font-extrabold text-lg rounded-2xl shadow-xl shadow-cyan-600/30 active:scale-[0.98] transition-all flex items-center justify-center gap-3"
                        >
                            <i class="fa-solid fa-lock"></i>
                            <span>Proceed to Pay <span id="btnPayAmount">₹900</span></span>
                        </button>
                        <p class="text-center text-xs text-slate-500 flex items-center justify-center gap-1.5">
                            <i class="fa-solid fa-shield-halved text-emerald-600"></i> 256-Bit Encrypted Simulated Fast Checkout
                        </p>
                    </form>
                </div>

                <!-- Right: Dynamic Live Pass Preview -->
                <div class="lg:col-span-5 sticky top-28">
                    <div class="text-xs font-bold uppercase tracking-wider text-slate-500 mb-2 flex items-center justify-between">
                        <span>Live E-Ticket Preview</span>
                        <span class="text-cyan-600 flex items-center gap-1"><span class="w-2 h-2 rounded-full bg-emerald-500 animate-ping"></span> Live Preview</span>
                    </div>

                    <!-- Ticket Graphic Element -->
                    <div class="relative bg-white rounded-3xl shadow-2xl border border-slate-200 overflow-hidden">
                        
                        <!-- Top Header of the Ticket -->
                        <div class="bg-gradient-to-r from-cyan-600 via-sky-600 to-blue-600 p-6 text-white relative">
                            <div class="flex justify-between items-start">
                                <div>
                                    <h4 class="text-xl font-extrabold tracking-tight">AD WATER PARK</h4>
                                    <p class="text-xs text-cyan-100 font-medium">Summer All-Access Splash Pass</p>
                                </div>
                                <span class="bg-white/20 text-white px-2.5 py-1 rounded-md text-xs font-bold border border-white/30 backdrop-blur-sm">
                                    ₹900 / TICKET
                                </span>
                            </div>
                        </div>

                        <!-- Ticket Body -->
                        <div class="p-6 space-y-4">
                            <div class="grid grid-cols-2 gap-4 pb-4 border-b border-slate-100">
                                <div>
                                    <span class="text-[10px] uppercase font-bold text-slate-400 block tracking-wider">Visitor Name</span>
                                    <span class="text-sm font-extrabold text-slate-800 truncate block" id="previewName">Rahul Sharma</span>
                                </div>
                                <div>
                                    <span class="text-[10px] uppercase font-bold text-slate-400 block tracking-wider">Visit Date</span>
                                    <span class="text-sm font-extrabold text-cyan-700 block" id="previewDate">Select Date</span>
                                </div>
                            </div>

                            <div class="grid grid-cols-2 gap-4 pb-4 border-b border-slate-100">
                                <div>
                                    <span class="text-[10px] uppercase font-bold text-slate-400 block tracking-wider">Pass Quantity</span>
                                    <span class="text-sm font-extrabold text-slate-800" id="previewQty">1 Visitor</span>
                                </div>
                                <div>
                                    <span class="text-[10px] uppercase font-bold text-slate-400 block tracking-wider">Total Value</span>
                                    <span class="text-sm font-black text-slate-900" id="previewPrice">₹900</span>
                                </div>
                            </div>

                            <div class="pt-1 flex items-center justify-between">
                                <div>
                                    <span class="text-[10px] uppercase font-bold text-slate-400 block tracking-wider">Pass Type</span>
                                    <span class="text-xs font-bold text-emerald-600 bg-emerald-50 px-2 py-0.5 rounded border border-emerald-200">Full Day Unlimited</span>
                                    <span class="text-[10px] text-slate-400 block mt-2">Entry: 10:00 AM - 6:00 PM</span>
                                </div>
                                
                                <div class="text-center">
                                    <div class="w-16 h-16 bg-slate-100 p-1.5 rounded-xl border border-slate-200 flex items-center justify-center text-slate-400">
                                        <i class="fa-solid fa-qrcode text-3xl text-slate-700"></i>
                                    </div>
                                    <span class="text-[9px] text-slate-400 mt-1 block">Validates at Gate</span>
                                </div>
                            </div>
                        </div>

                        <!-- Ticket Notch Cutouts -->
                        <div class="ticket-cutout-left"></div>
                        <div class="ticket-cutout-right"></div>

                        <!-- Footer stub -->
                        <div class="bg-slate-50 px-6 py-3 border-t border-dashed border-slate-300 flex items-center justify-between text-xs text-slate-500">
                            <span>Booking Ref: <strong class="text-slate-700" id="previewRef">AD-PENDING</strong></span>
                            <span class="text-cyan-600 font-semibold"><i class="fa-solid fa-circle-check"></i> Instant Pass</span>
                        </div>
                    </div>

                    <!-- Trust indicators -->
                    <div class="mt-4 flex items-center justify-center gap-6 text-xs text-slate-500">
                        <span class="flex items-center gap-1"><i class="fa-solid fa-rotate-left text-cyan-600"></i> Free Date Reschedule</span>
                        <span class="flex items-center gap-1"><i class="fa-solid fa-mobile-screen text-cyan-600"></i> Show on Mobile</span>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- FAQs Section -->
    <section id="faqs" class="py-20 bg-white border-t border-slate-200">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <span class="text-cyan-700 font-bold text-xs uppercase bg-cyan-100 px-3 py-1 rounded-full">Got Questions?</span>
                <h2 class="text-3xl font-extrabold text-slate-900 mt-3">Frequently Asked Questions</h2>
            </div>

            <div class="space-y-4">
                <details class="group bg-slate-50 rounded-2xl p-5 border border-slate-200 [&_summary::-webkit-details-marker]:hidden">
                    <summary class="flex items-center justify-between cursor-pointer font-bold text-slate-800">
                        <span>What is included in the ₹900 ticket?</span>
                        <span class="text-cyan-600 transition group-open:rotate-180"><i class="fa-solid fa-chevron-down"></i></span>
                    </summary>
                    <p class="text-sm text-slate-600 mt-3 leading-relaxed">
                        The ₹900 pass includes all-day admission, unrestricted access to all 25+ water slides, wave pools, rain dance arena, tube floats, lockers, and changing rooms.
                    </p>
                </details>

                <details class="group bg-slate-50 rounded-2xl p-5 border border-slate-200 [&_summary::-webkit-details-marker]:hidden">
                    <summary class="flex items-center justify-between cursor-pointer font-bold text-slate-800">
                        <span>Are swimsuits required? Can we rent them inside?</span>
                        <span class="text-cyan-600 transition group-open:rotate-180"><i class="fa-solid fa-chevron-down"></i></span>
                    </summary>
                    <p class="text-sm text-slate-600 mt-3 leading-relaxed">
                        Yes, nylon or lycra swimwear is mandatory for pool cleanliness and ride safety. You can bring your own or buy/rent affordable swimwear at the park entrance kiosk.
                    </p>
                </details>

                <details class="group bg-slate-50 rounded-2xl p-5 border border-slate-200 [&_summary::-webkit-details-marker]:hidden">
                    <summary class="flex items-center justify-between cursor-pointer font-bold text-slate-800">
                        <span>What are the park timings?</span>
                        <span class="text-cyan-600 transition group-open:rotate-180"><i class="fa-solid fa-chevron-down"></i></span>
                    </summary>
                    <p class="text-sm text-slate-600 mt-3 leading-relaxed">
                        AD Water Park operates daily from 10:00 AM to 6:00 PM. The wave pool sessions operate every 45 minutes and the live DJ runs all afternoon!
                    </p>
                </details>

                <details class="group bg-slate-50 rounded-2xl p-5 border border-slate-200 [&_summary::-webkit-details-marker]:hidden">
                    <summary class="flex items-center justify-between cursor-pointer font-bold text-slate-800">
                        <span>Do I need to print the ticket?</span>
                        <span class="text-cyan-600 transition group-open:rotate-180"><i class="fa-solid fa-chevron-down"></i></span>
                    </summary>
                    <p class="text-sm text-slate-600 mt-3 leading-relaxed">
                        No physical printout required! Simply show the digital e-ticket with the QR code on your mobile phone screen at the turnstile gate for instantaneous scanning.
                    </p>
                </details>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-slate-900 text-slate-400 py-12 border-t border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 grid grid-cols-1 md:grid-cols-4 gap-8">
            <div class="space-y-4">
                <div class="flex items-center gap-2 text-white">
                    <div class="w-10 h-10 rounded-xl bg-cyan-500 flex items-center justify-center text-white text-xl">
                        <i class="fa-solid fa-water"></i>
                    </div>
                    <span class="text-xl font-black">AD WATER PARK</span>
                </div>
                <p class="text-xs leading-relaxed">
                    The ultimate water entertainment destination featuring thrilling rides, pristine pools, and lifelong memories.
                </p>
            </div>

            <div>
                <h4 class="text-white font-bold text-sm mb-3">Quick Links</h4>
                <ul class="text-xs space-y-2">
                    <li><a href="#attractions" class="hover:text-cyan-400">Rides & Slides</a></li>
                    <li><a href="#pricing" class="hover:text-cyan-400">Pass Pricing (₹900)</a></li>
                    <li><a href="#booking-section" class="hover:text-cyan-400">Online Booking</a></li>
                    <li><a href="#faqs" class="hover:text-cyan-400">Rules & Guidelines</a></li>
                </ul>
            </div>

            <div>
                <h4 class="text-white font-bold text-sm mb-3">Park Location & Hours</h4>
                <p class="text-xs leading-relaxed">
                    Waterfront Fun City Highway, Sector 4<br>
                    Open 7 Days a Week<br>
                    10:00 AM – 6:00 PM
                </p>
            </div>

            <div>
                <h4 class="text-white font-bold text-sm mb-3">Support & Enquiries</h4>
                <p class="text-xs text-slate-300"><i class="fa-solid fa-phone text-cyan-400 mr-1.5"></i> +91 98765 43210</p>
                <p class="text-xs text-slate-300 mt-1"><i class="fa-solid fa-envelope text-cyan-400 mr-1.5"></i> support@adwaterpark.com</p>
                <div class="mt-4 flex gap-3 text-base text-slate-400">
                    <a href="#" class="hover:text-cyan-400"><i class="fa-brands fa-facebook"></i></a>
                    <a href="#" class="hover:text-cyan-400"><i class="fa-brands fa-instagram"></i></a>
                    <a href="#" class="hover:text-cyan-400"><i class="fa-brands fa-youtube"></i></a>
                </div>
            </div>
        </div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mt-10 pt-6 border-t border-slate-800 text-center text-xs">
            © <span id="currentYear"></span> AD Water Park. All rights reserved. Ticket Price ₹900 per visitor.
        </div>
    </footer>

    <!-- Payment & Digital Ticket Modal -->
    <div id="bookingModal" class="fixed inset-0 z-50 flex items-center justify-center p-4 bg-slate-900/80 backdrop-blur-sm hidden opacity-0 transition-opacity duration-300">
        <div class="bg-white rounded-3xl max-w-lg w-full p-6 sm:p-8 shadow-2xl transform scale-95 transition-transform duration-300 max-h-[92vh] overflow-y-auto" id="modalContainer">
            
            <!-- Stage 1: Simulated Payment Flow -->
            <div id="paymentStage" class="space-y-6">
                <div class="flex items-center justify-between border-b pb-4">
                    <div>
                        <h3 class="text-xl font-extrabold text-slate-900">Secure Payment</h3>
                        <p class="text-xs text-slate-500">AD Water Park Fast Gateway</p>
                    </div>
                    <button onclick="closeModal()" class="w-8 h-8 rounded-full bg-slate-100 text-slate-500 hover:bg-slate-200 flex items-center justify-center">
                        <i class="fa-solid fa-xmark"></i>
                    </button>
                </div>

                <div class="bg-cyan-50 p-4 rounded-2xl border border-cyan-100 flex items-center justify-between">
                    <div>
                        <span class="text-xs text-cyan-800 font-semibold block">Total Amount Due</span>
                        <span class="text-2xl font-black text-cyan-700" id="modalPayAmount">₹900</span>
                    </div>
                    <span class="text-xs bg-white text-cyan-900 font-bold px-3 py-1 rounded-full border border-cyan-200">
                        <span id="modalVisitorCount">1</span> Pass(es)
                    </span>
                </div>

                <div class="space-y-3">
                    <label class="text-xs font-bold text-slate-700 uppercase">Select Payment Mode</label>
                    <div class="grid grid-cols-3 gap-2">
                        <label class="border-2 border-cyan-600 bg-cyan-50/50 rounded-xl p-3 text-center cursor-pointer flex flex-col items-center">
                            <input type="radio" name="paymethod" checked class="hidden">
                            <i class="fa-solid fa-bolt text-cyan-600 text-lg mb-1"></i>
                            <span class="text-xs font-bold text-slate-800">UPI / QR</span>
                        </label>
                        <label class="border border-slate-200 rounded-xl p-3 text-center cursor-pointer flex flex-col items-center hover:bg-slate-50">
                            <input type="radio" name="paymethod" class="hidden">
                            <i class="fa-regular fa-credit-card text-slate-600 text-lg mb-1"></i>
                            <span class="text-xs font-bold text-slate-800">Card</span>
                        </label>
                        <label class="border border-slate-200 rounded-xl p-3 text-center cursor-pointer flex flex-col items-center hover:bg-slate-50">
                            <input type="radio" name="paymethod" class="hidden">
                            <i class="fa-solid fa-building-columns text-slate-600 text-lg mb-1"></i>
                            <span class="text-xs font-bold text-slate-800">NetBanking</span>
                        </label>
                    </div>
                </div>

                <div class="p-4 bg-slate-50 border border-slate-200 rounded-xl text-center">
                    <p class="text-xs text-slate-600 mb-2">Simulated Sandbox Payment: Click below to confirm instant payment.</p>
                    <button 
                        type="button" 
                        onclick="completeBookingPayment()" 
                        id="payButton"
                        class="w-full py-3.5 bg-emerald-600 hover:bg-emerald-700 text-white font-extrabold rounded-xl shadow-lg shadow-emerald-600/30 transition flex items-center justify-center gap-2"
                    >
                        <i class="fa-solid fa-circle-check"></i>
                        <span>Pay & Generate Pass (<span id="modalBtnAmount">₹900</span>)</span>
                    </button>
                </div>
            </div>

            <!-- Stage 2: Final Confirmed Digital Ticket Pass -->
            <div id="confirmedStage" class="hidden text-center space-y-6">
                <div class="w-16 h-16 bg-emerald-100 text-emerald-600 rounded-full flex items-center justify-center mx-auto text-3xl shadow-inner">
                    <i class="fa-solid fa-check"></i>
                </div>

                <div>
                    <h3 class="text-2xl font-black text-slate-900">Booking Confirmed!</h3>
                    <p class="text-xs text-slate-500 mt-1">Your AD Water Park pass has been generated successfully.</p>
                </div>

                <!-- Printable Digital Pass Voucher -->
                <div id="ticketVoucher" class="border-2 border-dashed border-cyan-400 bg-cyan-50/40 rounded-2xl p-6 text-left relative overflow-hidden">
                    <div class="flex justify-between items-center pb-3 border-b border-cyan-200">
                        <div>
                            <span class="font-extrabold text-cyan-900 text-lg tracking-tight">AD WATER PARK</span>
                            <span class="text-[10px] text-cyan-700 block uppercase font-bold">Official E-Ticket</span>
                        </div>
                        <span class="px-2.5 py-1 bg-emerald-500 text-white text-[11px] font-bold rounded-lg shadow-sm">CONFIRMED</span>
                    </div>

                    <div class="my-4 grid grid-cols-2 gap-3 text-xs">
                        <div>
                            <span class="text-slate-400 uppercase text-[10px] font-bold">Booking ID</span>
                            <p class="font-mono font-bold text-slate-800" id="finalBookingId">AD-12345</p>
                        </div>
                        <div>
                            <span class="text-slate-400 uppercase text-[10px] font-bold">Visit Date</span>
                            <p class="font-bold text-slate-800" id="finalDate">--</p>
                        </div>
                        <div>
                            <span class="text-slate-400 uppercase text-[10px] font-bold">Lead Guest</span>
                            <p class="font-bold text-slate-800" id="finalGuest">--</p>
                        </div>
                        <div>
                            <span class="text-slate-400 uppercase text-[10px] font-bold">Passes</span>
                            <p class="font-bold text-cyan-700" id="finalPassCount">1 Person (₹900)</p>
                        </div>
                    </div>

                    <!-- QR Code Generated Output -->
                    <div class="flex flex-col items-center justify-center pt-2 border-t border-cyan-200">
                        <div id="qrcode" class="p-2 bg-white rounded-xl shadow-sm border border-slate-200"></div>
                        <span class="text-[10px] text-slate-500 mt-2 font-medium">Scan this QR code at Entry Gate Turnstiles</span>
                    </div>
                </div>

                <div class="flex flex-col sm:flex-row gap-3">
                    <button onclick="window.print()" class="flex-1 py-3 bg-slate-900 hover:bg-slate-800 text-white rounded-xl text-xs font-bold flex items-center justify-center gap-2 shadow">
                        <i class="fa-solid fa-print"></i> Print / Save Pass
                    </button>
                    <button onclick="closeModal()" class="flex-1 py-3 bg-cyan-600 hover:bg-cyan-700 text-white rounded-xl text-xs font-bold transition shadow">
                        Done & Close
                    </button>
                </div>
            </div>

        </div>
    </div>

    <!-- JavaScript Logic -->
    <script>
        const TICKET_PRICE = 900;
        let currentTicketCount = 1;
        let qrCodeInstance = null;

        // Set default visit date as tomorrow
        window.addEventListener('DOMContentLoaded', () => {
            document.getElementById('currentYear').textContent = new Date().getFullYear();
            
            const tomorrow = new Date();
            tomorrow.setDate(tomorrow.getDate() + 1);
            const tomorrowStr = tomorrow.toISOString().split('T')[0];
            
            const dateInput = document.getElementById('visitDate');
            dateInput.min = new Date().toISOString().split('T')[0];
            dateInput.value = tomorrowStr;

            updateTicketCount(0);
            updatePreview();
        });

        // Update ticket count & price computations
        function updateTicketCount(delta) {
            const newCount = currentTicketCount + delta;
            if (newCount >= 1 && newCount <= 50) {
                currentTicketCount = newCount;
                document.getElementById('ticketCount').value = currentTicketCount;
                
                const totalAmount = currentTicketCount * TICKET_PRICE;
                
                // Form calculations
                document.getElementById('calcTicketCount').textContent = currentTicketCount;
                document.getElementById('calcSubtotal').textContent = `₹${totalAmount.toLocaleString('en-IN')}`;
                document.getElementById('calcTotal').textContent = `₹${totalAmount.toLocaleString('en-IN')}`;
                document.getElementById('btnPayAmount').textContent = `₹${totalAmount.toLocaleString('en-IN')}`;
                
                // Live preview updates
                document.getElementById('previewQty').textContent = `${currentTicketCount} Visitor${currentTicketCount > 1 ? 's' : ''}`;
                document.getElementById('previewPrice').textContent = `₹${totalAmount.toLocaleString('en-IN')}`;
                
                updatePreview();
            }
        }

        // Keep dynamic preview synchronized with inputs
        function updatePreview() {
            const name = document.getElementById('visitorName').value.trim();
            const date = document.getElementById('visitDate').value;
            
            document.getElementById('previewName').textContent = name || 'Rahul Sharma';
            
            if (date) {
                const formattedDate = new Date(date).toLocaleDateString('en-US', {
                    day: 'numeric',
                    month: 'short',
                    year: 'numeric'
                });
                document.getElementById('previewDate').textContent = formattedDate;
            } else {
                document.getElementById('previewDate').textContent = 'Select Date';
            }
            
            document.getElementById('previewRef').textContent = 'AD-' + Math.floor(100000 + Math.random() * 900000);
        }

        document.getElementById('visitDate').addEventListener('change', updatePreview);

        // Open Modal for simulated payment
        function handleProceedToPay(e) {
            e.preventDefault();
            const totalAmount = currentTicketCount * TICKET_PRICE;

            document.getElementById('modalPayAmount').textContent = `₹${totalAmount.toLocaleString('en-IN')}`;
            document.getElementById('modalBtnAmount').textContent = `₹${totalAmount.toLocaleString('en-IN')}`;
            document.getElementById('modalVisitorCount').textContent = currentTicketCount;

            // Show payment stage, hide confirmation stage
            document.getElementById('paymentStage').classList.remove('hidden');
            document.getElementById('confirmedStage').classList.add('hidden');

            const modal = document.getElementById('bookingModal');
            modal.classList.remove('hidden');
            setTimeout(() => {
                modal.classList.remove('opacity-0');
                document.getElementById('modalContainer').classList.remove('scale-95');
            }, 10);
        }

        // Close Modal
        function closeModal() {
            const modal = document.getElementById('bookingModal');
            modal.classList.add('opacity-0');
            document.getElementById('modalContainer').classList.add('scale-95');
            setTimeout(() => {
                modal.classList.add('hidden');
            }, 300);
        }

        // Simulate Booking Payment & Generate QR Code Pass
        function completeBookingPayment() {
            const payBtn = document.getElementById('payButton');
            payBtn.innerHTML = '<i class="fa-solid fa-spinner fa-spin mr-2"></i> Processing Securely...';
            payBtn.disabled = true;

            setTimeout(() => {
                payBtn.innerHTML = '<i class="fa-solid fa-circle-check"></i> Pay & Generate Pass';
                payBtn.disabled = false;

                const bookingRef = 'AD-' + Math.floor(100000 + Math.random() * 900000);
                const guestName = document.getElementById('visitorName').value || 'Visitor';
                const dateVal = document.getElementById('visitDate').value;
                const formattedDate = new Date(dateVal).toLocaleDateString('en-US', {
                    day: 'numeric',
                    month: 'short',
                    year: 'numeric'
                });
                const totalCost = currentTicketCount * TICKET_PRICE;

                // Update confirmed ticket details
                document.getElementById('finalBookingId').textContent = bookingRef;
                document.getElementById('finalGuest').textContent = guestName;
                document.getElementById('finalDate').textContent = formattedDate;
                document.getElementById('finalPassCount').textContent = `${currentTicketCount} Pass (${currentTicketCount} × ₹900 = ₹${totalCost.toLocaleString('en-IN')})`;

                // Render dynamic QR code
                const qrContainer = document.getElementById('qrcode');
                qrContainer.innerHTML = '';
                const qrPayload = JSON.stringify({
                    park: "AD Water Park",
                    ref: bookingRef,
                    name: guestName,
                    visitors: currentTicketCount,
                    total: totalCost,
                    date: dateVal,
                    status: "PAID_VERIFIED"
                });

                qrCodeInstance = new QRCode(qrContainer, {
                    text: qrPayload,
                    width: 120,
                    height: 120,
                    colorDark: "#0f172a",
                    colorLight: "#ffffff",
                    correctLevel: QRCode.CorrectLevel.M
                });

                // Transition to confirmation stage
                document.getElementById('paymentStage').classList.add('hidden');
                document.getElementById('confirmedStage').classList.remove('hidden');
            }, 1200);
        }
    </script>
</body>
</html>
```