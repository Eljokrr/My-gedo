<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>متجر الأناقة</title>
    <style>
        body {
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 20px;
        }
        h1 { font-size: 2rem; }
        .products { display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; }
        .product {
            background: #222;
            padding: 10px;
            border-radius: 10px;
            width: 150px;
            transition: transform 0.3s;
        }
        .product img { width: 100%; border-radius: 10px; }
        .product:hover { transform: scale(1.1); }
    </style>
</head>
<body>

    <h1>🛍️ متجر الأناقة</h1>
    <p>تسوق أحدث صيحات الموضة</p>

    <div class="products">
        <div class="product">
            <img src="https://via.placeholder.com/150" alt="منتج">
            <p>ساعة فاخرة - $199</p>
        </div>
        <div class="product">
            <img src="https://via.placeholder.com/150" alt="منتج">
            <p>حقيبة جلدية - $249</p>
        </div>
        <div class="product">
            <img src="https://via.placeholder.com/150" alt="منتج">
            <p>حذاء رياضي - $179</p>
        </div>
    </div>

</body>
</html>
