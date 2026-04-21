# My-project-work-
School project 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FixNow Ghana - Project Portfolio</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }
        body { background: #f5f5f5; color: #444; line-height: 1.6; }
        header { background: #0A4D68; color: white; padding: 1rem 0; position: sticky; top: 0; z-index: 100; }
        nav { max-width: 1100px; margin: auto; display: flex; justify-content: space-between; align-items: center; padding: 0 20px; }
        nav ul { display: flex; list-style: none; gap: 20px; }
        nav a { color: white; text-decoration: none; font-weight: bold; }
        nav a:hover { color: #FFB100; }
       .container { max-width: 1100px; margin: auto; padding: 40px 20px; }
        section { background: white; margin-bottom: 30px; padding: 30px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
        h1, h2, h3 { color: #0A4D68; margin-bottom: 15px; }
        h1 { font-size: 2.5rem; }
        h2 { font-size: 2rem; border-bottom: 3px solid #FFB100; padding-bottom: 10px; }
       .hero { text-align: center; background: #088395; color: white; }
       .hero h1 { color: white; }
       .btn { display: inline-block; background: #FFB100; color: #0A4D68; padding: 12px 25px; margin-top: 15px; text-decoration: none; border-radius: 5px; font-weight: bold; border: none; cursor: pointer; }
       .btn:hover { background: #e09b00; }
       .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-top: 20px; }
       .card { border: 1px solid #ddd; padding: 20px; border-radius: 8px; }
       .card h3 { color: #088395; }
       .tag { display: inline-block; background: #E7F6F2; color: #0A4D68; padding: 5px 10px; margin: 5px 5px 5px 0; border-radius: 15px; font-size: 0.9rem; }
       .budget-table { width: 100%; border-collapse: collapse; margin-top: 15px; }
       .budget-table th,.budget-table td { border: 1px solid #ddd; padding: 12px; text-align: left; }
       .budget-table th { background: #0A4D68; color: white; }
        footer { background: #0A4D68; color: white; text-align: center; padding: 20px; margin-top: 30px; }

        /* Payment Page Styles */
       .payment-logos { display: flex; flex-wrap: wrap; gap: 15px; margin: 20px 0; }
       .payment-logo { width: 80px; height: 50px; border: 1px solid #ddd; border-radius: 8px; display: flex; align-items: center; justify-content: center; font-weight: bold; font-size: 0.8rem; }
       .mtn { background: #FFC600; color: #000; }
       .telecel { background: #E60000; color: white; }
       .at { background: #0099D8; color: white; }
       .visa { background: #1A1F71; color: white; }

        /* Booking Form Styles */
       .form-group { margin-bottom: 15px; }
       .form-group label { display: block; margin-bottom: 5px; font-weight: bold; color: #0A4D68; }
       .form-group input,.form-group select,.form-group textarea {
            width: 100%; padding: 10px; border: 1px solid #ddd; border-radius: 5px; font-size: 1rem;
        }
       .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; }
        #bookingForm { background: #E7F6F2; padding: 25px; border-radius: 8px; margin-top: 20px; }
       .success-msg { display: none; background: #4CAF50; color: white; padding: 15px; border-radius: 5px; margin-top: 15px; text-align: center; }
    </style>
</head>
<body>
    <header>
        <nav>
            <h3>FixNow Ghana</h3>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#pages">Pages</a></li>
                <li><a href="#demo">Demo</a></li>
                <li><a href="#payment">Payment</a></li>
                <li><a href="#budget">Budget</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="container">
            <h1>FixNow Ghana</h1>
            <p>E-Commerce Platform Connecting Ghanaians to Verified Technicians</p>
            <p><strong>Project Type:</strong> Startup Business Plan & Website Prototype</p>
            <a href="#demo" class="btn">Try Demo Booking</a>
        </div>
    </section>

    <div class="container">
        <section id="about">
            <h2>1. Project Overview</h2>
            <p><strong>Problem:</strong> Finding reliable plumbers, electricians, and carpenters in Ghana is difficult. Users face delays, price scams, and unverified workers.</p>
            <p><strong>Solution:</strong> FixNow Ghana is a mobile-first platform where users can search, book, and pay verified technicians online via Mobile Money.</p>
            <p><strong>Revenue Model:</strong> 10% commission per service + technician subscription fees.</p>
            <div>
                <span class="tag">E-Commerce</span>
                <span class="tag">Service Booking</span>
                <span class="tag">Mobile Money</span>
                <span class="tag">Ghana Tech</span>
            </div>
        </section>

        <section id="pages">
            <h2>2. Website Pages & Functions</h2>
            <div class="grid">
                <div class="card">
                    <h3>Home Page</h3>
                    <p>Welcome message, "How it works", featured technicians, and main search bar.</p>
                </div>
                <div class="card">
                    <h3>Services Page</h3>
                    <p>Search/filter technicians by type: plumbers, electricians, carpenters. Shows ratings, location.</p>
                </div>
                <div class="card">
                    <h3>Booking/Checkout Page</h3>
                    <p>User selects technician, picks date/time, and confirms job details.</p>
                </div>
                <div class="card">
                    <h3>Payment Page</h3>
                    <p>Secure payments via MTN MoMo, Telecel Cash, AT Money, Visa/Mastercard, Bank Transfer.</p>
                </div>
                <div class="card">
                    <h3>Customer Support</h3>
                    <p>FAQs, live chat widget, report an issue form, and contact hotline: 030-123-4567</p>
                </div>
                <div class="card">
                    <h3>User/Tech Dashboards</h3>
                    <p>Users track bookings. Technicians manage jobs, see earnings, set availability.</p>
                </div>
            </div>
        </section>

        <section id="demo">
            <h2>3. Demo: Booking/Checkout Page</h2>
            <p>This is how the actual booking form will work on FixNow Ghana:</p>

            <form id="bookingForm">
                <div class="form-row">
                    <div class="form-group">
                        <label for="service">Select Service</label>
                        <select id="service" required>
                            <option value="">-- Choose --</option>
                            <option value="plumber">Plumber - GHS 50+</option>
                            <option value="electrician">Electrician - GHS 60+</option>
                            <option value="carpenter">Carpenter - GHS 70+</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="technician">Choose Technician</label>
                        <select id="technician" required>
                            <option value="">-- Select --</option>
                            <option value="kofi">Kofi Mensah - 4.9★ - Accra</option>
                            <option value="ama">Ama Boateng - 4.8★ - Kumasi</option>
                            <option value="yaw">Yaw Osei - 4.7★ - Tema</option>
                        </select>
                    </div>
                </div>

                <div class="form-row">
                    <div class="form-group">
                        <label for="date">Date</label>
                        <input type="date" id="date" required>
                    </div>
                    <div class="form-group">
                        <label for="time">Time</label>
                        <input type="time" id="time" required>
                    </div>
                </div>

                <div class="form-group">
                    <label for="address">Your Address in Accra</label>
                    <input type="text" id="address" placeholder="e.g. East Legon, Hse No. 5" required>
                </div>

                <div class="form-group">
                    <label for="job">Describe the Job</label>
                    <textarea id="job" rows="3" placeholder="e.g. Kitchen sink is leaking" required></textarea>
                </div>

                <button type="submit" class="btn">Proceed to Payment - GHS 50</button>
                <div class="success-msg" id="successMsg">Booking confirmed! Redirecting to Payment Page...</div>
            </form>
        </section>

        <section id="payment">
            <h2>4. Payment Page</h2>
            <p><strong>Why Mobile Money first?</strong> Over 70% of Ghanaians prefer MoMo over bank cards. FixNow uses Paystack to accept all networks in one checkout.</p>

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
                <h3>Mobile Money Payment Demo</h3>
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
                <button class="btn">Pay GHS 50 Now</button>
                <p style="margin-top:10px; font-size:0.9rem;"><em>Note: For this demo, clicking won’t charge money. In real site, user gets MoMo prompt on phone.</em></p>
            </div>
        </section>

        <section id="budget">
            <h2>5. Project Budget: GHS 50,000</h2>
            <table class="budget-table">
                <tr>
                    <th>Item</th>
                    <th>Amount (GHS)</th>
                    <th>Notes</th>
                </tr>
                <tr>
                    <td>Platform Development</td>
                    <td>10,000</td>
                    <td>WordPress + Bookly Pro + Customization</td>
                </tr>
                <tr>
                    <td>Payment Integration</td>
                    <td>2,000</td>
                    <td>Paystack setup for MTN, Telecel, AT MoMo</td>
                </tr>
                <tr>
                    <td>Marketing</td>
                    <td>12,000</td>
                    <td>Social media ads, hostel posters</td>
                </tr>
                <tr>
                    <td>Technician Verification</td>
                    <td>5,500</td>
                    <td>ID checks, background checks</td>
                </tr>
                <tr>
                    <td>Operations/Staff</td>
                    <td>10,000</td>
                    <td>First 3 months</td>
                </tr>
                <tr>
                    <td><strong>Total Used</strong></td>
                    <td><strong>40,000</strong></td>
                    <td><strong>GHS 10,000 contingency</strong></td>
                </tr>
            </table>
        </section>
    </div>

    <footer>
        <p><strong>FixNow Ghana Project Portfolio</strong> | Created for BDT/Entrepreneurship | Accra, Ghana | 2026</p>
        <p>This is a conceptual demo built with HTML, CSS & JavaScript. No real payments are processed.</p>
    </footer>

    <script>
        // Makes the booking form work for demo
        document.getElementById('bookingForm').addEventListener('submit', function(e) {
            e.preventDefault();
            document.getElementById('successMsg').style.display = 'block';
            setTimeout(() => {
                document.getElementById('payment').scrollIntoView({ behavior: 'smooth' });
            }, 1000);
        });

        // Set min date to today
        document.getElementById('date').min = new Date().toISOString().split('T')[0];
    </script>
</body>
</html>
