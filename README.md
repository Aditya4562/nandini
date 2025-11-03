[index.html](https://github.com/user-attachments/files/23304572/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
    <link href="css/style.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/OwlCarousel2/2.3.4/assets/owl.carousel.min.css" integrity="sha512-tS3S5qG0BlhnQROyJXvNjeEM4UpMXHrQfTGmbQ1gKmelCxlSEBUaxhRBj/EFTzpbP4RVSrpEikbmdJobCvhE3g==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/OwlCarousel2/2.3.4/assets/owl.theme.default.min.css" integrity="sha512-sMXtMNL1zRzolHYKEujM2AqCLUR9F2C4/05cdbxjjLSRvMQIciEPCQZo++nk7go3BtSuK9kfa/s+a4f4i5pLkw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.1/jquery.min.js"></script>
  




  <nav class="navbar navbar-expand-sm navbar-dark bg-dar">
    <div class="container-fluid">
      <div class="nav-logo">[style.css](https://github.com/user-attachments/files/23304577/style.css)html,
body,
div,
span,
applet,[custom.js](https://github.com/user-attachments/files/23304587/custom.js)const slider = document.querySelector('.slider');

function activate(e) {
  const items = document.querySelectorAll('.item');
  e.target.matches('.next') && slider.append(items[0])
  e.target.matches('.prev') && slider.prepend(items[items.length-1]);
}

document.addEventListener('click',activate,false);














// ---------Responsive-navbar-active-animation-----------
function test(){
	var tabsNewAnim = $('#navbarSupportedContent');
	var selectorNewAnim = $('#navbarSupportedContent').find('li').length;
	var activeItemNewAnim = tabsNewAnim.find('.active');
	var activeWidthNewAnimHeight = activeItemNewAnim.innerHeight();
	var activeWidthNewAnimWidth = activeItemNewAnim.innerWidth();
	var itemPosNewAnimTop = activeItemNewAnim.position();
	var itemPosNewAnimLeft = activeItemNewAnim.position();
	$(".hori-selector").css({
		"top":itemPosNewAnimTop.top + "px", 
		"left":itemPosNewAnimLeft.left + "px",
		"height": activeWidthNewAnimHeight + "px",
		"width": activeWidthNewAnimWidth + "px"
	});
	$("#navbarSupportedContent").on("click","li",function(e){
		$('#navbarSupportedContent ul li').removeClass("active");
		$(this).addClass('active');
		var activeWidthNewAnimHeight = $(this).innerHeight();
		var activeWidthNewAnimWidth = $(this).innerWidth();
		var itemPosNewAnimTop = $(this).position();
		var itemPosNewAnimLeft = $(this).position();
		$(".hori-selector").css({
			"top":itemPosNewAnimTop.top + "px", 
			"left":itemPosNewAnimLeft.left + "px",
			"height": activeWidthNewAnimHeight + "px",
			"width": activeWidthNewAnimWidth + "px"
		});
	});
}
$(document).ready(function(){
	setTimeout(function(){ test(); });
});
$(window).on('resize', function(){
	setTimeout(function(){ test(); }, 500);
});
$(".navbar-toggler").click(function(){
	$(".navbar-collapse").slideToggle(300);
	setTimeout(function(){ test(); });
});



// --------------add active class-on another-page move----------
jQuery(document).ready(function($){
	// Get current path and find target link
	var path = window.location.pathname.split("/").pop();

	// Account for home page with empty path
	if ( path == '' ) {
		path = 'index.html';
	}

	var target = $('#navbarSupportedContent ul li a[href="'+path+'"]');
	// Add active class to target link
	target.parent().addClass('active');
});




// Add active class on another page linked
// ==========================================
// $(window).on('load',function () {
//     var current = location.pathname;
//     console.log(current);
//     $('#navbarSupportedContent ul li a').each(function(){
//         var $this = $(this);
//         // if the current path is like this link, make it active
//         if($this.attr('href').indexOf(current) !== -1){
//             $this.parent().addClass('active');
//             $this.parents('.menu-submenu').addClass('show-dropdown');
//             $this.parents('.menu-submenu').parent().addClass('active');
//         }else{
//             $this.parent().removeClass('active');
//         }
//     })
// });












function prev() {
	document.getElementById("slider-container").scrollLeft -= 270;
}

function next() {
	document.getElementById("slider-container").scrollLeft += 270;
}

$(".slide img").on("click", function () {
	$(this).toggleClass("zoomed");
	$(".overlay").toggleClass("active");
});







object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,tar
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: Oxanium;
  vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}
body {
  line-height: 1;
  background-color: #F3E7D6;
}
ol,
ul {
  list-style: none;
}
blockquote,
q {
  quotes: none;
}
blockquote:before,
blockquote:after,
q:before,
q:after {
  content: "";
  content: none;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}

/*end of reset css*/

.continer-fluid {
    width: 100%;
    height: auto;
}

.container {
    width: 1600px;
    height: auto;
    margin: 0 auto;
}










.carousel-caption h3{
  font-size: 45px;
  color: #175030;
  text-shadow: 4px 2px #0000002b;
}
.carousel-caption p{
  margin-bottom: 312px;
}






.item {
  width: 200px;
  height: 300px;
  list-style-type: none;
  position: absolute;
  top: 85%;
  transform: translateY(-50%);
  z-index: 1;
  background-position: center;
  background-size: cover;
  border-radius: 20px;
  box-shadow: 0 20px 30px rgba(255,255,255,0.3) inset;
  transition: transform 0.1s, left 0.75s, top 0.75s, width 0.75s, height 0.75s;

  &:nth-child(1), &:nth-child(2) {
    left: 0;
    top: 182px;
    width: 100%;
    height: 100%;
    transform: none;
    border-radius: 0;
    box-shadow: none;
    opacity: 1;
  }

  &:nth-child(3) { left: 50%; }
  &:nth-child(4) { left: calc(50% + 220px); }
  &:nth-child(5) { left: calc(50% + 440px); }
  &:nth-child(6) { left: calc(50% + 660px); opacity: 0; }
}

.bg-dar {
    --bs-bg-opacity: 1;
    background-color: rgb(255 255 255) !important;
}

.navber-text a{
  color: #000000;
  padding-right: 50px;
}
.navber-text a:hover{
  color: #7FB047;
}
.parformans{
    margin-top: 5%;
}
.imagess-text{
    margin-left: 20px;
}
.imagess-text h5{
  font-size: 60px;
  text-align: right;
  color: #7FB047;
}
.imagess-text-1 {
  margin-left: 20px;
}
.imagess-text-1 h5{
  font-size: 60px;
  text-align: left;
  color: #7FB047;
}
.d-flex a{
  text-decoration: none;
  color: #000000;
  margin-right: 130px;
}

.d-flex a:hover{
  color: #7FB047;
  transition: 0.2s;
}






.title{
  color: #175030;
  font-weight: 700;
  margin-left: 3px;
  font-size: 60px
}




@import url('https://fonts.googleapis.com/css?family=Roboto');

body{
	font-family: 'Roboto', sans-serif;
}
* {
	margin: 0;
	padding: 0;
}
i {
	margin-right: 10px;
}
/*----------bootstrap-navbar-css------------*/
.navbar-logo{
	padding: 15px;
	color: #fff;
}
.navbar-mainbg{
	background-color: #5161ce;
	padding: 0px;
}
#navbarSupportedContent{
	overflow: hidden;
	position: relative;
}
#navbarSupportedContent ul{
	padding: 0px;
	margin: 0px;
}
#navbarSupportedContent ul li a i{
	margin-right: 5.7px;
}
#navbarSupportedContent li {
	list-style-type: none;
	float: left;
  margin-right: 41px;
}
#navbarSupportedContent ul li a{
	color: rgba(255,255,255,0.5);
    text-decoration: none;
    font-size: 15px;
    display: block;
    padding: 20px 32px;
    transition-duration:0.6s;
	transition-timing-function: cubic-bezier(0.68, -0.55, 0.265, 1.55);
    position: relative;
}
#navbarSupportedContent>ul>li.active>a{
	color: #7EC1B2;
	background-color: transparent;
	transition: all 0.7s;
}
#navbarSupportedContent a:not(:only-child):after {
	content: "\f105";
	position: absolute;
	right: 20px;
	top: 10px;
	font-size: 14px;
	font-family: "Font Awesome 5 Free";
	display: inline-block;
	padding-right: 3px;
	vertical-align: middle;
	font-weight: 900;
	transition: 0.5s;
}
#navbarSupportedContent .active>a:not(:only-child):after {
	transform: rotate(90deg);
}
.hori-selector{
	display:inline-block;
	position:absolute;
	height: 100%;
	top: 0px;
	left: 0px;
	transition-duration:0.6s;
	transition-timing-function: cubic-bezier(0.68, -0.55, 0.265, 1.55);
	background-color: #fff;
	border-top-left-radius: 15px;
	border-top-right-radius: 15px;
	margin-top: 10px;
}
.hori-selector .right,
.hori-selector .left{
	position: absolute;
	width: 25px;
	height: 25px;
	background-color: #fff;
	bottom: 10px;
}
.hori-selector .right{
	right: -25px;
}
.hori-selector .left{
	left: -25px;
}
.hori-selector .right:before,
.hori-selector .left:before{
	content: '';
    position: absolute;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background-color: #5161ce;
}
.hori-selector .right:before{
	bottom: 0;
    right: -25px;
    background-color: #7FB047;
}
.hori-selector .left:before{
	bottom: 0;
    left: -25px;
    background-color: #7FB047;
}
.bnn-tex{
      margin-right: 79px;
          margin-bottom: -12px;
}


@media(min-width: 992px){
	.navbar-expand-custom {
	    -ms-flex-flow: row nowrap;
	    flex-flow: row nowrap;
	    -ms-flex-pack: start;
	    justify-content: flex-start;
	}
	.navbar-expand-custom .navbar-nav {
	    -ms-flex-direction: row;
	    flex-direction: row;
	}
	.navbar-expand-custom .navbar-toggler {
	    display: none;
	}
	.navbar-expand-custom .navbar-collapse {
	    display: -ms-flexbox!important;
	    display: flex!important;
	    -ms-flex-preferred-size: auto;
	    flex-basis: auto;
	}
}


@media (max-width: 991px){
	#navbarSupportedContent ul li a{
		padding: 12px 30px;
	}
	.hori-selector{
		margin-top: 0px;
		margin-left: 10px;
		border-radius: 0;
		border-top-left-radius: 25px;
		border-bottom-left-radius: 25px;
	}
	.hori-selector .left,
	.hori-selector .right{
		right: 10px;
	}
	.hori-selector .left{
		top: -25px;
		left: auto;
	}
	.hori-selector .right{
		bottom: -25px;
	}
	.hori-selector .left:before{
		left: -25px;
		top: -25px;
	}
	.hori-selector .right:before{
		bottom: -25px;
		left: -25px;
	}
}
.content h2{
  font-size: 52px;
}







    .link-button {
      display: inline-block;
      background-color: #f38484;
      color: white;
      padding: 12px 24px;
      text-decoration: none;
      font-size: 16px;
      font-weight: bold;
      border-radius: 8px;
      transition: all 0.3s ease;
    }

    .link-button:hover {
      background-color: #ff6767;
      transform: scale(1.05);
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
    }








.fancy-btn {
  position: relative;
  display: inline-block;
  padding: 12px 30px;
  font-size: 16px;
  font-weight: bold;
  color: white;
  background: linear-gradient(45deg, #7FB047, #C9FE8D);
  border: none;
  border-radius: 50px;
  overflow: hidden;
  cursor: pointer;
  transition: all 0.3s ease;
  z-index: 1;
}
.fancy-btn{
  margin-top: 5%;
      margin-left: -2px;
      text-decoration: none;
}
.bnn{
  margin-left: 80%;
  margin-top: 5%;
}
.bnn a{
  text-decoration: none;
  color: #ffffff;
}
.bnn-1 a{
  text-decoration: none;
  color: #ffffff;
}
.fancy-btn::before {
  content: "";
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: rgba(255, 255, 255, 0.2);
  transition: all 0.4s ease;
  z-index: 0;
}

.fancy-btn:hover::before {
  left: 100%;
}

.fancy-btn:hover {
  transform: scale(1.05);
  box-shadow: 0 8px 16px rgba(232, 99, 98, 0.4);
}











@import "https://fonts.googleapis.com/css?family=Open+Sans:800&display=swap";
body {
	width: 100%;
	margin: 0;
	padding: 0;
	font-family: open sans;
	background: #f8f8f8;
}
h3 {
	text-align: center;
	margin: 6% auto;
	font-size: 1.8rem;
	font-weight: 800;
	color: #444;
}
.slider {
	display: flex;
  justify-content: space-evenly;
  margin-left: 86px;
	height: 350px;
	max-height: auto;
	overflow-y: hidden;
	overflow-x: scroll !important;
	padding: 16px;
	transform: scroll(calc(var(--i, 0) / var(--n) * -100%));
	scroll-behavior: smooth;
}
.slider::-webkit-scrollbar {
	height: 5px;
	width: 150px;
	display: none;
}
.slider::-webkit-scrollbar-track {
	background: transparent;
}
.slider::-webkit-scrollbar-thumb {
	background: #888;
}
.slider::-webkit-scrollbar-thumb:hover {
	background: #555;
}
.slider img:hover {
	transform: scale(1.05);
	box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.15);
}
.slide {
	position: relative;
  
}
.sil-tex h2{
  text-align: center;
  font-size: 45px;
  margin-top: 3%;
  margin-bottom: 2%;
   color: #175030;
  font-weight: 700;
}
.si-te a {
      color: #ffffff;
    position: absolute;
    font-weight: 700;
    top: 3%;
    right: 6%;
    font-size: 14px;
    text-decoration: none;
    background-color: #ff8787;
    padding-left: 14px;
    padding-right: 14px;
    border-radius: 30px;
}

.si-te a:hover{
  color: #ff8787;
  background-color: #ffffff;
}
.si-te h2 {
    color: #7FB047;
    position: absolute;
    font-weight: 700;
    top: 68%;
    right: 18%;
    text-shadow: 2px 2px #00000078;
    font-size: 18px;
    text-decoration: none;
}
.si-te p{
color: #ffffff;
    position: absolute;
    top: 79%;
    right: 0%;
    font-size: 10px;
    left: 0%;
    text-align: center;
}



.si-te-2 a {
     color: #7FB047;
    position: absolute;
    font-weight: 700;
    top: 3%;
    right: 6%;
    font-size: 14px;
    text-decoration: none;
    background-color: #ff8787;
    padding-left: 14px;
    padding-right: 14px;
    border-radius: 30px;
}
.si-te-2 a:hover{
  color: #ff8787;
  background-color: #ffffff;
}
.si-te-2 h2{
  color: #7FB047;
    position: absolute;
    top: 68%;
    right: 18%;
    text-shadow: 2px 2px #00000078;
    font-size: 18px;
}
.si-te-2 p{
  color: #ffffff;
    position: absolute;
    top: 79%;
    right: 0%;
    font-size: 10px;
    left: 0%;
    text-align: center;
}




.si-te-3 a {
     color: #ffffff;
    position: absolute;
    font-weight: 700;
    top: 3%;
    right: 6%;
    font-size: 14px;
    text-decoration: none;
    background-color: #ff8787;
    padding-left: 14px;
    padding-right: 14px;
    border-radius: 30px;
}
.si-te-3 a:hover{
  color: #ff8787;
  background-color: #ffffff;
}
.si-te-3 h2{
  color: #7FB047;
    position: absolute;
    top: 68%;
    right: 18%;
    text-shadow: 2px 2px #00000078;
    font-size: 18px;
}
.si-te-3 p{
  color: #ffffff;
    position: absolute;
    top: 79%;
    right: 0%;
    font-size: 10px;
    left: 0%;
    text-align: center;
}




.si-te-4 a {
    color: #ffffff;
    position: absolute;
    font-weight: 700;
    top: 3%;
    right: 6%;
    font-size: 14px;
    text-decoration: none;
    background-color: #ff8787;
    padding-left: 14px;
    padding-right: 14px;
    border-radius: 30px;
  padding-right: 7px;
}
.si-te-4 a:hover{
  color: #ff8787;
  background-color: #ffffff;
}
.si-te-4 h2{
  color: #7FB047;
    position: absolute;
    top: 68%;
    right: 18%;
    text-shadow: 2px 2px #00000078;
    font-size: 18px;
}
.si-te-4 p{
  color: #ffffff;
    position: absolute;
    top: 79%;
    right: 0%;
    font-size: 10px;
    left: 0%;
    text-align: center;
}




.si-te-5 a {
      color: #ffffff;
    position: absolute;
    font-weight: 700;
    top: 3%;
    right: 6%;
    font-size: 14px;
    text-decoration: none;
    background-color: #ff8787;
    padding-left: 14px;
    padding-right: 14px;
    border-radius: 30px;
}
.si-te-5 a:hover{
  color: #ff8787;
  background-color: #ffffff;
}
.si-te-5 h2{
  color: #7FB047;
    position: absolute;
    top: 68%;
    right: 18%;
    text-shadow: 2px 2px #00000078;
    font-size: 18px;
}
.si-te-5 p{
  color: #ffffff;
    position: absolute;
    top: 79%;
    right: 0%;
    font-size: 10px;
    left: 0%;
    text-align: center;
}



.si-te-6 a {
      color: #ffffff;
    position: absolute;
    font-weight: 700;
    top: 3%;
    right: 6%;
    font-size: 14px;
    text-decoration: none;
    background-color: #ff8787;
    padding-left: 14px;
    padding-right: 14px;
    border-radius: 30px;
}
.si-te-6 a:hover{
  background-color: #ffffff;
  color: #ff8787;
  
}
.si-te-6 h2{
  color: #7FB047;
    position: absolute;
    top: 68%;
    right: 18%;
    text-shadow: 2px 2px #00000078;
    font-size: 18px;
}
.si-te-6 p{
  color: #ffffff;
    position: absolute;
    top: 79%;
    right: 0%;
    font-size: 10px;
    left: 0%;
    text-align: center;
}
.slide img {
	height: 800px;
	width: 250px;
  filter: brightness(88%);
	object-fit: cover;
	cursor: pointer;
	transition: 0.25s ease-in-out;
}


.overlay {
	position: absolute;
	height: 100%;
	width: 100%;
	background: rgba(0, 0, 0, 0.45);
	top: 0;
	display: none;
}

@media only screen and (max-width: 420px) {
	.slider {
		padding: 0;
	}
	.slide {
		padding: 16px 10px;
	}
	.slide img {
		margin: 0;
	}
	.control-prev-btn {
		top: 37%;
	}
	.control-next-btn {
		top: 37%;
	}
}

























.content {
  width: min(44vw, 884px);
  position: absolute;
  top: 50%;
  left: 3rem;
  transform: translateY(-50%);
  font: 400 0.85rem helvetica,sans-serif;
  color: white;
  text-shadow: 0 3px 8px rgba(0,0,0,0.5);
  opacity: 0;
  display: none;

  & .title {
    font-family: 'arial-black';
    text-transform: none;
  }

  & .description {
    line-height: 1.7;
    margin: 1rem 0 1.5rem;
    font-size: 0.8rem;
    color: #000;
  }

  & button {
    width: fit-content;
    background-color: rgba(0,0,0,0.1);
    color: white;
    border: 2px solid white;
    border-radius: 0.25rem;
    padding: 0.75rem;
    cursor: pointer;
  }
}

.item:nth-of-type(2) .content {
  display: block;
  animation: show 0.75s ease-in-out 0.3s forwards;
}

@keyframes show {
  0% {
    filter: blur(5px);
    transform: translateY(calc(-50% + 75px));
  }
  100% {
    opacity: 1;
    filter: blur(0);
  }
}

.nav {
  position: absolute;
  bottom: -7rem;
  left: 50%;
  transform: translateX(-50%);
  z-index: 5;
  user-select: none;

  & .btn {
    background-color: rgba(255,255,255,0.5);
    color: rgba(0,0,0,0.7);
    border: 2px solid rgba(0,0,0,0.6);
    margin: 0 0.25rem;
    padding: 0.75rem;
    border-radius: 50%;
    cursor: pointer;

    &:hover {
      background-color: rgba(255,255,255,0.3);
    }
  }
}

@media (width > 650px) and (width < 900px) {
  .content {
    & .title        { font-size: 1rem; }
    & .description  { font-size: 0.7rem; }
    & button        { font-size: 0.7rem; }
  }
  .item {
    width: 160px;
    height: 270px;

    &:nth-child(3) { left: 50%; }
    &:nth-child(4) { left: calc(50% + 170px); }
    &:nth-child(5) { left: calc(50% + 340px); }
    &:nth-child(6) { left: calc(50% + 510px); opacity: 0; }
  }
}

@media (width < 650px) {
  .content {
    & .title        { font-size: 0.9rem; }
    & .description  { font-size: 0.65rem; }
    & button        { font-size: 0.7rem; }
  }
  .item {
    width: 130px;
    height: 220px;

    &:nth-child(3) { left: 50%; }
    &:nth-child(4) { left: calc(50% + 140px); }
    &:nth-child(5) { left: calc(50% + 280px); }
    &:nth-child(6) { left: calc(50% + 420px); opacity: 0; }
  }
}











body {
	color: #333;
	font-family: 'Open Sans', sans-serif;
	font-weight: 300;
}
h1,
h1+p {
	margin: 30px 15px 0;
	font-weight: 300;
}
h1+p a {
	color: #333;
}
h1+p a:hover {
	text-decoration: none;
}
h2 {
	margin: 60px 15px 0;
	padding: 0;
	font-weight: 300;
}
h2 span {
	margin-left: 1em;
	color: #aaa;
	font-size: 85%;
}
.column {
	margin: 15px 15px 0;
	padding: 0;
}

.column::after {
	content: '';
	clear: both;
	display: block;
}

.column div:first-child {
	margin-left: 0;
}
.column div span {
	position: absolute;
	bottom: -20px;
	left: 0;
	z-index: -1;
	display: block;
	width: 300px;
	margin: 0;
	padding: 0;
	color: #444;
	font-size: 18px;
	text-decoration: none;
	text-align: center;
	-webkit-transition: .3s ease-in-out;
	transition: .3s ease-in-out;
	opacity: 0;
}
.imagess img{
    width: 500px;
    height: 519px;
}
figure:hover+span {
	bottom: -36px;
	opacity: 1;
}
/* Sepia 
.hover09 figure img {
	-webkit-filter: sepia(100%);
	filter: sepia(100%);
	-webkit-transition: .3s ease-in-out;
	transition: .3s ease-in-out;
}*/
.hover09 figure:hover img {
	-webkit-filter: sepia(0);
	filter: sepia(0);
}
.i-t-p{
    display: flex;
    justify-content: space-between;
}
.img-tet{
  
  display: flex
}
.img-tet img{
  margin-right: 46px;
}























.white-button {
      background-color: white;
      color: #E86362;
      border: 2px solid #E86362;
      padding: 12px 24px;
      font-size: 16px;
      font-weight: bold;
      border-radius: 8px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .white-button:hover {
      background-color: #E86362;
      color: white;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
    }








.fixed-bg {
  background-image: url("../Images/banner-2.jpeg");
  min-height: 625px;
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
      margin-top: 3%;
    margin-bottom: 3%;
}
.review h1{
  font-size: 45px;
  text-align: center;
  margin-top: 3%;
  color: #175030;
  font-weight: 700;
}
.reviwe-img{
  display: flex;
  height: 50px;
}
.reviwe-text h1{
  color: #000000;
  font-size: 24px;
}
.reviwe-ster img{
  padding-left: 58px;
    height: 18px;
    margin-top: -32px;
}
.rev-p p{
  font-size: 16spx;
}
.rev-BG{
  background-image: url(../Images/Rectangle\ 28.png);
  
      width: 540px;
    height: 511px;
}
.rev-M{
  padding-left: 33px;
    padding-right: 33px;
    padding-top: 105px;
}
.rev-all{
  padding-top: 61px;
}
.revi-dis{
  display: flex;
  justify-content: space-between;
}










.off-bg{
  background-image: url(../Images/30%\ off.png);
    height: 593px;
    width: 1905px;
}

.off-text h2{
  font-size: 55px;
  color: #ffffff;
  font-weight: 700;
  padding-top: 7%;
}
.off-text p{
  color: #ffffff;
  margin-top: 2%;
}









.last-one{
  background-image: url(../Images/footer-bg.png);
  margin-top: 3%;
}
.last-logo a img{
  padding-top: 3%;
  margin-bottom: -60px;
}
.last-pa p{
  font-size: 15px;
  color: #939393;
  line-height: 1.61;
  margin-top: -223px;
}
.last-tex h1{
  color: #7FB047;
  font-size: 20px;
  font-weight: 700;
  
}
.last-tex a:hover{
  color: #7FB047;
  border-bottom: 2px solid #7FB047;
  transition: 0.2s;
}
.last-but-1 ul li a{
  color: #707070ad;
  text-decoration: none;
  font-size: 16px;
  padding-top: 15px;
  line-height: 2.61;
  margin-left: -17px;
}
.last-but-2 ul li a{
  color: #707070ad;
  text-decoration: none;
  font-size: 16px;
  padding-top: 15px;
  line-height: 2.61;
  margin-left: -17px;
}
.last-but-3 ul li a{
  color: #707070ad;
  text-decoration: none;
  font-size: 16px;
  padding-top: 15px;
  line-height: 2.61;
  margin-left: -17px;
}
.last-tex{
  display: flex;
  justify-content: space-evenly;
  padding-left: 34%;
}
.last-img a img{
  width: 170px;
  position: relative;
  bottom: 39px;
  margin-bottom: -7%;
}

.network h1{
  color: #ffffff;
  font-size: 30px;
  margin-top: 7%;
}
.network a img{
  width: 170px;
  margin-top: 2%;
}
.copyright a{
  text-decoration: none;
  color: #ffffff;
  margin-left: 41%;
}
.copyright{
  border-top: solid 2px #ffffff99;
  margin-top: 6%;
  line-height: 5.2;
}

      <a class="navbar-brand" href="javascript:void(0)">
        <img src="Images/logo-4.png" style="width: 205px; margin-left: 86px;"></a></div>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#mynavbar">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navber-text" id="mynavbar">
        <ul class="navbar-nav me-auto">
          <li class="nav-item">
            <a class="nav-link" href="javascript:void(0)" style="padding-right: 70px;">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="javascript:void(0)" style="padding-right: 70px;">Pages</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="javascript:void(0)" style="padding-right: 70px;">Contact</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="javascript:void(0)" style="padding-right: 70px;">Book Appointment</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="javascript:void(0)" style="padding-right: 70px;">About us</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="javascript:void(0)" style="padding-right: 70px;">More</a>
          </li>
        </ul></div>
        <form class="d-flex">
         <a href="https://thriving-daffodil-fc5523.netlify.app/">Login / Registasoin</a>
        </form>
      
    </div>
  </nav>
  










<nav class="navbar navbar-expand-custom navbar-mainbg" style="background-color: #7FB047;">
        <a class="navbar-brand navbar-logo" href="#"></a>
        <button class="navbar-toggler" type="button" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <i class="fas fa-bars text-white"></i>
        </button>
        <div class="bnn-tex">
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ml-auto" style="margin-right: 360px;">
                <div class="hori-selector"><div class="left"></div><div class="right"></div></div>
                <li class="nav-item">
                    <a class="nav-lin" href="javascript:void(0);"><i class="fas fa-tachometer-alt"></i>Healthy Straegy</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-lin" href="javascript:void(0);"><i class="far fa-address-book"></i>Nutritional Levels</a>
                </li>
                <li class="nav-item">
                    <a class="nav-lin" href="javascript:void(0);"><i class="far fa-clone"></i>Healthy Diet</a>
                </li>
                <li class="nav-item">
                    <a class="nav-lin" href="javascript:void(0);"><i class="far fa-calendar-alt"></i>Meal Plans</a>
                </li>
                <li class="nav-item">
                    <a class="nav-lin" href="javascript:void(0);"><i class="far fa-chart-bar"></i>Check BMI</a>
                </li>
                
            </ul>
        </div>
        </div>
    </nav>












<!-- Carousel -->
<div id="demo" class="carousel slide" data-bs-ride="carousel">

  <!-- Indicators/dots -->
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#demo" data-bs-slide-to="0" class="active"></button>
    <button type="button" data-bs-target="#demo" data-bs-slide-to="1"></button>
    <button type="button" data-bs-target="#demo" data-bs-slide-to="2"></button>
    <button type="button" data-bs-target="#demo" data-bs-slide-to="3"></button>
  </div>
  
  <!-- The slideshow/carousel -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="Images/banner-1.jpeg" alt="Los Angeles" class="d-block" style="width:100%">
      <div class="carousel-caption">
        <h3>Welcome To Your Personalzed Diet Plan</h3>
        <p>There are many variations of passages of Lorem Ipsum available, but the majority have<br>
          suffered alteration in some form, by injected humour.</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="Images/banner-2.jpeg" alt="Chicago" class="d-block" style="width:100%">
      <div class="carousel-caption">
        <h3>Welcome To Your Personalzed Diet Plan</h3>
        <p>There are many variations of passages of Lorem Ipsum available, but the majority have<br>
          suffered alteration in some form, by injected humour.</p>
      </div> 
    </div>
    <div class="carousel-item">
      <img src="Images/banner-3.jpeg" alt="New York" class="d-block" style="width:100%">
      <div class="carousel-caption">
        <h3>Welcome To Your Personalzed Diet Plan</h3>
        <p>There are many variations of passages of Lorem Ipsum available, but the majority have<br>
          suffered alteration in some form, by injected humour.</p>
      </div>  
    </div>
     <div class="carousel-item">
      <img src="Images/banner-4.jpg" alt="New York" class="d-block" style="width:100%">
      <div class="carousel-caption">
        <h3>Welcome To Your Personalzed Diet Plan</h3>
        <p>There are many variations of passages of Lorem Ipsum available, but the majority have<br>
          suffered alteration in some form, by injected humour.</p>
      </div>  
    </div>
     
  </div>
  
  <!-- Left and right controls/icons -->
  <button class="carousel-control-prev" type="button" data-bs-target="#demo" data-bs-slide="prev">
    <span class="carousel-control-prev-icon"></span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#demo" data-bs-slide="next">
    <span class="carousel-control-next-icon"></span>
  </button>
</div>











<script type="module" src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.esm.js"></script>
<script nomodule src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.js"></script>




<div class="container">
<div class="parformans">
  
<div class="hover09 column">
  <div class="i-t-p">
    <div class="img-tet">
  <div class="imagess">
  <div>
    <figure><img src="Images/pr-1.jpeg" /></figure>
  </div>
</div>
<div class="imagess-text">
  <h5>Eat Smart
Life Better</h5>

<p style="
    text-align: right;
">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been<br>
  the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of<br>
  type and scrambled it to make a type specimen book. It has survived not only five centuries.</p>
   <div class="bnn">
<a href="#" class="fancy-btn">Read Now</a>
</div>
</div>

</div>


</div>
</div>
</div>


<div class="parformans">
  
  <div class="hover09 column">
    <div class="i-t-p">
    
  <div class="imagess-text-1">
    <h5>Your Journey To A<br>
Healthier You Starts Here</h5>
  
  <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been<br>
    the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of<br>
    type and scrambled it to make a type specimen book. It has survived not only five centuries.</p>
   <div class="bnn-1">
  <div class="fancy-btn"><a href="#">Choose Your Meal Type</a></div></div>
  </div>

  <div class="imagess">
    <div>
      <figure><img src="Images/pr-2.jpeg" /></figure>
    </div>
  </div>
  </div>
  </div>
  </div>


</div>













<div class="continer-fluid">
  <div class="review"><h1>People Review</h1></div>
<div class="fixed-bg">
<div class="container">
  
<div class="revi-dis">



<div class="rev-all">
  <div class="rev-BG">
    <div class="rev-M">
<div class="reviwe">
<div class="reviwe-img">
  <img src="Images/profil.png">
  <div class="reviwe-text">
    <h1>Raj Saha</h1>
  </div>
</div>


</div>
<div class="reviwe-ster">
  <img src="Images/Group 29.png">
</div>
<div class="rev-p">
  <p>Lorem Ipsum is simply dummy text of the printing and
    typesetting industry. Lorem Ipsum has been
     the industry's standard dummy text ever since the 1500s,
      when an unknown printer took a galley of 
     type and scrambled it to make a type specimen book. It 
     has survived not only five centuries.
    Lorem Ipsum is simply dummy text of the printing and
    typesetting industry. Lorem Ipsum has been
     the industry's standard dummy text ever since the 1500s,
      when an unknown printer took a galley of 
     type and scrambled it to make a type specimen book. It 
     has survived not only five centuries</p>
</div>
</div>

</div>
</div>









<div class="rev-all">
  <div class="rev-BG">
    <div class="rev-M">
<div class="reviwe">
<div class="reviwe-img">
  <img src="Images/Ellipse 6.png">
  <div class="reviwe-text">
    <h1>Helen Marco</h1>
  </div>
</div>


</div>
<div class="reviwe-ster">
  <img src="Images/Group 29.png">
</div>
<div class="rev-p">
  <p>Lorem Ipsum is simply dummy text of the printing and
    typesetting industry. Lorem Ipsum has been
     the industry's standard dummy text ever since the 1500s,
      when an unknown printer took a galley of 
     type and scrambled it to make a type specimen book. It 
     has survived not only five centuries.
    Lorem Ipsum is simply dummy text of the printing and
    typesetting industry. Lorem Ipsum has been
     the industry's standard dummy text ever since the 1500s,
      when an unknown printer took a galley of 
     type and scrambled it to make a type specimen book. It 
     has survived not only five centuries</p>
</div>
</div>

</div>
</div>










</div>
</div>
    
  </div>

</div>
















<div class="container-fluid">
<div class="sil-tex">
    <h2>Most Popular</h2>
  </div>
<div id="slider-container" class="slider">
  
	<div class="slide">
		<img src="Images/sld-1.jpeg" alt="">
    <div class="si-te">
   
    <h2>Most Popular</h2>
    <p>kjbkjb nkmn lkn lknknk;m nlknlknlknnoi hobikbboo bnlnlbnohjbn lnlboboblbnl lboib nbob l o bkbb<br>
      kbuivui; sfu kb k o jkbbb bkbb ib bk bb kb b</p>
  </div>
	</div>
	<div class="slide">
		<img src="Images/sld-2.jpeg" alt="">
    <div class="si-te-2">
      
    <h2>Most Popular</h2>
    <p>kjbkjb nkmn lkn lknknk;m nlknlknlknnoi hobikbboo bnlnlbnohjbn lnlboboblbnl lboib nbob l o bkbb<br>
      kbuivui; sfu kb k o jkbbb bkbb ib bk bb kb b</p>
  </div>
	</div>
	<div class="slide">
		<img src="Images/sld-3.jpeg" alt="">
    <div class="si-te-3">
      
    <h2>Most Popular</h2>
    <p>kjbkjb nkmn lkn lknknk;m nlknlknlknnoi hobikbboo bnlnlbnohjbn lnlboboblbnl lboib nbob l o bkbb<br>
      kbuivui; sfu kb k o jkbbb bkbb ib bk bb kb b</p>
  </div>
	</div>
	<div class="slide">
		<img src="Images/sld-4.jpeg" alt="">
    <div class="si-te-4">
     
    <h2>Most Popular</h2>
    <p>kjbkjb nkmn lkn lknknk;m nlknlknlknnoi hobikbboo bnlnlbnohjbn lnlboboblbnl lboib nbob l o bkbb<br>
      kbuivui; sfu kb k o jkbbb bkbb ib bk bb kb b</p>
  </div>
	</div>
	<div class="slide">
		<img src="Images/sld-5.jpeg" alt="">
    <div class="si-te-5">
      
    <h2>Most Popular</h2>
    <p>kjbkjb nkmn lkn lknknk;m nlknlknlknnoi hobikbboo bnlnlbnohjbn lnlboboblbnl lboib nbob l o bkbb<br>
      kbuivui; sfu kb k o jkbbb bkbb ib bk bb kb b</p>
  </div>
	</div>
	<div class="slide">
		<img src="Images/sld-6.jpeg" alt="">
    <div class="si-te-6">
    
    <h2>Most Popular</h2>
    <p>kjbkjb nkmn lkn lknknk;m nlknlknlknnoi hobikbboo bnlnlbnohjbn lnlboboblbnl lboib nbob l o bkbb<br>
      kbuivui; sfu kb k o jkbbb bkbb ib bk bb kb b</p>
  </div>
	</div>

	
	<div onclick="prev()" class="control-prev-btn">
		<i class="fas fa-arrow-left"></i>
	</div>
	<div onclick="next()" class="control-next-btn">
		<i class="fas fa-arrow-right"></i>
	</div>
</div>

<div class="overlay"></div>

</div>




























<div class="container-fluid">
<div class="last-one">
<div class="container">
<div class="last-logo">
    <a href="#"><img src="Images/logo-4.png" style="width: 208px; margin-left: -46px;" ></a>
</div>
<div class="last-tex">
    <div class="L-T-1">
    <h1>Get Inspired</h1>
    <div class="last-but-1">
    <ul>
    <li><a href="#">Design Ideas</a></li>
    <li><a href="#">Magazine</a></li>
    </ul>
</div>
</div>


<div class="L-T-2">
    <h1>Company</h1>
    <div class="last-but-2">
    <ul>
    <li><a href="#">Refer a friend</a></li>
    <li><a href="#">How it works</a></li>
    <li><a href="#">Careers</a></li>
    <li><a href="#">Policies</a></li>
    <li><a href="#">About us</a></li>
    <li><a href="#">Privacy</a></li>
    </ul>
    </div>
</div>

    <div class="L-T-3">
    <h1>Contact Us</h1>
<div class="last-but-3">
    <ul>
        <li><a href="#">Call us<br>
        91+ 8777513164</a></li>
        <li><a href="#">Email<br>
        adi254@gmail.com</a></li>
</ul>
</div>
</div>




</div>
<div class="last-pa">
    <p>Leo vel fringilla est ullamcorper eget nulla facilisi etiam. At urna<br>
    condimentum mattis pellentesque id nibh tortor. Eget magna<br>
    fermentum iaculis eu non diam phasellus vestibulum lorem.<br>
    Elementum sagittis vitae et leo duis ut diam.</p>
</div>
<div class="last-img">
    <a href="#"><img src="Images/f-x-i.png"></a>
    
</div>

</div>
<div class="container">
<div class="copyright">
    <a href="#">Copyright 2024, Wedesigntech. All rights reserved</a>

</div>
</div>
</div>


</div>










  <script src="Custom.js/custom.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.7.1/jquery.min.js" integrity="sha512-v2CJ7UaYy4JwqLDIrZUI/4hqeoQieOmAZNXBeQyjo21dadnwR+8ZaIJVT8EE2iyI61OV8e6M8PP2/4hpQINQ/g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/OwlCarousel2/2.3.4/owl.carousel.min.js" integrity="sha512-bPs7Ae6pVvhOSiIcyUClR7/q2OAsRiovw4vAkX+zJbw3ShAeeqezq50RIIcIURq7Oa20rW2n2q+fyXBNcU9lrw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

</body>
</html>
