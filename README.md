# ayodhyahomestay
Ayodhya Home Stay
<!DOCTYPE html>
<html lang="en-US">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Ayodhya Home Stay | Pathardih</title>
    <style>
        :root {
            --primary: #05051E;
            --accent: #6752EC;
            --text-dark: #181818;
            --bg-gray: #f4f4f9;
            --success: #25D366;
            --star: #FFD700;
            --warning: #f39c12;
            --festival: #e74c3c;
            --eco: #27ae60;
            --craft: #a0522d;
            --season: #3498db;
        }

        body, html { margin: 0; padding: 0; font-family: 'Segoe UI', Arial, sans-serif; color: var(--text-dark); scroll-behavior: smooth; overflow-x: hidden; }

        /* Navigation */
        header { display: flex; justify-content: space-between; align-items: center; padding: 15px 10%; background: #fff; position: sticky; top: 0; z-index: 2000; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
        .logo { font-size: 22px; font-weight: 800; color: var(--primary); }
        .nav-links a { text-decoration: none; color: var(--text-dark); margin-left: 20px; font-weight: 600; font-size: 13px; text-transform: uppercase; }
        .book-btn-nav { background: var(--accent); color: white !important; padding: 8px 15px; border-radius: 5px; }

        /* Hero Slider */
        .hero-slider { position: relative; height: 60vh; width: 100%; overflow: hidden; }
        .slide { position: absolute; width: 100%; height: 100%; opacity: 0; transition: opacity 1s ease-in-out; background-size: cover; background-position: center; }
        .slide.active { opacity: 1; }
        .slide::after { content: ''; position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: rgba(5, 5, 30, 0.5); }
        
        .hero-content { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); text-align: center; color: white; z-index: 10; width: 80%; }
        .hero-content h1 { font-size: 3rem; margin-bottom: 10px; }

        /* Video Tour Section [New Section] */
        .video-container { position: relative; width: 100%; max-width: 900px; margin: 0 auto; border-radius: 20px; overflow: hidden; box-shadow: 0 20px 40px rgba(0,0,0,0.2); background: #000; }
        .video-wrapper { position: relative; padding-bottom: 56.25%; height: 0; }
        .video-wrapper iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0; }

        /* Best Time Section */
        .season-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; }
        .season-card { background: white; padding: 25px; border-radius: 12px; border-top: 5px solid var(--season); box-shadow: 0 4px 10px rgba(0,0,0,0.05); }

        /* Photo Gallery */
        .nature-gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; }
        .gallery-card { position: relative; border-radius: 12px; overflow: hidden; height: 250px; box-shadow: 0 4px 12px rgba(0,0,0,0.1); }
        .gallery-card img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.3s ease; }
        .gallery-card:hover img { transform: scale(1.1); }

        /* Weather Section */
        .weather-card { max-width: 400px; margin: 0 auto; background: white; padding: 20px; border-radius: 15px; display: flex; align-items: center; gap: 20px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); }

        /* Booking Card */
        .booking-card { max-width: 600px; margin: 0 auto; background: #fff; padding: 30px; border-radius: 15px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); }
        .whatsapp-btn { width: 100%; padding: 15px; background: var(--success); color: white; border: none; border-radius: 8px; font-weight: 700; cursor: pointer; }

        footer { background: var(--primary); color: #fff; padding: 40px 10%; text-align: center; }
        .section { padding: 60px 10%; }
        h2 { color: var(--primary); margin-bottom: 30px; text-align: center; }
    </style>
</head>
<body>

<header>
    <div class="logo">AYODHYA HOME STAY</div>
    <nav class="nav-links">
        <a href="#about">About</a>
        <a href="#tour">Video Tour</a>
        <a href="#seasons">Best Time</a>
        <a href="#booking" class="book-btn-nav">Book Now</a>
    </nav>
</header>

<div class="hero-slider">
    <div class="slide active" style="background-image: url('https://images.unsplash.com/photo-1566073771259-6a8506099945?auto=format&fit=crop&w=1600&q=80');"></div>
    <div class="slide" style="background-image: url('https://images.unsplash.com/photo-1542314831-068cd1dbfeeb?auto=format&fit=crop&w=1600&q=80');"></div>
    <div class="hero-content">
        <h1>Ayodhya Home Stay</h1>
        <p>Experience Pure Comfort in Pathardih</p>
    </div>
</div>

<section class="section" id="weather-status" style="background: var(--bg-gray);">
    <div class="weather-card">
        <div style="font-size: 50px;">☀️</div>
        <div class="weather-info">
            <h4>Local Climate - Pathardih</h4>
            <div class="weather-temp">24°C</div>
            <p style="margin: 0; font-size: 14px; color: #666;">Perfect for Trekking</p>
        </div>
    </div>
</section>

<section class="section" id="tour">
    <h2>Take a Video Tour</h2>
    <div class="video-container">
        <div class="video-wrapper">
            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="Home Stay Tour" allowfullscreen></iframe>
        </div>
    </div>
    <p style="text-align: center; margin-top: 20px; color: #666;">Experience the ambiance and the scenic surroundings of our property.</p>
</section>

<section class="section" id="about" style="background-color: var(--bg-gray);">
    <h2>Welcome to Your Home in Purulia</h2>
    <p style="text-align: center; max-width: 800px; margin: 0 auto; line-height: 1.8;">Nestled in Pathardih, West Bengal, Ayodhya Home Stay offers a serene escape with modern amenities and traditional hospitality.</p>
</section>

<section class="section" id="seasons">
    <h2>Best Time to Visit</h2>
    <div class="season-grid">
        <div class="season-card">
            <span style="color: var(--season); font-weight: 800; font-size: 14px; display: block; margin-bottom: 10px;">October - February (Winter)</span>
            <p>The **ideal time for trekking**. Cool weather and clear skies.</p>
        </div>
        <div class="season-card">
            <span style="color: var(--season); font-weight: 800; font-size: 14px; display: block; margin-bottom: 10px;">March - April (Spring)</span>
            <p>Witness the **Palash Festival**. Landscape turns fiery red.</p>
        </div>
        <div class="season-card">
            <span style="color: var(--season); font-weight: 800; font-size: 14px; display: block; margin-bottom: 10px;">July - September (Monsoon)</span>
            <p>Best for **nature lovers**. The hills become lush green.</p>
        </div>
    </div>
</section>

<section class="section" id="gallery" style="background-color: var(--bg-gray);">
    <h2>Explore the Beauty of Purulia</h2>
    <div class="nature-gallery">
        <div class="gallery-card"><img src="https://images.unsplash.com/photo-1626583223726-b259a1ba244c?w=500"><div style="position: absolute; bottom: 0; width: 100%; background: rgba(0,0,0,0.6); color: white; padding: 10px; font-size: 14px; text-align: center;">Ayodhya Hills</div></div>
        <div class="gallery-card"><img src="https://images.unsplash.com/photo-1596333757424-4091f044030d?w=500"><div style="position: absolute; bottom: 0; width: 100%; background: rgba(0,0,0,0.6); color: white; padding: 10px; font-size: 14px; text-align: center;">Marble Lake</div></div>
        <div class="gallery-card"><img src="https://images.unsplash.com/photo-1589182373726-e4f658ab50f0?w=500"><div style="position: absolute; bottom: 0; width: 100%; background: rgba(0,0,0,0.6); color: white; padding: 10px; font-size: 14px; text-align: center;">Forest Trails</div></div>
    </div>
</section>

<section class="section" id="crafts">
    <h2>Local Market & Handicrafts</h2>
    <div style="display: flex; flex-wrap: wrap; gap: 25px;">
        <div style="flex: 1; min-width: 280px; background: #fff; padding: 20px; border-radius: 12px; border-bottom: 4px solid var(--craft); box-shadow: 0 4px 10px rgba(0,0,0,0.05);">
            <h4 style="color: var(--craft);">🎭 Charida Chhau Masks</h4>
            <p>Visit Charida village nearby, world-famous for handcrafted masks.</p>
        </div>
        <div style="flex: 1; min-width: 280px; background: #fff; padding: 20px; border-radius: 12px; border-bottom: 4px solid var(--craft); box-shadow: 0 4px 10px rgba(0,0,0,0.05);">
            <h4 style="color: var(--craft);">👜 Babui Grass Items</h4>
            <p>Discover beautiful items hand-woven by local tribal women.</p>
        </div>
    </div>
</section>

<section class="section" id="eco" style="background-color: var(--bg-gray);">
    <div style="background: #e8f5e9; padding: 40px; border-radius: 20px; border: 1px dashed var(--eco); text-align: center;">
        <h2 style="color: var(--eco);">🌿 Committed to Eco-Tourism</h2>
        <p>We follow sustainable practices to ensure your stay leaves a positive footprint.</p>
    </div>
</section>

<section class="section" id="sightseeing">
    <h2>Nearby Sightseeing Spots</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px;">
        <div style="background: white; padding: 20px; border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.05);"><h4>Marble Lake</h4><span>📍 12 km</span></div>
        <div style="background: white; padding: 20px; border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.05);"><h4>Bamni Falls</h4><span>📍 15 km</span></div>
        <div style="background: white; padding: 20px; border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.05);"><h4>Hanuman Mandir</h4><span>📍 2 min walk</span></div>
    </div>
</section>

<section class="section" id="events" style="background-color: var(--bg-gray);">
    <h2>Local Events & Festivals</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
        <div style="border-left: 5px solid var(--festival); background: white; padding: 20px; border-radius: 10px;"><h3>Purulia Chau Dance</h3><p>Witness the world-famous UNESCO recognized mask dance.</p></div>
    </div>
</section>

<section class="section" id="host">
    <h2>Meet Your Host</h2>
    <div style="display: flex; align-items: center; gap: 40px; flex-wrap: wrap; background: #fff; padding: 40px; border-radius: 20px; box-shadow: 0 10px 30px rgba(0,0,0,0.05);">
        <div style="width: 150px; height: 150px; border-radius: 50%; overflow: hidden; border: 5px solid var(--accent);"><img src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?w=400" style="width:100%; height:100%; object-fit:cover;"></div>
        <div style="flex:1;"><h3>Namaste, I'm Your Host!</h3><p>I started <strong>Ayodhya Home Stay</strong> to share the hidden beauty of Purulia.</p></div>
    </div>
</section>

<section class="section" id="transport" style="background-color: var(--bg-gray);">
    <h2>How to Reach Us</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
        <div style="background: white; padding: 25px; border-radius: 12px; box-shadow: 0 4px 10px rgba(0,0,0,0.05);"><span>🚂</span><h4>By Train</h4><p>Purulia Junction is the nearest station.</p></div>
        <div style="background: white; padding: 25px; border-radius: 12px; box-shadow: 0 4px 10px rgba(0,0,0,0.05);"><span>🚗</span><h4>By Road</h4><p>Search "Ayodhya Home Stay Pathardih" on Maps.</p></div>
    </div>
</section>

<section class="section" id="activities">
    <h2>Things to Do</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; text-align: center;">
        <div style="background:white; padding:20px; border-radius:10px; box-shadow: 0 4px 10px rgba(0,0,0,0.05);"><h3>🥾 Trekking</h3></div>
        <div style="background:white; padding:20px; border-radius:10px; box-shadow: 0 4px 10px rgba(0,0,0,0.05);"><h3>📸 Photography</h3></div>
    </div>
</section>

<section class="section" id="dining" style="background-color: var(--bg-gray);">
    <h2>Traditional Food & Dining</h2>
    <div style="display: flex; flex-wrap: wrap; gap: 30px; align-items: center;">
        <div style="flex: 1; min-width: 300px;"><img src="https://images.unsplash.com/photo-1512621776951-a57141f2eefd?w=800" style="width:100%; border-radius:15px;"></div>
        <div style="flex: 1.5; min-width: 300px;"><h4>Authentic Bengali Thalis</h4><p>Prepared with farm-fresh local ingredients.</p></div>
    </div>
</section>

<section class="section" id="safety">
    <h2>Safety & Property Guidelines</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px;">
        <div style="background: #fff7e6; padding: 20px; border-radius: 10px; border-top: 4px solid var(--warning);"><h4>🛡️ Stay Secure</h4><p>Keep your room locked when heading out.</p></div>
    </div>
</section>

<section class="section" id="facilities" style="background-color: var(--bg-gray);">
    <h2>Amenities & Facilities</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px;">
        <div style="background: #fff; padding: 30px; border-radius: 12px; text-align: center; box-shadow: 0 4px 15px rgba(0,0,0,0.05);">🚗 Free Parking</div>
        <div style="background: #fff; padding: 30px; border-radius: 12px; text-align: center; box-shadow: 0 4px 15px rgba(0,0,0,0.05);">📶 High-Speed Wi-Fi</div>
    </div>
</section>

<section class="section" id="faq">
    <h2>Common Questions</h2>
    <div style="max-width: 800px; margin: 0 auto; background: #fff; padding: 15px; border-radius: 10px;"><strong>ID Proof?</strong> Government ID mandatory for all guests.</div>
</section>

<section class="section" id="reviews" style="background-color: var(--bg-gray);">
    <h2>Guest Reviews</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
        <div style="background: white; padding: 20px; border-radius: 15px; border-left: 5px solid var(--accent);">"Peaceful environment!" - Sneha</div>
    </div>
</section>

<section class="section" id="booking">
    <h2>Book Your Stay</h2>
    <div class="booking-card">
        <select id="roomType" style="width:100%; padding:12px; margin-bottom:20px; border-radius:8px; border:1px solid #ddd;">
            <option>Executive Double (₹2,500)</option>
            <option>Classic Family Suite (₹4,500)</option>
        </select>
        <button class="whatsapp-btn" onclick="sendWhatsApp()">Check Availability on WhatsApp</button>
    </div>
</section>

<section class="section" id="visit" style="background-color: var(--bg-gray);">
    <div style="display: flex; align-items: center; gap: 40px; flex-wrap: wrap;">
        <div style="flex: 1.2; min-width: 300px;">
            <h2>Visit Us</h2>
            <p>Beside Hanuman Mandir Gosaidih, Pathardih, WB 723152</p>
            <p>Contact: +91 98540 76606</p>
            <a href="#" style="display: inline-block; margin-top: 15px; padding: 12px 25px; background: var(--accent); color: white; text-decoration: none; border-radius: 5px; font-weight: 600;">📍 Get Directions</a>
        </div>
        <div style="flex: 1; min-width: 300px; height: 350px; border-radius: 15px; overflow: hidden;">
            <iframe src="https://www.google.com/maps/embed" style="width:100%; height:100%; border:0;" allowfullscreen="" loading="lazy"></iframe>
        </div>
    </div>
</section>

<footer>
    <p><strong>Ayodhya Home Stay</strong> - Pathardih, West Bengal</p>
    <p>© 2026 All Rights Reserved.</p>
</footer>

<script>
    const slides = document.querySelectorAll('.slide');
    let currentSlide = 0;
    function nextSlide() {
        slides[currentSlide].classList.remove('active');
        currentSlide = (currentSlide + 1) % slides.length;
        slides[currentSlide].classList.add('active');
    }
    setInterval(nextSlide, 4000);

    function sendWhatsApp() {
        const room = document.getElementById('roomType').value;
        const msg = `Hello! I'd like to check availability for ${room} at Ayodhya Home Stay.`;
        window.open(`https://wa.me/919854076606?text=${encodeURIComponent(msg)}`, '_blank');
    }
</script>

</body>
</html>
