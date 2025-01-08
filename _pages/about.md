---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DT工作室</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --primary: #FF4500;
            --secondary: #1A1A1A;
            --light: #FFFFFF;
            --text: #333;
        }

        body {
            font-family: 'Noto Sans SC', sans-serif;
            color: var(--text);
            overflow-x: hidden;
            background-color: var(--light);
        }

        .hero {
            height: 100vh;
            background: var(--primary);
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
        }

        .hero-image {
            position: absolute;
            right: -5%;
            top: 50%;
            transform: translateY(-50%);
            width: 65%;
            height: auto;
            z-index: 1;
        }

        .hero-content {
            position: relative;
            z-index: 2;
            color: var(--light);
            padding-left: 5%;
        }

        .category-section {
            padding: 80px 0;
            background: var(--light);
        }

        .category-card {
            position: relative;
            border-radius: 15px;
            overflow: hidden;
            margin-bottom: 30px;
            aspect-ratio: 1;
        }

        .category-card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .category-card:hover img {
            transform: scale(1.05);
        }

        .category-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            padding: 20px;
            background: linear-gradient(transparent, rgba(0,0,0,0.8));
            color: white;
        }

        .product-showcase {
            background: #f8f8f8;
            padding: 80px 0;
        }

        .product-card {
            background: var(--light);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .product-image {
            width: 100%;
            aspect-ratio: 16/9;
            object-fit: cover;
        }

        .resources-hub {
            background: var(--primary);
            color: var(--light);
            padding: 60px 0;
            margin: 80px 0;
        }

        .review-card {
            background: var(--light);
            border-radius: 15px;
            overflow: hidden;
            margin-bottom: 30px;
        }

        .review-image {
            width: 100%;
            aspect-ratio: 16/9;
            object-fit: cover;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 40px 0;
        }

        .social-links a {
            color: var(--secondary);
            font-size: 24px;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: var(--primary);
        }

        .navbar {
            background: transparent;
            padding: 20px 0;
            transition: all 0.3s ease;
        }

        .navbar.scrolled {
            background: var(--secondary);
            padding: 10px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
            font-weight: bold;
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 3px;
            background: var(--primary);
        }
    </style>
</head>
<body>
    <!-- 导航栏 -->
    <nav class="navbar navbar-expand-lg fixed-top">
        <div class="container">
            <a class="navbar-brand text-white" href="#">DT工作室</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link text-white" href="#categories">分类</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-white" href="#products">产品</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-white" href="#resources">资源</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-white" href="#reviews">测评</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero部分 -->
    <section class="hero">
        <div class="container">
            <div class="row">
                <div class="col-lg-6 hero-content">
                    <h1 class="display-4 fw-bold mb-4">RIDE BEYOND<br>BOUNDARIES</h1>
                    <p class="lead mb-4">突破界限，探索无限可能</p>
                    <button class="btn btn-light btn-lg px-4">立即探索</button>
                </div>
            </div>
        </div>
        <img src="https://source.unsplash.com/random/1200x800?bicycle" alt="Hero Bike" class="hero-image">
    </section>

    <!-- 分类部分 -->
    <section id="categories" class="category-section">
        <div class="container">
            <h2 class="section-title">产品分类</h2>
            <div class="row">
                <div class="col-md-4">
                    <div class="category-card">
                        <img src="https://source.unsplash.com/random/800x800?mountain-bike" alt="Mountain">
                        <div class="category-overlay">
                            <h3>Mountain</h3>
                            <button class="btn btn-outline-light">查看详情</button>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="category-card">
                        <img src="https://source.unsplash.com/random/800x800?commuter-bike" alt="Commuter">
                        <div class="category-overlay">
                            <h3>Commuter</h3>
                            <button class="btn btn-outline-light">查看详情</button>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="category-card">
                        <img src="https://source.unsplash.com/random/800x800?road-bike" alt="Step Through">
                        <div class="category-overlay">
                            <h3>Step Through</h3>
                            <button class="btn btn-outline-light">查看详情</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 资源中心 -->
    <section id="resources" class="resources-hub">
        <div class="container">
            <h2 class="section-title text-white">资源中心</h2>
            <div class="row justify-content-center">
                <div class="col-md-3 text-center">
                    <i class="fas fa-tools fa-3x mb-3"></i>
                    <h4>维修指南</h4>
                </div>
                <div class="col-md-3 text-center">
                    <i class="fas fa-map-marked-alt fa-3x mb-3"></i>
                    <h4>骑行路线</h4>
                </div>
                <div class="col-md-3 text-center">
                    <i class="fas fa-book fa-3x mb-3"></i>
                    <h4>使用手册</h4>
                </div>
                <div class="col-md-3 text-center">
                    <i class="fas fa-video fa-3x mb-3"></i>
                    <h4>视频教程</h4>
                </div>
            </div>
        </div>
    </section>

    <!-- 测评部分 -->
    <section id="reviews" class="py-5">
        <div class="container">
            <h2 class="section-title">开箱测评</h2>
            <div class="row">
                <div class="col-md-4">
                    <div class="review-card">
                        <img src="https://source.unsplash.com/random/800x600?bike-review" class="review-image" alt="测评">
                        <div class="p-3">
                            <h5>全地形测试</h5>
                            <p class="text-muted">探索不同地形下的性能表现</p>
                        </div>
                    </div>
                </div>
                <!-- 可以添加更多测评卡片 -->
            </div>
        </div>
    </section>

    <!-- 社交媒体链接 -->
    <section class="py-5">
        <div class="container text-center">
            <h2 class="section-title">关注我们</h2>
            <div class="social-links">
                <a href="#"><i class="fab fa-youtube"></i></a>
                <a href="#"><i class="fab fa-tiktok"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-facebook"></i></a>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer class="bg-dark text-white py-4">
        <div class="container">
            <div class="row">
                <div class="col-md-3">
                    <h5>关于我们</h5>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-white-50">公司简介</a></li>
                        <li><a href="#" class="text-white-50">联系方式</a></li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h5>产品系列</h5>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-white-50">Mountain</a></li>
                        <li><a href="#" class="text-white-50">Commuter</a></li>
                        <li><a href="#" class="text-white-50">Step Through</a></li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h5>支持服务</h5>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-white-50">维修服务</a></li>
                        <li><a href="#" class="text-white-50">配件购买</a></li>
                        <li><a href="#" class="text-white-50">保修政策</a></li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h5>订阅更新</h5>
                    <p class="text-white-50">获取最新产品信息和优惠资讯</p>
                    <form class="mt-3">
                        <div class="input-group">
                            <input type="email" class="form-control" placeholder="输入邮箱地址">
                            <button class="btn btn-primary">订阅</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.js"></script>
    <script>
        // 初始化AOS动画
        AOS.init({
            duration: 1000,
            once: true
        });

        // 导航栏滚动效果
        window.addEventListener('scroll', function() {
            const nav = document.querySelector('.navbar');
            if (window.scrollY > 50) {
                nav.classList.add('scrolled');
            } else {
                nav.classList.remove('scrolled');
            }
        });
    </script>
</body>
</html> 
