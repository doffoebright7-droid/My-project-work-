<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apex Gift Solution – Elevating Every Gesture</title>
    <style>
        :root {
            --navy: #0A2240;
            --gold: #C9A961;
            --light-gold: #F5F0E6;
            --white: #FFFFFF;
            --grey: #5D6D7E;
            --light-bg: #FAFBFC;
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Arial, sans-serif; }
        body { background: var(--light-bg); color: #333; line-height: 1.7; }
        header { background: var(--navy); color: white; padding: 1rem 0; position: sticky; top: 0; z-index: 100; box-shadow: 0 2px 10px rgba(10,34,64,0.2); }
        nav { max-width: 1200px; margin: auto; display: flex; justify-content: space-between; align-items: center; padding: 0 20px; }
        .logo { display: flex; align-items: center; gap: 12px; }
        .logo img { height: 50px; }
        .logo-text { font-size: 1.3rem; font-weight: 700; }
        .logo-text span { display: block; font-size: 0.7rem; color: var(--gold); font-weight: 400; letter-spacing: 1px; }
        nav ul { display: flex; list-style: none; gap: 25px; flex-wrap: wrap; }
        nav a { color: white; text-decoration: none; font-weight: 600; transition: 0.3s; }
        nav a:hover { color: var(--gold); }
       .container { max-width: 1200px; margin: auto; padding: 50px 20px; }
        section { background: white; margin-bottom: 35px; padding: 40px; border-radius: 12px; box-shadow: 0 2px 15px rgba(10,34,64,0.08); }
        h1, h2, h3, h4 { color: var(--navy); margin-bottom: 15px; }
        h1 { font-size: 2.8rem; line-height: 1.2; }
        h2 { font-size: 2.2rem; border-bottom: 3px solid var(--gold); padding-bottom: 12px; display: inline-block; }
        h3 { font-size: 1.5rem; color: var(--navy); }
       .hero { text-align: center; background: linear-gradient(135deg, var(--navy) 0%, #1A3A5F 100%); color: white; padding: 80px 20px; }
       .hero h1 { color: white; margin-bottom: 20px; }
       .hero p { font-size: 1.2rem; max-width: 700px; margin: 0 auto 10px; opacity: 0.95; }
       .tagline { color: var(--gold); font-style: italic; font-size: 1.3rem; margin: 20px 0; letter-spacing: 1px; }
       .btn { display: inline-block; background: var(--gold); color: var(--navy); padding: 14px 30px; margin: 10px 8px 0; text-decoration: none; border-radius: 30px; font-weight: 700; border: none; cursor: pointer; transition: 0.3s; }
       .btn:hover { background: #B8965A; transform: translateY(-2px); }
       .btn-dark { background: var(--navy); color: white; }
       .btn-dark:hover { background: #071A30; }
       .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 25px; margin-top: 25px; }
       .card { border: 1px solid #E5E8EC; padding: 25px; border-radius: 12px; transition: 0.3s; background: white; }
       .card:hover { transform: translateY(-5px); box-shadow: 0 8px 25px rgba(10,34,64,0.15); border-color: var(--gold); }
       .card-icon { font-size: 2.5rem; margin-bottom: 15px; }
       .price { color: #C0392B; font-weight: 800; font-size: 1.4rem; margin: 12px 0; }
       .tag { display: inline-block; background: var(--light-gold); color: var(--navy); padding: 6px 14px; margin: 5px 5px 5px 0; border-radius: 20px; font-size: 0.85rem; font-weight: 600; }
       .two-col { display: grid; grid-template-columns: 1fr 1fr; gap: 40px; align-items: start; }
       .highlight-box { background: var(--light-gold); border-left: 4px solid var(--gold); padding: 25px; border-radius: 8px; margin: 20px 0; }
       .budget-table, .comparison-table { width: 100%; border-collapse: collapse; margin-top: 20px; font-size: 0.95rem; }
       .budget-table th, .budget-table td, .comparison-table th, .comparison-table td { border: 1px solid #E5E8EC; padding: 14px; text-align: left; }
       .budget-table th, .comparison-table th { background: var(--navy); color: white; }
       .comparison-table .check { color: #27AE60; font-weight: bold; }
       .comparison-table .cross { color: #C0392B; }
        footer { background: var(--navy); color: white; padding: 40px 20px 20px; margin-top: 40px; }
        .footer-grid { max-width: 1200px; margin: auto; display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px; margin-bottom: 30px; }
        footer h4 { color: var(--gold); margin-bottom: 15px; }
        footer a { color: #BDC3C7; text-decoration: none; display: block; margin: 8px 0; }
        footer a:hover { color: var(--gold); }
        .footer-bottom { text-align: center; padding-top: 20px; border-top: 1px solid #2C3E50; color: #95A5A6; font-size: 0.9rem; }

        /* Payment Logos */
       .payment-logos { display: flex; flex-wrap: wrap; gap: 15px; margin: 25px 0; }
       .payment-logo { width: 90px; height: 55px; border: 1px solid #ddd; border-radius: 8px; display: flex; align-items: center; justify-content: center; font-weight: bold; font-size: 0.8rem; }
       .mtn { background: #FFC600; color: #000; }
       .telecel { background: #E60000; color: white; }
       .at { background: #0099D8; color: white; }
       .visa { background: #1A1F71; color: white; }

        /* Forms */
       .form-group { margin-bottom: 18px; }
       .form-group label { display: block; margin-bottom: 6px; font-weight: 600; color: var(--navy); }
       .form-group input,.form-group select,.form-group textarea {
            width: 100%; padding: 12px; border: 1px solid #D5DB; border-radius: 6px; font-size: 1rem; transition: 0.3s;
        }
       .form-group input:focus,.form-group textarea:focus { border-color: var(--gold); outline: none; }
       .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; }
       .form-box { background: var(--light-gold); padding: 30px; border-radius: 12px; margin-top: 25px; }
       .success-msg { display: none; background: #27AE60; color: white; padding: 15px; border-radius: 6px; margin-top: 15px; text-align: center; font-weight: 600; }
       .cart-item { display: flex; justify-content: space-between; padding: 12px 0; border-bottom: 1px dashed #D5DBDB; }

        /* Tracker */
       .tracker { display: none; margin-top: 25px; }
       .track-steps { display: flex; justify-content: space-between; margin: 35px 0; position: relative; }
       .track-steps::before { content: ''; position: absolute; top: 20px; left: 0; right: 0; height: 4px; background: #E5E8EC; z-index: 1; }
       .track-progress { position: absolute; top: 20px; left: 0; height: 4px; background: var(--gold); z-index: 2; width: 0%; transition: 1s; }
       .step { text-align: center; z-index: 3; position: relative; width: 25%; }
       .step-circle { width: 42px; height: 42px; border-radius: 50%; background: #E5E8EC; margin: 0 auto 10px; display: flex; align-items: center; justify-content: center; color: var(--grey); font-weight: bold; border: 3px solid white; }
       .step.active .step-circle { background: var(--gold); color: var(--navy); }
       .step p { font-size: 0.9rem; font-weight: 600; }
       .order-details { background: white; border: 1px solid #E5E8EC; padding: 25px; border-radius: 8px; margin-top: 25px; }

        @media (max-width: 768px) {
            .two-col, .form-row { grid-template-columns: 1fr; }
            nav ul { gap: 15px; font-size: 0.9rem; }
            h1 { font-size: 2rem; }
            h2 { font-size: 1.7rem; }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">
                <img src="apex-logo.png" alt="Apex Gift Solution Logo">
                <div class="logo-text">
                    APEX
                    <span>GIFT SOLUTION</span>
                </div>
            </div>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#solutions">Solutions</a></li>
                <li><a href="#corporate">Corporate</a></li>
                <li><a href="#track">Track Order</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="container">
            <h1>Apex Gift Solution</h1>
            <p class="tagline">“Elevating Every Gesture”</p>
            <p>We firmly believe that truly powerful gifts do more than merely occupy a space—they elegantly forge meaningful connections.</p>
            <p><strong>Premier online gifting studio for emotional & professional solutions</strong></p>
            <a href="#solutions" class="btn">Explore Solutions</a>
            <a href="#corporate" class="btn btn-dark">Corporate Gifting</a>
        </div>
    </section>

    <div class="container">
        <section id="about">
            <h2>Why Apex Gift Solution?</h2>
            <div class="two-col">
                <div>
                    <p><strong>Gifting is more than a transaction; it’s a language.</strong> Apex is built on the idea that finding the "perfect" gift requires understanding the heart of the occasion.</p>
                    <div class="highlight-box">
                        <h3>Our Value Proposition</h3>
                        <p><strong>"More than just a gift—we help you say what words can’t."</strong></p>
                        <p>We reduce customer anxiety about picking the "wrong" thing. We provide emotional intelligence needed to mend a bridge or celebrate a bond.</p>
                    </div>
                </div>
                <div>
                    <h3>What Sets Us Apart</h3>
                    <div class="card">
                        <h4>1. Expert Consultation</h4>
                        <p>Personalized guidance for sensitive moments. Not sure what to say in an apology? We help you craft the message + match it with a gesture that shows you care.</p>
                    </div>
                    <div class="card">
                        <h4>2. Bespoke Curation</h4>
                        <p>Every card and gift is customized to reflect the unique personality of the recipient and depth of your relationship.</p>
                    </div>
                    <div class="card">
                        <h4>3. Professionalism & Heart</h4>
                        <p>We serve individuals seeking a "fresh start" to businesses strengthening corporate culture through meaningful appreciation.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="solutions">
            <h2>Our E-Commerce Model: Product + Service Bundle</h2>
            <p>Instead of just selling a card for GHS 50, we sell <strong>"The Apology Package" or "The Birthday Solution"</strong></p>
            
            <div class="grid">
                <div class="card">
                    <div class="card-icon">💔</div>
                    <h3>The Apology Package</h3>
                    <p>Includes: 15-min consultation + custom card + curated gift + written apology script</p>
                    <div class="price">GHS 250 - GHS 400</div>
                    <p><strong>Revenue Benefit:</strong> We sell "peace of mind" and "expert advice," not just paper and ink.</p>
                    <button class="btn" onclick="addToCart('Apology Package', 300)">Start Consultation</button>
                </div>
                <div class="card">
                    <div class="card-icon">🎂</div>
                    <h3>Birthday Solution Box</h3>
                    <p>Guided discovery form + personalized gift + same-day delivery in Accra</p>
                    <div class="price">GHS 150 - GHS 500</div>
                    <p><strong>Why it works:</strong> Captures last-minute buyers. Order by 12pm for same-day delivery.</p>
                    <button class="btn" onclick="addToCart('Birthday Solution Box', 200)">Build Box</button>
                </div>
                <div class="card">
                    <div class="card-icon">🏆</div>
                    <h3>Corporate Milestone</h3>
                    <p>Automated employee birthdays & anniversaries + branded packaging</p>
                    <div class="price">From GHS 200/mo</div>
                    <p><strong>Revenue Benefit:</strong> Creates recurring revenue. We handle it, HR doesn't lift a finger.</p>
                    <button class="btn" onclick="document.getElementById('corporate').scrollIntoView()">Learn More</button>
                </div>
            </div>
        </section>

        <section id="corporate">
            <h2>Corporate "Gifts-as-a-Service" (B2B)</h2>
            <div class="two-col">
                <div>
                    <h3>Subscription / Retainer Model</h3>
                    <p>Companies pay us a monthly fee or bulk deposit. We track employee birthdays and work anniversaries and automatically send custom cards and gifts on their behalf.</p>
                    <div class="highlight-box">
                        <h4>Employee Milestone Tracking</h4>
                        <p>Corporate clients set up automated triggers so the platform proactively suggests gifts throughout the year.</p>
                        <h4>Budget & Approval Workflows</h4>
                        <p>Larger companies manage gifting spend through a dedicated login, ensuring all gifts align with policy.</p>
                    </div>
                <div>
                    <h3>Regional E-tailer Advantage</h3>
                    <p><strong>Logistics Advantage:</strong> Same-Day or Next-Day delivery — massive selling point for urgent apologies.</p>
                    <p><strong>Local Trust:</strong> We use regional language, cultural nuances in apology consultations, and partner with local florists/bakeries.</p>
                    <p><strong>Lower Shipping Costs:</strong> Staying regional keeps overhead down and makes solutions more affordable.</p>
                    <button class="btn btn-dark">Book Corporate Demo</button>
                </div>
            </div>
        </section>

        <section id="cart">
            <h2>Checkout: Build Your Solution</h2>
            <div class="form-box">
                <h3>Your Cart</h3>
                <div id="cartItems">
                    <p id="emptyCart">Your cart is empty. Select a solution above.</p>
                </div>
                <hr style="margin: 15px 0; border: none; border-top: 1px solid #D5DBDB;">
                <div class="cart-item">
                    <strong>Subtotal:</strong>
                    <strong id="subtotal">GHS 0</strong>
                </div>
                <div class="cart-item">
                    <span>Apex Flash Delivery (2-4hrs, Accra):</span>
                    <span>GHS 30</span>
                </div>
                <div class="cart-item">
                    <strong>Total:</strong>
                    <strong id="total">GHS 30</strong>
                </div>

                <h3 style="margin-top: 25px;">Recipient Details</h3>
                <div class="form-row">
                    <div class="form-group">
                        <label for="name">Your Name</label>
                        <input type="text" id="name" placeholder="Nora Mensah" required>
                    </div>
                    <div class="form-group">
                        <label for="phone">Your Phone</label>
                        <input type="tel" id="phone" placeholder="024 XXX XXXX" required>
                    </div>
                </div>
                <div class="form-group">
                    <label for="recipient">Recipient Name & Address</label>
                    <input type="text" id="recipient" placeholder="Kofi Annan, East Legon, Accra" required>
                </div>
                <div class="form-group">
                    <label for="occasion">Occasion & Tone Needed</label>
                    <select id="occasion">
                        <option>Apology - Sincere & Humble</option>
                        <option>Apology - Professional</option>
                        <option>Birthday - Joyful</option>
                        <option>Corporate - Appreciation</option>
                        <option>Corporate - Milestone</option>
                    </select>
                </div>

                <button type="button" class="btn" onclick="proceedToPay()">Proceed to Payment</button>
                <div class="success-msg" id="successMsg">Order #AGS2026 confirmed! Proceed to payment below.</div>
            </div>
        </section>

        <section id="payment">
            <h2>Payment Model: Mobile Money First</h2>
            <p>Over 80% of online transactions in our region use mobile wallets. We support all major providers for instant, secure payment.</p>

            <h3>Select Payment Method:</h3>
            <div class="payment-logos">
                <div class="payment-logo mtn">MTN<br>MoMo</div>
                <div class="payment-logo telecel">Telecel<br>Cash</div>
                <div class="payment-logo at">AT<br>Money</div>
                <div class="payment-logo visa">VISA</div>
                <div class="payment-logo" style="background:#0073CF;color:white;">Master<br>card</div>
                <div class="payment-logo" style="background:#f5f5f5;">Bank<br>Transfer</div>
            </div>

            <div class="card">
                <h3>Pay with Mobile Money</h3>
                <div class="form-group">
                    <label for="momo-number">Enter Mobile Money Number</label>
                    <input type="tel" id="momo-number" placeholder="024 XXX XXXX">
                </div>
                <div class="form-group">
                    <label for="network">Select Network</label>
                    <select id="network">
                        <option>MTN Mobile Money</option>
                        <option>Telecel Cash</option>
                        <option>AT Money</option>
                    </select>
                </div>
                <button class="btn" onclick="alert('Demo: In live site, you would get a MoMo prompt on your phone to approve payment via Paystack/Hubtel.')">Pay Now</button>
                <p style="margin-top:12px; font-size:0.9rem;"><em>For B2B: Bank transfer & monthly invoicing available for verified corporate partners.</em></p>
            </div>
        </section>

        <section id="track">
            <h2>Track Your Order: End-to-End Visibility</h2>
            <p>Enter your order number to see live delivery updates. For demo, use: <strong>AGS2026</strong></p>
            
            <div class="form-box">
                <div class="form-group">
                    <label for="orderNumber">Order Number</label>
                    <input type="text" id="orderNumber" placeholder="e.g. AGS2026">
                </div>
                <button class="btn" onclick="trackOrder()">Track Order</button>
                
                <div class="tracker" id="tracker">
                    <div class="order-details">
                        <h3>Order #AGS2026 - The Apology Package</h3>
                        <p><strong>Status:</strong> <span id="trackStatus">Order Confirmed - Sentiment Specialist reviewing tone</span></p>
                        <p><strong>Recipient:</strong> <span id="trackRecipient">East Legon, Accra</span></p>
                        <p><strong>Delivery Type:</strong> Apex Flash (2-4 Hours)</p>
                    </div>

                    <div class="track-steps">
                        <div class="track-progress" id="trackProgress"></div>
                        <div class="step active" id="step1">
                            <div class="step-circle">1</div>
                            <p>Consultation<br>Complete</p>
                        </div>
                        <div class="step" id="step2">
                            <div class="step-circle">2</div>
                            <p>Apex-Wrapped<br>Packaging</p>
                        </div>
                        <div class="step" id="step3">
                            <div class="step-circle">3</div>
                            <p>Out for<br>Delivery</p>
                        </div>
                        <div class="step" id="step4">
                            <div class="step-circle">4</div>
                            <p>Proof of<br>Sentiment</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="competitive">
            <h2>Competitive Advantage: Pure Play Regional E-tailer</h2>
            <table class="comparison-table">
                <tr>
                    <th>Feature</th>
                    <th>Mass Retailers</th>
                    <th>Social Vendors</th>
                    <th>Apex Gift Solution</th>
                </tr>
                <tr>
                    <td>Customization</td>
                    <td class="cross">Very Low</td>
                    <td class="check">High</td>
                    <td class="check">Bespoke (High End)</td>
                </tr>
                <tr>
                    <td>Emotional Advice</td>
                    <td class="cross">None</td>
                    <td class="cross">Informal</td>
                    <td class="check">Professional Consultation</td>
                </tr>
                <tr>
                    <td>Corporate Focus</td>
                    <td class="cross">Bulk Only</td>
                    <td class="cross">Inconsistent</td>
                    <td class="check">Automated B2B Solutions</td>
                </tr>
                <tr>
                    <td>Delivery Speed</td>
                    <td>Standard</td>
                    <td class="cross">Variable</td>
                    <td class="check">Guaranteed Apex Flash 2-4hrs</td>
                </tr>
                <tr>
                    <td>Cost Structure</td>
                    <td>High Retail Rent</td>
                    <td>Low but No Scale</td>
                    <td class="check">Pure Play - Low Overhead</td>
                </tr>
            </table>
            <div class="highlight-box">
                <h4>Our "Moat": The Apex Apology Framework</h4>
                <p>Proprietary consultation method + copyrighted message scripts that customers can only get from us. We don't compete on price — we compete on "peace of mind" worth GHS 1,000+.</p>
            </div>
        </section>

    </div>

    <footer id="contact">
        <div class="footer-grid">
            <div>
                <h4>Apex Gift Solution</h4>
                <p>“Elevating Every Gesture”</p>
                <p>Premier online gifting studio for emotional & professional solutions in Accra, Ghana.</p>
            </div>
            <div>
                <h4>Solutions</h4>
                <a href="#solutions">Apology Package</a>
                <a href="#solutions">Birthday Solution</a>
                <a href="#corporate">Corporate Gifting</a>
                <a href="#track">Track Order</a>
            </div>
            <div>
                <h4>Company</h4>
                <a href="#">About Us</a>
                <a href="#">Our Mission</a>
                <a href="#">Become a Partner</a>
                <a href="#">Careers</a>
            </div>
            <div>
                <h4>Contact</h4>
                <p>📍 Accra, Ghana</p>
                <p>📞 055-123-4567</p>
                <p>📧 hello@apexgift.com</p>
                <p>💬 WhatsApp: Click to Chat</p>
            </div>
        <div class="footer-bottom">
            <p><strong>Nora Gift Project Portfolio</strong> | Budget: GHS 50,000 | Team: 9 Members | 2026</p>
            <p>This is a conceptual demo. Apex delivers results—mended bonds, joyous celebrations, and lasting professional respect.</p>
        </div>
    </footer>

    <script>
        let cart = [];
        let deliveryFee = 30;
        let currentOrder = null;

        function addToCart(name, price) {
            cart.push({ name: name, price: price });
            updateCart();
            document.getElementById('cart').scrollIntoView({ behavior: 'smooth' });
        }

        function updateCart() {
            const cartItemsDiv = document.getElementById('cartItems');
            const emptyCart = document.getElementById('emptyCart');
            
            if (cart.length === 0) {
                emptyCart.style.display = 'block';
                cartItemsDiv.innerHTML = '<p id="emptyCart">Your cart is empty. Select a solution above.</p>';
            } else {
                emptyCart.style.display = 'none';
                let itemsHTML = '';
                let subtotal = 0;
                cart.forEach(item => {
                    itemsHTML += `<div class="cart-item"><span>${item.name}</span><span>GHS ${item.price}</span></div>`;
                    subtotal += item.price;
                });
                cartItemsDiv.innerHTML = itemsHTML;
                document.getElementById('subtotal').innerText = `GHS ${subtotal}`;
                document.getElementById('total').innerText = `GHS ${subtotal + deliveryFee}`;
            }
        }

        function proceedToPay() {
            if (cart.length === 0) {
                alert('Your cart is empty. Please select a solution first!');
                return;
            }
            if (document.getElementById('name').value === '' || document.getElementById('phone').value === '') {
                alert('Please fill in your name and phone number.');
                return;
            }
            currentOrder = {
                id: 'AGS2026',
                items: cart.map(i => i.name).join(', '),
                total: cart.reduce((sum, i) => sum + i.price, 0) + deliveryFee,
                recipient: document.getElementById('recipient').value
            };
            document.getElementById('successMsg').style.display = 'block';
            setTimeout(() => {
                document.getElementById('payment').scrollIntoView({ behavior: 'smooth' });
            }, 1000);
        }

        function trackOrder() {
            const orderNum = document.getElementById('orderNumber').value.trim();
            if (orderNum === 'AGS2026') {
                document.getElementById('tracker').style.display = 'block';
                document.getElementById('trackRecipient').innerText = currentOrder ? currentOrder.recipient : 'East Legon, Accra';
                
                let step = 1;
                const statuses = [
                    'Consultation Complete - Sentiment Specialist approved tone',
                    'Apex-Wrapped Packaging - Premium magnetic box + handwritten note',
                    'Out for Delivery - Apex Flash rider dispatched. ETA 1 hour',
                    'Proof of Sentiment - Photo confirmation sent to your WhatsApp'
                ];
                
                const interval = setInterval(() => {
                    step++;
                    document.getElementById('trackProgress').style.width = ((step - 1) * 33.33) + '%';
                    document.getElementById('step' + step).classList.add('active');
                    document.getElementById('trackStatus').innerText = statuses[step-1];
                    if (step === 4) clearInterval(interval);
                }, 1800);
            } else {
                alert('Order not found. For demo, use AGS2026');
            }
        }
    </script>
</body>
</html>
