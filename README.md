<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript Counter Example</title>
</head>
<body>
    <h2>Kādas ir iespējas ar JavaScript?</h2>

    <p>JavaScript var mainīt atribūtu vērtības HTML.</p>  
    <p>Šajā gadījumā JavaScript maina attēla atribūtu src (avota) vērtību zīmējumā.</p>

    <button onclick="like()">Man patīk</button>
    <img id="myImage" src="dislike.png" style="width:100px">
    
    <button onclick="dislike()">Man nepatīk</button>
    <h3 id="counter">Saskaitītājs: 0</h3>

    <script>
        let count = 0;

        function like() {
            document.getElementById('myImage').src = 'like.png';
            count++;
            updateCounter();
        }

        function dislike() {
            document.getElementById('myImage').src = 'dislike.png';
            count++;
            updateCounter();
        }

        function updateCounter() {
            document.getElementById('counter').innerText = "Saskaitītājs: " + count;
        }
    </script>
</body>
</html>


