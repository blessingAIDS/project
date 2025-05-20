# Project Responsive Web Design using Bootstrap
# Date:20.05.2025
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Design Portfolio</title>
</head>
<style>
    /* Reset and basic styles */
body, h1, h2, p, a, input, button {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f5f5f5;
    color: #333;
}

/* Top Bar Styling */
.top-bar {
    display: flex;
    align-items: center;
    background-color: #ffffff;
    padding: 10px 20px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.search-bar {
    margin-right: 15px;
    padding: 8px;
    border: 1px solid #ddd;
    border-radius: 4px;
    outline: none;
}

.nav-item {
    margin: 0 10px;
    color: #333;
    text-decoration: none;
}

.blue-text {
    color: #007bff;
    font-weight: bold;
}

.blue-text:hover {
    text-decoration: underline;
}

/* Header Section */
header {
    background-image: url('download.jpg');   /* Add your header image */
    background-size: cover;
    padding: 80px 20px;
    text-align: center;
    color: #fff;
}

.header-content h1 {
    font-size: 36px;
    margin-bottom: 10px;
}

.header-content p {
    font-size: 18px;
    margin-bottom: 20px;
}

.search-input {
    padding: 10px;
    width: 60%;
    max-width: 500px;
    border: none;
    border-radius: 4px;
    outline: none;
}

/* Trending Searches Section */
.trending {
    padding: 20px;
    text-align: center;
}

.trending h2 {
    font-size: 24px;
    margin-bottom: 10px;
}

.trending-tags {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.trending-tags span {
    background-color: #007bff;
    color: #fff;
    padding: 5px 10px;
    margin: 5px;
    border-radius: 4px;
    font-size: 14px;
}

/* Gallery Section */
.gallery {
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
    width: 200px;
    text-align: center;
}

.card img {
    width: 100%;
    height: auto;
}

.card h3 {
    font-size: 16px;
    margin: 10px 0;
}

.card p {
    font-size: 12px;
    color: #555;
    margin-bottom: 10px;
}

/* Gallery Section */
.gallery {
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
    width: 200px;
    text-align: center;
    position: relative;
}

.card img {
    width: 100%;
    height: auto;
    transition: transform 0.3s ease;
}

.card:hover img {
    transform: scale(1.2); /* Scale image to 120% on hover */
}

.card h3 {
    font-size: 16px;
    margin: 10px 0;
}

.card p {
    font-size: 12px;
    color: #555;
    margin-bottom: 10px;
}

/* Footer Section */
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px 20px;
    margin-top: 20px;
}
</style>
<body>
    <!-- Top Navigation Bar -->
    <div class="top-bar">
        <input type="text" class="search-bar" placeholder="Search...">
        <a href="#" class="nav-item">Explore</a>
        <a href="#" class="nav-item">Hire a Developer</a>
        <a href="#" class="nav-item">Designs</a>
        <a href="#" class="nav-item">Blog</a>
        <a href="#" class="nav-item blue-text">Sign up</a>
        <a href="#" class="nav-item blue-text">Log in</a>
    </div>

    <!-- Header Section -->
    <header>
        <div class="header-content">
            <h1>𝓓𝓲𝓼𝓬𝓸𝓿𝓮𝓻 𝓾𝓷𝓲𝓺𝓾𝓮 𝓪𝓷𝓭 𝓭𝓮𝓼𝓲𝓻𝓮𝓭 𝓭𝓮𝓼𝓲𝓰𝓷𝓼</h1>
            <p>𝕎𝕙𝕒𝕥 𝕒𝕣𝕖 𝕪𝕠𝕦 𝕘𝕠𝕟𝕟𝕒 𝕕𝕖𝕤𝕚𝕘𝕟 𝕥𝕠𝕕𝕒𝕪?</p>
            <input type="text" class="search-input" placeholder="What are you looking for?">
        </div>
    </header>

    <!-- Trending Searches Section -->
    <section class="trending">
        <h2>Trending Searches</h2>
        <div class="trending-tags">
            <span>Brouchers</span>
            <span>Posters</span>
            <span>Insta story</span>
            <span>logo design</span>
            <span>Thumbnail</span>
            <span>Icons</span>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="gallery">

        <div class="card">
            <img src="Screenshot 2025-05-16 001631.png" alt="Design Sample 1">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-15 233406.png" alt="Design Sample 2">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-15 233656.png" alt="Design Sample 3">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-15 232311.png" alt="Design Sample 4">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-15 231144.png" alt="Design Sample 5">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-15 230414.png" alt="Design Sample 6">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-15 230359.png" alt="Design Sample 7">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-15 230118.png" alt="Design Sample 8">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-15 225539.png" alt="Design Sample 9">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-15 225110.png" alt="Design Sample 10">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-14 092843.png" alt="Design Sample 11">
        </div>

        <div class="card">
            <img src="Screenshot 2025-05-14 092808.png" alt="Design Sample 12">
        </div>
        <!-- Add more cards as needed -->
    </section>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2025 Design Portfolio. All rights reserved.</p>
    </footer>

    <script>
        // Search functionality
const searchBar = document.querySelector('.search-bar');

searchBar.addEventListener('keydown', function(event) {
    if (event.key === 'Enter') {
        event.preventDefault(); // Prevent default form submission
        alert(Searching for: ${searchBar.value});
    }
});
    </script>
</body>
</html>
```
# OUTPUT:
![image](https://github.com/user-attachments/assets/f1c40aed-fe64-461f-b646-29260fe9c780)

![image](https://github.com/user-attachments/assets/014661be-c50e-426f-ac0f-024823e4f276)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
