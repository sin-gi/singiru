/********** Template CSS **********/
:root {
    --primary: #0463FA;
    --light: #EFF5FF;
    --dark: #1B2C51;
}

.fw-medium {
    font-weight: 500 !important;
}

.fw-bold {
    font-weight: 700 !important;
}

.fw-black {
    font-weight: 900 !important;
}

.back-to-top {
    position: fixed;
    display: none;
    right: 45px;
    bottom: 45px;
    z-index: 99;
}


/*** Spinner ***/
#spinner {
    opacity: 0;
    visibility: hidden;
    transition: opacity .5s ease-out, visibility 0s linear .5s;
    z-index: 99999;
}

#spinner.show {
    transition: opacity .5s ease-out, visibility 0s linear 0s;
    visibility: visible;
    opacity: 1;
}


/*** Button ***/
.btn {
    font-weight: 500;
    transition: .5s;
}

.btn.btn-primary,
.btn.btn-secondary {
    color: #ffffff;
}

.btn-square {
    width: 38px;
    height: 38px;
}

.btn-sm-square {
    width: 32px;
    height: 32px;
}

.btn-lg-square {
    width: 48px;
    height: 48px;
}

.btn-square,
.btn-sm-square,
.btn-lg-square {
    padding: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: normal;
}


/*** Navbar ***/
.navbar .dropdown-toggle::after {
    border: none;
    content: "\f107";
    font-family: "Font Awesome 5 Free";
    font-weight: 900;
    vertical-align: middle;
    margin-left: 8px;
}

.navbar .navbar-nav .nav-link {
    margin-right: 30px;
    padding: 25px 0;
    color: #FFFFFF;
    font-size: 15px;
    font-weight: 500;
    text-transform: uppercase;
    outline: none;
}

.navbar .navbar-nav .nav-link:hover,
.navbar .navbar-nav .nav-link.active {
    color: var(--primary);
}

@media (max-width: 991.98px) {
    .navbar .navbar-nav .nav-link  {
        margin-right: 0;
        padding: 10px 0;
    }

    .navbar .navbar-nav {
        border-top: 1px solid #EEEEEE;
    }
}

.navbar .navbar-brand,
.navbar a.btn {
    height: 75px;
}

.navbar .navbar-nav .nav-link {
    color: var(--dark);
    font-weight: 500;
}

.navbar.sticky-top {
    top: -100px;
    transition: .5s;
}

@media (min-width: 992px) {
    .navbar .nav-item .dropdown-menu {
        display: block;
        border: none;
        margin-top: 0;
        top: 150%;
        opacity: 0;
        visibility: hidden;
        transition: .5s;
    }

    .navbar .nav-item:hover .dropdown-menu {
        top: 100%;
        visibility: visible;
        transition: .5s;
        opacity: 1;
    }
}


/*** Header ***/
.header-carousel .owl-carousel-text {
    position: absolute;
    width: 100%;
    height: 100%;
    padding: 3rem;
    top: 0;
    left: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    text-shadow: 0 0 30px rgba(0, 0, 0, .1);
}

.header-carousel .owl-nav {
    position: absolute;
    width: 200px;
    height: 45px;
    bottom: 30px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    justify-content: space-between;
}

.header-carousel .owl-nav .owl-prev,
.header-carousel .owl-nav .owl-next {
    width: 45px;
    height: 45px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #FFFFFF;
    background: transparent;
    border: 1px solid #FFFFFF;
    border-radius: 45px;
    font-size: 22px;
    transition: .5s;
}

.header-carousel .owl-nav .owl-prev:hover,
.header-carousel .owl-nav .owl-next:hover {
    background: var(--primary);
    border-color: var(--primary);
}

.header-carousel .owl-dots {
    position: absolute;
    height: 45px;
    bottom: 30px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    align-items: center;
    justify-content: center;
}

.header-carousel .owl-dot {
    position: relative;
    display: inline-block;
    margin: 0 5px;
    width: 15px;
    height: 15px;
    background: transparent;
    border: 1px solid #FFFFFF;
    border-radius: 15px;
    transition: .5s;
}

.header-carousel .owl-dot::after {
    position: absolute;
    content: "";
    width: 5px;
    height: 5px;
    top: 4px;
    left: 4px;
    background: #FFFFFF;
    border-radius: 5px;
}

.header-carousel .owl-dot.active {
    background: var(--primary);
    border-color: var(--primary);
}

.page-header {
    background: url(/img/vaner6.png) top center no-repeat;
    background-size: cover;
    text-shadow: 0 0 30px rgba(0, 0, 0, .1);
}

.breadcrumb-item + .breadcrumb-item::before {
    color: var(--light);
}


/*** Service ***/
.service-item {
    transition: .5s;
}

.service-item:hover {
    margin-top: -10px;
    box-shadow: 0 .5rem 1.5rem rgba(0, 0, 0, .08);
}

.service-item .btn {
    width: 40px;
    height: 40px;
    display: inline-flex;
    align-items: center;
    background: #FFFFFF;
    border-radius: 40px;
    white-space: nowrap;
    overflow: hidden;
    transition: .5s;
}

.service-item:hover .btn {
    width: 140px;
}


/*** Feature ***/
@media (min-width: 992px) {
    .container.feature {
        max-width: 100% !important;
    }

    .feature-text  {
        padding-left: calc(((100% - 960px) / 2) + .75rem);
    }
}

@media (min-width: 1200px) {
    .feature-text  {
        padding-left: calc(((100% - 1140px) / 2) + .75rem);
    }
}

@media (min-width: 1400px) {
    .feature-text  {
        padding-left: calc(((100% - 1320px) / 2) + .75rem);
    }
}


/*** Team ***/
.team-item img {
    position: relative;
    top: 0;
    transition: .5s;
}

.team-item:hover img {
    top: -30px;
}

.team-item .team-text {
    position: relative;
    height: 100px;
    transition: .5s;
}

.team-item:hover .team-text {
    margin-top: -60px;
    height: 160px;
}

.team-item .team-text .team-social {
    opacity: 0;
    transition: .5s;
}

.team-item:hover .team-text .team-social {
    opacity: 1;
}

.team-item .team-social .btn {
    display: inline-flex;
    color: var(--primary);
    background: #FFFFFF;
    border-radius: 40px;
}

.team-item .team-social .btn:hover {
    color: #FFFFFF;
    background: var(--primary);
}


/*** Appointment ***/
.bootstrap-datetimepicker-widget.bottom {
    top: auto !important;
}

.bootstrap-datetimepicker-widget .table * {
    border-bottom-width: 0px;
}

.bootstrap-datetimepicker-widget .table th {
    font-weight: 500;
}

.bootstrap-datetimepicker-widget.dropdown-menu {
    padding: 10px;
    border-radius: 2px;
}

.bootstrap-datetimepicker-widget table td.active,
.bootstrap-datetimepicker-widget table td.active:hover {
    background: var(--primary);
}

.bootstrap-datetimepicker-widget table td.today::before {
    border-bottom-color: var(--primary);
}


/*** Testimonial ***/
.testimonial-carousel::before {
    position: absolute;
    content: "";
    top: 0;
    left: 0;
    height: 100%;
    width: 0;
    background: linear-gradient(to right, rgba(255, 255, 255, 1) 0%, rgba(255, 255, 255, 0) 100%);
    z-index: 1;
}

.testimonial-carousel::after {
    position: absolute;
    content: "";
    top: 0;
    right: 0;
    height: 100%;
    width: 0;
    background: linear-gradient(to left, rgba(255, 255, 255, 1) 0%, rgba(255, 255, 255, 0) 100%);
    z-index: 1;
}

@media (min-width: 768px) {
    .testimonial-carousel::before,
    .testimonial-carousel::after {
        width: 200px;
    }
}

@media (min-width: 992px) {
    .testimonial-carousel::before,
    .testimonial-carousel::after {
        width: 300px;
    }
}

.testimonial-carousel .owl-item .testimonial-text {
    background: var(--light);
    transform: scale(.8);
    transition: .5s;
}

.testimonial-carousel .owl-item.center .testimonial-text {
    background: var(--primary);
    transform: scale(1);
}

.testimonial-carousel .owl-item .testimonial-text *,
.testimonial-carousel .owl-item .testimonial-item img {
    transition: .5s;
}

.testimonial-carousel .owl-item.center .testimonial-text * {
    color: var(--light) !important;
}

.testimonial-carousel .owl-item.center .testimonial-item img {
    background: var(--primary) !important;
} 

.testimonial-carousel .owl-nav {
    position: absolute;
    width: 350px;
    top: 15px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    justify-content: space-between;
    opacity: 0;
    transition: .5s;
    z-index: 1;
}

.testimonial-carousel:hover .owl-nav {
    width: 300px;
    opacity: 1;
}

.testimonial-carousel .owl-nav .owl-prev,
.testimonial-carousel .owl-nav .owl-next {
    position: relative;
    color: var(--primary);
    font-size: 45px;
    transition: .5s;
}

.testimonial-carousel .owl-nav .owl-prev:hover,
.testimonial-carousel .owl-nav .owl-next:hover {
    color: var(--dark);
}


/*** Footer ***/
.footer .btn.btn-social {
    margin-right: 5px;
    width: 35px;
    height: 35px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: var(--light);
    border: 1px solid #FFFFFF;
    transition: .3s;
}

.footer .btn.btn-social:hover {
    color: var(--primary);
}

.footer .btn.btn-link {
    display: block;
    margin-bottom: 5px;
    padding: 0;
    text-align: left;
    color: #FFFFFF;
    font-size: 15px;
    font-weight: normal;
    text-transform: capitalize;
    transition: .3s;
}

.footer .btn.btn-link::before {
    position: relative;
    content: "\f105";
    font-family: "Font Awesome 5 Free";
    font-weight: 900;
    margin-right: 10px;
}

.footer .btn.btn-link:hover {
    color: var(--primary);
    letter-spacing: 1px;
    box-shadow: none;
}

.footer .copyright {
    padding: 25px 0;
    font-size: 15px;
    border-top: 1px solid rgba(256, 256, 256, .1);
}

.footer .copyright a {

    color: var(--light);
}

.footer .copyright a:hover {
    color: var(--primary);
}

<!DOCTYPE html>
<html lang="Ko">
<!-- 구분
Home-home
Program-프로그램소개
Role-등장인물
Video-동영상
Photo_포토갤러리
appointmen-이벤트
배너 img 바꾸기/css/page header-->

<head>
    <meta charset="utf-8">
    <title>신기루 홈페이지</title>
    <meta content="width=device-width, initial-scale=1.0" name="viewport">
    <meta content="" name="keywords">
    <meta content="" name="description">

    <!-- Favicon -->
    <link href="img/favicon.ico" rel="icon">

    <!-- Google Web Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;500&family=Roboto:wght@500;700;900&display=swap" rel="stylesheet"> 

    <!-- Icon Font Stylesheet -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.10.0/css/all.min.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.4.1/font/bootstrap-icons.css" rel="stylesheet">

    <!-- Libraries Stylesheet -->
    <link href="lib/animate/animate.min.css" rel="stylesheet">
    <link href="lib/owlcarousel/assets/owl.carousel.min.css" rel="stylesheet">
    <link href="lib/tempusdominus/css/tempusdominus-bootstrap-4.min.css" rel="stylesheet" />

    <!-- Customized Bootstrap Stylesheet -->
    <link href="css/bootstrap.min.css" rel="stylesheet">

    <!-- Template Stylesheet -->
    <link href="css/style.css" rel="stylesheet">
</head>

<body>
    <!-- Spinner Start -->
    <div id="spinner" class="show bg-white position-fixed translate-middle w-100 vh-100 top-50 start-50 d-flex align-items-center justify-content-center">
        <div class="spinner-grow text-primary" style="width: 3rem; height: 3rem;" role="status">
            <span class="sr-only">Loading...</span>
        </div>
    </div>
    <!-- Spinner End -->

    <!-- Topbar Start -->
<div class="container-fluid bg-light p-0 wow fadeIn" data-wow-delay="0.1s">
    <div class="row gx-0 d-none d-lg-flex">
        <div class="col-lg-20 px-5.1 text-end">
                <div class="topbar-top ms-auto p-4 p-lg-0">
                    <a href="log.html" class=" ">로그인</a>
                    <a href="join.html" class=" ">회원가입</a>
                        <input type="text" placeholder="search" type=/>
                        <button type="submit">검색</button>
                </div>
        </div>
    </div>
</div>
<!-- Topbar End -->

    <!-- Navbar Start -->
    <nav class="navbar navbar-expand-lg bg-white navbar-light sticky-top p-0 wow fadeIn" data-wow-delay="0.1s">
        <a href="Home.html" class="navbar-brand d-flex align-items-center px-4 px-lg-5">
            <h1 class="m-0 text-primary"></i>신기루</h1>
        </a>
        <button type="button" class="navbar-toggler me-4" data-bs-toggle="collapse" data-bs-target="#navbarCollapse">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarCollapse">
            <div class="navbar-nav ms-auto p-4 p-lg-0">
                <a href="Home.html" class="nav-item nav-link active">Home</a>
                <a href="Program.html" class="nav-item nav-link ">프로그램소개</a>
                <a href="Role.html" class="nav-item nav-link">등장인물</a>
                <a href="Storyboard.html" class="nav-item nav-link">스토리보드</a>
                <a href="Video.html" class="nav-item nav-link">동영상</a>
                <a href="Photo.html" class="nav-item nav-link">포토 갤러리</a>
                <a href="Event.html" class="nav-item nav-link">이벤트</a>
            </div>
            
        </div>
    </nav>
    <!-- Navbar End -->


    <!-- Header Start -->
    <div class="container-fluid header bg-primary p-0 mb-5">
        <div class="row g-0 align-items-center flex-column-reverse flex-lg-row">
            <div class="col-lg-6 p-5 wow fadeIn" data-wow-delay="0.1s">
                <h1 class="display-4 text-white mb-5">내 삶의 주인공은 나다</h1>
                <div class="row g-4">
                    <div class="col-sm-4">
                        <div class="border-start border-light ps-4">
                            <p class="text-light mb-0">‘하린’의 성장 이야기와 마을 사람들의 사랑, 그리고 사춘기를 겪으며 자신감을 찾는 과정을 담은 드라마</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-lg-6 wow fadeIn" data-wow-delay="0.5s">
                <div class="owl-carousel header-carousel">
                    <div class="owl-carousel-item position-relative">
                        <img class="img-fluid" src="/img/title image.jpg" alt="">
                        <div class="owl-carousel-text">
                            <h1 class="display-1 text-white mb-0"></h1>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Header End -->

    


    <!-- Program Start -->
    <div class="container-xxl py-5">
        <div class="container">
            <div class="row g-5">
                <div class="col-lg-6 wow fadeIn" data-wow-delay="0.1s">
                    <div class="d-flex flex-column">
                        <img class="img-fluid rounded w-75 bg-white pt-3 pe-3" src="img/title2.JPG" alt="">
                    </div>
                </div>
                <div class="col-lg-6 wow fadeIn" data-wow-delay="0.5s">
                    <p class="d-inline-block border rounded-pill py-1 px-4">프로그램소개</p>
                    <h1 class="mb-4">신기루</h1>
                    <p>"내 삶의 주인공은 나"라는 메시지를 주제로 ‘하린’의 성장 이야기와 마을 사람들의 사랑,</br>
                        그리고 사춘기를 겪으며 자신감을 찾는 과정을 담은 드라마</p>
                </div>
            </div>
        </div>
    </div>
    <!-- Program End -->


    <!-- Role Start -->
    <div class="container-xxl py-5">
        <div class="container">
            <div class="text-center mx-auto mb-5 wow fadeInUp" data-wow-delay="0.1s" style="max-width: 600px;">
                <p class="d-inline-block border rounded-pill py-1 px-4">등장인물</p>
                <h1>인물 소개</h1>
            </div>
            <div class="row g-4">
                <div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.1s">
                    <div class="team-item position-relative rounded overflow-hidden">
                        <div class="overflow-hidden">
                            <img class="img-fluid" src="img/person.png" alt="">
                        </div>
                        <div class="team-text bg-light text-center p-4">
                            <h5>하린 역</h5>
                            <p class="text-primary">이하린</p>
                            <div class="team-social text-center">
                                <a class="btn btn-square" href=""><i class="fab fa-facebook-f"></i></a>
                                <a class="btn btn-square" href=""><i class="fab fa-twitter"></i></a>
                                <a class="btn btn-square" href=""><i class="fab fa-instagram"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.3s">
                    <div class="team-item position-relative rounded overflow-hidden">
                        <div class="overflow-hidden">
                            <img class="img-fluid" src="img/person.png" alt="">
                        </div>
                        <div class="team-text bg-light text-center p-4">
                            <h5>신루 역</h5>
                            <p class="text-primary">김수환</p>
                            <div class="team-social text-center">
                                <a class="btn btn-square" href=""><i class="fab fa-facebook-f"></i></a>
                                <a class="btn btn-square" href=""><i class="fab fa-twitter"></i></a>
                                <a class="btn btn-square" href=""><i class="fab fa-instagram"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.5s">
                    <div class="team-item position-relative rounded overflow-hidden">
                        <div class="overflow-hidden">
                            <img class="img-fluid" src="img/person.png" alt="">
                        </div>
                        <div class="team-text bg-light text-center p-4">
                            <h5>아주머니 역</h5>
                            <p class="text-primary">이정연</p>
                            <div class="team-social text-center">
                                <a class="btn btn-square" href=""><i class="fab fa-facebook-f"></i></a>
                                <a class="btn btn-square" href=""><i class="fab fa-twitter"></i></a>
                                <a class="btn btn-square" href=""><i class="fab fa-instagram"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.7s">
                    <div class="team-item position-relative rounded overflow-hidden">
                        <div class="overflow-hidden">
                            <img class="img-fluid" src="img/person.png" alt="">
                        </div>
                        <div class="team-text bg-light text-center p-4">
                            <h5>아저씨 역</h5>
                            <p class="text-primary">박선진</p>
                            <div class="team-social text-center">
                                <a class="btn btn-square" href=""><i class="fab fa-facebook-f"></i></a>
                                <a class="btn btn-square" href=""><i class="fab fa-twitter"></i></a>
                                <a class="btn btn-square" href=""><i class="fab fa-instagram"></i></a>
                            </div>
                    </div>
                </div>
            </div>
            <div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.9s">
                <div class="team-item position-relative rounded overflow-hidden">
                    <div class="overflow-hidden">
                        <img class="img-fluid" src="img/person.png" alt="">
                    </div>
                    <div class="team-text bg-light text-center p-4">
                        <h5>어린 하린 역</h5>
                        <p class="text-primary">정이담</p>
                        <div class="team-social text-center">
                            <a class="btn btn-square" href=""><i class="fab fa-facebook-f"></i></a>
                            <a class="btn btn-square" href=""><i class="fab fa-twitter"></i></a>
                            <a class="btn btn-square" href=""><i class="fab fa-instagram"></i></a>
                        </div>    
                    </div>
                </div>
            </div>
        </div>
        </div>
    </div>
    <!-- Role End -->

    <!-- Storyboard Start -->
    <div class="container-xxl py-5">
        <div class="container">
            <div class="text-center mx-auto mb-5 wow fadeInUp" data-wow-delay="0.1s" style="max-width: 600px;">
                <p class="d-inline-block border rounded-pill py-1 px-4">스토리보드</p>
                <h1></h1>
            </div>
            <div class="owl-carousel testimonial-carousel wow fadeInUp" data-wow-delay="0.1s">
                
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-squard p-2 mx-auto mb-4" src="img/MT.png" style="width: 100px; height: 100px;">
                    <div class="text-center">
                        <h5>S#1. MT</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" src="img/birth.jpg" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#2. 하린</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/hospital.png" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#3. 병원</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/kindergarden.png" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#4. 유치원</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/home.png" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#5. 집</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/market.jpg" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#6. 시장</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/festival.png" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#7. 학예회</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/land.png" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#8. 놀이공원</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/drama.png" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#9. 드라마</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/exam.png" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#10. 수능</h5>
                    </div>
                </div>

                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/present.jpg" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#11. 생일</h5>
                    </div>
                </div>
                <div class="스토리보드-item text center">
                    
                    <img class="img-fluid bg-light rounded-suard p-2 mx-auto mb-4" img src="img/book.png" style="width: 130px; height: 130px;">
                    <div class="text-center">
                        <h5>S#12. 에필로그</h5>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Storyboard End -->

    <!-- Video Start -->
    <div class="container-xxl py-5">
        <div class="container">
            <div class="row g-4">
                <div class="col-lg-4"></div>
            </div>
        </div>
    </div>
                </div>
                <div class="col-lg-6 wow fadeIn" data-wow-delay="0.1s">
                    <div class="bg-light rounded p-5">
                        <p class="d-inline-block border rounded-pill py-1 px-4">동영상</p>
                        <h1 class="mb-4">추후 추가될 예정입니다.</h1>
                        <p class="mb-4">드라마 촬영후 업로드 됩니다...</p>
                </div>
            </div>
        </div>
    </div>
    <!-- Video End -->


    <!-- Photo Start -->
    <div class="container-xxl py-5">
        <div class="container">
            <div class="row g-4">
                <div class="col-lg-4"></div>
            </div>
        </div>
    </div>
                </div>
                <div class="col-lg-6 wow fadeIn" data-wow-delay="0.1s">
                    <div class="bg-light rounded p-5">
                        <p class="d-inline-block border rounded-pill py-1 px-4">현장포토</p>
                        <h1 class="mb-4">추후 추가될 예정입니다.</h1>
                        <p class="mb-4">드라마 촬영후 업로드 됩니다...</p>
                </div>
            </div>
        </div>
    </div>
    <!-- Photo End -->

    <!-- Event Start -->
    <div class="container-xxl py-5">
        <div class="container">
            <div class="text-center mx-auto mb-5 wow fadeInUp" data-wow-delay="0.1s" style="max-width: 600px;">
                <p class="d-inline-block border rounded-pill py-1 px-4">이벤트</p>
                <h1>드라마 관련</h1>
                <p class="mb-4"> 추첨을 통해 경품을 드립니다.</p>
            </div>

    
                    <div class="bg-light rounded d-flex align-items-center p-5 mb-4">
                        <div class="d-flex flex-shrink-0 align-items-center justify-content-center" style="width: 55px; height: 55px;">
                        </div>
                        <div class="ms-4">
                            <h5 class="mb-0">기대평</h5>
                            <p class="mb-2">단막극<신기루>의 기대평을 남겨주세요.</br>
                                추첨을 통하여 경품을 드립니다.</p>                           
                        </div>
                    </div>
                    <div class="bg-light rounded d-flex align-items-center p-5">
                        <div class="d-flex flex-shrink-0 align-items-center justify-content-center" style="width: 55px; height: 55px;">
                        </div>
                        <div class="ms-4">
                            <h5 class="mb-0">본방사수</h5>
                            <p class="mb-2">드라마의 첫 대사와 마지막 대사는 무엇일까요?</br>
                                본방사수를 통해 확인한 정답을 아래 빈칸에 입력해주세요.</p></p>
                        </div>
                    </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Event End -->

    <!-- Footer Start -->
    
        <div class="container-fluid bg-dark text-light footer mt-5 pt-5 wow fadeIn" data-wow-delay="0.1s">
        <div class="container py-5">
            <div class="row g-5">
                <div class="col-lg-6 col-md-6">
                    <h5 class="text-light mb-6">
                    <a class=" " href="Program.html"> 프로그램소개 &nbsp;</a>
                    <a class=" " href="Role.html"> 등장인물 &nbsp;</a>
                    <a class=" " href="Storyboard.html"> 스토리보드 &nbsp;</a>
                    <a class=" " href="Video.html"> 동영상 &nbsp;</a>
                    <a class=" " href="Photo.html"> 포토갤러리 &nbsp;</a>
                    <a class=" " href="Event.html"> 이벤트 </a> </h5>
                </div>
                <div class="col-lg-5 col-md-6">
                    <h5 class="text-light mb-4">CEO. SINRU</h5>
                    <p class="mb-2"><i class="fa fa-map-marker-alt me-3"></i>(61743) 광주광역시 남구 효덕로 277 문헌정보학과</p>
                    <p class="mb-2"><i class="fa fa-phone-alt me-3"></i>Tel. 062-670-2566</p>
                    <p class="mb-2"><i class="fa fa-envelope me-3"></i>sinru@drama.com</p>
                    <div class="d-flex pt-2">
                        <a class="btn btn-outline-light btn-social rounded-circle" href="404.html"><i class="fab fa-twitter"></i></a>
                        <a class="btn btn-outline-light btn-social rounded-circle" href="404.html"><i class="fab fa-facebook-f"></i></a>
                        <a class="btn btn-outline-light btn-social rounded-circle" href="404.html"><i class="fab fa-youtube"></i></a>
                        <a class="btn btn-outline-light btn-social rounded-circle" href="404.html"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
            </div>   
        </div>
    </div>
    
        <div class="container">
            <div class="copyright">
                <div class="row">
                    <div class="col-md-6 text-center text-md-start mb-3 mb-md-0">
                        &copy; <a class="border-bottom" href="#">SINRU</a>, All Right Reserved.
                    </div>
                    <div class="col-md-6 text-center text-md-end">
                        <!--/*** This template is free as long as you keep the footer author’s credit link/attribution link/backlink. If you'd like to use the template without the footer author’s credit link/attribution link/backlink, you can purchase the Credit Removal License from "https://htmlcodex.com/credit-removal". Thank you for your support. ***/-->
                        Designed By <a class="border-bottom" href="https://htmlcodex.com">HTML Codex</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Footer End -->




    <!-- Back to Top -->
    <a href="#" class="btn btn-lg btn-primary btn-lg-square rounded-circle back-to-top"><i class="bi bi-arrow-up"></i></a>


    <!-- JavaScript Libraries -->
    <script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0/dist/js/bootstrap.bundle.min.js"></script>
    <script src="lib/wow/wow.min.js"></script>
    <script src="lib/easing/easing.min.js"></script>
    <script src="lib/waypoints/waypoints.min.js"></script>
    <script src="lib/counterup/counterup.min.js"></script>
    <script src="lib/owlcarousel/owl.carousel.min.js"></script>
    <script src="lib/tempusdominus/js/moment.min.js"></script>
    <script src="lib/tempusdominus/js/moment-timezone.min.js"></script>
    <script src="lib/tempusdominus/js/tempusdominus-bootstrap-4.min.js"></script>

    <!-- Template Javascript -->
    <script src="js/main.js"></script>
</body>

</html>
