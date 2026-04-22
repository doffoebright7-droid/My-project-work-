<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nora Gift Shop - Track Your Order</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Arial, sans-serif; }
        body { background: #FFF9F5; color: #333; line-height: 1.6; }
        header { background: #8E44AD; color: white; padding: 1rem 0; position: sticky; top: 0; z-index: 100; }
        nav { max-width: 1100px; margin: auto; display: flex; justify-content: space-between; align-items: center; padding: 0 20px; }
        nav ul { display: flex; list-style: none; gap: 20px; flex-wrap: wrap; }
        nav a { color: white; text-decoration: none; font-weight: bold; }
        nav a:hover { color: #F7DC6F; }
       .container { max-width: 1100px; margin: auto; padding: 40px 20px; }
        section { background: white; margin-bottom: 30px; padding: 30px; border-radius: 12px; box-shadow: 0 2px 10px rgba(142,68,173,0.1); }
        h1, h2, h3 { color: #8E44AD; margin-bottom: 15px; }
        h1 { font-size: 2.5rem; }
        h2 { font-size: 2rem; border-bottom: 3px solid #F7DC6F; padding-bottom: 10px; }
       .hero { text-align: center; background: linear-gradient(135deg, #8E44AD, #C39BD3); color: white; }
       .hero h1 { color: white; }
       .btn { display: inline-block; background: #F7DC6F; color: #8E44AD; padding: 12px 25px; margin-top: 15px; text-decoration: none; border-radius: 25px; font-weight: bold; border: none; cursor: pointer; }
       .btn:hover { background: #f4d03f; }
       .btn-secondary { background: #8E44AD; color: white; }
       .btn-secondary:hover { background: #7D3C98; }
       .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-top: 20px; }
       .card { border: 1px solid #FADBD8; padding: 20px; border-radius: 12px; transition: 0.3s; }
       .card:hover { transform: translateY(-5px); box-shadow: 0 5px 15px rgba(142,68,173,0.2); }
       .card img { width: 100%; height: 180px; object-fit: cover; border-radius: 8px; margin-bottom: 10px; background: #FADBD8; }
       .card h3 { color: #8E44AD; }
       .price { color: #E74C3C; font-weight: bold; font-size: 1.2rem; margin: 10px 0; }
       .tag { display: inline-block; background: #F5EEF8; color: #8E44AD; padding: 5px 10px; margin: 5px 5px 5px 0; border-radius: 15px; font-size: 0.9rem; }
        footer { background: #8E44AD; color: white; text-align: center; padding: 20px; margin-top: 30px; }

        /* Payment Page Styles */
       .payment-logos { display: flex; flex-wrap: wrap; gap: 15px; margin: 20px 0; }
       .payment-logo { width: 80px; height: 50px; border: 1px solid #ddd; border-radius: 8px; display: flex; align-items: center; justify-content: center; font-weight: bold; font-size: 0.8rem; }
       .mtn { background: #FFC600; color: #000; }
       .telecel { background: #E60000; color: white; }
       .at { background: #0099D8; color: white; }
       .visa { background: #1A1F71; color: white; }

        /* Form Styles */
       .form-group { margin-bottom: 15px; }
       .form-group label { display: block; margin-bottom: 5px; font-weight: bold; color: #8E44AD; }
       .form-group input,.form-group select,.form-group textarea {
            width: 100%; padding: 10px; border: 1px solid #ddd; border-radius: 5px; font-size: 1rem;
        }
       .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; }
        #cartForm, #trackForm { background: #F5EEF8; padding: 25px; border-radius: 12px; margin-top: 20px; }
       .success-msg { display: none; background: #2ECC71; color: white; padding: 15px; border-radius: 5px; margin-top: 15px; text-align: center; }
       .cart-item { display: flex; justify-content: space-between; padding: 10px 0; border-bottom: 1px dashed #ddd; }

        /* Track Order Styles */
       .tracker { display: none; margin-top: 20px; }
       .track-steps { display: flex; justify-content: space-between; margin: 30px 0; position: relative; }
       .track-steps::before { content: ''; position: absolute; top: 20px; left: 0; right: 0; height: 4px; background: #ddd; z-index: 1; }
       .track-progress { position: absolute; top: 20px; left: 0; height: 4px; background: #2ECC71; z-index: 2; width: 0%; transition: 1s; }
       .step { text-align: center; z-index: 3; position: relative; width: 25%; }
       .step-circle { width: 40px; height: 40px; border-radius: 50%; background: #ddd; margin: 0 auto 10px; display: flex; align-items: center; justify-content: center; color: white; font-weight: bold; }
       .step.active .step-circle { background: #2ECC71; }
       .step p { font-size: 0.9rem; }
       .order-details { background: white; border: 1px solid #FADBD8; padding: 20px; border-radius: 8px; margin-top: 20px; }
    </style>
</head>
<body>
    <header>
        <nav>
            <h3>🎁 Adom Gifts</h3>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#shop">Shop</a></li>
                <li><a href="#cart">Cart</a></li>
                <li><a href="#track">Track Order</a></li>
                <li><a href="#payment">Payment</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="container">
            <h1>Adom Gifts</h1>
            <p>Beautiful Gifts for Birthdays, Weddings, Graduations & All Special Moments</p>
            <p><strong>Location:</strong> Accra, Ghana | <strong>Delivery:</strong> Same-Day in Accra</p>
            <a href="#shop" class="btn">Shop Now</a>
            <a href="#track" class="btn btn-secondary">Track Your Order</a>
        </div>
    </section>

    <div class="container">
        <section id="shop">
            <h2>1. Shop: Gift Categories</h2>
            <p><em>To change products: Replace names/prices in the `addToCart()` buttons below</em></p>
            <div class="grid">
                <div class="card">
                    <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='250' height='180'%3E%3Crect width='250' height='180' fill='%23FADBD8'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%238E44AD'%3EBirthday Box%3C/text%3E%3C/svg%3E" alt="Birthday Gift Box">
                    <h3>Birthday Surprise Box</h3>
                    <p>Mug, chocolate, scented candle, birthday card</p>
                    <div class="price">GHS 150</div>
                    <button class="btn" onclick="addToCart('Birthday Surprise Box', 150)">Add to Cart</button>
                </div>
                <div class="card">
                    <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='250' height='180'%3E%3Crect width='250' height='180' fill='%23FADBD8'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%238E44AD'%3ELove Hamper%3C/text%3E%3C/svg%3E" alt="Love Hamper">
                    <h3>Love Hamper</h3>
                    <p>Teddy bear, roses, wine, custom note</p>
                    <div class="price">GHS 280</div>
                    <button class="btn" onclick="addToCart('Love Hamper', 280)">Add to Cart</button>
                </div>
                <div class="card">
                    <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='250' height='180'%3E%3Crect width='250' height='180' fill='%23FADBD8'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%238E44AD'%3EGraduation Pack%3C/text%3E%3C/svg%3E" alt="Graduation Pack">
                    <h3>Graduation Pack</h3>
                    <p>Journal, pen set, sash, “Congrats” frame</p>
                    <div class="price">GHS 200</div>
                    <button class="btn" onclick="addToCart('Graduation Pack', 200)">Add to Cart</button>
                </div>
                <div class="card">
                    <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='250' height='180'%3E%3Crect width='250' height='180' fill='%23FADBD8'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%238E44AD'%3ECustom Hamper%3C/text%3E%3C/svg%3E" alt="Custom Hamper">
                    <h3>Build Your Own Hamper</h3>
                    <p>Choose 5 items. We wrap it beautifully.</p>
                    <div class="price">From GHS 100</div>
                    <button class="btn" onclick="addToCart('Custom Hamper', 100)">Start Building</button>
                </div>
            </div>
        </section>

        <section id="cart">
            <h2>2. Shopping Cart & Checkout</h2>
            <div id="cartForm">
                <h3>Your Cart</h3>
                <div id="cartItems">
                    <p id="emptyCart">Your cart is empty. Add items from the shop above.</p>
                </div>
                <hr style="margin: 15px 0;">
                <div class="cart-item">
                    <strong>Subtotal:</strong>
                    <strong id="subtotal">GHS 0</strong>
                </div>
                <div class="cart-item">
                    <span>Delivery Fee (Accra):</span>
                    <span>GHS 20</span>
                </div>
                <div class="cart-item">
                    <strong>Total:</strong>
                    <strong id="total">GHS 20</strong>
                </div>

                <h3 style="margin-top: 20px;">Delivery Details</h3>
                <div class="form-row">
                    <div class="form-group">
                        <label for="name">Full Name</label>
                        <input type="text" id="name" placeholder="Ama Serwaa" required>
                    </div>
                    <div class="form-group">
                        <label for="phone">Phone Number</label>
                        <input type="tel" id="phone" placeholder="024 XXX XXXX" required>
                    </div>
                </div>
                <div class="form-group">
                    <label for="address">Delivery Address</label>
                    <input type="text" id="address" placeholder="Hse No. 5, East Legon, Accra" required>
                </div>

                <button type="button" class="btn" onclick="proceedToPay()">Proceed to Payment</button>
                <div class="success-msg" id="successMsg">Order #AD2026 confirmed! Scroll down to pay.</div>
            </div>
        </section>

        <section id="track">
            <h2>3. Track Your Order</h2>
            <p>Enter your order number to see live delivery updates. For demo, use: <strong>AD2026</strong></p>
            
            <div id="trackForm">
                <div class="form-group">
                    <label for="orderNumber">Order Number</label>
                    <input type="text" id="orderNumber" placeholder="e.g. AD2026">
                </div>
                <button class="btn" onclick="trackOrder()">Track Order</button>
                
                <div class="tracker" id="tracker">
                    <div class="order-details">
                        <h3>Order #AD2026</h3>
                        <p><strong>Items:</strong> <span id="trackItems">Love Hamper</span></p>
                        <p><strong>Total Paid:</strong> <span id="trackTotal">GHS 300</span></p>
                        <p><strong>Delivery to:</strong> East Legon, Accra</p>
                    </div>

                    <div class="track-steps">
                        <div class="track-progress" id="trackProgress"></div>
                        <div class="step active" id="step1">
                            <div class="step-circle">1</div>
                            <p>Order<br>Confirmed</p>
                        </div>
                        <div class="step" id="step2">
                            <div class="step-circle">2</div>
                            <p>Packaging<br>Gift</p>
                        </div>
                        <div class="step" id="step3">
                            <div class="step-circle">3</div>
                            <p>Out for<br>Delivery</p>
                        </div>
                        <div class="step" id="step4">
                            <div class="step-circle">4</div>
                            <p>Delivered</p>
                        </div>
                    </div>
                    <p id="trackStatus" style="text-align: center; font-weight: bold; color: #2ECC71;">Status: Order Confirmed - We’re preparing your gift!</p>
                </div>
            </div>
        </section>

        <section id="payment">
            <h2>4. Payment Page</h2>
            <p><strong>Why Mobile Money first?</strong> Over 70% of Ghanaians shop online using MoMo. Adom Gifts uses Paystack to accept all networks safely.</p>

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
                <button class="btn" onclick="alert('Demo: In real site, you would get a MoMo prompt on your phone to approve payment.')">Pay Now</button>
                <p style="margin-top:10px; font-size:0.9rem;"><em>Note: This is a demo. No real money will be charged.</em></p>
            </div>
        </section>
    </div>

    <footer>
        <p><strong>Adom Gifts Project Portfolio</strong> | Created for Entrepreneurship Class | Accra, Ghana | 2026</p>
        <p>Contact: 055-123-4567 | Instagram: @adomgifts_gh | This is a conceptual demo.</p>
    </footer>

    <script>
        let cart = [];
        let deliveryFee = 20;
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
                cartItemsDiv.innerHTML = '<p id="emptyCart">Your cart is empty. Add items from the shop above.</p>';
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
                alert('Your cart is empty. Please add a gift first!');
                return;
            }
            if (document.getElementById('name').value === '' || document.getElementById('phone').value === '') {
                alert('Please fill in your name and phone number.');
                return;
            }
            currentOrder = {
                id: 'AD2026',
                items: cart.map(i => i.name).join(', '),
                total: cart.reduce((sum, i) => sum + i.price, 0) + deliveryFee
            };
            document.getElementById('successMsg').style.display = 'block';
            setTimeout(() => {
                document.getElementById('payment').scrollIntoView({ behavior: 'smooth' });
            }, 1000);
        }

        function trackOrder() {
            const orderNum = document.getElementById('orderNumber').value.trim();
            if (orderNum === 'AD2026') {
                document.getElementById('tracker').style.display = 'block';
                document.getElementById('trackItems').innerText = currentOrder ? currentOrder.items : 'Love Hamper';
                document.getElementById('trackTotal').innerText = currentOrder ? `GHS ${currentOrder.total}` : 'GHS 300';
                
                // Animate progress for demo
                let step = 1;
                const interval = setInterval(() => {
                    step++;
                    document.getElementById('trackProgress').style.width = ((step - 1) * 33.33) + '%';
                    document.getElementById('step' + step).classList.add('active');
                    
                    const statuses = [
                        'Order Confirmed - We’re preparing your gift!',
                        'Packaging Your Gift - Adding ribbons & card',
                        'Out for Delivery - Rider is on the way!',
                        'Delivered - Enjoy your gift!'
                    ];
                    document.getElementById('trackStatus').innerText = `Status: ${statuses[step-1]}`;
                    
                    if (step === 4) clearInterval(interval);
                }, 1500);
            } else {
                alert('Order not found. For demo, use AD2026');
            }
        }
    </script>
</body>
</html>
