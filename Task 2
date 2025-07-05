<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple E-Commerce Website</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    header {
      background-color: #333;
      color: #fff;
      padding: 1em;
      text-align: center;
    }

    nav {
      background: #444;
      padding: 1em;
      text-align: center;
    }

    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
    }

    .product-list {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
      padding: 20px;
    }

    .product {
      border: 1px solid #ccc;
      padding: 10px;
      text-align: center;
      background-color: #f9f9f9;
    }

    .product img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .product button {
      background-color: #28a745;
      color: white;
      border: none;
      padding: 10px;
      cursor: pointer;
      margin-top: 10px;
    }

    .cart {
      background-color: #f1f1f1;
      padding: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>My E-Commerce Store</h1>
  </header>
  <nav>
    <a href="#home">Home</a>
    <a href="#products">Products</a>
    <a href="#cart">Cart</a>
  </nav>

  <main>
    <section class="product-list" id="products">
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Product 1">
        <h3>Product 1</h3>
        <p>₹499</p>
        <button onclick="addToCart('Product 1', 499)">Add to Cart</button>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Product 2">
        <h3>Product 2</h3>
        <p>₹699</p>
        <button onclick="addToCart('Product 2', 699)">Add to Cart</button>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Product 3">
        <h3>Product 3</h3>
        <p>₹899</p>
        <button onclick="addToCart('Product 3', 899)">Add to Cart</button>
      </div>
    </section>

    <section class="cart" id="cart">
      <h2>Shopping Cart</h2>
      <ul id="cart-items"></ul>
      <h3 id="total">Total: ₹0</h3>
    </section>
  </main>

  <script>
    const cartItems = [];

    function addToCart(productName, price) {
      cartItems.push({ name: productName, price: price });
      renderCart();
    }

    function renderCart() {
      const cartList = document.getElementById('cart-items');
      cartList.innerHTML = '';
      let total = 0;

      cartItems.forEach(item => {
        const li = document.createElement('li');
        li.textContent = `${item.name} - ₹${item.price}`;
        cartList.appendChild(li);
        total += item.price;
      });

      document.getElementById('total').textContent = `Total: ₹${total}`;
    }
  </script>
</body>
</html>
