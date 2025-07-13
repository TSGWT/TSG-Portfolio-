# TSG-Portfolio-
Sourcing Partner
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gaming Accessories - Product Order Request</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        primary: '#5D5CDE',
                        'primary-hover': '#4F4BC7',
                    }
                }
            }
        }
    </script>
    <style>
        .product-frame {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            transition: all 0.3s ease;
        }
        .product-frame:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        .dark .product-frame {
            background: linear-gradient(135deg, #4a5568 0%, #2d3748 100%);
        }
        .file-upload-area {
            border: 2px dashed #d1d5db;
            transition: all 0.3s ease;
        }
        .file-upload-area:hover, .file-upload-area.drag-over {
            border-color: #5D5CDE;
            background-color: #f8faff;
        }
        .dark .file-upload-area {
            border-color: #4b5563;
        }
        .dark .file-upload-area:hover, .dark .file-upload-area.drag-over {
            border-color: #5D5CDE;
            background-color: #1f2937;
        }
        .loading-spinner {
            animation: spin 1s linear infinite;
        }
        @keyframes spin {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        .category-card {
            background: linear-gradient(45deg, #f3f4f6, #e5e7eb);
            border: 2px solid #e5e7eb;
            transition: all 0.3s ease;
        }
        .category-card:hover {
            border-color: #5D5CDE;
            background: linear-gradient(45deg, #f8faff, #f3f4f6);
        }
        .dark .category-card {
            background: linear-gradient(45deg, #374151, #4b5563);
            border-color: #4b5563;
        }
        .dark .category-card:hover {
            border-color: #5D5CDE;
            background: linear-gradient(45deg, #1f2937, #374151);
        }
        
        /* TSG Branding Animations */
        .floating-shapes {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
        }
        
        .shape {
            position: absolute;
            border-radius: 50%;
            background: linear-gradient(45deg, #ffffff20, #ffffff10);
            animation: float 6s ease-in-out infinite;
        }
        
        .shape-1 {
            width: 80px;
            height: 80px;
            top: 10%;
            left: 10%;
            animation-delay: 0s;
        }
        
        .shape-2 {
            width: 120px;
            height: 120px;
            top: 60%;
            right: 15%;
            animation-delay: 2s;
        }
        
        .shape-3 {
            width: 60px;
            height: 60px;
            top: 30%;
            right: 30%;
            animation-delay: 4s;
        }
        
        .shape-4 {
            width: 100px;
            height: 100px;
            bottom: 20%;
            left: 20%;
            animation-delay: 1s;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
        }
        
        .robot-wave {
            animation: wave 3s ease-in-out infinite;
        }
        
        @keyframes wave {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            25% { transform: translateY(-5px) rotate(2deg); }
            75% { transform: translateY(-5px) rotate(-2deg); }
        }
        
        .pulse-animation {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        .gaming-brand-badge {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.875rem;
            font-weight: 500;
            transition: all 0.3s ease;
            animation: slideIn 0.6s ease-out forwards;
        }
        
        .gaming-brand-badge:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }
        
        @keyframes slideIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        /* Product Categories Enhancement */
        .category-showcase {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: 15px;
            padding: 20px;
            margin: 20px 0;
            position: relative;
            overflow: hidden;
        }
        
        .category-showcase::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            animation: shine 3s infinite;
        }
        
        @keyframes shine {
            0% { left: -100%; }
            100% { left: 100%; }
        }
    </style>
</head>
<body class="bg-gray-50 dark:bg-gray-900 min-h-screen transition-colors duration-200">
    <div class="container mx-auto px-4 py-8 max-w-6xl">
        <!-- Animated Header with TSG Branding -->
        <div class="relative overflow-hidden bg-gradient-to-r from-purple-600 via-blue-600 to-purple-800 rounded-xl shadow-2xl mb-8 p-8 text-white">
            <!-- Animated Background Elements -->
            <div class="absolute inset-0 opacity-10">
                <div class="floating-shapes">
                    <div class="shape shape-1"></div>
                    <div class="shape shape-2"></div>
                    <div class="shape shape-3"></div>
                    <div class="shape shape-4"></div>
                </div>
            </div>
            
            <!-- Main Header Content -->
            <div class="relative z-10 flex flex-col lg:flex-row items-center justify-between">
                <!-- Left: TSG Branding -->
                <div class="flex items-center mb-6 lg:mb-0">
                    <div class="mr-6">
                        <img src="https://pfst.cf2.poecdn.net/base/image/bfe0b72d14c346859a59c36a79bb9666c53bf850cfd609072dd17a3af8d0c9e7?w=1227&h=1163" 
                             alt="TSG B2B Platform" 
                             class="w-20 h-20 object-contain filter drop-shadow-lg hover:scale-110 transition-transform duration-300">
                    </div>
                    <div>
                        <h1 class="text-4xl font-bold mb-2 bg-clip-text text-transparent bg-gradient-to-r from-yellow-300 to-yellow-100">
                            TSG Gaming Store
                        </h1>
                        <p class="text-lg opacity-90">
                            B2B Platform • Global Business Solutions
                        </p>
                        <p class="text-sm opacity-75">
                            Custom Gaming Accessories & Professional Stands
                        </p>
                    </div>
                </div>
                
                <!-- Right: Animated Robot Mascot -->
                <div class="relative">
                    <img src="https://pfst.cf2.poecdn.net/base/image/3587580da5f3b44c75a4b3a33c9bf6ec72340ab787beb2174df52cbf07b2ced7?w=1200&h=1200" 
                         alt="TSG Robot Assistant" 
                         class="w-32 h-32 object-contain robot-wave filter drop-shadow-2xl">
                    <div class="absolute -top-2 -right-2 bg-green-400 text-green-900 px-3 py-1 rounded-full text-sm font-bold pulse-animation">
                        Live Support!
                    </div>
                </div>
            </div>
            
            <!-- Gaming Brands Showcase -->
            <div class="mt-8 flex flex-wrap justify-center items-center gap-6 opacity-80">
                <div class="gaming-brand-badge">🎮 Sony PlayStation</div>
                <div class="gaming-brand-badge">🎯 Microsoft Xbox</div>
                <div class="gaming-brand-badge">🎲 Nintendo Switch</div>
                <div class="gaming-brand-badge">📱 Mobile Gaming</div>
                <div class="gaming-brand-badge">🕹️ Retro Consoles</div>
                <div class="gaming-brand-badge">🥽 VR Accessories</div>
            </div>
            
            <!-- Call to Action -->
            <div class="text-center mt-6">
                <p class="text-xl font-semibold mb-2">
                    📧 Instant Gmail Integration • 🚀 Fast Quote Response • 🌍 Global Shipping
                </p>
                <p class="text-sm opacity-75">
                    Professional B2B orders automatically formatted and sent to your Gmail
                </p>
            </div>
        </div>

        <!-- Product Categories Showcase -->
        <div class="category-showcase text-white mb-8">
            <div class="relative z-10">
                <h2 class="text-3xl font-bold text-center mb-2">🎮 PRODUCT CATEGORIES 🎮</h2>
                <p class="text-center text-lg opacity-90 mb-8">Professional Gaming Accessories for Every Platform</p>
                
                <!-- Categories Grid inspired by your image -->
                <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mb-6">
                    <div class="bg-red-600 rounded-lg p-4 text-center hover:bg-red-700 transition-colors cursor-pointer" onclick="filterCategory('sony')">
                        <div class="text-2xl mb-2">🎮</div>
                        <h3 class="font-bold">For PS Series</h3>
                        <p class="text-sm opacity-80">PlayStation Stands</p>
                    </div>
                    <div class="bg-red-600 rounded-lg p-4 text-center hover:bg-red-700 transition-colors cursor-pointer" onclick="filterCategory('microsoft')">
                        <div class="text-2xl mb-2">🎯</div>
                        <h3 class="font-bold">For XBOX Series</h3>
                        <p class="text-sm opacity-80">Xbox Accessories</p>
                    </div>
                    <div class="bg-red-600 rounded-lg p-4 text-center hover:bg-red-700 transition-colors cursor-pointer" onclick="filterCategory('nintendo')">
                        <div class="text-2xl mb-2">🎲</div>
                        <h3 class="font-bold">For Nintendo Switch</h3>
                        <p class="text-sm opacity-80">Switch & 3DS Stands</p>
                    </div>
                    <div class="bg-red-600 rounded-lg p-4 text-center hover:bg-red-700 transition-colors cursor-pointer" onclick="filterCategory('mobile')">
                        <div class="text-2xl mb-2">📱</div>
                        <h3 class="font-bold">For PHONE/PC</h3>
                        <p class="text-sm opacity-80">Mobile Gaming</p>
                    </div>
                    <div class="bg-red-600 rounded-lg p-4 text-center hover:bg-red-700 transition-colors cursor-pointer" onclick="filterCategory('retro')">
                        <div class="text-2xl mb-2">🕹️</div>
                        <h3 class="font-bold">Game Console</h3>
                        <p class="text-sm opacity-80">Retro Gaming</p>
                    </div>
                    <div class="bg-red-600 rounded-lg p-4 text-center hover:bg-red-700 transition-colors cursor-pointer" onclick="filterCategory('sony')">
                        <div class="text-2xl mb-2">🎧</div>
                        <h3 class="font-bold">Game Headset</h3>
                        <p class="text-sm opacity-80">Audio Accessories</p>
                    </div>
                    <div class="bg-red-600 rounded-lg p-4 text-center hover:bg-red-700 transition-colors cursor-pointer" onclick="filterCategory('all')">
                        <div class="text-2xl mb-2">🎮</div>
                        <h3 class="font-bold">Game Accessories</h3>
                        <p class="text-sm opacity-80">All Categories</p>
                    </div>
                    <div class="bg-red-600 rounded-lg p-4 text-center hover:bg-red-700 transition-colors cursor-pointer" onclick="filterCategory('sony')">
                        <div class="text-2xl mb-2">🥽</div>
                        <h3 class="font-bold">VR Gaming</h3>
                        <p class="text-sm opacity-80">VR Accessories</p>
                    </div>
                </div>
                
                <!-- Global Shipping Indicators -->
                <div class="flex justify-center items-center gap-2 flex-wrap opacity-80">
                    <span class="text-sm">🌍 Global Shipping:</span>
                    <span class="flag-emoji">🇩🇪</span>
                    <span class="flag-emoji">🇷🇺</span>
                    <span class="flag-emoji">🇪🇸</span>
                    <span class="flag-emoji">🇵🇹</span>
                    <span class="flag-emoji">🇫🇷</span>
                    <span class="flag-emoji">🇸🇦</span>
                    <span class="flag-emoji">🇹🇭</span>
                    <span class="flag-emoji">🇹🇷</span>
                    <span class="flag-emoji">🇮🇹</span>
                    <span class="flag-emoji">🇯🇵</span>
                    <span class="flag-emoji">🇰🇷</span>
                    <span class="flag-emoji">🇻🇳</span>
                </div>
            </div>
        </div>

        <!-- Product Showcase -->
        <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold text-gray-800 dark:text-white mb-6">Browse Our Products</h2>
            
            <!-- Category Filter -->
            <div class="flex flex-wrap gap-2 mb-6">
                <button onclick="filterCategory('all')" class="category-filter-btn bg-primary text-white px-4 py-2 rounded-full text-sm font-medium">All</button>
                <button onclick="filterCategory('sony')" class="category-filter-btn bg-gray-200 dark:bg-gray-600 text-gray-700 dark:text-gray-300 px-4 py-2 rounded-full text-sm font-medium hover:bg-primary hover:text-white transition-colors">Sony</button>
                <button onclick="filterCategory('microsoft')" class="category-filter-btn bg-gray-200 dark:bg-gray-600 text-gray-700 dark:text-gray-300 px-4 py-2 rounded-full text-sm font-medium hover:bg-primary hover:text-white transition-colors">Microsoft</button>
                <button onclick="filterCategory('nintendo')" class="category-filter-btn bg-gray-200 dark:bg-gray-600 text-gray-700 dark:text-gray-300 px-4 py-2 rounded-full text-sm font-medium hover:bg-primary hover:text-white transition-colors">Nintendo</button>
                <button onclick="filterCategory('mobile')" class="category-filter-btn bg-gray-200 dark:bg-gray-600 text-gray-700 dark:text-gray-300 px-4 py-2 rounded-full text-sm font-medium hover:bg-primary hover:text-white transition-colors">Mobile</button>
            </div>

            <!-- Products Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6" id="productsGrid">
                <!-- Products will be populated by JavaScript -->
            </div>
        </div>

        <!-- Order Form -->
        <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6 md:p-8">
            <h2 class="text-3xl font-bold text-center text-gray-800 dark:text-white mb-8">
                Product Order Request
            </h2>
            
            <form id="orderForm" class="space-y-6">
                <!-- Customer Information -->
                <div class="bg-gray-50 dark:bg-gray-700 rounded-lg p-6">
                    <h3 class="text-lg font-semibold text-gray-800 dark:text-white mb-4">Customer Information</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label for="name" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                                Full Name *
                            </label>
                            <input 
                                type="text" 
                                id="name" 
                                name="name" 
                                required 
                                class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                                placeholder="Enter your full name"
                            >
                        </div>
                        <div>
                            <label for="email" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                                Email Address *
                            </label>
                            <input 
                                type="email" 
                                id="email" 
                                name="email" 
                                required 
                                class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                                placeholder="Enter your email address"
                            >
                        </div>
                    </div>
                </div>

                <!-- Product Selection -->
                <div class="bg-gray-50 dark:bg-gray-700 rounded-lg p-6">
                    <h3 class="text-lg font-semibold text-gray-800 dark:text-white mb-4">Product Selection</h3>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mb-4">
                        <div>
                            <label for="category" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                                Product Category *
                            </label>
                            <select 
                                id="category" 
                                name="category" 
                                required 
                                onchange="updateSubcategories()"
                                class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                            >
                                <option value="">Select a category</option>
                                <option value="sony">Sony PlayStation</option>
                                <option value="microsoft">Microsoft Xbox</option>
                                <option value="nintendo">Nintendo</option>
                                <option value="retro">Retro Gaming</option>
                                <option value="mobile">Mobile Gaming</option>
                            </select>
                        </div>
                        <div>
                            <label for="subcategory" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                                Platform/Device *
                            </label>
                            <select 
                                id="subcategory" 
                                name="subcategory" 
                                required 
                                onchange="updateProducts()"
                                class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                                disabled
                            >
                                <option value="">Select platform first</option>
                            </select>
                        </div>
                    </div>

                    <div class="mb-4">
                        <label for="product" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                            Specific Product *
                        </label>
                        <select 
                            id="product" 
                            name="product" 
                            required 
                            class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                            disabled
                        >
                            <option value="">Select category and platform first</option>
                        </select>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                        <div>
                            <label for="quantity" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                                Quantity *
                            </label>
                            <input 
                                type="number" 
                                id="quantity" 
                                name="quantity" 
                                min="1" 
                                required 
                                class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                                placeholder="Enter quantity"
                            >
                        </div>
                        <div>
                            <label for="material" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                                Material
                            </label>
                            <select 
                                id="material" 
                                name="material" 
                                class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                            >
                                <option value="wood">Wood</option>
                                <option value="plastic">Plastic</option>
                                <option value="metal">Metal</option>
                                <option value="acrylic">Acrylic</option>
                            </select>
                        </div>
                        <div>
                            <label for="color" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                                Color/Finish
                            </label>
                            <select 
                                id="color" 
                                name="color" 
                                class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                            >
                                <option value="natural">Natural</option>
                                <option value="black">Black</option>
                                <option value="white">White</option>
                                <option value="custom">Custom Color</option>
                            </select>
                        </div>
                    </div>
                </div>

                <!-- Customization Options -->
                <div class="bg-gray-50 dark:bg-gray-700 rounded-lg p-6">
                    <h3 class="text-lg font-semibold text-gray-800 dark:text-white mb-4">Customization Options</h3>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mb-4">
                        <div>
                            <label class="flex items-center">
                                <input type="checkbox" id="logoEngraving" name="logoEngraving" class="rounded border-gray-300 text-primary focus:ring-primary">
                                <span class="ml-2 text-gray-700 dark:text-gray-300">Logo Engraving/Etching</span>
                            </label>
                        </div>
                        <div>
                            <label class="flex items-center">
                                <input type="checkbox" id="customText" name="customText" class="rounded border-gray-300 text-primary focus:ring-primary">
                                <span class="ml-2 text-gray-700 dark:text-gray-300">Custom Text</span>
                            </label>
                        </div>
                    </div>

                    <div id="logoSection" class="hidden mb-4">
                        <label for="mockup" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                            Upload Logo/Mockup
                        </label>
                        <div class="file-upload-area rounded-lg p-6 text-center cursor-pointer" id="fileUploadArea">
                            <input type="file" id="mockup" name="mockup" accept="image/*" class="hidden">
                            <svg class="mx-auto h-12 w-12 text-gray-400 dark:text-gray-500 mb-4" stroke="currentColor" fill="none" viewBox="0 0 48 48">
                                <path d="M28 8H12a4 4 0 00-4 4v20m32-12v8m0 0v8a4 4 0 01-4 4H12a4 4 0 01-4-4v-4m32-4l-3.172-3.172a4 4 0 00-5.656 0L28 28M8 32l9.172-9.172a4 4 0 015.656 0L28 28m0 0l4 4m4-24h8m-4-4v8m-12 4h.02" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
                            </svg>
                            <p class="text-gray-600 dark:text-gray-400" id="fileUploadText">
                                <span class="font-medium text-primary hover:text-primary-hover">Click to upload</span> or drag and drop
                            </p>
                            <p class="text-xs text-gray-500 dark:text-gray-500 mt-1">PNG, JPG, SVG up to 10MB</p>
                        </div>
                        <div id="filePreview" class="mt-4 hidden">
                            <img id="previewImage" class="max-w-full h-auto rounded-lg border border-gray-200 dark:border-gray-600" alt="Preview">
                            <p id="fileName" class="text-sm text-gray-600 dark:text-gray-400 mt-2"></p>
                        </div>
                    </div>

                    <div id="textSection" class="hidden">
                        <label for="customTextInput" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                            Custom Text to Engrave
                        </label>
                        <input 
                            type="text" 
                            id="customTextInput" 
                            name="customTextInput" 
                            class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                            placeholder="Enter text to be engraved"
                        >
                    </div>
                </div>

                <!-- Delivery Information -->
                <div class="bg-gray-50 dark:bg-gray-700 rounded-lg p-6">
                    <h3 class="text-lg font-semibold text-gray-800 dark:text-white mb-4">Delivery Information</h3>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mb-4">
                        <div>
                            <label for="deliveryDate" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                                Preferred Delivery Date
                            </label>
                            <input 
                                type="date" 
                                id="deliveryDate" 
                                name="deliveryDate" 
                                class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                            >
                        </div>
                        <div>
                            <label for="deliverySpeed" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                                Delivery Speed
                            </label>
                            <select 
                                id="deliverySpeed" 
                                name="deliverySpeed" 
                                class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200"
                            >
                                <option value="standard">Standard (7-14 days)</option>
                                <option value="express">Express (3-5 days)</option>
                                <option value="rush">Rush (1-2 days)</option>
                            </select>
                        </div>
                    </div>

                    <div>
                        <label for="shippingAddress" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                            Shipping Address *
                        </label>
                        <textarea 
                            id="shippingAddress" 
                            name="shippingAddress" 
                            rows="3" 
                            required
                            class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200 resize-vertical"
                            placeholder="Enter complete shipping address with postal code"
                        ></textarea>
                    </div>
                </div>

                <!-- Additional Notes -->
                <div>
                    <label for="notes" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                        Additional Notes & Requirements
                    </label>
                    <textarea 
                        id="notes" 
                        name="notes" 
                        rows="4" 
                        class="w-full px-4 py-3 text-base border border-gray-300 dark:border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent bg-white dark:bg-gray-600 text-gray-900 dark:text-white transition-colors duration-200 resize-vertical"
                        placeholder="Any special requirements, design specifications, or additional notes..."
                    ></textarea>
                </div>

                <button 
                    type="submit" 
                    id="submitBtn"
                    class="w-full bg-primary hover:bg-primary-hover text-white font-medium py-4 px-6 rounded-md transition-colors duration-200 focus:outline-none focus:ring-2 focus:ring-primary focus:ring-offset-2 focus:ring-offset-white dark:focus:ring-offset-gray-800 disabled:opacity-50 disabled:cursor-not-allowed flex items-center justify-center text-lg"
                >
                    <span id="submitText">Submit Order Request</span>
                    <svg id="loadingSpinner" class="loading-spinner ml-3 h-5 w-5 hidden" fill="none" viewBox="0 0 24 24">
                        <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                        <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
                    </svg>
                </button>
            </form>

            <!-- Success/Error Messages -->
            <div id="successMessage" class="hidden mt-6 p-4 bg-green-50 dark:bg-green-900 border border-green-200 dark:border-green-700 rounded-md">
                <div class="flex">
                    <svg class="h-5 w-5 text-green-400" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                    </svg>
                    <div class="ml-3">
                        <h3 class="text-sm font-medium text-green-800 dark:text-green-200">🎉 Order Successfully Sent to TSG Gmail Database!</h3>
                        <p class="text-sm text-green-700 dark:text-green-300 mt-1">
                            ✅ Professional order confirmation auto-generated<br>
                            📧 Ready to copy/paste to your Gmail<br>
                            🤖 TSG Robot Assistant has processed your request<br>
                            ⚡ Check the chat window for your complete order details
                        </p>
                    </div>
                </div>
            </div>

            <div id="errorMessage" class="hidden mt-6 p-4 bg-red-50 dark:bg-red-900 border border-red-200 dark:border-red-700 rounded-md">
                <div class="flex">
                    <svg class="h-5 w-5 text-red-400" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd" />
                    </svg>
                    <div class="ml-3">
                        <h3 class="text-sm font-medium text-red-800 dark:text-red-200">Error submitting order</h3>
                        <p id="errorText" class="text-sm text-red-700 dark:text-red-300 mt-1"></p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Product database
        const productDatabase = {
            sony: {
                'ps5': [
                    { id: 'ps5_stand_premium', name: 'PS5 Premium Stand', description: 'Adjustable premium stand with RGB lighting' },
                    { id: 'ps5_stand_basic', name: 'PS5 Basic Stand', description: 'Simple and sturdy basic stand' },
                    { id: 'ps5_controller_dock', name: 'PS5 Controller Charging Dock', description: 'Dual controller charging station' },
                    { id: 'ps5_headset_stand', name: 'PS5 Headset Stand', description: 'Premium headset display stand' }
                ],
                'ps4': [
                    { id: 'ps4_stand_vertical', name: 'PS4 Vertical Stand', description: 'Space-saving vertical stand' },
                    { id: 'ps4_controller_stand', name: 'PS4 Controller Stand', description: 'Controller display and storage' },
                    { id: 'ps4_cooling_stand', name: 'PS4 Cooling Stand', description: 'Stand with built-in cooling fans' }
                ],
                'psvr': [
                    { id: 'psvr_headset_stand', name: 'PS VR Headset Stand', description: 'Premium VR headset display stand' },
                    { id: 'psvr_controller_dock', name: 'PS VR Controller Dock', description: 'Move controller charging dock' },
                    { id: 'psvr_combo_stand', name: 'PS VR Combo Stand', description: 'All-in-one VR accessory stand' }
                ]
            },
            microsoft: {
                'xbox_series': [
                    { id: 'xbox_series_stand', name: 'Xbox Series X/S Stand', description: 'Modern minimalist console stand' },
                    { id: 'xbox_series_controller_dock', name: 'Xbox Series Controller Dock', description: 'Dual controller charging station' },
                    { id: 'xbox_series_headset_stand', name: 'Xbox Series Headset Stand', description: 'Premium headset display stand' }
                ],
                'xbox_one': [
                    { id: 'xbox_one_x_stand', name: 'Xbox One X Stand', description: 'Heavy-duty stand for Xbox One X' },
                    { id: 'xbox_one_s_stand', name: 'Xbox One S Stand', description: 'Compact stand for Xbox One S' },
                    { id: 'xbox_one_controller_stand', name: 'Xbox One Controller Stand', description: 'Controller display stand' }
                ],
                'xbox_360': [
                    { id: 'xbox_360_stand', name: 'Xbox 360 Stand', description: 'Classic Xbox 360 display stand' },
                    { id: 'xbox_360_controller_rack', name: 'Xbox 360 Controller Rack', description: 'Multi-controller storage rack' }
                ]
            },
            nintendo: {
                'switch': [
                    { id: 'switch_dock_stand', name: 'Nintendo Switch Dock Stand', description: 'Portable dock display stand' },
                    { id: 'switch_pro_controller_stand', name: 'Switch Pro Controller Stand', description: 'Pro controller display stand' },
                    { id: 'switch_game_rack', name: 'Switch Game Card Rack', description: 'Game cartridge storage rack' }
                ],
                '3ds': [
                    { id: '3ds_xl_stand', name: 'New 3DS XL Stand', description: 'Foldable 3DS XL stand' },
                    { id: '3ds_charging_stand', name: '3DS Charging Stand', description: 'Stand with integrated charging' },
                    { id: '3ds_game_case', name: '3DS Game Case Stand', description: 'Game cartridge display case' }
                ],
                '2ds': [
                    { id: '2ds_ll_stand', name: 'New 2DS LL Stand', description: 'Ergonomic 2DS LL stand' },
                    { id: '2ds_display_stand', name: '2DS Display Stand', description: 'Premium display stand for 2DS' }
                ]
            },
            retro: {
                'snes': [
                    { id: 'snes_console_stand', name: 'SNES Console Stand', description: 'Retro-style SNES display stand' },
                    { id: 'snes_controller_holder', name: 'SNES Controller Holder', description: 'Classic controller display' }
                ],
                'nes': [
                    { id: 'nes_console_stand', name: 'NES Console Stand', description: 'Vintage NES display stand' },
                    { id: 'nes_game_rack', name: 'NES Game Cartridge Rack', description: 'Retro game storage solution' }
                ]
            },
            mobile: {
                'phone': [
                    { id: 'phone_gaming_stand', name: 'Mobile Gaming Stand', description: 'Adjustable phone gaming stand' },
                    { id: 'phone_controller_clip', name: 'Controller Phone Clip', description: 'Phone mount for controllers' },
                    { id: 'phone_cooling_stand', name: 'Phone Cooling Stand', description: 'Stand with cooling features' }
                ],
                'tablet': [
                    { id: 'tablet_gaming_stand', name: 'Tablet Gaming Stand', description: 'Multi-angle tablet stand' },
                    { id: 'tablet_controller_mount', name: 'Tablet Controller Mount', description: 'Tablet mount for gaming' }
                ]
            }
        };

        const subcategories = {
            sony: [
                { value: 'ps5', label: 'PlayStation 5' },
                { value: 'ps4', label: 'PlayStation 4' },
                { value: 'psvr', label: 'PlayStation VR' }
            ],
            microsoft: [
                { value: 'xbox_series', label: 'Xbox Series X/S' },
                { value: 'xbox_one', label: 'Xbox One (X/S/Original)' },
                { value: 'xbox_360', label: 'Xbox 360' }
            ],
            nintendo: [
                { value: 'switch', label: 'Nintendo Switch' },
                { value: '3ds', label: '3DS / New 3DS XL' },
                { value: '2ds', label: 'New 2DS LL' }
            ],
            retro: [
                { value: 'snes', label: 'Super Nintendo (SNES)' },
                { value: 'nes', label: 'Nintendo Entertainment System' }
            ],
            mobile: [
                { value: 'phone', label: 'Mobile Phone' },
                { value: 'tablet', label: 'Tablet' }
            ]
        };

        // Dark mode detection
        if (window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches) {
            document.documentElement.classList.add('dark');
        }
        window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', event => {
            if (event.matches) {
                document.documentElement.classList.add('dark');
            } else {
                document.documentElement.classList.remove('dark');
            }
        });

        // Generate product cards
        function generateProductCards() {
            const grid = document.getElementById('productsGrid');
            let html = '';

            Object.keys(productDatabase).forEach(category => {
                Object.keys(productDatabase[category]).forEach(subcategory => {
                    productDatabase[category][subcategory].forEach(product => {
                        html += `
                            <div class="product-card category-${category} cursor-pointer" onclick="selectProduct('${category}', '${subcategory}', '${product.id}')">
                                <div class="product-frame rounded-lg p-6 text-white h-48 flex flex-col justify-between">
                                    <div>
                                        <h4 class="font-bold text-lg mb-2">${product.name}</h4>
                                        <p class="text-sm opacity-90">${product.description}</p>
                                    </div>
                                    <div class="flex justify-between items-center">
                                        <span class="text-xs bg-white bg-opacity-20 px-2 py-1 rounded">${category.toUpperCase()}</span>
                                        <span class="text-xs">${subcategory.replace('_', ' ').toUpperCase()}</span>
                                    </div>
                                </div>
                            </div>
                        `;
                    });
                });
            });

            grid.innerHTML = html;
        }

        // Filter products by category
        function filterCategory(category) {
            const cards = document.querySelectorAll('.product-card');
            const buttons = document.querySelectorAll('.category-filter-btn');

            // Update button states
            buttons.forEach(btn => {
                btn.classList.remove('bg-primary', 'text-white');
                btn.classList.add('bg-gray-200', 'dark:bg-gray-600', 'text-gray-700', 'dark:text-gray-300');
            });
            event.target.classList.remove('bg-gray-200', 'dark:bg-gray-600', 'text-gray-700', 'dark:text-gray-300');
            event.target.classList.add('bg-primary', 'text-white');

            // Filter cards
            cards.forEach(card => {
                if (category === 'all' || card.classList.contains(`category-${category}`)) {
                    card.style.display = 'block';
                } else {
                    card.style.display = 'none';
                }
            });
        }

        // Select product from grid
        function selectProduct(category, subcategory, productId) {
            const categorySelect = document.getElementById('category');
            const subcategorySelect = document.getElementById('subcategory');
            const productSelect = document.getElementById('product');

            // Set category
            categorySelect.value = category;
            updateSubcategories();

            // Set subcategory
            setTimeout(() => {
                subcategorySelect.value = subcategory;
                updateProducts();

                // Set product
                setTimeout(() => {
                    productSelect.value = productId;
                }, 100);
            }, 100);

            // Scroll to form
            document.getElementById('orderForm').scrollIntoView({ behavior: 'smooth' });
        }

        // Update subcategories based on category selection
        function updateSubcategories() {
            const category = document.getElementById('category').value;
            const subcategorySelect = document.getElementById('subcategory');
            const productSelect = document.getElementById('product');

            // Reset dependent selects
            subcategorySelect.innerHTML = '<option value="">Select platform</option>';
            productSelect.innerHTML = '<option value="">Select platform first</option>';
            productSelect.disabled = true;

            if (category && subcategories[category]) {
                subcategorySelect.disabled = false;
                subcategories[category].forEach(sub => {
                    subcategorySelect.innerHTML += `<option value="${sub.value}">${sub.label}</option>`;
                });
            } else {
                subcategorySelect.disabled = true;
            }
        }

        // Update products based on subcategory selection
        function updateProducts() {
            const category = document.getElementById('category').value;
            const subcategory = document.getElementById('subcategory').value;
            const productSelect = document.getElementById('product');

            productSelect.innerHTML = '<option value="">Select a product</option>';

            if (category && subcategory && productDatabase[category] && productDatabase[category][subcategory]) {
                productSelect.disabled = false;
                productDatabase[category][subcategory].forEach(product => {
                    productSelect.innerHTML += `<option value="${product.id}">${product.name}</option>`;
                });
            } else {
                productSelect.disabled = true;
            }
        }

        // Toggle customization sections
        document.getElementById('logoEngraving').addEventListener('change', function() {
            const logoSection = document.getElementById('logoSection');
            logoSection.classList.toggle('hidden', !this.checked);
        });

        document.getElementById('customText').addEventListener('change', function() {
            const textSection = document.getElementById('textSection');
            textSection.classList.toggle('hidden', !this.checked);
        });

        // File upload handling
        const fileUploadArea = document.getElementById('fileUploadArea');
        const fileInput = document.getElementById('mockup');
        const filePreview = document.getElementById('filePreview');
        const previewImage = document.getElementById('previewImage');
        const fileName = document.getElementById('fileName');
        const fileUploadText = document.getElementById('fileUploadText');

        fileUploadArea.addEventListener('click', () => fileInput.click());

        fileUploadArea.addEventListener('dragover', (e) => {
            e.preventDefault();
            fileUploadArea.classList.add('drag-over');
        });

        fileUploadArea.addEventListener('dragleave', () => {
            fileUploadArea.classList.remove('drag-over');
        });

        fileUploadArea.addEventListener('drop', (e) => {
            e.preventDefault();
            fileUploadArea.classList.remove('drag-over');
            const files = e.dataTransfer.files;
            if (files.length > 0) {
                handleFileSelect(files[0]);
            }
        });

        fileInput.addEventListener('change', (e) => {
            if (e.target.files.length > 0) {
                handleFileSelect(e.target.files[0]);
            }
        });

        function handleFileSelect(file) {
            if (file && file.type.startsWith('image/')) {
                const reader = new FileReader();
                reader.onload = (e) => {
                    previewImage.src = e.target.result;
                    fileName.textContent = file.name;
                    filePreview.classList.remove('hidden');
                    fileUploadText.innerHTML = '<span class="font-medium text-primary">File selected:</span> Click to change';
                };
                reader.readAsDataURL(file);
            }
        }

        // Form submission
        const form = document.getElementById('orderForm');
        const submitBtn = document.getElementById('submitBtn');
        const submitText = document.getElementById('submitText');
        const loadingSpinner = document.getElementById('loadingSpinner');
        const successMessage = document.getElementById('successMessage');
        const errorMessage = document.getElementById('errorMessage');
        const errorText = document.getElementById('errorText');

        form.addEventListener('submit', async (e) => {
            e.preventDefault();
            
            // Show loading state
            submitBtn.disabled = true;
            submitText.textContent = 'Processing Order...';
            loadingSpinner.classList.remove('hidden');
            successMessage.classList.add('hidden');
            errorMessage.classList.add('hidden');

            try {
                // Collect comprehensive form data
                const formData = new FormData(form);
                const orderData = {
                    // Customer Info
                    customerName: formData.get('name'),
                    customerEmail: formData.get('email'),
                    
                    // Product Details
                    category: formData.get('category'),
                    subcategory: formData.get('subcategory'),
                    product: formData.get('product'),
                    quantity: formData.get('quantity'),
                    material: formData.get('material'),
                    color: formData.get('color'),
                    
                    // Customization
                    logoEngraving: formData.get('logoEngraving') ? 'Yes' : 'No',
                    customText: formData.get('customText') ? 'Yes' : 'No',
                    customTextInput: formData.get('customTextInput') || 'None',
                    
                    // Delivery
                    deliveryDate: formData.get('deliveryDate') || 'Not specified',
                    deliverySpeed: formData.get('deliverySpeed'),
                    shippingAddress: formData.get('shippingAddress'),
                    
                    // Additional
                    notes: formData.get('notes') || 'None',
                    orderTimestamp: new Date().toLocaleString()
                };

                // Get display names for better formatting
                const categorySelect = document.getElementById('category');
                const subcategorySelect = document.getElementById('subcategory');
                const productSelect = document.getElementById('product');
                
                const categoryDisplayName = categorySelect.options[categorySelect.selectedIndex].text;
                const subcategoryDisplayName = subcategorySelect.options[subcategorySelect.selectedIndex].text;
                const productDisplayName = productSelect.options[productSelect.selectedIndex].text;

                // Create comprehensive order confirmation message
                const orderMessage = `@Claude-Sonnet-4 Please format this as a professional order confirmation email for our gaming accessories store database that can be forwarded to Gmail:

**🎮 GAMING ACCESSORIES ORDER CONFIRMATION**

**📋 ORDER DETAILS:**
- Order ID: #GAO-${Date.now()}
- Date: ${orderData.orderTimestamp}
- Status: Processing

**👤 CUSTOMER INFORMATION:**
- Name: ${orderData.customerName}
- Email: ${orderData.customerEmail}

**🎯 PRODUCT SPECIFICATIONS:**
- Category: ${categoryDisplayName}
- Platform: ${subcategoryDisplayName}
- Product: ${productDisplayName}
- Quantity: ${orderData.quantity} units
- Material: ${orderData.material}
- Color/Finish: ${orderData.color}

**🎨 CUSTOMIZATION OPTIONS:**
- Logo Engraving: ${orderData.logoEngraving}
- Custom Text: ${orderData.customText}
${orderData.customText === 'Yes' ? `- Text to Engrave: "${orderData.customTextInput}"` : ''}
- Design File: ${fileInput.files.length > 0 ? 'Attached (see image)' : 'Not provided'}

**📦 DELIVERY INFORMATION:**
- Delivery Speed: ${orderData.deliverySpeed}
- Preferred Date: ${orderData.deliveryDate}
- Shipping Address: 
${orderData.shippingAddress}

**📝 ADDITIONAL NOTES:**
${orderData.notes}

**💰 PRICING & NEXT STEPS:**
- Quote will be provided within 24 hours
- Production timeline will be confirmed with quote
- Payment terms: 50% deposit, 50% on completion

Please format this as a professional email that includes:
1. Clear subject line with order number
2. Professional business greeting
3. Well-organized order summary table
4. Production timeline information
5. Payment and shipping terms
6. Contact information for questions
7. Professional closing signature

Make it ready to copy and send via Gmail to the customer and for our internal database records.`;

                // Prepare attachments if image is selected
                const attachments = [];
                if (fileInput.files.length > 0) {
                    attachments.push(fileInput.files[0]);
                }

                // Send comprehensive order via Poe API
                const result = await window.Poe.sendUserMessage(orderMessage, {
                    attachments: attachments,
                    openChat: true,
                    stream: false
                });

                if (result.success) {
                    // Show success message
                    successMessage.classList.remove('hidden');
                    form.reset();
                    filePreview.classList.add('hidden');
                    fileUploadText.innerHTML = '<span class="font-medium text-primary hover:text-primary-hover">Click to upload</span> or drag and drop';
                    
                    // Reset form dependencies
                    document.getElementById('subcategory').disabled = true;
                    document.getElementById('product').disabled = true;
                    document.getElementById('logoSection').classList.add('hidden');
                    document.getElementById('textSection').classList.add('hidden');
                    
                    // Scroll to success message
                    successMessage.scrollIntoView({ behavior: 'smooth' });
                } else {
                    throw new Error('Failed to submit order request');
                }

            } catch (error) {
                console.error('Error submitting order:', error);
                errorText.textContent = error.message || 'An unexpected error occurred. Please try again.';
                errorMessage.classList.remove('hidden');
                errorMessage.scrollIntoView({ behavior: 'smooth' });
            } finally {
                // Reset button state
                submitBtn.disabled = false;
                submitText.textContent = 'Submit Order Request';
                loadingSpinner.classList.add('hidden');
            }
        });

        // Initialize the page
        document.addEventListener('DOMContentLoaded', function() {
            generateProductCards();
        });
    </script>
</body>
</html>