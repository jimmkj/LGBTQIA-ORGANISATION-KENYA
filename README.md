
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
    <title>Upendo Kenya | LGBTQIA+ Rights & Safety Fund</title>
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Roboto, system-ui, -apple-system, sans-serif;
            background: linear-gradient(145deg, #0b0b1a 0%, #1a1a2e 100%);
            color: #e0d7ff;
            line-height: 1.6;
            padding: 1.5rem;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .container {
            max-width: 950px;
            width: 100%;
            background: rgba(18, 18, 30, 0.85);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border-radius: 3rem 3rem 2.5rem 2.5rem;
            padding: 2rem 2rem;
            box-shadow: 0 30px 50px rgba(0,0,0,0.7), 0 0 0 1px rgba(255, 215, 0, 0.2);
            border: 1px solid rgba(255, 255, 255, 0.08);
            margin: 1rem 0;
        }

        .header {
            text-align: center;
            margin-bottom: 1.8rem;
        }

        .logo-icon {
            font-size: 3.4rem;
            color: #f4b41a;
            background: rgba(244, 180, 26, 0.12);
            width: 85px;
            height: 85px;
            line-height: 85px;
            border-radius: 50%;
            margin: 0 auto 0.8rem;
            border: 2px solid #f4b41a;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        h1 {
            font-size: 2.6rem;
            font-weight: 700;
            letter-spacing: 1px;
            background: linear-gradient(to right, #f9d56e, #ffb347);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 0.3rem;
        }

        .subtitle {
            color: #b9a9ff;
            font-style: italic;
            font-size: 1.25rem;
            font-weight: 400;
            border-bottom: 1px dashed #6c63ff;
            display: inline-block;
            padding-bottom: 0.4rem;
        }

        .mission-badge {
            background: rgba(255, 87, 87, 0.18);
            color: #ffb3b3;
            padding: 0.8rem 1.8rem;
            border-radius: 3rem;
            font-weight: 600;
            margin: 1.2rem 0 0.2rem;
            display: inline-block;
            border: 1px solid #ff4d6d;
            backdrop-filter: blur(12px);
        }

        /* Story & Impact Section */
        .story-section {
            background: #12122a;
            border-radius: 2rem;
            padding: 2rem 1.8rem;
            margin: 1.8rem 0 2rem;
            border: 1px solid #4b3f7a;
            box-shadow: 0 10px 25px rgba(0,0,0,0.5);
        }

        .story-title {
            font-size: 1.8rem;
            font-weight: 700;
            color: #f4d03f;
            margin-bottom: 1.3rem;
            display: flex;
            align-items: center;
            gap: 0.6rem;
        }

        .story-text {
            color: #d9d0ff;
            margin-bottom: 1.5rem;
            font-size: 1.02rem;
        }

        .highlight-box {
            background: #1e1b3a;
            border-left: 6px solid #f4b41a;
            padding: 1.3rem 1.5rem;
            border-radius: 1rem;
            margin: 1.8rem 0;
            font-weight: 500;
        }

        .challenges-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.2rem;
            margin: 1.6rem 0;
        }

        .challenge-item {
            background: #0d0d24;
            padding: 1.2rem;
            border-radius: 1.5rem;
            text-align: center;
            border: 1px solid #5e4a8c;
        }

        .challenge-item i {
            font-size: 2rem;
            color: #f4b41a;
            margin-bottom: 0.5rem;
        }

        .impact-list {
            list-style: none;
            margin: 1.2rem 0;
        }

        .impact-list li {
            margin-bottom: 0.8rem;
            display: flex;
            align-items: flex-start;
            gap: 0.7rem;
        }

        .impact-list i {
            color: #6fcf97;
            font-size: 1.2rem;
            margin-top: 0.2rem;
        }

        .progress-section {
            background: #0f0f23;
            border-radius: 2rem;
            padding: 1.5rem;
            margin: 2rem 0 2.2rem;
            border: 1px solid #3b2b5c;
        }

        .progress-bar {
            height: 16px;
            background: #2d2a4a;
            border-radius: 30px;
            overflow: hidden;
            margin: 1rem 0 0.5rem;
        }

        .progress-fill {
            width: 38%;
            height: 100%;
            background: linear-gradient(90deg, #f4b41a, #ff7b3d);
            border-radius: 30px;
            box-shadow: 0 0 18px #f4a261;
        }

        .amount-options {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
            justify-content: center;
            margin: 1.8rem 0 1.2rem;
        }

        .amount-btn {
            background: #232136;
            border: 1px solid #6d5acf;
            color: #ddd6ff;
            padding: 0.7rem 1.2rem;
            border-radius: 2.5rem;
            font-weight: bold;
            font-size: 1.1rem;
            cursor: pointer;
            transition: all 0.25s ease;
            min-width: 70px;
            backdrop-filter: blur(8px);
        }

        .amount-btn.active {
            background: #6c63ff;
            border-color: #f4b41a;
            color: white;
            box-shadow: 0 0 18px #8c7aff;
            font-weight: 700;
            transform: scale(1.03);
        }

        .amount-btn:hover {
            background: #4a3f9a;
            border-color: #f4b41a;
            color: white;
        }

        .donate-box {
            background: #18182c;
            border-radius: 2rem;
            padding: 1.8rem;
            margin: 1.8rem 0;
            border: 1px solid #44407a;
        }

        .recipient-details {
            background: #0d0d1f;
            padding: 1.2rem;
            border-radius: 1.5rem;
            margin: 1.5rem 0 1rem;
            font-size: 0.95rem;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 0.8rem;
            border: 1px solid #5f4b8b;
        }

        .detail-item {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            background: #1e1a38;
            padding: 0.6rem 0.8rem;
            border-radius: 1rem;
            word-break: break-word;
        }

        .detail-item i {
            color: #f4b41a;
            font-size: 1.2rem;
        }

        .payment-methods {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 1.3rem;
            margin-top: 2rem;
        }

        .method-card {
            background: #1a1932;
            border-radius: 1.8rem;
            padding: 1.3rem;
            border: 1px solid #3d3580;
            transition: 0.2s;
            display: flex;
            flex-direction: column;
        }

        .method-card:hover {
            border-color: #f4b41a;
            background: #1f1d3e;
        }

        .method-header {
            display: flex;
            align-items: center;
            gap: 0.8rem;
            margin-bottom: 1rem;
        }

        .method-header i {
            font-size: 2rem;
            color: #f4b41a;
        }

        .method-header span {
            font-weight: 700;
            font-size: 1.5rem;
            letter-spacing: -0.3px;
        }

        .steps {
            list-style: none;
            margin: 0.8rem 0 0.5rem;
            font-size: 0.9rem;
            color: #d3c8ff;
            flex: 1;
        }

        .steps li {
            margin-bottom: 0.6rem;
            display: flex;
            gap: 0.5rem;
            align-items: baseline;
        }

        .steps i.fa-circle-check {
            color: #6fcf97;
            font-size: 0.9rem;
            margin-top: 0.25rem;
        }

        .express-badge {
            background: #ffb703;
            color: #0a0a1a;
            font-weight: bold;
            padding: 0.2rem 1rem;
            border-radius: 2rem;
            font-size: 0.8rem;
            display: inline-block;
            margin-left: 0.5rem;
        }

        .btn-donate {
            background: #f4b41a;
            color: #0a0a1a;
            font-weight: 800;
            padding: 1rem 1.8rem;
            border-radius: 3rem;
            border: none;
            font-size: 1.2rem;
            width: 100%;
            margin-top: 1.2rem;
            cursor: pointer;
            transition: 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
            letter-spacing: 0.5px;
        }

        .btn-donate:hover {
            background: #ffc34d;
            box-shadow: 0 0 25px #f4b41a;
            transform: translateY(-2px);
        }

        .footer-note {
            text-align: center;
            margin-top: 2.2rem;
            color: #aa9fdf;
            font-size: 0.95rem;
            border-top: 1px solid #403d6b;
            padding-top: 1.8rem;
        }

        @media (max-width: 550px) {
            .container {
                padding: 1.5rem 1rem;
            }
            .recipient-details {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="logo-icon">
                <i class="fas fa-rainbow"></i>
            </div>
            <h1>UPENDO KENYA</h1>
            <div class="subtitle">LGBTQIA+ Dignity & Freedom Fund</div>
            <div class="mission-badge">
                <i class="fas fa-shield-haltered"></i> Stop persecution. Build acceptance. Protect lives.
            </div>
        </div>

        <!-- OUR STORY & WHY DONATE -->
        <div class="story-section">
            <div class="story-title">
                <i class="fas fa-book-open"></i> Our Story & The Urgent Fight
            </div>
            <div class="story-text">
                <p><strong>Upendo Kenya</strong> was born in the shadows of silence — founded by a small group of brave LGBTQIA+ Kenyans and allies who refused to let fear dictate their existence. In a country where same-sex intimacy can lead to 14 years in prison, and where mob violence, blackmail, and forced evictions are daily realities, we decided to become the family many have lost.</p>
            </div>
            <div class="highlight-box">
                <i class="fas fa-exclamation-triangle" style="color:#f4b41a; margin-right: 0.4rem;"></i>
                <strong>In Kenya and across Africa, LGBTQIA+ people face imprisonment, brutal persecution, conversion torture, and rejection by their own families.</strong> Laws criminalize love; police target our community; healthcare and employment are often denied. We exist in a constant state of survival.
            </div>
            
            <h3 style="color:#f4d03f; margin-top:1.5rem;"><i class="fas fa-gavel"></i> Harsh Realities Our Siblings Endure</h3>
            <div class="challenges-grid">
                <div class="challenge-item">
                    <i class="fas fa-handcuffs"></i>
                    <h4>Jailing & Arrests</h4>
                    <p style="font-size:0.9rem;">Colonial-era laws punish LGBTQIA+ identity with up to 14 years imprisonment.</p>
                </div>
                <div class="challenge-item">
                    <i class="fas fa-house-damage"></i>
                    <h4>Homelessness</h4>
                    <p style="font-size:0.9rem;">Youth are disowned by families, forced onto streets vulnerable to exploitation.</p>
                </div>
                <div class="challenge-item">
                    <i class="fas fa-heart-broken"></i>
                    <h4>Violence & Torture</h4>
                    <p style="font-size:0.9rem;">Corrective rape, mob attacks, and police brutality are common across the region.</p>
                </div>
                <div class="challenge-item">
                    <i class="fas fa-ban"></i>
                    <h4>Denied Rights</h4>
                    <p style="font-size:0.9rem;">Access to healthcare, housing, and legal protection is systematically blocked.</p>
                </div>
            </div>

            <div style="margin-top: 1.8rem;">
                <h3 style="color:#f4d03f;"><i class="fas fa-seedling"></i> What Your Donation Will Do</h3>
                <ul class="impact-list">
                    <li><i class="fas fa-check-circle"></i> <strong>Legal Defense & Bail Funds:</strong> Free LGBTQIA+ individuals unjustly jailed and provide court representation.</li>
                    <li><i class="fas fa-check-circle"></i> <strong>Safe Houses & Emergency Shelter:</strong> Run confidential shelters for those fleeing violence or family rejection.</li>
                    <li><i class="fas fa-check-circle"></i> <strong>Community Awareness Campaigns:</strong> Grassroots dialogues to reduce stigma and promote acceptance in local communities.</li>
                    <li><i class="fas fa-check-circle"></i> <strong>Mental Health & HIV Care:</strong> Provide crisis counseling, support groups, and linkage to friendly health services.</li>
                    <li><i class="fas fa-check-circle"></i> <strong>Advocacy & Movement Building:</strong> Push for decriminalization and policy change while training activists.</li>
                </ul>
            </div>
            <p style="margin-top:1.2rem; font-style:italic; background:#1f1b3a; padding:1rem; border-radius:1rem;">
                <i class="fas fa-quote-left" style="color:#f4b41a;"></i> 
                <strong>Every dollar shields someone from a prison cell, keeps a roof over a queer teen's head, and tells our community: you are not alone.</strong> 
                We are an officially registered NGO operating transparently in Kenya. Your donation directly funds freedom and dignity.
                <i class="fas fa-quote-right" style="color:#f4b41a;"></i>
            </p>
        </div>

        <!-- Fundraising progress -->
        <div class="progress-section">
            <div style="display: flex; justify-content: space-between; font-weight: 600;">
                <span><i class="fas fa-heart" style="color:#ff6b6b;"></i> $3,800 raised</span>
                <span>Goal: $10,000</span>
            </div>
            <div class="progress-bar">
                <div class="progress-fill"></div>
            </div>
            <p style="margin-top: 0.4rem; font-size: 0.9rem; color: #b7adff;">Community legal aid, safe houses & advocacy · Every dollar protects a life.</p>
        </div>

        <!-- Amount selector -->
        <div style="text-align: center;">
            <p style="font-weight: 600; margin-bottom: 0.2rem;"><i class="fas fa-hand-holding-heart"></i> Choose your donation (USD)</p>
            <div class="amount-options" id="amountButtons">
                <button class="amount-btn active" data-amount="5">$5</button>
                <button class="amount-btn" data-amount="25">$25</button>
                <button class="amount-btn" data-amount="50">$50</button>
                <button class="amount-btn" data-amount="100">$100</button>
                <button class="amount-btn" data-amount="250">$250</button>
                <button class="amount-btn" data-amount="500">$500</button>
                <button class="amount-btn" data-amount="1000">$1000</button>
            </div>
            <p style="font-size: 0.9rem; color: #b7adff;">Selected: <strong id="selectedAmountDisplay">$5</strong></p>
        </div>

        <!-- Recipient details (fixed) -->
        <div class="donate-box">
            <h3 style="display: flex; align-items: center; gap: 0.5rem; color: #f4d03f;"><i class="fas fa-user-circle"></i> Recipient Details (NGO Account)</h3>
            <div class="recipient-details">
                <div class="detail-item"><i class="fas fa-user"></i> <strong>James Warigithi Karanja</strong></div>
                <div class="detail-item"><i class="fas fa-mobile-alt"></i> M-Pesa: <strong>+254715869346</strong></div>
                <div class="detail-item"><i class="fas fa-globe"></i> Country: <strong>Kenya</strong></div>
                <div class="detail-item"><i class="fas fa-bolt"></i> Speed: <span class="express-badge">EXPRESS</span></div>
            </div>
            <p style="margin: 1rem 0 0.3rem; font-weight: 600;"><i class="fas fa-university"></i> Send via Remitly, Revolut or Wise</p>
        </div>

        <!-- Payment Methods Instructions -->
        <div class="payment-methods">
            <!-- Remitly Card -->
            <div class="method-card">
                <div class="method-header">
                    <i class="fas fa-paper-plane"></i>
                    <span>Remitly</span>
                </div>
                <ul class="steps">
                    <li><i class="fas fa-circle-check"></i> Open Remitly app or remitly.com</li>
                    <li><i class="fas fa-circle-check"></i> Select <strong>Kenya</strong> as destination.</li>
                    <li><i class="fas fa-circle-check"></i> Choose <strong>Mobile Money (M-Pesa)</strong>.</li>
                    <li><i class="fas fa-circle-check"></i> Enter amount: <span id="remitlyAmount">$5</span> USD.</li>
                    <li><i class="fas fa-circle-check"></i> Recipient: <strong>James Warigithi Karanja</strong></li>
                    <li><i class="fas fa-circle-check"></i> M-Pesa number: <strong>+254715869346</strong></li>
                    <li><i class="fas fa-circle-check"></i> Delivery: <span class="express-badge">Express</span> (minutes)</li>
                </ul>
                <button class="btn-donate" onclick="alert('Thank you for using Remitly! Please complete the transfer in the app. Asante sana! 🌈')"><i class="fas fa-external-link-alt"></i> Donate with Remitly</button>
            </div>

            <!-- Revolut Card -->
            <div class="method-card">
                <div class="method-header">
                    <i class="fas fa-exchange-alt"></i>
                    <span>Revolut</span>
                </div>
                <ul class="steps">
                    <li><i class="fas fa-circle-check"></i> Open Revolut app → Payments.</li>
                    <li><i class="fas fa-circle-check"></i> Add new beneficiary: <strong>Kenya</strong>.</li>
                    <li><i class="fas fa-circle-check"></i> Choose <strong>Mobile Wallet (M-Pesa)</strong>.</li>
                    <li><i class="fas fa-circle-check"></i> Amount: <span id="revolutAmount">$5</span> USD.</li>
                    <li><i class="fas fa-circle-check"></i> Full name: <strong>James Warigithi Karanja</strong></li>
                    <li><i class="fas fa-circle-check"></i> Phone: <strong>+254715869346</strong></li>
                    <li><i class="fas fa-circle-check"></i> Select <strong>Express</strong> transfer.</li>
                </ul>
                <button class="btn-donate" onclick="alert('Thank you! Complete the transfer in Revolut. Your support saves lives. 🏳️‍🌈')"><i class="fas fa-external-link-alt"></i> Donate with Revolut</button>
            </div>

            <!-- Wise Card -->
            <div class="method-card">
                <div class="method-header">
                    <i class="fas fa-globe-americas"></i>
                    <span>Wise</span>
                </div>
                <ul class="steps">
                    <li><i class="fas fa-circle-check"></i> Go to Wise app or wise.com</li>
                    <li><i class="fas fa-circle-check"></i> Send to <strong>Kenya</strong> → Mobile money.</li>
                    <li><i class="fas fa-circle-check"></i> Amount: <span id="wiseAmount">$5</span> USD.</li>
                    <li><i class="fas fa-circle-check"></i> Recipient: <strong>James Warigithi Karanja</strong></li>
                    <li><i class="fas fa-circle-check"></i> M-Pesa: <strong>+254715869346</strong></li>
                    <li><i class="fas fa-circle-check"></i> Choose <strong>Express</strong> (fast delivery).</li>
                    <li><i class="fas fa-circle-check"></i> Review fee & confirm payment.</li>
                </ul>
                <button class="btn-donate" onclick="alert('Wise transfer ready! Please proceed in Wise. Together we rise. ✊🏾')"><i class="fas fa-external-link-alt"></i> Donate with Wise</button>
            </div>
        </div>

        <div class="footer-note">
            <p><i class="fas fa-lock" style="color:#6fcf97;"></i> <strong>Upendo Kenya</strong> is a registered NGO advocating for LGBTQIA+ rights, safety, and community acceptance. Your donation directly funds legal support, safe spaces, and awareness campaigns.</p>
            <p style="margin-top: 0.8rem; font-size: 0.9rem;">🌈 <i>“Haki kwa wote” – Justice for all.</i> Thank you <strong>Kimi</strong> for standing with us.</p>
        </div>
    </div>

    <script>
        (function() {
            const amountButtons = document.querySelectorAll('.amount-btn');
            const selectedDisplay = document.getElementById('selectedAmountDisplay');
            const remitlySpan = document.getElementById('remitlyAmount');
            const revolutSpan = document.getElementById('revolutAmount');
            const wiseSpan = document.getElementById('wiseAmount');

            function updateAmounts(amount) {
                if (selectedDisplay) selectedDisplay.textContent = '$' + amount;
                if (remitlySpan) remitlySpan.textContent = '$' + amount;
                if (revolutSpan) revolutSpan.textContent = '$' + amount;
                if (wiseSpan) wiseSpan.textContent = '$' + amount;
            }

            amountButtons.forEach(btn => {
                btn.addEventListener('click', function(e) {
                    amountButtons.forEach(b => b.classList.remove('active'));
                    this.classList.add('active');
                    const amount = this.getAttribute('data-amount');
                    updateAmounts(amount);
                });
            });

            const activeBtn = document.querySelector('.amount-btn.active');
            if (activeBtn) {
                updateAmounts(activeBtn.getAttribute('data-amount'));
            } else {
                updateAmounts('5');
            }
        })();
    </script>
</body>
</html>
