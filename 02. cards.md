```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cards with HTML & CSS</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f2f2f2;
        }

        .container {
            max-width: 1200px;
            margin: 50px auto;
            padding: 0 20px;
        }

        .card-container {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
        }

        .card {
            background-color: white;
            border: 1px solid #ddd;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            padding: 20px;
            text-align: center;
            position: relative;
            min-height: 250px;
        }

        .card img {
            width: 100px;
            height: 100px;
            object-fit: cover;
            margin-bottom: 15px;
            border-radius: 4px;
        }

        .card h5 {
            margin: 10px 0;
            font-size: 18px;
            color: #333;
        }

        .card p {
            font-size: 14px;
            color: #666;
            margin-bottom: 40px;
        }

        .btn {
            display: inline-block;
            padding: 8px 16px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 4px;
            text-decoration: none;
            font-size: 14px;
            cursor: pointer;
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
        }

        .btn:hover {
            background-color: #0056b3;
        }

        @media (max-width: 768px) {
            .card-container {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 480px) {
            .card-container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="card-container">
            <!-- Card 1 -->
            <div class="card">
                <img src="./images/1.jpg" alt="Card Image">
                <h5>Card Title 1</h5>
                <p>This is a simple card with an image, title, and text.</p>
                <a href="#" class="btn">Go somewhere</a>
            </div>
            <!-- Card 2 -->
            <div class="card">
                <img src="./images/2.jpg" alt="Card Image">
                <h5>Card Title 2</h5>
                <p>This is another example of a simple card layout.</p>
                <a href="#" class="btn">Learn more</a>
            </div>
            <!-- Card 3 -->
            <div class="card">
                <img src="./images/3.jpg" alt="Card Image">
                <h5>Card Title 3</h5>
                <p>A simple and responsive card using HTML and CSS.</p>
                <a href="#" class="btn">Check out</a>
            </div>
            <!-- Card 4 -->
            <div class="card">
                <img src="./images/4.jpg" alt="Card Image">
                <h5>Card Title 4</h5>
                <p>This is the fourth card in the container.
                </p>
                <a href="#" class="btn">Read more</a>
            </div>


            <!-- Card 5 -->
            <div class="card">
                <img src="./images/5.jpg" alt="Card Image">
                <h5>Card Title 5</h5>
                <p>This card will start a new row below the first four cards.</p>
                <a href="#" class="btn">Discover</a>
            </div>

            <div class="card">
                <img src="./images/4.jpg" alt="Card Image">
                <h5>Card Title 4</h5>
                <p>This is the fourth card in the container.</p>
                <a href="#" class="btn">Read more</a>
            </div>

        </div>
    </div>
</body>

</html>
```
