layout: page
title: "Password generator"
permalink: /password


<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <title>Mitch Pearce</title>
    <meta name="description" content="">
    <meta name="author" content="Mitch Pearce">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <link rel="stylesheet" href="css/normalize.css">
    <link rel="stylesheet" href="css/skeletal.css">
    <link rel="stylesheet" href="css/style.css">
    <link rel="icon" type="image/png" href="images/favicon.png">
</head>



<body class="code-snippets-visible">
    <div class="container">
        <!-- HERO -->
        <section class="u-center" id="about">

            <h1 style="font-size:4rem;margin-bottom:1rem;margin-top:10px;">Password generator</h1>

        </section>


        <div class="u-center">
          <!-- <h4>Password generator</h4> -->
          
          <!-- <input type="text"> -->

          <div class="pass" id="password-gen" style="margin:0 auto;">

            <br>
        </div>

      <button class="click" onclick="genPass(18)">Generate</button><br>

    </div>




    <style>
        .pass {
          height: fit-content;
          /* padding: 4px, 0; */
          width: 40rem;
          /* background-color: rgb(121, 121, 121); */
          /* background-color: rgb(121, 121, 121); */
        }
      </style>

      <script>
  
        function genPass(len) {
          var length = len + 6,
            charset = "abcdefghijklmnopqrstuvwxyz.,/@~#;:<>?!%$£ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789",
            res = "";
          for (var i = 0, n = charset.length; i < length; ++i) {
            res += charset.charAt(Math.floor(Math.random() * n));
          }
          document.getElementById("password-gen").innerHTML = res
        }
      </script>


</body>

</html>