<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>create love calculater</title>
    <style>
        * {
            margin: 0px;
            padding: 0px;
            box-sizing: border-box;
            font-size: 18px;
            text-align: center;
        }

        body {
            background-image: linear-gradient(rgba(184, 130, 130, .07), rgba(11, 235, 104, 0.07)), url(p2.jpg);
            background-size: cover;

        }

        .container {
            width: 50%;
            height: 270px;
            margin: auto;
            margin-top: 100px;
            text-align: center;

            background-color: rgb(0, 128, 90);
        }

        .card1 {
            background-color: grey;
            height: 40px;
            line-height: 40px;
        }

        .love {
            margin-top: 30px;

        }

        button {
            margin-top: 20px;
            font-size: 20px;
        }

        .percentage {

            margin-top: 20px;


        }

        .footer {
            margin-top: 50px;
            background-color: grey;
            height: 40px;
            line-height: 40px;
        }
        @media screen  and (min-width: 818px)and (max-width: 914px) {
            .container {
                display:block;
                height: 320px;
                   }
                   .love{
                       width: 50%;
                     margin-left: 95px;

                   }
        }
        @media screen and (min-width:459px ) and (max-width: 818px) {
            .container {
                display:block;
                height: 350px;
                   }
                   .love{
                       width: 60%;
                     /* margin: auto; */

                   }
                   .footer{
                       background-color: grey;
                       height: 70px;
                   }
        }
        @media screen   and  (max-width: 400px) {
            .container {
                display:block;
                height: 320px;
                width: 80%;

                   }
                   .love{
                     height: 70px;
                   }
                   .love input{
                       height: 20px;
                       margin: 10px auto;
                   }

                   .footer{
                       background-color: grey;
                       height: 70px;
                   }


        }
    </style>

</head>

<body>
    <div class="container">
        <div class="card1">LOVE CALCULATER</div>
        <div class="love">
            <input type="text"  id="boylover" placeholder="enter your name" value="">
            <span>+</span>
            <input type="text" id="girllover" placeholder="who your lover" value="">
        </div>
        <button class="btn" onclick="lover()">click here</button><br>
        <div class="percentage">

            <input id="lover" placeholder="love percentage" value="">
        </div>
        <div class="footer">IT IS TOO GOOD LOVER CALCULATER FOR YOU </div>
    </div>
    </div>

</body>
<script>
    function lover() {
        var boy = document.getElementById('boylover').value;
        var girl = document.getElementById('girllover').value;

        if (boy == "") {
            alert("please fill your name");
        }
        else if (boy.length <= 3) {
            alert("your name more the 3 characters");
        }
        else if (!isNaN(boy)) {
            alert("please entre only characters");

        }
        if (girl == "") {
            alert("please fill your lover name");
        }
        else if (girl.length <= 3) {
            alert("your lover name  more the 3 characters");
        }
        else if (!isNaN(girl)) {
            alert("please entre only characters");

        }
        else {

            var lovedata = Math.random() * 100;
            lovedata = Math.floor(lovedata);
            document.getElementById('lover').value = lovedata + "%";
        }



    }
</script>

</html> 
