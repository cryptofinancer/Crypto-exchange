I'll create a professional cryptocurrency selling website for you with the payment address you provided. Here's a complete, modern website:


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CryptoExchange - Buy Cryptocurrency Instantly</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.1);
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 28px;
            font-weight: bold;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 30px;
        }

        .nav-links a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #667eea;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 100px 0;
            color: white;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            animation: fadeInUp 1s;
        }

        .hero p {
            font-size: 20px;
            margin-bottom: 40px;
            animation: fadeInUp 1s 0.2s backwards;
        }

        .cta-button {
            background: white;
            color: #667eea;
            padding: 15px 40px;
            border: none;
            border-radius: 50px;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            animation: fadeInUp 1s 0.4s backwards;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }

        /* Crypto Cards Section */
        .crypto-section {
            background: white;
            padding: 80px 0;
        }

        .section-title {
            text-align: center;
            font-size: 36px;
            margin-bottom: 50px;
            color: #333;
        }

        .crypto-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 50px;
        }

        .crypto-card {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
            cursor: pointer;
        }

        .crypto-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.15);
        }

        .crypto-icon {
            font-size: 60px;
            margin-bottom: 15px;
        }

        .crypto-card h3 {
            font-size: 24px;
            margin-bottom: 10px;
            color: #333;
        }

        .crypto-card .symbol {
            color: #666;
            font-size: 14px;
            margin-bottom: 15px;
        }

        .price {
            font-size: 28px;
            font-weight: bold;
            color: #667eea;
            margin-bottom: 20px;
        }

        .buy-button {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 25px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.3s;
        }

        .buy-button:hover {
            transform: scale(1.05);
        }

        /* Payment Modal */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 1000;
            justify-content: center;
            align-items: center;
            animation: fadeIn 0.3s;
        }

        .modal-content {
            background: white;
            padding: 40px;
            border-radius: 20px;
            max-width: 500px;
            width: 90%;
            position: relative;
            animation: slideUp 0.3s;
        }

        .close {
            position: absolute;
            top: 15px;
            right: 20px;
            font-size: 30px;
            cursor: pointer;
            color: #666;
        }

        .close:hover {
            color: #333;
        }

        .modal h2 {
            margin-bottom: 20px;
            color: #333;
        }

        .payment-address {
            background: #f5f7fa;
            padding: 15px;
            border-radius: 10px;
            word-break: break-all;
            margin: 20px 0;
            font-family: monospace;
            font-size: 14px;
            border: 2px dashed #667eea;
        }

        .copy-button {
            background: #667eea;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 10px;
            cursor: pointer;
            width: 100%;
            font-size: 16px;
            margin-top: 10px;
            transition: background 0.3s;
        }

        .copy-button:hover {
            background: #5568d3;
        }

        .instruction {
            background: #fff3cd;
            border-left: 4px solid #ffc107;
            padding: 15px;
            margin: 20px 0;
            border-radius: 5px;
        }

        /* Features Section */
        .features {
            padding: 80px 0;
            background: #f9f9f9;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-top: 50px;
        }

        .feature-item {
            text-align: center;
        }

        .feature-icon {
            font-size: 50px;
            margin-bottom: 20px;
        }

        .feature-item h3 {
            font-size: 22px;
            margin-bottom: 10px;
            color: #333;
        }

        /* Footer */
        footer {
            background: #222;
            color: white;
            text-align: center;
            padding: 30px 0;
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes slideUp {
            from {
                transform: translateY(50px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 32px;
            }

            .nav-links {
                gap: 15px;
                font-size: 14px;
            }

            .section-title {
                font-size: 28px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <div class="logo">🚀 CryptoExchange</div>
                <ul class="nav-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#buy">Buy Crypto</a></li>
                    <li><a href="#features">Features</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Buy Cryptocurrency Instantly</h1>
            <p>Trade Bitcoin, Ethereum, Solana, and more with ease</p>
            <button class="cta-button" onclick="document.getElementById('buy').scrollIntoView({behavior: 'smooth'})">
                Start Trading Now
            </button>
        </div>
    </section>

    <!-- Crypto Cards Section -->
    <section class="crypto-section" id="buy">
        <div class="container">
            <h2 class="section-title">Available Cryptocurrencies</h2>
            <div class="crypto-grid">
                <!-- Bitcoin -->
                <div class="crypto-card">
                    <div class="crypto-icon">₿</div>
                    <h3>Bitcoin</h3>
                    <p class="symbol">BTC</p>
                    <div class="price">$65,000</div>
                    <button class="buy-button" onclick="openModal('Bitcoin', 'BTC')">Buy Now</button>
                </div>

                <!-- Ethereum -->
                <div class="crypto-card">
                    <div class="crypto-icon">Ξ</div>
                    <h3>Ethereum</h3>
                    <p class="symbol">ETH</p>
                    <div class="price">$3,200</div>
                    <button class="buy-button" onclick="openModal('Ethereum', 'ETH')">Buy Now</button>
                </div>

                <!-- Solana -->
                <div class="crypto-card">
                    <div class="crypto-icon">◎</div>
                    <h3>Solana</h3>
                    <p class="symbol">SOL</p>
                    <div class="price">$145</div>
                    <button class="buy-button" onclick="openModal('Solana', 'SOL')">Buy Now</button>
                </div>

                <!-- Polygon -->
                <div class="crypto-card">
                    <div class="crypto-icon">⬡</div>
                    <h3>Polygon</h3>
                    <p class="symbol">MATIC</p>
                    <div class="price">$0.85</div>
                    <button class="buy-button" onclick="openModal('Polygon', 'MATIC')">Buy Now</button>
                </div>

                <!-- Sui -->
                <div class="crypto-card">
                    <div class="crypto-icon">💧</div>
                    <h3>Sui</h3>
                    <p class="symbol">SUI</p>
                    <div class="price">$1.45</div>
                    <button class="buy-button" onclick="openModal('Sui', 'SUI')">Buy Now</button>
                </div>

                <!-- Dogecoin -->
                <div class="crypto-card">
                    <div class="crypto-icon">Ð</div>
                    <h3>Dogecoin</h3>
                    <p class="symbol">DOGE</p>
                    <div class="price">$0.12</div>
                    <button class="buy-button" onclick="openModal('Dogecoin', 'DOGE')">Buy Now</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features" id="features">
        <div class="container">
            <h2 class="section-title">Why Choose Us?</h2>
            <div class="features-grid">
                <div class="feature-item">
                    <div class="feature-icon">🔒</div>
                    <h3>Secure Trading</h3>
                    <p>Your transactions are protected with industry-leading security</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">⚡</div>
                    <h3>Instant Transfer</h3>
                    <p>Get your crypto delivered instantly to your wallet</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">💰</div>
                    <h3>Best Rates</h3>
                    <p>Competitive prices with low transaction fees</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">📞</div>
                    <h3>24/7 Support</h3>
                    <p>Our team is always here to help you</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Payment Modal -->
    <div id="paymentModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal()">&times;</span>
            <h2>Purchase <span id="cryptoName"></span></h2>
            
            <div class="instruction">
                <strong>⚠️ Important Instructions:</strong>
                <ol style="margin-top: 10px; padding-left: 20px;">
                    <li>Send your payment to the Ethereum address below</li>
                    <li>After payment, contact us with your transaction hash</li>
                    <li>Provide your wallet address to receive your crypto</li>
                </ol>
            </div>

            <p><strong>Payment Address (Ethereum):</strong></p>
            <div class="payment-address" id="paymentAddress">
                0x5446475616f4C860ecE4c30A9f9931eB2b5dEB7a
            </div>
            
            <button class="copy-button" onclick="copyAddress()">
                📋 Copy Address
            </button>

            <div style="margin-top: 20px; padding: 15px; background: #e7f3ff; border-radius: 10px;">
                <p style="font-size: 14px; color: #0066cc;">
                    <strong>Next Steps:</strong><br>
                    After sending payment, please email us at <strong>support@cryptoexchange.com</strong> with:
                    <br>• Transaction hash
                    <br>• Your wallet address
                    <br>• Amount of <span id="cryptoSymbol"></span> to purchase
                </p>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer id="contact">
        <div class="container">
            <p>&copy; 2024 CryptoExchange. All rights reserved.</p>
            <p>Email: support@cryptoexchange.com | Trade responsibly</p>
        </div>
    </footer>

    <script>
        function openModal(cryptoName, cryptoSymbol) {
            document.getElementById('cryptoName').textContent = cryptoName;
            document.getElementById('cryptoSymbol').textContent = cryptoSymbol;
            document.getElementById('paymentModal').style.display = 'flex';
        }

        function closeModal() {
            document.getElementById('paymentModal').style.display = 'none';
        }

        function copyAddress() {
            const address = document.getElementById('paymentAddress').textContent.trim();
            navigator.clipboard.writeText(address).then(() => {
                const button = event.target;
                const originalText = button.textContent;
                button.textContent = '✓ Copied!';
                button.style.background = '#28a745';
                
                setTimeout(() => {
                    button.textContent = originalText;
                    button.style.background = '#667eea';
                }, 2000);
            });
        }

        // Close modal when clicking outside
        window.onclick = function(event) {
            const modal = document.getElementById('paymentModal');
            if (event.target == modal) {
                closeModal();
            }
        }

        // Close modal with Escape key
        document.addEventListener('keydown', function(event) {
            if (event.key === 'Escape') {
                closeModal();
            }
        });
    </script>
</body>
</html>


**Features of this website:**


✅ **6 Cryptocurrencies**: Bitcoin, Ethereum, Solana, Polygon, Sui, and Dogecoin
✅ **Modern Design**: Gradient backgrounds, smooth animations, and responsive layout
✅ **Payment Integration**: Your Ethereum address (0x5446475616f4C860ecE4c30A9f9931eB2b5dEB7a) is embedded
✅ **Buy Buttons**: Each crypto has a "Buy Now" button that opens a payment modal
✅ **Copy Function**: Users can easily copy your payment address with one click
✅ **Mobile Responsive**: Works perfectly on all devices
✅ **Professional Sections**: Hero, crypto cards, features, and footer
✅ **Instructions**: Clear payment instructions for buyers


**To use this website:**

1. Save the code as `index.html`
2. Open it in any web browser
3. Users click "Buy Now" on any crypto
4. They see your Ethereum payment address
5. They can copy it and send payment


**⚠️ Important Notes:**
• This is a basic frontend template
• You'll need to manually process orders when customers contact you
• Consider adding a backend for automated order processing
• Update the crypto prices regularly
• Add your real contact email
• Consider adding SSL certificate when hosting live


Would you like me to add any additional features like a contact form, live price updates, or a shopping cart system?
