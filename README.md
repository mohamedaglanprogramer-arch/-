<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta name="description"
        content="بلح آل عجلان - أجود أنواع البلح من الوادي والواحات، بأوزان مختلفة وجودة ممتازة.">

    <title>بلح آل عجلان | طعم الطبيعة</title>

    <style>
        /* =========================
           الإعدادات العامة
        ========================= */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Tahoma, Arial, sans-serif;
            background:
                radial-gradient(circle at top, #3d220b 0%, #120904 55%, #080402 100%);
            color: white;
            min-height: 100vh;
            overflow-x: hidden;
        }

        body.no-scroll {
            overflow: hidden;
        }

        button,
        a {
            font-family: inherit;
        }

        /* =========================
           الخلفية
        ========================= */

        .page-bg {
            position: fixed;
            inset: 0;
            z-index: -2;

            background-image:
                linear-gradient(
                    rgba(15, 7, 2, 0.68),
                    rgba(15, 7, 2, 0.85)
                ),
                url("https://png.pngtree.com/background/20250122/original/pngtree-dates-sweet-food-islamic-holidays-decoration-ramadan-kareem-eid-mubarak-background-picture-image_16233606.jpg");

            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }

        .page-bg::after {
            content: "";
            position: absolute;
            inset: 0;

            background:
                radial-gradient(
                    circle at 50% 20%,
                    rgba(246, 196, 83, 0.12),
                    transparent 35%
                );
        }

        /* =========================
           الهيدر
        ========================= */

        header {
            width: 100%;
            padding: 22px 6%;

            display: flex;
            justify-content: space-between;
            align-items: center;

            border-bottom: 1px solid rgba(246, 196, 83, 0.15);

            background: rgba(10, 5, 2, 0.35);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);

            position: relative;
            z-index: 10;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 10px;

            color: #f6c453;
            font-size: 22px;
            font-weight: bold;
        }

        .logo-icon {
            width: 42px;
            height: 42px;

            display: flex;
            align-items: center;
            justify-content: center;

            border-radius: 50%;

            background:
                linear-gradient(135deg, #f6c453, #a96813);

            color: #241205;
            font-size: 22px;

            box-shadow:
                0 5px 20px rgba(246, 196, 83, 0.2);
        }

        .header-status {
            display: flex;
            align-items: center;
            gap: 8px;

            font-size: 14px;
            color: #e9e1d5;
        }

        .status-dot {
            width: 9px;
            height: 9px;
            border-radius: 50%;
            background: #25d366;

            box-shadow:
                0 0 12px rgba(37, 211, 102, 0.8);
        }

        /* =========================
           القسم الرئيسي
        ========================= */

        .hero {
            min-height: calc(100vh - 87px);

            display: flex;
            justify-content: center;
            align-items: center;

            padding: 60px 20px 80px;
        }

        .hero-content {
            width: 100%;
            max-width: 850px;

            text-align: center;

            padding: 55px 35px;

            background:
                linear-gradient(
                    145deg,
                    rgba(255, 255, 255, 0.08),
                    rgba(255, 255, 255, 0.025)
                );

            border: 1px solid rgba(246, 196, 83, 0.25);

            border-radius: 35px;

            backdrop-filter: blur(14px);
            -webkit-backdrop-filter: blur(14px);

            box-shadow:
                0 30px 80px rgba(0, 0, 0, 0.5);

            animation: heroShow 0.9s ease;
        }

        .hero-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;

            padding: 9px 18px;

            margin-bottom: 22px;

            border-radius: 50px;

            color: #f6c453;

            background: rgba(246, 196, 83, 0.1);

            border: 1px solid rgba(246, 196, 83, 0.25);

            font-size: 14px;
            font-weight: bold;
        }

        .hero h1 {
            font-size: clamp(42px, 7vw, 76px);

            color: #f6c453;

            margin-bottom: 18px;

            text-shadow:
                0 5px 25px rgba(0, 0, 0, 0.7);
        }

        .hero h1 span {
            color: white;
        }

        .hero p {
            max-width: 650px;
            margin: auto;

            color: #eee4d8;

            font-size: clamp(18px, 2.5vw, 23px);

            line-height: 1.9;
        }

        .hero-buttons {
            margin-top: 32px;

            display: flex;
            justify-content: center;
            align-items: center;
            gap: 14px;

            flex-wrap: wrap;
        }

        .main-btn {
            border: none;

            padding: 15px 30px;

            border-radius: 50px;

            background:
                linear-gradient(
                    135deg,
                    #f6c453,
                    #bd7c17
                );

            color: #241205;

            font-size: 18px;
            font-weight: bold;

            cursor: pointer;

            box-shadow:
                0 10px 30px rgba(201, 149, 46, 0.25);

            transition: 0.3s;
        }

        .main-btn:hover {
            transform: translateY(-4px);

            box-shadow:
                0 15px 35px rgba(201, 149, 46, 0.4);
        }

        .whatsapp-main {
            display: inline-flex;
            align-items: center;
            gap: 8px;

            padding: 14px 25px;

            border-radius: 50px;

            background: rgba(37, 211, 102, 0.12);

            border: 1px solid rgba(37, 211, 102, 0.4);

            color: #62ed93;

            text-decoration: none;

            font-size: 17px;
            font-weight: bold;

            transition: 0.3s;
        }

        .whatsapp-main:hover {
            background: #25d366;
            color: white;
            transform: translateY(-4px);
        }

        /* =========================
           مميزات
        ========================= */

        .features {
            display: grid;

            grid-template-columns:
                repeat(3, 1fr);

            gap: 15px;

            max-width: 750px;

            margin: 45px auto 0;
        }

        .feature {
            padding: 18px 12px;

            border-radius: 20px;

            background: rgba(0, 0, 0, 0.22);

            border: 1px solid rgba(255, 255, 255, 0.08);

            transition: 0.3s;
        }

        .feature:hover {
            transform: translateY(-5px);

            border-color:
                rgba(246, 196, 83, 0.3);
        }

        .feature-icon {
            font-size: 28px;
            margin-bottom: 8px;
        }

        .feature strong {
            display: block;

            color: #f6c453;

            margin-bottom: 5px;
        }

        .feature small {
            color: #d9d0c5;
        }

        /* =========================
           نافذة المنتجات
        ========================= */

        .products-modal {
            position: fixed;
            inset: 0;

            z-index: 9999;

            display: none;

            padding: 25px 15px;

            background:
                rgba(6, 3, 1, 0.94);

            overflow-y: auto;
        }

        .products-modal.show {
            display: block;

            animation: fadeIn 0.3s ease;
        }

        .modal-container {
            width: 100%;
            max-width: 1100px;

            margin: auto;
        }

        /* =========================
           رأس المنتجات
        ========================= */

        .modal-header {
            display: flex;
            align-items: center;
            justify-content: space-between;

            gap: 20px;

            padding: 10px 5px 30px;

            position: sticky;
            top: 0;

            z-index: 5;

            background:
                linear-gradient(
                    rgba(6, 3, 1, 0.98),
                    rgba(6, 3, 1, 0.9),
                    transparent
                );
        }

        .modal-title h2 {
            color: #f6c453;

            font-size: 32px;

            margin-bottom: 5px;
        }

        .modal-title p {
            color: #bfb4a8;
            font-size: 14px;
        }

        .close-btn {
            flex-shrink: 0;

            width: 48px;
            height: 48px;

            border: 1px solid
                rgba(246, 196, 83, 0.3);

            border-radius: 50%;

            background: #a96e17;

            color: white;

            font-size: 28px;

            cursor: pointer;

            transition: 0.3s;
        }

        .close-btn:hover {
            background: #e1aa39;
            transform: rotate(90deg);
        }

        /* =========================
           شبكة المنتجات
        ========================= */

        .products-grid {
            display: grid;

            grid-template-columns:
                repeat(2, 1fr);

            gap: 24px;

            padding-bottom: 50px;
        }

        .product-card {
            overflow: hidden;

            background:
                linear-gradient(
                    145deg,
                    rgba(255, 255, 255, 0.09),
                    rgba(255, 255, 255, 0.035)
                );

            border: 1px solid
                rgba(246, 196, 83, 0.2);

            border-radius: 28px;

            box-shadow:
                0 20px 50px rgba(0, 0, 0, 0.35);

            transition: 0.35s;

            animation: cardShow 0.6s ease both;
        }

        .product-card:hover {
            transform: translateY(-7px);

            border-color:
                rgba(246, 196, 83, 0.45);

            box-shadow:
                0 25px 60px rgba(0, 0, 0, 0.5);
        }

        .product-image-box {
            position: relative;

            width: 100%;

            padding: 18px;

            background:
                radial-gradient(
                    circle,
                    rgba(246, 196, 83, 0.12),
                    transparent 65%
                );

            text-align: center;
        }

        .product-image {
            width: 100%;
            height: 300px;

            object-fit: contain;

            border-radius: 20px;

            cursor: zoom-in;

            filter:
                drop-shadow(
                    0 15px 25px rgba(0, 0, 0, 0.45)
                );

            transition: 0.4s;
        }

        .product-card:hover .product-image {
            transform: scale(1.035);
        }

        .product-badge {
            position: absolute;

            top: 25px;
            right: 25px;

            padding: 7px 13px;

            border-radius: 30px;

            background:
                linear-gradient(
                    135deg,
                    #f6c453,
                    #a96813
                );

            color: #241205;

            font-size: 12px;
            font-weight: bold;
        }

        .product-content {
            padding: 5px 22px 24px;
        }

        .product-title {
            color: #f6c453;

            font-size: 25px;

            margin-bottom: 18px;
        }

        .product-details {
            display: flex;

            flex-direction: column;

            gap: 10px;
        }

        .detail {
            display: flex;

            align-items: center;

            gap: 10px;

            padding: 11px 13px;

            border-radius: 14px;

            background: rgba(0, 0, 0, 0.18);

            color: #e8dfd5;

            font-size: 15px;
        }

        .detail-icon {
            width: 30px;
            height: 30px;

            min-width: 30px;

            display: flex;

            align-items: center;
            justify-content: center;

            border-radius: 50%;

            background:
                rgba(246, 196, 83, 0.12);
        }

        .detail strong {
            color: #f6c453;
        }

        .order-btn {
            width: 100%;

            display: flex;

            align-items: center;
            justify-content: center;

            gap: 10px;

            margin-top: 16px;

            padding: 14px;

            border-radius: 15px;

            background:
                linear-gradient(
                    135deg,
                    #25d366,
                    #169b4a
                );

            color: white;

            text-decoration: none;

            font-weight: bold;
            font-size: 16px;

            box-shadow:
                0 8px 22px rgba(37, 211, 102, 0.18);

            transition: 0.3s;
        }

        .order-btn:hover {
            transform: translateY(-3px);

            box-shadow:
                0 12px 28px rgba(37, 211, 102, 0.3);
        }

        .product-note {
            text-align: center;

            color: #d8b55c;

            font-size: 13px;

            margin-top: 14px;

            line-height: 1.7;
        }

        /* =========================
           تكبير الصور
        ========================= */

        .image-viewer {
            position: fixed;
            inset: 0;

            z-index: 20000;

            display: none;

            align-items: center;
            justify-content: center;

            padding: 25px;

            background:
                rgba(0, 0, 0, 0.95);
        }

        .image-viewer.show {
            display: flex;
        }

        .viewer-image {
            max-width: 95%;
            max-height: 90vh;

            object-fit: contain;

            border-radius: 18px;

            box-shadow:
                0 20px 70px rgba(0, 0, 0, 0.7);

            animation: zoomImage 0.3s ease;
        }

        .viewer-close {
            position: fixed;

            top: 20px;
            right: 20px;

            width: 48px;
            height: 48px;

            border: none;

            border-radius: 50%;

            background: #bd7c17;

            color: white;

            font-size: 28px;

            cursor: pointer;
        }

        /* =========================
           زر واتساب عائم
        ========================= */

        .floating-whatsapp {
            position: fixed;

            left: 20px;
            bottom: 20px;

            z-index: 1000;

            width: 58px;
            height: 58px;

            display: flex;
            align-items: center;
            justify-content: center;

            border-radius: 50%;

            background: #25d366;

            color: white;

            text-decoration: none;

            font-size: 28px;

            box-shadow:
                0 8px 25px rgba(0, 0, 0, 0.4);

            animation: pulse 2s infinite;
        }

        /* =========================
           زر أعلى الصفحة
        ========================= */

        .top-btn {
            position: fixed;

            right: 20px;
            bottom: 20px;

            z-index: 1000;

            width: 45px;
            height: 45px;

            display: flex;

            align-items: center;
            justify-content: center;

            border: 1px solid
                rgba(246, 196, 83, 0.3);

            border-radius: 50%;

            background:
                rgba(20, 10, 4, 0.8);

            color: #f6c453;

            cursor: pointer;

            opacity: 0;
            visibility: hidden;

            transition: 0.3s;
        }

        .top-btn.show {
            opacity: 1;
            visibility: visible;
        }

        /* =========================
           الفوتر
        ========================= */

        footer {
            padding: 30px 20px;

            text-align: center;

            border-top:
                1px solid rgba(246, 196, 83, 0.12);

            color: #a99e91;

            font-size: 13px;

            background:
                rgba(0, 0, 0, 0.25);
        }

        footer strong {
            color: #f6c453;
        }

        /* =========================
           الحركات
        ========================= */

        @keyframes heroShow {
            from {
                opacity: 0;
                transform: translateY(30px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }

            to {
                opacity: 1;
            }
        }

        @keyframes cardShow {
            from {
                opacity: 0;
                transform: translateY(20px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes zoomImage {
            from {
                opacity: 0;
                transform: scale(0.8);
            }

            to {
                opacity: 1;
                transform: scale(1);
            }
        }

        @keyframes pulse {
            0% {
                box-shadow:
                    0 0 0 0 rgba(37, 211, 102, 0.45);
            }

            70% {
                box-shadow:
                    0 0 0 14px rgba(37, 211, 102, 0);
            }

            100% {
                box-shadow:
                    0 0 0 0 rgba(37, 211, 102, 0);
            }
        }

        /* =========================
           الموبايل
        ========================= */

        @media (max-width: 700px) {

            header {
                padding: 16px 18px;
            }

            .logo {
                font-size: 17px;
            }

            .logo-icon {
                width: 36px;
                height: 36px;
                font-size: 18px;
            }

            .header-status {
                font-size: 11px;
            }

            .hero {
                padding:
                    35px 12px 55px;
            }

            .hero-content {
                padding: 40px 20px;

                border-radius: 25px;
            }

            .hero h1 {
                font-size: 40px;
            }

            .hero p {
                font-size: 17px;
            }

            .hero-buttons {
                flex-direction: column;
            }

            .main-btn,
            .whatsapp-main {
                width: 100%;
                justify-content: center;
            }

            .features {
                grid-template-columns: 1fr;

                max-width: 320px;
            }

            .products-grid {
                grid-template-columns: 1fr;

                gap: 18px;
            }

            .modal-header {
                padding-bottom: 22px;
            }

            .modal-title h2 {
                font-size: 25px;
            }

            .product-image {
                height: 250px;
            }

            .product-content {
                padding:
                    5px 16px 20px;
            }

            .product-title {
                font-size: 22px;
            }

            .floating-whatsapp {
                left: 15px;
                bottom: 15px;

                width: 54px;
                height: 54px;
            }

            .top-btn {
                right: 15px;
                bottom: 15px;

                width: 42px;
                height: 42px;
            }
        }
    </style>
</head>

<body>

    <div class="page-bg"></div>

    <!-- =========================
         الهيدر
    ========================== -->

    <header>

        <div class="logo">

            <div class="logo-icon">
                🌴
            </div>

            <span>
                بلح آل عجلان
            </span>

        </div>

        <div class="header-status">

            <span class="status-dot"></span>

            متوفر للطلب

        </div>

    </header>


    <!-- =========================
         الصفحة الرئيسية
    ========================== -->

    <main class="hero">

        <div class="hero-content">

            <div class="hero-badge">
                ⭐ جودة نختارها لك
            </div>

            <h1>
                بلح <span>آل عجلان</span>
            </h1>

            <p>
                بلح طبيعي بمذاق غني وحلاوة لا تُقاوم
                <br>
                من الوادي والواحات إلى بيتك 🌴
            </p>


            <div class="hero-buttons">

                <button
                    class="main-btn"
                    onclick="openProducts()"
                >
                    🛍️ اكتشف المنتجات
                </button>


                <a
                    class="whatsapp-main"
                    href="https://wa.me/201141013558?text=مرحباً، أريد الاستفسار عن منتجات بلح آل عجلان"
                    target="_blank"
                >
                    🟢 تواصل معنا
                </a>

            </div>


            <!-- المميزات -->

            <div class="features">

                <div class="feature">

                    <div class="feature-icon">
                        🌴
                    </div>

                    <strong>
                        طبيعي
                    </strong>

                    <small>
                        طعم غني ومميز
                    </small>

                </div>


                <div class="feature">

                    <div class="feature-icon">
                        ⭐
                    </div>

                    <strong>
                        جودة ممتازة
                    </strong>

                    <small>
                        نهتم بكل حبة
                    </small>

                </div>


                <div class="feature">

                    <div class="feature-icon">
                        📦
                    </div>

                    <strong>
                        أوزان متنوعة
                    </strong>

                    <small>
                        للأفراد والجملة
                    </small>

                </div>

            </div>

        </div>

    </main>


    <!-- =========================
         نافذة المنتجات
    ========================== -->

    <section
        class="products-modal"
        id="productsModal"
    >

        <div class="modal-container">


            <div class="modal-header">

                <div class="modal-title">

                    <h2>
                        🌴 منتجاتنا
                    </h2>

                    <p>
                        اختر الوزن المناسب وتواصل معنا مباشرة
                    </p>

                </div>


                <button
                    class="close-btn"
                    onclick="closeProducts()"
                    aria-label="إغلاق"
                >
                    ×
                </button>

            </div>


            <div class="products-grid">


                <!-- =========================
                     المنتج 1
                ========================== -->

                <article class="product-card">

                    <div class="product-image-box">

                        <span class="product-badge">
                            الأكثر طلبًا
                        </span>

                        <img
                            class="product-image"
                            src="https://chatgpt.com/backend-api/estuary/public_content/enc/eyJpZCI6Im1fNmE3Y2FlZmNmY2Y0ODE5MTkwMGY1NDJhNzY4ZjA0MWY6ZmlsZV8wMDAwMDAwMDY0M2M4MWY0YmJjYmIxMGIwMjJiMjVhMyIsImdpem1vX2lkIjpudWxsLCJ3aWQiOm51bGwsIm9pZCI6bnVsbCwic2lkIjpudWxsLCJjcyI6bnVsbCwiZm4iOm51bGwsImNkIjpudWxsLCJ0cyI6IjIwNjc3IiwicCI6InB5aSIsImNpZCI6IjEiLCJzaWciOiI4YmM5NzRkMjY0NDNiNDI1NzNmMWYxM2RkMTk3ZTA0ZWFjOGVjYjA3MTA3MmY1NDEwYzNkMmEwY2JmMjc3ZjRmIiwidiI6IjAiLCJjZG4iOm51bGwsImNwIjpudWxsLCJtYSI6bnVsbH0="
                            alt="بلح آل عجلان 10 كيلو"
                            onclick="zoomImage(this.src)"
                        >

                    </div>


                    <div class="product-content">

                        <h3 class="product-title">
                            🌴 بلح العجلان
                        </h3>


                        <div class="product-details">

                            <div class="detail">

                                <span class="detail-icon">
                                    ⚖️
                                </span>

                                الوزن:
                                <strong>
                                    10 كيلو
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    📍
                                </span>

                                النوع:
                                <strong>
                                    الوادي والواحات
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    ⭐
                                </span>

                                الجودة:
                                <strong>
                                    أجود أنواع البلح
                                </strong>

                            </div>

                        </div>


                        <a
                            class="order-btn"
                            href="https://wa.me/201141013558?text=مرحباً، أريد طلب بلح آل عجلان وزن 10 كيلو"
                            target="_blank"
                        >
                            🟢 اطلب هذا المنتج
                        </a>


                        <p class="product-note">
                            طعم طبيعي • جودة ممتازة • حلاوة مميزة
                        </p>

                    </div>

                </article>


                <!-- =========================
                     المنتج 2
                ========================== -->

                <article class="product-card">

                    <div class="product-image-box">

                        <span class="product-badge">
                            اختيار ممتاز
                        </span>

                        <img
                            class="product-image"
                            src="https://chatgpt.com/backend-api/estuary/public_content/enc/eyJpZCI6Im1fNmE3Y2IwMTQ3ZDkwODE5MWI3MDU5NzYxNmM2ZDBjZDk6ZmlsZV8wMDAwMDAwMDNhMmM4MWY0YTBjYmEzZWU5ZWVjOTk2ZiIsImdpem1vX2lkIjpudWxsLCJ3aWQiOm51bGwsIm9pZCI6bnVsbCwic2lkIjpudWxsLCJjcyI6bnVsbCwiZm4iOm51bGwsImNkIjpudWxsLCJ0cyI6IjIwNjc3IiwicCI6InB5aSIsImNpZCI6IjEiLCJzaWciOiI1YjU5OGIzNjIwYTlmMjIxZjU5NmI5YTEyOWQ0MWFkYjA5OTU5MzMzYTMwNTk0MmIyNTBjZDkzZDhlYzU2OTViIiwidiI6IjAiLCJjZG4iOm51bGwsImNwIjpudWxsLCJtYSI6bnVsbH0="
                            alt="بلح آل عجلان 5 كيلو"
                            onclick="zoomImage(this.src)"
                        >

                    </div>


                    <div class="product-content">

                        <h3 class="product-title">
                            🌴 بلح العجلان
                        </h3>


                        <div class="product-details">

                            <div class="detail">

                                <span class="detail-icon">
                                    ⚖️
                                </span>

                                الوزن:
                                <strong>
                                    5 كيلو
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    📍
                                </span>

                                النوع:
                                <strong>
                                    الوادي والواحات
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    ⭐
                                </span>

                                الجودة:
                                <strong>
                                    أجود أنواع البلح
                                </strong>

                            </div>

                        </div>


                        <a
                            class="order-btn"
                            href="https://wa.me/201141013558?text=مرحباً، أريد طلب بلح آل عجلان وزن 5 كيلو"
                            target="_blank"
                        >
                            🟢 اطلب هذا المنتج
                        </a>


                        <p class="product-note">
                            طعم طبيعي • جودة ممتازة • حلاوة مميزة
                        </p>

                    </div>

                </article>


                <!-- =========================
                     المنتج 3
                ========================== -->

                <article class="product-card">

                    <div class="product-image-box">

                        <span class="product-badge">
                            جملة
                        </span>

                        <img
                            class="product-image"
                            src="https://chatgpt.com/backend-api/estuary/public_content/enc/eyJpZCI6Im1fNmE3Y2FhYjRhOTQ4ODE5MTkyNjcwMjc2YWM0NzdkZWU6ZmlsZV8wMDAwMDAwMGZmMWM4MWY0YTAzNzE0YzRhZWIyMjExYSIsImdpem1vX2lkIjpudWxsLCJ3aWQiOm51bGwsIm9pZCI6bnVsbCwic2lkIjpudWxsLCJjcyI6bnVsbCwiZm4iOm51bGwsImNkIjpudWxsLCJ0cyI6IjIwNjc3IiwicCI6InB5aSIsImNpZCI6IjEiLCJzaWciOiJkNjA0ZmFjMmYxYmFmYjQwZDY5ZDE3MzhjZDAzN2ExY2ZhOTdmMjg1ODJiMDU1OTRjOGY0MTRiYjQ5ZmEzZDkwIiwidiI6IjAiLCJjZG4iOm51bGwsImNwIjpudWxsLCJtYSI6bnVsbH0="
                            alt="بلح آل عجلان 2200 كيلو"
                            onclick="zoomImage(this.src)"
                        >

                    </div>


                    <div class="product-content">

                        <h3 class="product-title">
                            🌴 بلح العجلان
                        </h3>


                        <div class="product-details">

                            <div class="detail">

                                <span class="detail-icon">
                                    ⚖️
                                </span>

                                الوزن:
                                <strong>
                                    2,200 كيلو
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    📍
                                </span>

                                النوع:
                                <strong>
                                    الوادي والواحات
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    📦
                                </span>

                                مناسب:
                                <strong>
                                    للطلبات الكبيرة
                                </strong>

                            </div>

                        </div>


                        <a
                            class="order-btn"
                            href="https://wa.me/201141013558?text=مرحباً، أريد الاستفسار عن بلح آل عجلان وزن 2200 كيلو"
                            target="_blank"
                        >
                            🟢 استفسر عن المنتج
                        </a>


                        <p class="product-note">
                            للطلبات الكبيرة والجملة
                        </p>

                    </div>

                </article>


                <!-- =========================
                     المنتج 4
                ========================== -->

                <article class="product-card">

                    <div class="product-image-box">

                        <span class="product-badge">
                            جملة
                        </span>

                        <img
                            class="product-image"
                            src="https://chatgpt.com/backend-api/estuary/public_content/enc/eyJpZCI6Im1fNmE3Y2FkMTlmZmI0ODE5MWE2OGI4OTM3NmNkZDZlZTg6ZmlsZV8wMDAwMDAwMDgzZTA4MjBhODkyMGY0ZmExYmUzNzQ3NCIsImdpem1vX2lkIjpudWxsLCJ3aWQiOm51bGwsIm9pZCI6bnVsbCwic2lkIjpudWxsLCJjcyI6bnVsbCwiZm4iOm51bGwsImNkIjpudWxsLCJ0cyI6IjIwNjc3IiwicCI6InB5aSIsImNpZCI6IjEiLCJzaWciOiJkMGVmYmE2OGYxMTg3OTZjYTdjMWZiOTQyMmJhODU5MmU3ZGU2NWFkMWU3NDI5ZjQzOTE3YWIzMDcwNzA2YzhmIiwidiI6IjAiLCJjZG4iOm51bGwsImNwIjpudWxsLCJtYSI6bnVsbH0="
                            alt="بلح آل عجلان 1400 كيلو"
                            onclick="zoomImage(this.src)"
                        >

                    </div>


                    <div class="product-content">

                        <h3 class="product-title">
                            🌴 بلح العجلان
                        </h3>


                        <div class="product-details">

                            <div class="detail">

                                <span class="detail-icon">
                                    ⚖️
                                </span>

                                الوزن:
                                <strong>
                                    1400 كيلو
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    📍
                                </span>

                                النوع:
                                <strong>
                                    الوادي والواحات
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    📦
                                </span>

                                مناسب:
                                <strong>
                                    للطلبات الكبيرة
                                </strong>

                            </div>

                        </div>


                        <a
                            class="order-btn"
                            href="https://wa.me/201141013558?text=مرحباً، أريد الاستفسار عن بلح آل عجلان وزن 1400 كيلو"
                            target="_blank"
                        >
                            🟢 استفسر عن المنتج
                        </a>


                        <p class="product-note">
                            للطلبات الكبيرة والجملة
                        </p>

                    </div>

                </article>


                <!-- =========================
                     المنتج 5
                ========================== -->

                <article class="product-card">

                    <div class="product-image-box">

                        <span class="product-badge">
                            حجم صغير
                        </span>

                        <img
                            class="product-image"
                            src="https://chatgpt.com/backend-api/estuary/public_content/enc/eyJpZCI6Im1fNmE3Y2FlMWMwMTJjODE5MTg5ZmRkYjVkYWI3NTZlY2I6ZmlsZV8wMDAwMDAwMDdiNjQ4MWY0YjMzYmE3YzU3NGQxNTE4NSIsImdpem1vX2lkIjpudWxsLCJ3aWQiOm51bGwsIm9pZCI6bnVsbCwic2lkIjpudWxsLCJjcyI6bnVsbCwiZm4iOm51bGwsImNkIjpudWxsLCJ0cyI6IjIwNjc3IiwicCI6InB5aSIsImNpZCI6IjEiLCJzaWciOiI3NzlhNDI1NWIzNWQ4YzEwYWYwODliNWM4MWI4YmYyNTYwMmI3YWEzNGFmNmUwYTk2YzliYjFmYTZiMDEwM2U5IiwidiI6IjAiLCJjZG4iOm51bGwsImNwIjpudWxsLCJtYSI6bnVsbH0="
                            alt="بلح آل عجلان 700 جرام"
                            onclick="zoomImage(this.src)"
                        >

                    </div>


                    <div class="product-content">

                        <h3 class="product-title">
                            🌴 بلح العجلان
                        </h3>


                        <div class="product-details">

                            <div class="detail">

                                <span class="detail-icon">
                                    ⚖️
                                </span>

                                الوزن:
                                <strong>
                                    700 جرام
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    📍
                                </span>

                                النوع:
                                <strong>
                                    الوادي والواحات
                                </strong>

                            </div>


                            <div class="detail">

                                <span class="detail-icon">
                                    ⭐
                                </span>

                                الجودة:
                                <strong>
                                    أجود أنواع البلح
                                </strong>

                            </div>

                        </div>


                        <a
                            class="order-btn"
                            href="https://wa.me/201141013558?text=مرحباً، أريد طلب بلح آل عجلان وزن 700 جرام"
                            target="_blank"
                        >
                            🟢 اطلب هذا المنتج
                        </a>


                        <p class="product-note">
                            طعم طبيعي • جودة ممتازة • حلاوة مميزة
                        </p>

                    </div>

                </article>

            </div>

        </div>

    </section>


    <!-- =========================
         تكبير الصورة
    ========================== -->

    <div
        class="image-viewer"
        id="imageViewer"
        onclick="closeZoom(event)"
    >

        <button
            class="viewer-close"
            onclick="closeZoom()"
        >
            ×
        </button>

        <img
            class="viewer-image"
            id="viewerImage"
            src=""
            alt="صورة المنتج"
        >

    </div>


    <!-- =========================
         واتساب عائم
    ========================== -->

    <a
        class="floating-whatsapp"
        href="https://wa.me/201141013558?text=مرحباً، أريد الاستفسار عن منتجات بلح آل عجلان"
        target="_blank"
        aria-label="واتساب"
    >
        🟢
    </a>


    <!-- =========================
         زر لأعلى
    ========================== -->

    <button
        class="top-btn"
        id="topBtn"
        onclick="window.scrollTo({top: 0, behavior: 'smooth'})"
        aria-label="العودة للأعلى"
    >
        ↑
    </button>


    <!-- =========================
         الفوتر
    ========================== -->

    <footer>

        <p>
            🌴 <strong>بلح آل عجلان</strong>
            — طعم الطبيعة في كل حبة
        </p>

        <p style="margin-top: 8px;">
            للتواصل والطلبات عبر واتساب
        </p>

    </footer>


    <!-- =========================
         JavaScript
    ========================== -->

    <script>

        const modal =
            document.getElementById("productsModal");

        const viewer =
            document.getElementById("imageViewer");

        const viewerImage =
            document.getElementById("viewerImage");

        const topBtn =
            document.getElementById("topBtn");


        /* فتح المنتجات */

        function openProducts() {

            modal.classList.add("show");

            document.body.classList.add("no-scroll");

            modal.scrollTop = 0;
        }


        /* إغلاق المنتجات */

        function closeProducts() {

            modal.classList.remove("show");

            document.body.classList.remove("no-scroll");
        }


        /* تكبير الصورة */

        function zoomImage(src) {

            viewerImage.src = src;

            viewer.classList.add("show");

            document.body.classList.add("no-scroll");
        }


        /* إغلاق الصورة */

        function closeZoom(event) {

            if (
                !event ||
                event.target === viewer ||
                event.target === document.querySelector(".viewer-close")
            ) {

                viewer.classList.remove("show");

                document.body.classList.remove("no-scroll");

            }
        }


        /* الضغط على ESC */

        document.addEventListener(
            "keydown",
            function (event) {

                if (event.key === "Escape") {

                    closeProducts();

                    viewer.classList.remove("show");

                    document.body.classList.remove("no-scroll");
                }

            }
        );


        /* الضغط على خلفية نافذة المنتجات */

        modal.addEventListener(
            "click",
            function (event) {

                if (event.target === modal) {

                    closeProducts();

                }

            }
        );


        /* زر العودة للأعلى */

        window.addEventListener(
            "scroll",
            function () {

                if (window.scrollY > 400) {

                    topBtn.classList.add("show");

                } else {

                    topBtn.classList.remove("show");

                }

            }
        );

    </script>

</body>

</html>
