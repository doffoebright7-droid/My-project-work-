<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apex Gift Solution – Elevating Every Gesture</title>
    <link rel="icon" type="image/png" href="apex-logo.png">
    <style>
        :root {
            --navy: #0A2240;
            --gold: #C9A961;
            --light-gold: #FDF8F0;
            --white: #FFFFFF;
            --grey: #5D6D7E;
            --light-bg: #FFFEF7;
            --success: #27AE60;
            --danger: #C0392B;
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Arial, sans-serif; }
        body { background: var(--light-bg); color: #333; line-height: 1.7; }
        header { background: var(--navy); color: white; padding: 1rem 0; position: sticky; top: 0; z-index: 100; box-shadow: 0 2px 10px rgba(10,34,64,0.2); }
        nav { max-width: 1200px; margin: auto; display: flex; justify-content: space-between; align-items: center; padding: 0 20px; }
        .logo { display: flex; align-items: center; gap: 12px; }
        .logo img { height: 55px; width: auto; }
        .logo-text { font-size: 1.4rem; font-weight: 700; line-height: 1.1; }
        .logo-text span { display: block; font-size: 0.7rem; color: var(--gold); font-weight: 400; letter-spacing: 1.5px; }
        nav ul { display: flex; list-style: none; gap: 25px; flex-wrap: wrap; }
        nav a { color: white; text-decoration: none; font-weight: 600; transition: 0.3s; }
        nav a:hover { color: var(--gold); }
       .container { max-width: 1200px; margin: auto; padding: 50px 20px; }
        section { background: white; margin-bottom: 35px; padding: 40px; border-radius: 12px; box-shadow: 0 2px 15px rgba(201,169,97,0.15); border: 1px solid var(--light-gold); }
        h1, h2, h3, h4 { color: var(--navy); margin-bottom: 15px; }
        h1 { font-size: 2.8rem; line-height: 1.2; }
        h2 { font-size: 2.2rem; border-bottom: 3px solid var(--gold); padding-bottom: 12px; display: inline-block; }
        h3 { font-size: 1.5rem; color: var(--navy); }
       .hero { text-align: center; background: linear-gradient(135deg, var(--gold) 0%, #E6D4A8 100%); color: var(--navy); padding: 80px 20px; }
       .hero-logo { height: 120px; margin-bottom: 20px; }
       .hero h1 { color: var(--navy); margin-bottom: 15px; }
       .hero p { font-size: 1.2rem; max-width: 700px; margin: 0 auto 10px; color: var(--navy); opacity: 0.9; }
       .tagline { color: var(--navy); font-style: italic; font-size: 1.3rem; margin: 20px 0; letter-spacing: 1px; font-weight: 600; }
       .btn { display: inline-block; background: var(--navy); color: white; padding: 14px 30px; margin: 10px 8px 0; text-decoration: none; border-radius: 30px; font-weight: 700; border: none; cursor: pointer; transition: 0.3s; }
       .btn:hover { background: #071A30; transform: translateY(-2px); }
       .btn-dark { background: var(--gold); color: var(--navy); }
       .btn-dark:hover { background: #B8965A; }
       .btn-outline { background: transparent; color: var(--navy); border: 2px solid var(--navy); }
       .btn-outline:hover { background: var(--navy); color: white; }
       .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 25px; margin-top: 25px; }
       .card { border: 2px solid var(--light-gold); padding: 0; border-radius: 12px; transition: 0.3s; background: white; overflow: hidden; }
       .card:hover { transform: translateY(-5px); box-shadow: 0 8px 25px rgba(201,169,97,0.25); border-color: var(--gold); }
       .card img { width: 100%; height: 220px; object-fit: cover; }
       .card-content { padding: 25px; }
       .price { color: var(--danger); font-weight: 800; font-size: 1.4rem; margin: 12px 0; }
       .tag { display: inline-block; background: var(--light-gold); color: var(--navy); padding: 6px 14px; margin: 5px 0; border-radius: 20px; font-size: 0.85rem; font-weight: 600; }
       .two-col { display: grid; grid-template-columns: 1fr 1fr; gap: 40px; align-items: start; }
       .highlight-box { background: var(--light-gold); border-left: 4px solid var(--gold); padding: 25px; border-radius: 8px; margin: 20px 0; }
       .gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; margin-top: 25px; }
       .gallery img { width: 100%; height: 250px; object-fit: cover; border-radius: 12px; transition: 0.3s; border: 2px solid var(--light-gold); }
       .gallery img:hover { transform: scale(1.03); box-shadow: 0 8px 25px rgba(201,169,97,0.3); }
        footer { background: var(--navy); color: white; padding: 40px 20px 20px; margin-top: 40px; }
        .footer-grid { max-width: 1200px; margin: auto; display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px; margin-bottom: 30px; }
        .footer-logo { height: 70px; margin-bottom: 15px; filter: brightness(0) invert(1); }
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
       .success-msg { display: none; background: var(--success); color: white; padding: 15px; border-radius: 6px; margin-top: 15px; text-align: center; font-weight: 600; }
       .error-msg { display: none; background: var(--danger); color: white; padding: 15px; border-radius: 6px; margin-top: 15px; text-align: center; font-weight: 600; }
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

        /* Calendar Styles */
       .calendar { background: white; border: 1px solid #E5E8EC; border-radius: 8px; padding: 20px; }
       .calendar-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 20px; }
       .calendar-grid { display: grid; grid-template-columns: repeat(7, 1fr); gap: 8px; text-align: center; }
       .calendar-day { padding: 10px 5px; border-radius: 6px; cursor: pointer; transition: 0.2s; }
       .calendar-day:hover { background: var(--light-gold); }
       .calendar-day.selected { background: var(--gold); color: var(--navy); font-weight: bold; }
       .calendar-day.disabled { color: #BDC3C7; cursor: not-allowed; }
       .calendar-day.header { font-weight: 700; color: var(--navy); cursor: default; }
       .time-slots { display: grid; grid-template-columns: repeat(auto-fit, minmax(100px, 1fr)); gap: 10px; margin-top: 20px; }
       .time-slot { padding: 10px; border: 1px solid #D5DBDB; border-radius: 6px; text-align: center; cursor: pointer; transition: 0.2s; }
       .time-slot:hover { border-color: var(--gold); }
       .time-slot.selected { background: var(--gold); color: var(--navy); border-color: var(--gold); font-weight: 700; }
       .time-slot.booked { background: #F8F9F9; color: #BDC3C7; cursor: not-allowed; text-decoration: line-through; }

        /* Modal Styles */
       .modal { display: none; position: fixed; z-index: 1000; left: 0; top: 0; width: 100%; height: 100%; background: rgba(10,34,64,0.7); overflow: auto; }
       .modal-content { background: white; margin: 3% auto; padding: 0; border-radius: 12px; width: 90%; max-width: 650px; animation: modalFade 0.3s; }
       @keyframes modalFade { from {opacity: 0; transform: translateY(-50px);} to {opacity: 1; transform: translateY(0);} }
       .modal-header { background: var(--navy); color: white; padding: 20px 25px; border-radius: 12px 12px 0 0; display: flex; justify-content: space-between; align-items: center; }
       .modal-header h3 { color: white; margin: 0; }
       .modal-close { color: white; font-size: 28px; font-weight: bold; cursor: pointer; }
       .modal-body { padding: 25px; }
       .dashboard-stats { display: grid; grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); gap: 15px; margin: 20px 0; }
       .stat-card { background: var(--light-gold); padding: 20px; border-radius: 8px; text-align: center; }
       .stat-number { font-size: 2rem; font-weight: 800; color: var(--navy); }
       .stat-label { font-size: 0.9rem; color: var(--grey); }
       .employee-list { max-height: 200px; overflow-y: auto; border: 1px solid #E5E8EC; border-radius: 6px; margin-top: 15px; }
       .employee-row { display: flex; justify-content: space-between; padding: 12px 15px; border-bottom: 1px solid #E5E8EC; }
       .employee-row:last-child { border-bottom: none; }

        @media (max-width: 768px) {
            .two-col, .form-row { grid-template-columns: 1fr; }
            nav ul { gap: 15px; font-size: 0.9rem; }
            h1 { font-size: 2rem; }
            h2 { font-size: 1.7rem; }
            .logo-text { display: none; }
            .calendar-grid { gap: 4px; }
            .calendar-day { padding: 8px 2px; font-size: 0.9rem; }
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
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#solutions">Solutions</a></li>
                <li><a href="#booking">Book Consult</a></li>
                <li><a href="#corporate">Corporate</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#" onclick="openCorporateLogin()">Portal Login</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="container">
            <img src="apex-logo.png" alt="Apex Gift Solution" class="hero-logo">
            <h1>Apex Gift Solution</h1>
            <p class="tagline">“Elevating Every Gesture”</p>
            <p>We firmly believe that truly powerful gifts do more than merely occupy a space—they elegantly forge meaningful connections.</p>
            <p><strong>Premier online gifting studio for emotional & professional solutions</strong></p>
            <a href="#solutions" class="btn">Explore Solutions</a>
            <a href="#booking" class="btn btn-dark">Book Consultation</a>
        </div>
    </section>

    <div class="container">
        <section id="gallery">
            <h2>Our Work: Real Apex Solutions</h2>
            <p>From corporate milestones to heartfelt apologies — we don’t just deliver packages; we deliver results.</p>
            <div class="gallery">
                <img src="corp-gifts-1.jpg" alt="Corporate celebration with balloons and gift boxes">
                <img src="corp-gifts-2.jpg" alt="Executive team with premium corporate gifts">
                <img src="birthday-hamper.jpg" alt="Personalized birthday hamper for Clara">
                <img src="apology-chocolate.jpg" alt="I'm Sorry chocolate gift box">
                <img src="apology-balloon.jpg" alt="I'm Sorry Babe balloon bouquet">
                <img src="love-bouquet.jpg" alt="Teddy bear and roses love bouquet">
            </div>
        </section>

        <section id="solutions">
            <h2>Product + Service Bundle</h2>
            <p>Instead of just selling a card for GHS 50, we sell <strong>"The Apology Package" or "The Birthday Solution"</strong></p>
            
            <div class="grid">
                <div class="card">
                    <img src="apology-chocolate.jpg" alt="Apology Package">
                    <div class="card-content">
                        <h3>The Apology Package</h3>
                        <p>Includes: 15-min consultation + custom card + curated gift + written apology script</p>
                        <div class="price">GHS 250 - GHS 400</div>
                        <p><strong>Revenue Benefit:</strong> We sell "peace of mind" and "expert advice," not just paper and ink.</p>
                        <button class="btn" onclick="addToCart('Apology Package', 300)">Start Consultation</button>
                    </div>
                </div>
                <div class="card">
                    <img src="birthday-hamper.jpg" alt="Birthday Solution">
                    <div class="card-content">
                        <h3>Birthday Solution Box</h3>
                        <p>Guided discovery form + personalized gift + same-day delivery in Accra</p>
                        <div class="price">GHS 150 - GHS 500</div>
                        <p><strong>Why it works:</strong> Captures last-minute buyers. Order by 12pm for same-day delivery.</p>
                        <button class="btn" onclick="addToCart('Birthday Solution Box', 200)">Build Box</button>
                    </div>
                </div>
                <div class="card">
                    <img src="corp-gifts-2.jpg" alt="Corporate Milestone">
                    <div class="card-content">
                        <h3>Corporate Milestone</h3>
                        <p>Automated employee birthdays & anniversaries + branded packaging</p>
                        <div class="price">From GHS 200/mo</div>
                        <p><strong>Revenue Benefit:</strong> Creates recurring revenue. We handle it, HR doesn't lift a finger.</p>
                        <button class="btn" onclick="document.getElementById('corporate').scrollIntoView()">Learn More</button>
                    </div>
                </div>
            </div>
        </section>

        <section id="booking">
            <h2>Book Your Consultation</h2>
            <p>For apologies, corporate strategies, or high-stakes birthdays. Our Sentiment Specialists help you get the tone right.</p>
            
            <div class="form-box">
                <h3>1. Select Service Type</h3>
                <div class="form-row">
                    <div class="form-group">
                        <label for="consultType">Consultation Type</label>
                        <select id="consultType" onchange="updateConsultPrice()">
                            <option value="150">Apology Concierge - GHS 150 (15 min)</option>
                            <option value="300">Premium Apology - GHS 300 (30 min)</option>
                            <option value="500">Corporate Strategy - GHS 500 (45 min)</option>
                            <option value="0">Free Guide - GHS 0 (Automated)</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="consultName">Your Name</label>
                        <input type="text" id="consultName" placeholder="Nora Mensah" required>
                    </div>
                </div>

                <h3 style="margin-top: 25px;">2. Pick a Date & Time</h3>
                <div class="calendar">
                    <div class="calendar-header">
                        <button class="btn btn-outline" onclick="changeMonth(-1)" style="padding: 8px 15px;">← Prev</button>
                        <h4 id="monthYear">April 2026</h4>
                        <button class="btn btn-outline" onclick="changeMonth(1)" style="padding: 8px 15px;">Next →</button>
                    </div>
                    <div class="calendar-grid" id="calendarGrid"></div>
                    <div id="timeSlots" style="display: none;">
                        <h4 style="margin: 20px 0 10px;">Available Times for <span id="selectedDateText"></span></h4>
                        <div class="time-slots">
                            <div class="time-slot" onclick="selectTime(this)">09:00 AM</div>
                            <div class="time-slot" onclick="selectTime(this)">10:30 AM</div>
                            <div class="time-slot" onclick="selectTime(this)">02:00 PM</div>
                            <div class="time-slot booked">03:30 PM</div>
                            <div class="time-slot" onclick="selectTime(this)">05:00 PM</div>
                        </div>
                    </div>
                </div>

                <div class="form-group" style="margin-top: 25px;">
                    <label for="consultNotes">Brief: What’s the occasion? (Optional)</label>
                    <textarea id="consultNotes" rows="3" placeholder="e.g. Need to apologize to my boss for missing deadline..."></textarea>
                </div>

                <button class="btn" onclick="bookConsultation()">Confirm Booking - GHS <span id="consultPrice">150</span></button>
                <div class="success-msg" id="bookingSuccess">Booking confirmed! Check your email for Zoom link. Our specialist will call you 5 mins before.</div>
            </div>
        </section>

        <section id="corporate">
            <h2>Corporate "Gifts-as-a-Service" (B2B)</h2>
            <div class="two-col">
                <div>
                    <img src="corp-gifts-1.jpg" alt="Corporate gifting" style="width: 100%; border-radius: 12px; margin-bottom: 20px;">
                    <h3>Subscription / Retainer Model</h3>
                    <p>Companies pay us a monthly fee or bulk deposit. We track employee birthdays and work anniversaries and automatically send custom cards and gifts on their behalf.</p>
                    <div class="highlight-box">
                        <h4>Employee Milestone Tracking</h4>
                        <p>Corporate clients set up automated triggers so the platform proactively suggests gifts throughout the year.</p>
                        <h4>Budget & Approval Workflows</h4>
                        <p>Larger companies manage gifting spend through a dedicated login, ensuring all gifts align with policy.</p>
                    </div>
                    <button class="btn btn-dark" onclick="openCorporateLogin()">Corporate Portal Login</button>
                    <button class="btn btn-outline" onclick="alert('Demo: Our corporate team will contact you within 2 hours to set up your dashboard.')">Request Demo</button>
                </div>
                <div>
                    <img src="corp-gifts-2.jpg" alt="Executive gifts" style="width: 100%; border-radius: 12px; margin-bottom: 20px;">
                    <h3>Regional E-tailer Advantage</h3>
                    <p><strong>Logistics Advantage:</strong> Same-Day or Next-Day delivery — massive selling point for urgent apologies.</p>
                    <p><strong>Local Trust:</strong> We use regional language, cultural nuances in apology consultations, and partner with local florists/bakeries.</p>
                    <p><strong>Lower Shipping Costs:</strong> Staying regional keeps overhead down and makes solutions more affordable.</p>
                    <div class="card" style="margin-top: 20px;">
                        <h4>B2B Payment Options</h4>
                        <p>✓ Bank Transfer for large sums</p>
                        <p>✓ Monthly Invoicing (Retainer)</p>
                        <p>✓ Dedicated Account Manager</p>
                        <p>✓ White-Label Delivery</p>
                    </div>
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
                        <input type="tel" id="phone" placeholder="024 XXXX" required>
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
            <p>Over 80% of online transactions in our region use mobile wallets. We support all major providers for instant, secure payment via Paystack/Hubtel.</p>

            <h3>Select Payment Method:</h3>
            <div class="payment-logos">
                <div class="payment-logo mtn">MTN<br>MoMo</div>
                <div class="payment-logo telecel">Telecel<br>Cash</div>
                <div class="payment-logo at">AT<br>Money</div>
                <div class="payment-logo visa">VISA</div>
                <div class="payment-logo" style="background:#0073CF;color:white;">Master<br>card</div>
                <div class="payment-logo" style="background:#f5f5;">Bank<br>Transfer</div>
            </div>

            <div class="card">
                <h3>Pay with Mobile Money</h3>
                <div class="form-group">
                    <label for="momo-number">Enter Mobile Money Number</label>
                    <input type="tel" id="momo-number" placeholder="024 XXXX">
                </div>
                <div class="form-group">
                    <label for="network">Select Network</label>
                    <select id="network">
                        <option>MTN Mobile Money</option>
                        <option>Telecel Cash</option>
                        <option>AT Money</option>
                    </select>
                </div>
                <button class="btn" onclick="alert('Demo: In live site, you would get a MoMo prompt on your phone to approve payment.')">Pay Now</button>
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
    </div>

    <!-- Corporate Portal Modal -->
    <div id="corporateModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3>🏢 Corporate Portal Login</h3>
                <span class="modal-close" onclick="closeCorporateLogin()">&times;</span>
            </div>
            <div class="modal-body">
                <p><strong>Gifts-as-a-Service Dashboard</strong> for HR Managers & Admins</p>
                <div class="form-group">
                    <label for="corpEmail">Company Email</label>
                    <input type="email" id="corpEmail" placeholder="hr@company.com.gh">
                </div>
                <div class="form-group">
                    <label for="corpPass">Password</label>
                    <input type="password" id="corpPass" placeholder="••••">
                </div>
                <button class="btn" onclick="loginCorporate()">Login to Dashboard</button>
                <div class="error-msg" id="loginError">Invalid credentials. For demo, use: demo@apexgift.com / password123</div>
                
                <div id="corporateDashboard" style="display: none; margin-top: 25px;">
                    <h4>Welcome, CalBank HR Team</h4>
                    <div class="dashboard-stats">
                        <div class="stat-card">
                            <div class="stat-number">47</div>
                            <div class="stat-label">Employees Tracked</div>
                        </div>
                        <div class="stat-card">
                            <div class="stat-number">12</div>
                            <div class="stat-label">Gifts This Month</div>
                        </div>
                        <div class="stat-card">
                            <div class="stat-number">GHS 2,400</div>
                            <div class="stat-label">Monthly Spend</div>
                        </div>
                    </div>
                    <h4>Upcoming Milestones - Next 30 Days</h4>
                    <div class="employee-list">
                        <div class="employee-row">
                            <span><strong>May 2:</strong> Ama Boateng - Birthday</span>
                            <span class="tag">Auto-Scheduled</span>
                        </div>
                        <div class="employee-row">
                            <span><strong>May 15:</strong> Kofi Mensah - 5yr Anniversary</span>
                            <span class="tag">Auto-Scheduled</span>
                        </div>
                        <div class="employee-row">
                            <span><strong>May 28:</strong> Yaw Osei - Promotion</span>
                            <span class="tag" style="background: #FADBD8; color: var(--danger);">Pending Approval</span>
                        </div>
                    </div>
                    <button class="btn btn-dark" style="margin-top: 20px;">Upload Employee CSV</button>
                    <button class="btn btn-outline">Download Invoice</button>
                </div>
            </div>
        </div>
    </div>

    <footer id="contact">
        <div class="footer-grid">
            <div>
                <img src="apex-logo.png" alt="Apex Gift Solution" class="footer-logo">
                <p><strong>“Elevating Every Gesture”</strong></p>
                <p>Premier online gifting studio for emotional & professional solutions in Accra, Ghana.</p>
            </div>
            <div>
                <h4>Solutions</h4>
                <a href="#booking">Apology Consultation</a>
                <a href="#solutions">Birthday Solution</a>
