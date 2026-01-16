# Myntra-bag-html-
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Practice</title>
    <link rel="stylesheet" href="css/practice.css">
    <style>
        .bag-button {
            padding: 10px;
            background-color: lightblue;
            border: none;
            cursor: pointer;
        }
        .wish-button {
            padding: 10px;
            background-color: pink;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1 id="cart-summary">Your bag has 5 items.</h1>

    <button class="bag-button" onclick="
        cartquantity++;
        document.querySelector('#cart-summary').innerText = `Your bag has ${cartquantity} items.`;
    ">Add to bag</button>

    <button class="wish-button" onclick="alert('Item has been added to wishlist')">❤️ Wishlist</button>

    <button class="bag-button" onclick="alert('Item has been added to bag')">Add 1+1 sale item</button>

    <script>
        let cartquantity = 5; // Initial cart value
        document.querySelector('#cart-summary').innerText = `Your bag has ${cartquantity} items.`;
    </script>
</body>
</html>
