<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<style>

.month {
  padding: 70px 25px;
  width: 100%;
  background: #43cfec;
  text-align: center;
}

.month ul {
  margin: 0;
  padding: 0;
}

.month ul li {
  color: white;
  font-size: 20px;
  text-transform: uppercase;
  letter-spacing: 3px;
}

.month .prev {
  float: left;
  padding-top: 10px;
}

.month .next {
  float: right;
  padding-top: 10px;
}

.weekdays {
  margin: 0;
  padding: 10px 0;
  background-color: #ddd;
}

.weekdays li {
  display: inline-block;
  width: 13.6%;
  color: #666;
  text-align: center;
}

.days {
  padding: 10px 0;
  background: #eee;
  margin: 0;
}

.days li {
  list-style-type: none;
  display: inline-block;
  width: 13.6%;
  text-align: center;
  margin-bottom: 5px;
  font-size:12px;
  color: #777;
}

.days li .active {
  padding: 5px;
  background: #1abc9c;
  color: white !important
}

/* Add media queries for smaller screens */
@media screen and (max-width:720px) {
  .weekdays li, .days li {width: 13.1%;}
}

@media screen and (max-width: 420px) {
  .weekdays li, .days li {width: 12.5%;}
  .days li .active {padding: 2px;}
}

@media screen and (max-width: 290px) {
  .weekdays li, .days li {width: 12.2%;}
}
body {
  font-family: Arial, Helvetica, sans-serif;
}

.navbar {
  overflow: hidden;
  background-color: #333;
}

.navbar a {
  float: left;
  font-size: 16px;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

.dropdown {
  float: left;
  overflow: hidden;
}

.dropdown .dropbtn {
  font-size: 16px;  
  border: none;
  outline: none;
  color: white;
  padding: 14px 16px;
  background-color: inherit;
  font-family: inherit;
  margin: 0;
}

.navbar a:hover, .dropdown:hover .dropbtn {
  background-color: red;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  float: none;
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {
  background-color: #ddd;
}

.dropdown:hover .dropdown-content {
  display: block;
}

.trailer {
  float: right;
}
* {box-sizing: border-box;}
body {font-family: Verdana, sans-serif;}
.mySlides {display: none;}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

.caption-container {
  text-align: center;
  background-color: #222;
  padding: 2px 16px;
  color: white;
}

.prev,
.next {
  cursor: pointer;
  position: absolute;
  top: 40%;
  width: auto;
  padding: 16px;
  margin-top: -50px;
  color: white;
  font-weight: bold;
  font-size: 20px;
  border-radius: 0 3px 3px 0;
  user-select: none;
  -webkit-user-select: none;
}

.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

.active {
  background-color: #717171;
}

.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@media only screen and (max-width: 300px) {
  .text {font-size: 11px}
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

.column {
  float: left;
  width: 33.33%;
}
/* Add a transparency effect for thumbnail images */
.demo {
  opacity: 0.6;
}

.active,
.demo:hover {
  opacity: 1;
}
</style>
</head>
<body>

<div class="navbar">
  <a href="https://mypages.valdosta.edu/thbeheler/FinalProject/HTML/index.html">Home</a>
  <div class="dropdown">
    <button class="dropbtn">About
      <i class="fa fa-caret-down"></i>
    </button>
    <div class="dropdown-content">
      <a href="https://mypages.valdosta.edu/thbeheler/FinalProject/HTML/history.html">History</a>
      <a href="https://mypages.valdosta.edu/thbeheler/FinalProject/HTML/MeettheCast.html">Meet the Cast</a>
      <a href="https://mypages.valdosta.edu/thbeheler/FinalProject/HTML/gallery.html">Gallery</a>
    </div>
  </div>
  <a href="https://mypages.valdosta.edu/thbeheler/FinalProject/HTML/ContactUs.html">Contact Us</a>
    <div class="dropdown">
    <button class="dropbtn">Group Events
      <i class="fa fa-caret-down"></i>
    </button>
    <div class="dropdown-content">
      <a href="https://mypages.valdosta.edu/thbeheler/FinalProject/HTML/PrivateEvents.html">Private Events</a>
      <a href="https://mypages.valdosta.edu/thbeheler/FinalProject/HTML/Workshops.html">Workshops</a>
    </div>
  </div>
</div>

<div class="heading">
<h2 style="text-align:center;">District Comedy</h2>
</div>

<div class="slideshow-container">

<div class="container">
  <div class="mySlides">
    <div class="numbertext">1 / 3</div>
    <img src="../images/phantom.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">2 / 3</div>
    <img src="../images/peterpan.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">3 / 3</div>
    <img src="../images/thetrial.jpg" style="width:100%">
  </div>
<a class="prev" onclick="plusSlides(-1)">❮</a>
  <a class="next" onclick="plusSlides(1)">❯</a>

  <div class="caption-container">
    <p id="caption"></p>
  </div>

  <div class="row">
    <div class="column">
      <img class="demo cursor" src="../images/phantom.jpg" style="width:100%" onclick="currentSlide(1)" alt="The Woods">
    </div>
    <div class="column">
      <img class="demo cursor" src="../images/peterpan.jpg" style="width:100%" onclick="currentSlide(2)" alt="Cinque Terre">
    </div>
    <div class="column">
      <img class="demo cursor" src="../images/thetrial.jpg" style="width:100%" onclick="currentSlide(3)" alt="Mountains and fjords">
    </div>
  </div>
</div>
<br>

<div style="text-align:center">
  <span class="dot"></span> 
  <span class="dot"></span> 
  <span class="dot"></span> 
</div>


<script>
var slideIndex = 0;
showSlides();

function showSlides() {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("column");
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  slideIndex++;
  if (slideIndex > slides.length) {slideIndex = 1}    
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " active";
  setTimeout(showSlides, 3000); // Change image every 3 seconds
}
</script>

<header>


<div class="trailer">
<iframe width="560" height="315" src="https://www.youtube.com/embed/-K3MzE1UsQI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<h2>Hello! District Comedy is Northern Virginia's premier destination for longform improv. Our mission is to unleash the creative power of improv in Washington, DC. We engage audiences with performances that exhilarate and inspire. We ignite the spirit of play in Washington with a revolutionary training program. We create a home for improv, connected to the life of the city.</h2>

<script type="text/javascript" src="//lgapi-us.libapps.com/web/jquery/js/1.12.1_jquery.min.js"></script>
    <script src="//code.jquery.com/ui/1.12.1/jquery-ui.min.js"></script>
    <script>
        1 || document.write('<script src="//lgapi-us.libapps.com/web/jquery/js/jquery-ui.min.js?2695">\x3C/script>');
    </script>
<script type="text/javascript" src="//lgapi-us.libapps.com/web/bootstrap/3.4.1/js/bootstrap.min.js"></script>
<script type="text/javascript" src="//lgapi-us.libapps.com/web/js1.36.7/springshare.public.min.js"></script>
<script type="text/javascript" src="//lgapi-us.libapps.com/web/js1.36.7/springshare.common.min.js"></script>
<script type="text/javascript" src="//lgapi-us.libapps.com/web/js1.36.7/common/springspace_sui_helptip.js"></script>
<link rel="stylesheet" href="//lgapi-us.libapps.com/web/jquery/css/jquery-ui.min.css?2695" />
<link rel="stylesheet" href="//lgapi-us.libapps.com/web/bootstrap/3.4.1/css/bootstrap.min.css" />
<link rel="stylesheet" href="//lgapi-us.libapps.com/web/css1.36.7/springshare.public.min.css" />
<link rel="stylesheet" href="//lgapi-us.libapps.com/web/css1.36.7/springshare.common.min.css" />
<link href="//lgapi-us.libapps.com/web/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
<link href="//lgapi-us.libapps.com/web/css1.36.7/common/springspace_sui_helptip.css" rel="stylesheet">
<script>
var springStats = springStats || {};
springStats.saConfig = springStats.saConfig || {
    site_id: 15762,
    tracking_parameters: {"_st_site_id":15762},
    tracking_server_host: "libguides-proc.springyaws.com"
};
</script>
<script async  src="//lgapi-us.libapps.com/web/js/sa.min.js?3116"></script>
<script>
    springSpace.Common = springSpace.Common || { };
    springSpace.Common.constant = { PROCESSING: { ACTION_DISPLAY_POLL: 159 }};
    springSpace.Common.baseURL = "//lgapi-us.libapps.com'/";
    springSpace.Common.apiLoad = true;
</script><script>
springshare_widget_config_1586187951653 = { path: 'boxes/23569724' };
</script>
<div id="s-lg-widget-1586187951653"></div>
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://lgapi-us.libapps.com/widgets.php?site_id=15762&widget_type=8&output_format=1&widget_title=General&widget_height=250&widget_width=100%25&widget_embed_type=1&guide_id=1025246&box_id=23569724&map_id=27654619&content_only=0&config_id=1586187951653";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","s-lg-widget-script-1586187951653");</script>

<div class="heading">
<h1>Upcoming Shows</h1>

<div class="month">      
  <ul>
    <li class="prev">&#10094;</li>
    <li class="next">&#10095;</li>
    <li>
      July<br>
      <span style="font-size:18px">2020</span>
    </li>
  </ul>
</div>

<ul class="weekdays">
  <li>Mo</li>
  <li>Tu</li>
  <li>We</li>
  <li>Th</li>
  <li>Fr</li>
  <li>Sa</li>
  <li>Su</li>
</ul>

<ul class="days">  
  <li>1</li>
  <li>2</li>
  <li>3</li>
  <li>4</li>
  <li>5</li>
  <li>6</li>
  <li>7</li>
  <li>8</li>
  <li><a href="https://www.eventbrite.com/manage/events">9</a></li>
  <li>10</li>
  <li>11</li>
  <li>12</li>
  <li>13</li>
  <li>14</li>
  <li>15</li>
  <li>16</li>
  <li>17</li>
  <li>18</li>
  <li>19</li>
  <li>20</li>
  <li>21</li>
  <li>22</li>
  <li>23</li>
  <li>24</li>
  <li>25</li>
  <li>26</li>
  <li>27</li>
  <li>28</li>
  <li>29</li>
  <li>30</li>
  <li>31</li>
</ul>
<h2>To subscribe our news letter, please fill out the form and submit by clicking the submission button. </h2>
 <h3>Tell us a bit about yourself:</h3> 
<form method=“post” action=“hello.php”>
<label for "firstname">First Name:</label>
<input type="text"id="firstname" name="firstname" size"32"/><br/>
<label for "lastname">Last Name:</label>
<input type="text"id="lastname" name="lastname" size"32"/><br/>
<label for "email">Email:</label>
<input type="text"id="email" name="email" size"32"/><br/>
<label for "age">Age:</label>
<input type="text"id="age" name="age" size"32"/><br/>
<input type="submit" value=Submit" name="submit"/>

</form>

</body>
</html>
