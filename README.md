<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Maro Shop - Game Recharge</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <style>
        /* General background and text */
        body {
            background: linear-gradient(135deg, #1f2937, #4b5563);
            color: #f3f4f6;
        }

        /* Shine effect for the site title */
        .shine {
            font-size: 3.5rem;
            font-weight: bold;
            background: linear-gradient(90deg, #f39c12, #f1c40f, #e67e22);
            background-size: 200% 200%;
            animation: shine 3s linear infinite;
            color: white;
            text-align: center;
            margin-bottom: 30px;
            text-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }

        @keyframes shine {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Cards (games) style */
        .game-card {
            transition: transform 0.4s, box-shadow 0.4s;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .game-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 24px rgba(0, 0, 0, 0.5);
        }

        /* Buttons */
        .option-btn {
            padding: 12px 24px;
            background-color: #f39c12;
            color: white;
            font-weight: bold;
            border-radius: 12px;
            transition: background-color 0.3s ease, transform 0.3s ease;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
        }

        .option-btn:hover {
            background-color: #f1c40f;
            transform: scale(1.05);
        }

        .contact-btn {
            background-color: #1abc9c;
            color: white;
            padding: 12px 24px;
            border-radius: 12px;
            font-weight: bold;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        .contact-btn:hover {
            background-color: #16a085;
            transform: scale(1.05);
        }

        /* Section Spacing */
        section {
            padding: 60px 0;
        }

        /* Footer */
        footer {
            background-color: #111827;
            padding: 30px;
            text-align: center;
            color: #f3f4f6;
        }
    </style>
</head>
<body class="font-sans">

    <!-- Header -->
    <header class="bg-gray-800 p-6 shadow-lg">
        <div class="container mx-auto flex justify-between items-center">
            <h1 class="shine">Maro Shop</h1>
            <nav>
                <ul class="flex space-x-6">
                    <li><a href="#home" class="hover:text-yellow-400">Home</a></li>
                    <li><a href="#games" class="hover:text-yellow-400">Games</a></li>
                    <li><a href="#contact" class="hover:text-yellow-400">Contact Us</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="bg-gray-700 text-center py-20">
        <h2 class="text-5xl font-bold mb-6">Best Game Recharge Services</h2>
        <p class="text-lg mb-8">Get your favorite currency for Free Fire, PUBG, Clash of Clans, PES, Clash Royale, FIFA, Roblox, and more quickly and securely.</p>
        <a href="#games" class="bg-yellow-400 text-gray-900 px-6 py-3 rounded-lg font-semibold hover:shadow-lg transition">Start Now</a>
    </section>

    <!-- Games Section -->
    <section id="games" class="py-20">
        <div class="container mx-auto text-center">
            <h2 class="text-4xl font-bold mb-6">Choose Your Game</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-8">

                <!-- PUBG Section -->
                <div class="game-card bg-gray-800 p-6 rounded-lg shadow-lg">
                    <h3 class="text-2xl font-bold mb-4">PUBG</h3>
                    <button onclick="showPrices('pubg-options')" class="bg-yellow-400 text-gray-900 px-6 py-3 rounded-lg font-semibold">Show Prices</button>
                    <div id="pubg-options" class="hidden mt-6 text-left">
                        <h4 class="text-xl font-bold">PUBG Global Prices</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">60 UC: 55L.E</li>
                            <li class="mb-2">120 UC: 110L.E</li>
                            <li class="mb-2">180 UC: 160L.E</li>
                            <li class="mb-2">240 UC: 195L.E</li>
                            <li class="mb-2">325 UC: 225L.E</li>
                            <li class="mb-2">355 UC: 250L.E</li>
                            <li class="mb-2">660 UC: 430L.E</li>
                            <li class="mb-2">720 UC: 470L.E</li>
                            <li class="mb-2">1800 UC: 1050L.E</li>
                            <li class="mb-2">3850 UC: 2175L.E</li>
                            <li class="mb-2">8100 UC: 4300L.E</li>
                        </ul>

                        <h4 class="text-xl font-bold mt-6">PUBG Korea Prices</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">60 UC: 60L.E</li>
                            <li class="mb-2">190 UC: 180L.E</li>
                            <li class="mb-2">310 UC: 280L.E</li>
                            <li class="mb-2">380 UC: 330L.E</li>
                            <li class="mb-2">660 UC: 525L.E</li>
                            <li class="mb-2">1800 UC: 1250L.E</li>
                        </ul>
                    </div>
                </div>

                <!-- Free Fire Section -->
                <div class="game-card bg-gray-800 p-6 rounded-lg shadow-lg">
                    <h3 class="text-2xl font-bold mb-4">Free Fire</h3>
                    <button onclick="showPrices('freefire-options')" class="bg-yellow-400 text-gray-900 px-6 py-3 rounded-lg font-semibold">Show Prices</button>
                    <div id="freefire-options" class="hidden mt-6 text-left">
                        <h4 class="text-xl font-bold">Free Fire Diamonds Prices</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">110 💎: 50 L.E</li>
                            <li class="mb-2">341 💎: 140 L.E</li>
                            <li class="mb-2">572 💎: 230 L.E</li>
                            <li class="mb-2">1023 💎: 380 L.E</li>
                            <li class="mb-2">2079 💎: 750 L.E</li>
                            <li class="mb-2">5016 💎: 1650 L.E</li>
                            <li class="mb-2">10032 💎: 3250 L.E</li>
                        </ul>

                        <h4 class="text-xl font-bold mt-6">Free Fire Drops & Memberships</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">Drob 1$: 60 L.E</li>
                            <li class="mb-2">Drob 2$: 100 L.E</li>
                            <li class="mb-2">Level Pass 570 💎: 70 L.E</li>
                            <li class="mb-2">Weekly Membership 450 💎: 85 L.E</li>
                            <li class="mb-2">ID - Weekly Membership 450 💎: 100 L.E</li>
                            <li class="mb-2">ID - Monthly Membership 2600 💎: 290 L.E</li>
                        </ul>
                    </div>
                </div>

                <!-- Clash of Clans Section -->
                <div class="game-card bg-gray-800 p-6 rounded-lg shadow-lg">
                    <h3 class="text-2xl font-bold mb-4">Clash of Clans</h3>
                    <button onclick="showPrices('clashofclans-options')" class="bg-yellow-400 text-gray-900 px-6 py-3 rounded-lg font-semibold">Show Prices</button>
                    <div id="clashofclans-options" class="hidden mt-6 text-left">
                        <h4 class="text-xl font-bold">Clash of Clans Gems Prices</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">500 🟢: 210 💸 L.E</li>
                            <li class="mb-2">1200 🟢: 415 💸 L.E</li>
                            <li class="mb-2">2500 🟢: 770 💸 L.E</li>
                            <li class="mb-2">6500 🟢: 1850 💸 L.E</li>
                            <li class="mb-2">14000 🟢: 3600 💸 L.E</li>
                        </ul>
                    </div>
                </div>

                <!-- PES Section -->
                <div class="game-card bg-gray-800 p-6 rounded-lg shadow-lg">
                    <h3 class="text-2xl font-bold mb-4">PES</h3>
                    <button onclick="showPrices('pes-options')" class="bg-yellow-400 text-gray-900 px-6 py-3 rounded-lg font-semibold">Show Prices</button>
                    <div id="pes-options" class="hidden mt-6 text-left">
                        <h4 class="text-xl font-bold">PES Coins Prices</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">130 coun: 60 L.E</li>
                            <li class="mb-2">550 coun: 200 L.E</li>
                            <li class="mb-2">750 coun: 280 L.E</li>
                            <li class="mb-2">1040 coun: 400 L.E</li>
                            <li class="mb-2">2130 coun: 750 L.E</li>
                            <li class="mb-2">3250 coun: 1250 L.E</li>
                            <li class="mb-2">5700 coun: 2000 L.E</li>
                        </ul>
                    </div>
                </div>

                <!-- Clash Royale Section -->
                <div class="game-card bg-gray-800 p-6 rounded-lg shadow-lg">
                    <h3 class="text-2xl font-bold mb-4">Clash Royale</h3>
                    <button onclick="showPrices('clashroyale-options')" class="bg-yellow-400 text-gray-900 px-6 py-3 rounded-lg font-semibold">Show Prices</button>
                    <div id="clashroyale-options" class="hidden mt-6 text-left">
                        <h4 class="text-xl font-bold">Clash Royale Gems Prices</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">500 👾: 210 💸 L.E</li>
                            <li class="mb-2">1200 👾: 415 💸 L.E</li>
                            <li class="mb-2">2500 👾: 770 💸 L.E</li>
                            <li class="mb-2">6500 👾: 1850 💸 L.E</li>
                            <li class="mb-2">14000 👾: 3600 💸 L.E</li>
                        </ul>

                        <h4 class="text-xl font-bold mt-6">Clash Royale Passes</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">Gold Pass: 270 L.E</li>
                            <li class="mb-2">Diamond Pass: 550 L.E</li>
                        </ul>
                    </div>
                </div>

                <!-- FIFA Section -->
                <div class="game-card bg-gray-800 p-6 rounded-lg shadow-lg">
                    <h3 class="text-2xl font-bold mb-4">FIFA</h3>
                    <button onclick="showPrices('fifa-options')" class="bg-yellow-400 text-gray-900 px-6 py-3 rounded-lg font-semibold">Show Prices</button>
                    <div id="fifa-options" class="hidden mt-6 text-left">
                        <h4 class="text-xl font-bold">FIFA Coins Prices</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">100 coun: 60 L.E</li>
                            <li class="mb-2">600 coun: 230 L.E</li>
                            <li class="mb-2">1200 coun: 450 L.E</li>
                            <li class="mb-2">2600 coun: 900 L.E</li>
                            <li class="mb-2">6900 coun: 2250 L.E</li>
                        </ul>
                    </div>
                </div>

                <!-- Roblox Section -->
                <div class="game-card bg-gray-800 p-6 rounded-lg shadow-lg">
                    <h3 class="text-2xl font-bold mb-4">Roblox</h3>
                    <button onclick="showPrices('roblox-options')" class="bg-yellow-400 text-gray-900 px-6 py-3 rounded-lg font-semibold">Show Prices</button>
                    <div id="roblox-options" class="hidden mt-6 text-left">
                        <h4 class="text-xl font-bold">Roblox Robux Prices</h4>
                        <ul class="mt-6 text-left">
                            <li class="mb-2">40 🔸: 35 L.E</li>
                            <li class="mb-2">80 🔸: 60 L.E</li>
                            <li class="mb-2">400 🔸: 230 L.E</li>
                            <li class="mb-2">800 🔸: 445 L.E</li>
                            <li class="mb-2">1700 🔸: 880 L.E</li>
                            <li class="mb-2">4500 🔸: 2200 L.E</li>
                            <li class="mb-2">10000 🔸: 4400 L.E</li>
                            <li class="mb-2">22500 🔸: 8800 L.E</li>
                        </ul>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="bg-gray-700 py-20">
        <div class="container mx-auto text-center">
            <h2 class="text-4xl font-bold mb-6">Contact Us</h2>
            <p class="text-lg mb-8">For any inquiries about recharge services, contact us directly or use the form below.</p>
            <button onclick="showContactLinks()" class="contact-btn">التواصل</button>
            <div id="contact-links" class="hidden mt-6">
                <a href="https://wa.me/+201271303100" class="block mt-2">WhatsApp</a>
                <a href="https://wa.me/+201024857074" class="block mt-2">WhatsApp</a>
                <a href="https://www.instagram.com/marwan_________kamal/profilecard/?igsh=MTB2c2cweWY4dzM1OA==" class="block mt-2">Instagram</a>
                <a href="https://www.facebook.com/profile.php?id=100072001516986&mibextid=LQQJ4d" class="block mt-2">Facebook</a>
                
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-center py-6">
        <p>&copy; 2024 All rights reserved - Maro Shop</p>
    </footer>

    <script>
        function showPrices(sectionId) {
            const allSections = ['pubg-options', 'freefire-options', 'clashofclans-options', 'pes-options', 'clashroyale-options', 'fifa-options', 'roblox-options'];
            allSections.forEach(section => {
                if (section !== sectionId) {
                    document.getElementById(section).classList.add('hidden');
                }
            });
            document.getElementById(sectionId).classList.toggle('hidden');
        }

        function showContactLinks() {
            document.getElementById('contact-links').classList.toggle('hidden');
        }
    </script>
</body>
</html>
