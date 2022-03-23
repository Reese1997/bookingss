<template>
  <div class="container">
  <div class="row">
    	<div class="col-md-12">
    	    <footer class="footer">				
		<div class="container">
			<div class="row">
				<div class="col-md-3 m-b-30">
					<div class="footer-title m-t-5 m-b-20 p-b-8">
						About us
					</div>	
					<p class="white-text" >It's not how good you are, 
						it's how good you want to be.
					</p>
				</div>
				<div class="col-md-3 m-b-30">
					<div class="footer-title m-t-5 m-b-20 p-b-8">
						Latest themes
					</div>	
					<div class="footer-links">
						<a href="#">
							Appointment
						</a>
						<a href="#">
							Health center
						</a>
						<a href="#">
							Quality
						</a>
						<a href="#">
							Wallstreet
						</a>
					</div>
				</div>
				<div class="col-md-3 m-b-30">
					<div class="footer-title m-t-5 m-b-20 p-b-8">
						Quick Links
					</div>	
					<div class="footer-links">
						<a href="#">
							Blog
						</a>
						<a href="#">
							FAQ
						</a>
						<a href="#">
							Terms & conditions
						</a>
						<a href="#">
							Privacy policy
						</a>
					</div>
				</div>
				<div class="col-md-3 m-b-30">
					<div class="footer-title m-t-5 m-b-20 p-b-8">
						Support
					</div>	
					<div class="footer-links">
						<a href="#">
							Affiliate
						</a>
						<a href="#">
							Login
						</a>
						<a href="#">
							All theme package
						</a>
						<a href="#">
							Support forum
						</a>
					</div>

					<div class="footer-social-links m-t-30">
						<li>
							<a href="#">
								<i class="fa fa-facebook" aria-hidden="true"></i>
							</a>
							<a href="#">
								<i class="fa fa-twitter" aria-hidden="true"></i>
							</a>
							<a href="#">
								<i class="fa fa-linkedin" aria-hidden="true"></i>
							</a>
							<a href="#">
								<i class="fa fa-youtube" aria-hidden="true"></i>
							</a>
						</li>
					</div>
				</div>
			</div>
		</div>
	</footer>
	<div class="footer-bottom">
		Copyright TRUECADENCE© 2022, All Rights Reserved
	</div>
    	</div>
	</div>
</div>
</template>

<script>
export default {

}
</script>

<style>
.footer{
	padding-top: 60px;
	padding-right: 0%;
	padding-bottom: 0%;
	padding-left: 0%;
    width: 100%;
    background: #a50505;
    color: #fff;
   
}
.footer-title{
	position: relative;
    color: #fff;
	font-size: 24px;
    font-weight: 600;
    margin-top: 5px;
    margin-bottom: 20px;
    border-bottom: 1px solid #4e4e4e;
}
.footer-title:after{
	position: absolute;
	content: '';
	left: 0;
	bottom: 0;
	width: 30px;
	height: 4px;
	background: #ff304d;
}
.footer-links a{
	padding: 10px 0;
	border-bottom: 1px solid #404040;
	color: #fff;
	display: block;
	transition: color 0.5s ease-in-out;
   text-decoration:none;
}
.footer-links a:hover{
	color: #ff304d;
}
.footer-social-links li{
	display: inline-block;
}
.footer-social-links a{
	width: 40px;
	height: 40px;
	font-size: 16px;
	float: left;
	margin-right: 10px;
	padding: 10px;
	border: 1px solid #404040;
	border-radius: 50px;
	text-align: center;
	color: #fff;
	line-height: 1;
	-webkit-transition: background 0.3s ease-in-out;
	-moz-transition: background 0.3s ease-in-out;
	transition: background 0.3s ease-in-out;
  background:#0c0b0e;
}
.footer-social-links a:hover{
	background: #bd0000;
}
/* g. Footer bottom section */
.footer-bottom{
	width: 100%;
	padding: 25px 0;
	text-align: center;
	color: #fff;
	background: rgb(0, 0, 0);
}
</style>