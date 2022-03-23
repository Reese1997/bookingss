<template>
 <div class="container-fluid">
				<div class="row">
					<div class="col-md-8 col-xs-12">
						<!-- <div id="title">Check This Out</div> -->
					</div><!-- end col-md-12-->
					<div class="col-md-4 col-xs-12">
						
					</div><!-- end col-md-4 -->
				</div><!--end row -->
			</div><!--end container-->
		
		<section id="about-me">
			<div class="container animate__animated animate__zoomIn">
				<div class="row">
					<div class="col-md-12">
						<div id="about-me-box">
							<div class="row">
								<div class="col-md-6 col-xs-12">
									<img class="max-width-xs" src="https://images.unsplash.com/photo-1606224547099-b15c94ca5ef2?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTF8fGN5Y2xpbmd8ZW58MHx8MHx8&w=1000&q=80" />
								</div><!-- end col-md-7 -->
								<div class="col-md-6 col-xs-12">

                  <div class="text-center"><h2>About Me</h2></div>
									<p class="about-me">Hi! My name is Karina and this is True Cadence.
                    I am a qualified Personal Trainer and Sports Conditioning Coach.
                     I am a passionate Elite Cyclist, and I participate in local races.
                     I am passionate about getting an aspiring cyclist to where they want to be. 
                      I hope you find something worth enjoying. </p>
								</div><!-- end col-md-5-->
							</div><!--end row -->
						</div><!-- end about-me-box -->
					</div><!-- end col-md-12-->
				</div><!-- end row-->
			</div><!-- end container -->
		</section>
</template>

<script>
export default {

}
</script>

<style>
.about{
  min-height: 100vh;
}

img {
	width: 100%;	
}
a {
	text-decoration: none; 
	color: white;
}
ul {
	list-style: none;	
}
 h2 {
	 font-family: 'Bebas Neue', cursive;
font-family: 'League Gothic', sans-serif;
font-family: 'Smooch Sans', sans-serif;  -webkit-font-smoothing: antialiased; 
	 border-bottom: dotted 2px black;
	display: inline-block;
	margin: 100px 0 50px;
}
/* h2 { */
	/* font-family: 'Euphoria Script'; */
	/* font-size: 40px;
} */ */ */

/*class selector*/
.margin {
	margin: 50px 0;	
}
.dropdown {
	position: relative;	
	display: inline-block;
}

.text-center {
	text-align: center;	
}
/* ID Selector */
#title {
	font-size: 50px;
	font-family: 'Euphoria Script';
}
#about-me-box {
	margin: 50px 0;
	background-color: #fff; 
	box-shadow: 1px 2px 2px 2px rgba(0, 0, 0, 0.2);
	display: block;
	padding: 0 10px 0 0;
}


@media (max-width: 767px) {
	#about-me-box {
		padding: 0 10px;	
	}
	/*responsive helper classes*/
	.hidden-xs {
		display: none;
	}
	.max-width-xs {
		width: 100%;	
}
}
.about-me {
  font-size: 30px;
}

</style>