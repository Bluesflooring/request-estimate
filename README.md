# request-estimate
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Southern Carpet & Interiors</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }
        header {
            background: #004080;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            background: #003366;
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
        }
        .quote-form {
            background: white;
            padding: 20px;
            margin: 20px 0;
            border-radius: 5px;
        }
        .quote-form label, .quote-form input, .quote-form select, .quote-form textarea {
            display: block;
            width: 100%;
            margin-bottom: 10px;
        }
        .quote-form input, .quote-form select, .quote-form textarea {
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .quote-form button {
            background: #004080;
            color: white;
            padding: 10px;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <h1>Southern Carpet & Interiors</h1>
        <p>High-Quality Flooring Solutions for Your Home or Business</p>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#gallery">Gallery</a>
        <a href="#contact">Contact</a>
    </nav>
    <div class="container">
        <section id="request-quote" class="quote-form">
            <h2>Request a Quote</h2>
            <form action="submit_quote.php" method="POST" enctype="multipart/form-data">
                <label for="name">Full Name</label>
                <input type="text" id="name" name="name" required>
                
                <label for="phone">Phone Number</label>
                <input type="text" id="phone" name="phone" required>
                
                <label for="email">Email Address</label>
                <input type="email" id="email" name="email" required>
                
                <label for="address">Project Address</label>
                <input type="text" id="address" name="address" required>
                
                <label for="flooring">Type of Flooring</label>
                <select id="flooring" name="flooring">
                    <option value="Carpet">Carpet</option>
                    <option value="LVP">LVP</option>
                    <option value="Hardwood">Hardwood</option>
                    <option value="Tile">Tile</option>
                    <option value="Other">Other</option>
                </select>
                
                <label for="sqft">Square Footage (if known)</label>
                <input type="number" id="sqft" name="sqft">
                
                <label for="contact-method">Preferred Contact Method</label>
                <select id="contact-method" name="contact-method">
                    <option value="Phone">Phone</option>
                    <option value="Email">Email</option>
                    <option value="Text">Text</option>
                </select>
                
                <label for="details">Project Details</label>
                <textarea id="details" name="details" rows="4"></textarea>
                
                <label for="images">Upload Images (Optional)</label>
                <input type="file" id="images" name="images" accept="image/*">
                
                <button type="submit">Submit Quote Request</button>
            </form>
        </section>
    </div>
</body>
</html>
