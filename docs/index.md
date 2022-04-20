<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home</title>

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Alumni+Sans+Inline+One&family=Inspiration&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Orelega+One&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Lalezar&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Concert+One&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Concert+One&family=Roboto+Slab&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="css/style.css">
</head>

<body>
    <header>

        <nav id="navbar">
            <div id="logo">
                <img src="img/logo.jpeg" alt="logo">
                <h2 class="name">Cubicles</h2>
            </div>
            <ul>
                <li class="class"><a target="/blank" href="index.html">Home</a></li>
                <li class="class"><a target="/blank" href="career.html">Career</a></li>
                <li class="class"><a target="/blank" href="contact.html">Contact Us</a></li>
                <li class="class" id="hehehe"><a target="/blank" href="aboutus.html">About Us</a></li>
            </ul>

            <div class="searchbox">
                <form>
                    <input type="search" placeholder="Search...">
                    <button type="submit">Search</button>
                </form>
            </div>

        </nav>



    </header>

    <div class="Ach">
        <h2> <span style="font-weight: bold;
  font-size: 55px; position :absolute; top:180px;left:555px; text-align: center;">Achievments</span></h2>
    </div>
    <section>

        <div class="container centre">
            <div class="display-container mySlides">
                <img src="img/img1.png" style="width:100%"> im g/ </div>
            <div class="display-container mySlides">
                <img src="img/img2.png" style="width:100%">

            </div>
            <div class="display-container mySlides">
                <img src="img/img3.png" style="width:100%">

            </div>
            <!--  -->
            <!-- Slideshow next/previous buttons -->
            <div class="section">

                <div class="container dark-grey padding xlarge ">
                    <div class="item" id="item-1">
                        <div class="left" onclick="plusDivs(-1)"><i class="fa fa-chevron-left hover-text-teal"></i></div>
                    </div>
                    <div class="item" id="item-3">
                        <div class="right" onclick="plusDivs(1)"><i class="fa fa-chevron-right hover-text-teal"></i></div>
                    </div>

                    <div class="item" id="item-2">
                        <div class="center">
                            <span class="tag demodots border transparent hover-white" onclick="currentDiv(1)"></span>
                            <span class="tag demodots border transparent hover-white" onclick="currentDiv(2)"></span>
                            <span class="tag demodots border transparent hover-white" onclick="currentDiv(3)"></span>
                        </div>
                    </div>


                </div>
            </div>


    </section>
    <div class="row container">
        <div class="center padding-64 Ach " id="wwo">
            <h2 style="font-weight: bold; font-size:50px;">
                <span class="large bottombar border-dark-grey padding-16 ">What We Offer..</span>
            </h2>
        </div>
        <!-- Article -->
        <section id="article">
            <div class="feature fpallete" id="a1">
                <div>
                    <h1>Branding</h2>
                </div>
                <p>To compete in the sea of social media you need powerful and distinct branding.Our company masters in taking your brand value to new heights,ensuring an exponential growth</p>
            </div>
            <div class="feature fpallete" id="a2">
                <h1>Design</h1>
                <p>Design is not just what it looks like and feels like. Design is how it works.<br> So our great emhasis on designing is at the core of our marketing strategy</p>
            </div>
            <div class="feature fpallete" id="a3">
                <h1>Consultation</h1>
                <p> We rely on both creative thinking and practical, results-driven analysis.We are willing to work collaboratively to achieve the best possible results. </p>
            </div>
            <div class="feature fpallete" id="a4">
                <h1>Promises</h1>
                <p>Our relatioships with our clients is the driving force behind our continous pesistance.The level of comfort with our partners and fulfillment of our promises is the direct outcome of their faith in us.</p>
            </div>
        </section>

</body>
<script>
    // Slideshow
    var slideIndex = 1;
    showDivs(slideIndex);

    function plusDivs(n) {
        showDivs(slideIndex += n);
    }

    function currentDiv(n) {
        showDivs(slideIndex = n);
    }

    function showDivs(n) {
        var i;
        var x = document.getElementsByClassName("mySlides");
        var dots = document.getElementsByClassName("demodots");
        if (n > x.length) {
            slideIndex = 1
        }
        if (n < 1) {
            slideIndex = x.length
        };
        for (i = 0; i < x.length; i++) {
            x[i].style.display = "none";
        }
        for (i = 0; i < dots.length; i++) {
            dots[i].className = dots[i].className.replace(" white", "");
        }
        x[slideIndex - 1].style.display = "block";
        dots[slideIndex - 1].className += " white";
    }
</script>

</html>
