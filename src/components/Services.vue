<template>
<section class="service-grid pb-5 pt-5">
            <div class="container">
                <div class="row">
                    <div class="col-xl-12 text-center mb-4">
                        <div class="service-title">
                            <h4 class="serv">Our Services</h4>
                        </div>
                    </div>
                </div>
                <div class="row">
                    <div class="col-lg-4 col-md-6 text-center mb-3">
                        <div class="service-wrap">
                            <div class="service-icon">
                                <i class="fas fa-layer-group"></i>
                            </div>
                            <h4>Strength and conditioning</h4>
<!-- <p>sports and conditioning</p> -->
                            <a href="#">Read More</a>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 text-center mb-3">
                        <div class="service-wrap">
                            <div class="service-icon">
                                <i class="far fa-chart-bar"></i>
                            </div>
                            <h4>Mobility</h4>
                            <!-- <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry...</p> -->
                            <a href="#">Read More</a>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 text-center mb-3">
                        <div class="service-wrap">
                            <div class="service-icon">
                                <i class="fas fa-database"></i>
                            </div>
                            <h4>High Cadence</h4>
                            <!-- <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry...</p> -->
                            <a href="#">Read More</a>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 text-center mb-3">
                        <div class="service-wrap">
                            <div class="service-icon">
                                <i class="fas fa-cogs"></i>
                            </div>
                            <h4>service & plugins</h4>
                            <!-- <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry...</p> -->
                            <a href="#">Read More</a>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 text-center mb-3">
                        <div class="service-wrap">
                            <div class="service-icon">
                                <i class="fas fa-chart-pie"></i>
                            </div>
                            <h4>Sports Periodization</h4>
                            <!-- <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry...</p> -->
                            <a href="#">Read More</a>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 text-center mb-3">
                        <div class="service-wrap">
                            <div class="service-icon">
                                <i class="fas fa-thumbs-up"></i>
                            </div>
                            <h4>Dedicated support</h4>
                            <!-- <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry...</p> -->
                            <a href="#">Read More</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

</template>

<script>
export default {

}
</script>

<style>
.serv{
    color: black;
}
.service-grid {
    background: #fcfcfc;
}
    .service-title h4 {
    position: relative;
    display: inline-block;
}
.service-icon {
    position: relative;
}
.service-title p {
    padding: 0 190px;
    margin-bottom: 10px;
}
.about-info-text h2 {
    margin-bottom: 23px;
    text-transform: capitalize;
    font-weight: 700;
    line-height: .9;
}
.about-info-text p {
    padding: 0 100px;
    font-size: 18px;
    margin-bottom: 26px;
      position: relative;
}
.about-content p {
    margin-bottom: 0;
}
.about-info-text a {
    margin-bottom: 20px;
      position: relative;
}
.service-icon i {
    font-size: 40px;
    color: #e8bc00;
    margin-bottom: 20px;
    display: inline-block;
}
.service-wrap {
    border: 1px solid #e6e6e6;
    padding: 50px 30px;
      position: relative;
}

.service-wrap p{
      position: relative;
}

.service-wrap:hover {
    background-image: url("../assets/landpage.jpeg");
    background-size: cover;
    background-position: center center;
    background-attachment: local;
    transition: all .5s;
}

.service-wrap:hover:before {
    background: rgba(0, 0, 0, 0.2901960784313726);
    position: absolute;
    height: 100%;
    width: 100%;
    left: 0px;
    content: "";
    top: 0;
    opacity: 1;
}

.service-wrap:hover h4,.service-wrap:hover p{
    color: #fff;
}
.service-wrap h4 {
    font-weight: 600;
    color: #1e2331;
    margin-bottom: 17px;
    font-size: 18px;
    text-transform: capitalize;
      position: relative;
}
.service-wrap a {
    font-size: 14px;
    font-weight: 600;
      position: relative;

}
</style>