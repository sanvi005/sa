<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Riverside</title>
    <link href="https://fonts.googleapis.com/css2?family=Sofia&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700&display=swap" rel="stylesheet">
    <style>
    /* General Reset */
.{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Roboto', sans-serif;
    color: white;
    line-height: 1.5;
    background-color: black;
}
 
/* Hero Section */
.hero {
    position: relative;
    height: 100vh;
    background: url('https://www.shutterstock.com/image-photo/table-filled-dishes-food-set-600nw-2477073165.jpg')no-repeat center center/cover;
}

.overlay {
    background: rgba(0, 0, 0, 0.6); /* Transparent overlay */
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
}

.navbar .logo img {
    height: 50px;
}

.navbar .menu {
    font-size: 1.5rem;
    cursor: pointer;
}

.hero-content {
    text-align: center;
    margin-top: auto;
    margin-bottom: auto;
}

.hero-content .brand-name {
    font-family: 'Sofia', cursive;
    font-size: 3rem;
    letter-spacing: 2px;
    margin-bottom: 10px;
}

.hero-content .tagline {
    font-size: 1.2rem;
    letter-spacing: 1px;
    margin-bottom: 20px;
}

.buttons {
    display: flex;
    justify-content: center;
    gap: 15px;
}

.btn {
    text-decoration: none;
    padding: 10px 20px;
    border: 2px solid white;
    border-radius: 5px;
    transition: all 0.3s ease;
    font-size: 1rem;
    font-weight: 700;
}

.btn-primary {
    background: white;
    color: black;
}

.btn-primary:hover {
    background: transparent;
    color: white;
}

.btn-secondary:hover {
    background: white;
    color: black;
}

/* About Us Section */
.about-us {
    background-color: #f5f5dc; /* Beige background */
    color: #1c1c1c; /* Dark text color for contrast */
    padding: 60px 20px;
    text-align: center;
}

.about-us .container {
    max-width: 1200px;
    margin: 0 auto;
}

.about-heading h2 {
    font-family: 'Sofia', cursive; /* Heading font */
    font-size: 2.5rem;
    margin-bottom: 20px;
    color: #333;
}

.about-content p {
    font-family: 'Arial', sans-serif; /* Content font */
    font-size: 1.1rem;
    line-height: 1.8;
    color: #444;
    max-width: 800px;
    margin: 0 auto;
}

/* Menu Section */
.menu-section {
    display: flex;
    height: 100vh;
}

.menu-container {
    display: flex;
    width: 100%;
}

.menu-image {
    width: 50%;
    position: relative;
    overflow: hidden;
}

.menu-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    position: relative;
}

.menu-content {
    width: 50%;
    background-color: #f8d7dc; /* Powder pink background */
    padding: 50px 30px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: left;
}

.menu-heading {
    font-family: 'Sofia', cursive; /* Heading font */
    font-size: 2.5rem;
    margin-bottom: 20px;
    color: #333;
}

.menu-content p {
    font-family: 'Arial', sans-serif; /* Content font */
    font-size: 1.1rem;
    line-height: 1.6;
    color: #444;
    margin-bottom: 30px;
}
.menu-scroll{
            scroll-snap-type:y mandatory;
            scroll-snap-align:start;
        }
.view-menu-btn {
    padding: 10px 20px;
    background-color: #333;
    color: #fff;
    font-size: 1rem;
    font-family: 'Arial', sans-serif;
    border: none;
    cursor: pointer;
    border-radius: 5px;
    align-self: flex-start;
}

.view-menu-btn:hover {
    background-color: #555;
}

/* Menu Modal */
 .menu-modal {
    display: none;
    position: fixed;
    z-index: 1000;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
}
.modal-content {
    background-color: #f8d7dc;
    padding: 30px;
    border-radius: 10px;
    max-width: 800px;
    max-height:600px;
    overflow: hidden; /* Prevent content from overflowing the modal */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    margin: 50px auto;
    color: #333;
    text-align: left;
}

.modal-content h3 {
    font-family: 'Sofia', cursive;
    font-size: 1.8rem;
    margin-bottom: 10px;
}

.modal-content ul {
    list-style-type: none;
    padding: 0;
    margin-bottom: 20px;
}

.modal-content ul li {
    font-family: 'Arial', sans-serif;
    font-size: 1.1rem;
    margin-bottom: 5px;
}
.menu-scroll {
        max-height: calc(70% - 60px);
        overflow-y: auto; 
        padding: 5px;
        border-top: 1px solid #ddd;
        border-bottom: 1px solid #ddd;
    }

    .menu-scroll h4 {
        margin-top:5px;
        color: #333;
    }

    .menu-scroll ul {
        list-style-type: none;
        padding-left: 0;
        margin-bottom: 20px;
    }

    .menu-scroll li {
        padding: 5px 0;
        border-bottom: 1px solid #eee;
    }

.close-btn {
    color: #333;
    font-size: 1.5rem;
    float: right;
    cursor: pointer;
}

/* Gallery and Quote Section */
.gallery-quote-section {
    background-color: #f5f5dc; /* Beige background */
    padding: 50px 20px;
    position: relative;
    overflow: hidden;
}

/* Gallery and Quote Section */
.gallery-quote-section {
    background-color: #f5f5dc; /* Beige background */
    padding: 50px 20px;
    position: relative;
    overflow: hidden;
}

/* Gallery Images with Grid Layout */
.gallery-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); /* Responsive grid */
    gap: 20px; /* Space between images */
    justify-items: center;
    margin-bottom: 40px;
}

.gallery-container img {
    width: 100%;
    height: auto;
    max-width: 180px; /* Adjust maximum width for images */
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease;
}

.gallery-container img:hover {
    transform: scale(1.1);
}

/* Quote Section */
.quote-container {
    text-align: center;
    padding: 20px;
}

.quote {
    font-family: 'Sofia', cursive;
    font-size: 2rem;
    color: #333;
    margin: 0;
    line-height: 1.6;
    text-align: center;
}


/* Owner Review Section */
.owner-review-section {
    display: flex;
    height: 100vh; /* Full screen height */
}

/* Left Section */
.left-section {
    width: 50%;
    background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR_LTqwUnFW4Z6We8tdSbiyj40y8VLYldg9pQ&ss'); /* Replace with your actual image URL */
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    position: relative;
}

/* Logo */
.left-section .logo {
    position: absolute;
    top: 20px;
    left: 20px;
    width: 100px; /* Adjust logo size */
    z-index: 2;
}

/* Right Section */
.right-section {
    width: 50%;
    background-color: #2e8b57; /* Green background */
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 40px;
    text-align: center;
}

.review-heading {
    font-family: 'Sofia', cursive;
    font-size: 2.5rem;
    margin-bottom: 20px;
}

.review-message {
    font-family: 'Arial', sans-serif;
    font-size: 1.2rem;
    line-height: 1.8;
    margin-bottom: 40px;
}

.owner-signature {
    margin-top: auto;
    text-align: center;
}

.owner-name {
    font-size: 1.5rem;
    margin-bottom: 10px;
    font-family: 'Sofia', cursive;
}

/* Star Rating */
.star-rating {
    display: flex;
    justify-content: center;
    gap: 5px;
}

.star {
    font-size: 1.8rem;
    color: white;
    transition: color 0.3s ease;
    cursor: pointer;
}

.star:hover,
.star:hover ~ .star {
    color: #ffd700; /* Gold color */
}


/* Footer Section */
.footer-section {
    background-color: #000; /* Black background */
    color: #fff; /* White text */
    padding: 50px 20px;
    text-align: center;
    font-family: 'Arial', sans-serif;
}

/* Restaurant Name Styling */
.footer-heading h1 {
    font-family: 'Merriweather', serif;
    font-size: 3rem;
    font-weight: bold;
    margin-bottom: 40px;
    color: white;
}

/* Footer Containers Layout */
.footer-containers {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    margin-top: 20px;
    gap: 20px;
}

/* Individual Container */
.footer-container {
    text-align: center;
    min-width: 150px;
    flex: 1;
}

/* Styling for Lists */
.footer-container ol {
    list-style-type: decimal;
    padding: 0;
}

.footer-container ol li {
    margin-bottom: 10px;
    font-size: 1rem;
}

/* Styling for Bold Text */
.footer-container .bold-text {
    font-family: 'Merriweather', serif;
    font-size: 1.2rem;
    font-weight: bold;
    margin-bottom: 10px;
}

/* Responsive Design */
@media (max-width: 768px) {
    .footer-containers {
        flex-direction: column;
        align-items: center;
    }

    .footer-container {
        width: 100%;
        text-align: center;
    }
}
</style>
</head>
<body>
    <header class="hero">
        <div class="overlay">
            <div class="navbar">
                <div class="logo">
                     <img src="https://as1.ftcdn.net/v2/jpg/02/31/49/16/1000_F_231491645_55ZxP8esHsukMoJ0ZnL75Qy3i0tJVeNR.jpg" alt="Little Italy">
                </div>                   
                
            </div>
            <div class="hero-content">
                <h1 class="brand-name">Little Italy</h1>
                <p class="tagline">Bar &bull; Restaurant &bull; Café</p>
                <div class="buttons">
                    <a href="#order" class="btn btn-primary">Order Online</a>
                    <a href="#reserve" class="btn btn-secondary">Reservations</a>
                </div>
            </div>
        </div>
    </header>
    <section class="about-us">
    <div class="container">
        <div class="about-heading">
            <h2>About Us</h2>
        </div>
        <div class="about-content">
            <p>
                Established in 2020, Little Italy has been a cornerstone of fine dining, offering a harmonious blend of gourmet cuisine, exceptional service, and a cozy ambiance. Nestled by the serene riverside, our restaurant invites you to indulge in unforgettable culinary experiences. Whether you're dining with loved ones, enjoying a quiet café moment, or ordering from the comfort of your home, Little Italy is committed to delighting your senses. Our chefs craft every dish with passion, using only the freshest and finest ingredients. Join us and become part of our story, where tradition meets innovation.
            </p>
        </div>
    </div>
</section>


<section class="menu-section">
    <div class="menu-container">
        <!-- Left Section: Full-screen Image with Logo -->
        <div class="menu-image">
            <img src="https://media.istockphoto.com/id/857927726/photo/pasta-with-meat-tomato-sauce-and-vegetables.jpg?s=612x612&w=0&k=20&c=1bcoXcBKM7Hb1ASweDx-vcwXEgy-WrCGM71dVP2Cp0w=" alt="Little Italy" class="logo">
        </div>

        <!-- Right Section: Menu Description -->
        <div class="menu-content">
            <h2 class="menu-heading">Our Menu</h2>
            <p>
                Discover our carefully crafted menu that showcases the best of Italian cuisine, refreshing beverages, 
                and indulgent desserts. Whether you're craving a hearty meal or a sweet treat, we have something for everyone.
            </p>
            <button class="view-menu-btn" onclick="openMenu()">View Full Menu</button>
        </div>
    </div>
</section>
<!-- Modal for Full Menu -->
<div id="menuModal" class="menu-modal">
    <div class="modal-content">
        <span class="close-btn" onclick="closeMenu()">&times;</span>
        <h3 class="modal-heading">Our Full Menu</h3>
        <div class="menu-scroll">
            <h4>Main Course</h4>
            <ul>
                <li>Spaghetti Carbonara------------280/-</li>
                <li>Margherita Pizza---------------300/-</li>
                <li>Lasagna al Forno---------------240/-</li>
                <li>Risotto alla Milanese----------290/-</li>
                </ul>
            <h4>Beverages</h4>
            <ul>
                <li>Red Wine-----------------------450/-(per glass)</li>
                <li>White Sangria------------------400/-</li>
                </ul>
            <h4 id>Desserts</h4>
            <ul>
                <li>Tiramisu-----------------------260/-</li>
                <li>Panna Cotta--------------------280/-</li>
                </ul>
        </div>
    </div>
</div>
<section class="gallery-quote-section">
    <div class="gallery-container">
        <!-- Jumbled Images -->
        <div class="image jumbled-1">
            <img src="https://www.touchbistro.com/wp-content/uploads/2021/08/restaurant-interior-design-ideas-thumbnail.jpg" alt="View Image 1">
        </div>
        <div class="image jumbled-2">
            <img src="https://cdn.prod.website-files.com/61bcac7b8c69b74b8d5c2b99/654a38bfe3bf7526c162fce0_2%20(15).png" alt="View Image 2">
        </div>
        <div class="image jumbled-3">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQHPDTUNLaIh-mWx9Lxywd2E_ZoCLH7IiA1Yg&s" alt="View Image 3">
        </div>
        <div class="image jumbled-4">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSslbawN4U2ru7pPCW5cbERkS8nX44aG8JrLRqsO4RT5BXfOA7ZM2SdWZ0VqT4p93XPF4w&usqp=CAU" alt="View Image 4">
        </div>
        <div class="image jumbled-5">
            <img src="https://cdn.tatlerasia.com/tatlerasia/i/2023/09/21114713-la-rambla_cover_1599x1066.jpeg" alt="View Image 5">
         </div>
    </div>

    <!-- Quoted Text -->
    <div class="quote-container">
        <blockquote class="quote">
            "A Perfect Destination for all your Celebrations"
        </blockquote>
    </div>



<section class="owner-review-section">
    <!-- Left Section with Full-Screen Image -->
    <div class="left-section">
        <img class="logo" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR_LTqwUnFW4Z6We8tdSbiyj40y8VLYldg9pQ&s" alt="Logo">
    </div>

    <!-- Right Section with Review Content -->
    <div class="right-section">
        <h2 class="review-heading">A Special Message to Our Customers</h2>
        <p class="review-message">
            "Thank you for making Little Italy your destination for memorable dining experiences. 
            We cherish each visit and strive to bring joy to your table with every meal."
        </p>
        <div class="owner-signature">
            <p class="owner-name">- Evian</p>
            <div class="star-rating">
                <span class="star">&#9733;</span>
                <span class="star">&#9733;</span>
                <span class="star">&#9733;</span>
                <span class="star">&#9733;</span>
                <span class="star">&#9733;</span>
            </div>
        </div>
    </div>
</section>




<section class="footer-section">
    <!-- Restaurant Name -->
    <div class="footer-heading">
        <h1>LITTLE ITALY</h1>
    </div>

    <!-- Four Vertical Containers -->
    <div class="footer-containers">
        <!-- First Container: Links -->
        <div class="footer-container">
            
                <p>Menu</li>
                <p>Order Online</p>
                <p>Reservations</p>
                <p>About</p>
                <p>Contact Us</p>
            
        </div>

        <!-- Second Container: Opening Hours -->
        <div class="footer-container">
           
                <p class="bold-text">OPENING HOURS</p>
                <p>Tuesday to Friday, 9am to 7pm</p>
                <p>Saturday & Sunday, 10am to 7pm</p>
            
        </div>

        <!-- Third Container: Address -->
        <div class="footer-container">
            <p class="bold-text">Where We Are</p>
            <p>500 Kormangala, Bangalore</p>
            <p>123-456-7890</p>
            <p>riverside@u.com</p>
        </div>

        <!-- Fourth Container: Policies -->
        <div class="footer-container">
            
                <p>Terms & Conditions</p>
                <p>Refund Policy</p>
                <p>Privacy Policy</p>
                <p>Accessibility</p>
                <p>Statement</p>            
        </div>
    </div>
</section>		
<script>
function openMenu() {
    document.getElementById("menuModal").style.display = "block";
}

function closeMenu() {
    document.getElementById("menuModal").style.display = "none";
}
</script>
</body>
</html>
