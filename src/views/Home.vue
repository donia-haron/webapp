<template>
    <div>
        <!--  <div class="home">


            <div class="di">
                <div class="di1">
                    <img src="../assets/image1.jpg" />
                </div>

                <div class="di3">
                    <img src="../assets/images.jpg" />
                </div>
            </div>
        </div>-->

        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
            <ol class="carousel-indicators">
                <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
                <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
                <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
            </ol>
            <div id="slider" class="carousel-inner">

                <div class="content carousel-item active">
                    <h1 class="title">Welcome to VTP shop</h1>
                    <img class="d-block w-90 imgg" src="../assets/slider.jpg">
                </div>
                <div class="content carousel-item">
                    <img class="d-block w-90 imgg" src="../assets/d-2.png" alt="Second slide">
                </div>

                <div class="content carousel-item">
                    <img class="d-block w-90 imgg" src="../assets/79b1fccd-6714-40e0-9430-dae4a42baacb.jpg" alt="Third slide">
                </div>

            </div>
            <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </a>

        </div>
        <h4 class="text-center"><strong>BRANDS</strong></h4>
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                    <hr>
                    <div class="profile-card-6">
                        <img src="../assets/fashion-logo-design.jpg" class="img img-responsive">
                        <div class="profile-name">
                            Logo
                        </div>
                        <div class="profile-position">Dresses</div>
                        <div class="profile-overview">
                            <div class="row text-center">

                                <div class="col-s-4">
                                    <h3>35</h3>
                                    <p>Folowers</p>
                                </div>
                                <div class="col-s-4">
                                    <h3 class="rate">
                                        <i><font-awesome-icon :icon="['fas', 'star']" checked /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" checked /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" checked /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" /></i>

                                    </h3>
                                    <p>Rate</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="col-md-4">
                    <hr>
                    <div class="profile-card-6">
                        <img src="../assets/Elza-Sofie-Fashion-Logo.png" class="img img-responsive">
                        <div class="profile-name">
                            fashion logo
                        </div>
                        <div class="profile-position">Clothes</div>
                        <div class="profile-overview">

                            <div class="row text-center">

                                <div class="col-s-4">
                                    <h3>35</h3>
                                    <p>Folowers</p>
                                </div>
                                <div class="col-s-4">
                                    <h3 class="rate">
                                        <i><font-awesome-icon :icon="['fas', 'star']" checked variant="warning" /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" checked /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" checked /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" /></i>

                                    </h3>
                                    <p>Rate</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <hr>
                    <div class="profile-card-6">
                        <img src="../assets/Evellon-Boutique-Fashion-Logo.png" class="img img-responsive">
                        <div class="profile-name">
                            fashion logo
                        </div>
                        <div class="profile-position">Clothes</div>
                        <div class="profile-overview">

                            <div class="row text-center">

                                <div class="col-s-4">
                                    <h3>35</h3>
                                    <p>Folowers</p>
                                </div>
                                <div class="col-s-4">
                                    <h3 class="rate">
                                        <i><font-awesome-icon :icon="['fas', 'star']" checked variant="warning" /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" checked /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" checked /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" /></i>
                                        <i><font-awesome-icon :icon="['fas', 'star']" /></i>

                                    </h3>
                                    <p>Rate</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>





    </div>
</template>
<script>
    import $ from 'jquery';
    $("#slider > div:gt(0)").hide();

    setInterval(function () {
        $('#slider > div:first')
            .fadeOut(1000)
            .next()
            .fadeIn(1000)
            .end()
            .appendTo('#slider');
    }, 3000);
</script>
<script>
    // @ is an alias to /src


    export default {
        name: "Home",
        components: {

        }
    };
</script>

<style>
    .carousel-inner {
    }

    .imgg:hover {
        transform: scale(1.3);
    }

    .content {
        margin-left: 300px !important;
        transition: opacity .6s ease, transform .3s ease;
    }

    .title {
        margin-bottom: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        position: absolute;
        top: 0;
        right: 800px;
        font-weight: bold;
        width: 100%;
        height: 100%;
        font-size: 1rem;
        color: #ff006e;
        text-transform: uppercase;
        width: 100%;
        padding: 0 2em;
        font-size: 2em;
        font-weight: 300;
        margin: .5rem 0 0;
    }

    .di1 img {
        margin-left: 150px;
        float: left;
        margin-top: 50px;
        width: 30%;
        height: 450px;
    }


    .di3 img {
        margin-left: 150px;
        margin-top: 50px;
        height: 450px;
        float: left;
        width: 35%;
    }

    .container-fluid,
    .container {
        max-width: 1200px;
        display: inline-block;
        display: grid;
    }

    .rate {
        padding-left: 30px;
        font-size: 18px;
        padding-bottom: 12px;
    }

    .card-container {
        padding: 100px 0px;
    }

    .profile-card-6 {
        max-width: 300px;
        background-color: #FFF;
        border-radius: 5px;
        box-shadow: 0px 0px 25px rgba(0, 0, 0, 0.1);
        overflow: hidden;
        position: relative;
        margin: 10px auto;
        cursor: pointer;
    }

        .profile-card-6 img {
            transition: all 0.15s linear;
            width: 300px;
            height: 400px;
        }

        .profile-card-6 .profile-name {
            position: absolute;
            top: 10px;
            left: 10px;
            font-size: 25px;
            font-weight: bold;
            color: #FFF;
            padding: 15px 20px;
            background: linear-gradient(140deg, rgba(0, 0, 0, 0.4) 50%, rgba(255, 255, 0, 0) 50%);
            transition: all 0.15s linear;
        }

        .profile-card-6 .profile-position {
            position: absolute;
            color: rgba(255, 255, 255, 0.4);
            left: 30px;
            top: 100px;
            transition: all 0.15s linear;
        }

        .profile-card-6 .profile-overview {
            position: absolute;
            bottom: 0px;
            left: 0px;
            right: 0px;
            background: linear-gradient(0deg, rgba(0, 0, 0, 0.4) 50%, rgba(255, 255, 0, 0));
            color: #FFF;
            padding: 50px 0px 0px 30px;
            transition: all 0.15s linear;
        }

            .profile-card-6 .profile-overview h3 {
                font-weight: bold;
                margin-right: 10px;
            }

            .profile-card-6 .profile-overview p {
                color: rgba(255, 255, 255, 0.7);
            }

        .profile-card-6:hover img {
            filter: brightness(80%);
        }

        .profile-card-6:hover .profile-name {
            padding-left: 25px;
            padding-top: 20px;
        }

        .profile-card-6:hover .profile-position {
            left: 40px;
        }

        .profile-card-6:hover .profile-overview {
            padding-bottom: 25px;
        }
</style>

