<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Royal Taste Restaurant</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:#fafafa;
color:#333;
}

header{
background:#222;
color:white;
padding:20px;
display:flex;
justify-content:space-between;
align-items:center;
}

nav a{
color:white;
margin-left:20px;
text-decoration:none;
}

.hero{
height:80vh;
background:url("https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?w=1600") center/cover;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
color:white;
text-align:center;
}

.hero h1{
font-size:60px;
}

.hero p{
font-size:22px;
margin:20px;
}

button{
padding:15px 35px;
font-size:18px;
background:#ff5722;
border:none;
color:white;
cursor:pointer;
}

section{
padding:60px;
text-align:center;
}

.menu{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
margin-top:40px;
}

.card{
background:white;
padding:20px;
border-radius:10px;
box-shadow:0 0 10px rgba(0,0,0,.1);
}

.card img{
width:100%;
border-radius:10px;
}

footer{
background:#222;
color:white;
text-align:center;
padding:20px;
margin-top:40px;
}
</style>

</head>
<body>

<header>
<h2>Royal Taste</h2>

<nav>
<a href="#">Home</a>
<a href="#">Menu</a>
<a href="#">About</a>
<a href="#">Contact</a>
</nav>

</header>

<div class="hero">
<h1>Welcome to Royal Taste</h1>
<p>Fresh Food • Best Taste • Fast Delivery</p>
<button>Order Now</button>
</div>

<section>

<h2>Our Popular Dishes</h2>

<div class="menu">

<div class="card">
<img src="https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?w=600">
<h3>Pizza</h3>
<p>$12</p>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1550547660-d9450f859349?w=600">
<h3>Burger</h3>
<p>$10</p>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1544025162-d76694265947?w=600">
<h3>Steak</h3>
<p>$18</p>
</div>

</div>

</section>

<footer>
© 2026 Royal Taste Restaurant
</footer>

</body>
</html>
