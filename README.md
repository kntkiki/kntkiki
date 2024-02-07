<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fortune Teller</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            padding: 2rem;
            text-align: center;
        }

        h1 {
            color: #446688;
            margin-bottom: 2rem;
        }

        .fortune-teller {
            background-color: #ffffff;
            border: 1px solid #cccccc;
            padding: 2rem;
            display: inline-block;
        }

        .flap {
            display: none;
        }
    </style>
</head>
<body>
    <div class="fortune-teller">
        <h1>SEE UR FORTUNE</h1>
        <p class="flap">Your Fortune is 1</p>
         <p class="flap">Your Fortune is 2</p>
         <p class="flap">Your Fortune is 3</p>
          <p class="flap">Your Fortune is 4</p>
           <p class="flap">Your Fortune is 5</p>
            <p class="flap">Your Fortune is 6</p>
             <p class="flap">Your Fortune is 7</p>
              <p class="flap">Your Fortune is 8</p>
               <p class="flap">Your Fortune is 9</p>
                <p class="flap">Your Fortune is 10</p>
                <p class="flap">Your Fortune is 12</p>
         <p class="flap">Your Fortune is 12</p>
         <p class="flap">Your Fortune is 13</p>
          <p class="flap">Your Fortune is 14</p>
           <p class="flap">Your Fortune is 15</p>
            <p class="flap">Your Fortune is 16</p>
             <p class="flap">Your Fortune is 17</p>
              <p class="flap">Your Fortune is 18</p>
               <p class="flap">Your Fortune is 19</p>
                <p class="flap">Your Fortune is 20</p>
             
    </div>

    <script>
        // JavaScript to switch between fortunes randomly
        function switchFortune() {
            const flaps = document.querySelectorAll('.flap');
            const randomIndex = Math.floor(Math.random() * flaps.length);

            for (const flap of flaps) {
                flap.style.display = 'none';
            }
            flaps[randomIndex].style.display = 'block';
        }

        window.onload = switchFortune;
    </script>
</body>
</html>  
