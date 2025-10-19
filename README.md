<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vinh Danh Học Sinh Xuất Sắc - 20 Năm học</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;800;900&display=swap" rel="stylesheet">
    <style>
        /* ===== RESET & BASE STYLES ===== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Quicksand', sans-serif;
        }
        
        :root {
            --primary-color: #1a2a6c;
            --secondary-color: #2A4D9B;
            --accent-color: #3a6dc9;
            --gold-color: #FFD700;
            --gold-light: #FFEC8B;
            --orange-color: #FF8C42;
            --text-light: #F8F6F2;
            --text-dark: #0a192f;
            --shadow-light: rgba(255, 255, 255, 0.1);
            --shadow-dark: rgba(0, 0, 0, 0.3);
            --gradient-primary: linear-gradient(135deg, #1a2a6c, #2A4D9B, #3a6dc9);
            --gradient-gold: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            --gradient-card: linear-gradient(135deg, rgba(58, 109, 201, 0.8), rgba(42, 77, 155, 0.9));
            --gradient-orange: linear-gradient(135deg, rgba(255, 140, 66, 0.9), rgba(232, 106, 51, 0.9));
            --gradient-green: linear-gradient(135deg, rgba(76, 175, 80, 0.9), rgba(56, 142, 60, 0.9));
            --transition-slow: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            --transition-medium: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            --transition-fast: all 0.3s ease;
        }
        
        body {
            background: var(--gradient-primary);
            color: var(--text-light);
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
        }
        
        /* ===== BACKGROUND EFFECTS ===== */
        .dynamic-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -3;
            background: linear-gradient(-45deg, #1a2a6c, #2A4D9B, #3a6dc9, #4d8ae6, #1a2a6c);
            background-size: 400% 400%;
            animation: gradientShift 20s ease infinite;
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -2;
            overflow: hidden;
        }
        
        .particle {
            position: absolute;
            background: radial-gradient(circle, rgba(255, 215, 0, 0.7) 0%, rgba(255, 215, 0, 0) 70%);
            border-radius: 50%;
            animation: particleFloat 25s infinite linear;
            filter: blur(1px);
        }
        
        @keyframes particleFloat {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        .floating-elements {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .floating-element {
            position: absolute;
            background: rgba(255, 215, 0, 0.1);
            border-radius: 50%;
            animation: float 25s infinite linear;
            box-shadow: 0 0 30px rgba(255, 215, 0, 0.3);
        }
        
        @keyframes float {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-1000px) rotate(360deg);
                opacity: 0;
            }
        }
        
        .spotlight {
            position: fixed;
            width: 300px;
            height: 300px;
            border-radius: 50%;
            background: radial-gradient(circle, rgba(255,215,0,0.2) 0%, rgba(255,215,0,0) 70%);
            pointer-events: none;
            z-index: -1;
            animation: spotlightMove 20s infinite linear;
            filter: blur(15px);
        }
        
        @keyframes spotlightMove {
            0% { transform: translate(10vw, 10vh); }
            25% { transform: translate(80vw, 30vh); }
            50% { transform: translate(40vw, 70vh); }
            75% { transform: translate(70vw, 50vh); }
            100% { transform: translate(10vw, 10vh); }
        }
        
        /* ===== CONTAINER & LAYOUT ===== */
        .container {
            width: 100%;
            min-height: 100vh;
            background: rgba(10, 25, 47, 0.85);
            backdrop-filter: blur(20px);
            position: relative;
            overflow: hidden;
        }
        
        .container::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><defs><pattern id="grain" width="100" height="100" patternUnits="userSpaceOnUse"><circle cx="50" cy="50" r="1" fill="rgba(255,255,255,0.03)"/></pattern></defs><rect width="100" height="100" fill="url(%23grain)"/></svg>'),
                linear-gradient(135deg, transparent 0%, rgba(255, 215, 0, 0.05) 100%);
            pointer-events: none;
            z-index: 0;
        }
        
        /* ===== HEADER STYLES ===== */
        header {
            background: 
                linear-gradient(135deg, rgba(42, 77, 155, 0.9), rgba(58, 109, 201, 0.8)),
                url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><path d="M0,0 L100,0 L100,100 Z" fill="rgba(255,215,0,0.1)"/></svg>');
            color: var(--text-light);
            text-align: center;
            padding: 120px 20px 100px;
            position: relative;
            overflow: hidden;
            border-bottom: 1px solid rgba(255, 215, 0, 0.3);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        header::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 80%, rgba(255, 215, 0, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 215, 0, 0.1) 0%, transparent 50%);
            z-index: 1;
        }
        
        .header-content {
            position: relative;
            z-index: 2;
        }
        
        .header-logo {
            position: absolute;
            top: 30px;
            left: 50px;
            height: 180px;
            width: auto;
            z-index: 10;
            filter: drop-shadow(0 0 15px rgba(255, 215, 0, 0.7));
            transition: var(--transition-medium);
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            padding: 10px;
            backdrop-filter: blur(10px);
        }
        
        .header-logo:hover {
            transform: scale(1.1) rotate(5deg);
            filter: drop-shadow(0 0 20px rgba(255, 215, 0, 0.9));
        }
        
        .header-icon {
            font-size: 4rem;
            color: var(--gold-color);
            margin-bottom: 30px;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.7);
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }
        
        /* CHỈNH SỬA: Làm chữ VINH DANH to hơn */
        .glowing-text {
            font-size: 7rem; /* Tăng từ 5rem lên 7rem */
            margin-bottom: 20px;
            text-shadow: 0 0 10px rgba(254 , 224 , 255 , 0 ), 0 0 20px rgba(255, 215, 0, 0.5), 0 0 30px rgba(255, 215, 0, 0 );
            position: relative;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
            letter-spacing: 2px;
            animation: glow 3s ease-in-out infinite alternate;
            font-family: 'Playfair Display', serif;
        }
        
        @keyframes glow {
            0% {
                text-shadow: 0 0 10px rgba(255, 215, 0, 0), 0 0 20px rgba(255, 215, 0, 0.5), 0 0 30px rgba(255, 215, 0, 0 );
            }
            100% {
                text-shadow: 0 0 15px rgba(255, 215, 0, 0.8), 0 0 25px rgba(255, 215, 0, 0.6), 0 0 35px rgba(255, 215, 0, 0.4);
            }
        }
        
        .subtitle {
            font-size: 2.2rem;
            margin-bottom: 10px;
            position: relative;
            color: #e0e0ff;
            font-weight: 500;
        }
        
        .header-decoration {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 20px;
            background: linear-gradient(90deg, transparent, var(--gold-color), transparent);
            opacity: 0.5;
        }
        
        /* ===== MAIN CONTENT STYLES ===== */
        .main-content {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 80vh;
            padding: 80px 20px;
            flex-direction: column;
            gap: 100px;
        }
        
        .section-title {
            font-size: 3.5rem;
            text-align: center;
            margin-bottom: 60px;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            font-weight: 700;
            position: relative;
            display: inline-block;
            padding: 0 20px;
            font-family: 'Playfair Display', serif;
        }
        
        .section-title::after {
            content: "";
            position: absolute;
            bottom: -15px;
            left: 20%;
            width: 60%;
            height: 4px;
            background: linear-gradient(90deg, transparent, #FFD700, transparent);
            border-radius: 2px;
        }
        
        .section-title i {
            margin-right: 15px;
            font-size: 3rem;
            vertical-align: middle;
        }
        
        /* ===== YEAR CARDS STYLES ===== */
        .large-years {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 50px;
            width: 100%;
            max-width: 1600px;
        }
        
        .large-year {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.8), rgba(42, 77, 155, 0.9));
            border-radius: 25px;
            width: 320px;
            height: 380px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-size: 2.8rem;
            font-weight: bold;
            border: 2px solid rgba(255, 215, 0, 0.4);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3), 0 0 25px rgba(255, 215, 0, 0.2);
            cursor: pointer;
            text-align: center;
            padding: 30px;
            position: relative;
            overflow: hidden;
        }
        
        .large-year::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.1), transparent);
            transform: translateX(-100%) skewX(-15deg);
            transition: transform 0.8s;
        }
        
        .large-year:hover::before {
            transform: translateX(100%) skewX(-15deg);
        }
        
        .large-year:hover {
            transform: translateY(-15px) scale(1.05);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.4), 0 0 40px rgba(255, 215, 0, 0.4);
        }
        
        .large-year .year-icon {
            font-size: 7rem;
            margin-bottom: 30px;
            color: #FFD700;
            text-shadow: 0 0 20px rgba(255, 215, 0, 0.7);
            filter: drop-shadow(0 0 10px rgba(255, 215, 0, 0.5));
            transition: all 0.4s;
        }
        
        .large-year:hover .year-icon {
            transform: scale(1.2) rotate(10deg);
            filter: drop-shadow(0 0 15px rgba(255, 215, 0, 0.8));
        }
        
        .large-year .year-period {
            font-size: 3rem;
            margin-bottom: 15px;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .large-year .year-label {
            font-size: 1.6rem;
            opacity: 0.9;
            color: #e0e0ff;
            font-weight: 500;
        }
        
        /* ===== BACK BUTTON STYLES ===== */
        .back-section {
            width: 100%;
            text-align: center;
            margin-top: 30px;
        }
        
        .back-button {
            background: linear-gradient(135deg, rgba(76, 175, 80, 0.9), rgba(56, 142, 60, 0.9));
            border-radius: 35px;
            width: 650px;
            height: 240px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            font-weight: bold;
            border: 4px solid rgba(255, 215, 0, 0.7);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.5), 0 0 40px rgba(76, 175, 80, 0.6);
            cursor: pointer;
            text-align: center;
            padding: 40px;
            margin: 0 auto;
            position: relative;
            overflow: hidden;
        }
        
        .back-button::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.2), transparent);
            transform: translateX(-100%) skewX(-15deg);
            transition: transform 0.8s;
        }
        
        .back-button:hover::before {
            transform: translateX(100%) skewX(-15deg);
        }
        
        .back-button:hover {
            transform: translateY(-15px) scale(1.1);
            box-shadow: 0 35px 70px rgba(0, 0, 0, 0.6), 0 0 60px rgba(76, 175, 80, 0.8);
        }
        
        .back-button .button-icon {
            font-size: 5.5rem;
            margin-bottom: 20px;
            color: #FFD700;
            text-shadow: 0 0 30px rgba(255, 215, 0, 0.9);
            filter: drop-shadow(0 0 20px rgba(255, 215, 0, 0.7));
            transition: all 0.4s;
        }
        
        .back-button:hover .button-icon {
            transform: scale(1.3) rotate(-15deg);
            filter: drop-shadow(0 0 25px rgba(255, 215, 0, 1));
        }
        
        .back-button .button-text {
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 800;
            letter-spacing: 1px;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            line-height: 1.2;
        }
        
        /* ===== RESPONSIVE STYLES ===== */
        @media (max-width: 1200px) {
            .large-years {
                gap: 40px;
            }
            
            .large-year {
                width: 280px;
                height: 340px;
            }
            
            .back-button {
                width: 550px;
                height: 200px;
            }
        }
        
        @media (max-width: 992px) {
            .header-logo {
                position: relative;
                top: auto;
                left: auto;
                margin-bottom: 30px;
            }
            
            .glowing-text {
                font-size: 5rem;
            }
            
            .large-years {
                gap: 30px;
            }
            
            .large-year {
                width: 240px;
                height: 300px;
                font-size: 2.2rem;
            }
            
            .large-year .year-icon {
                font-size: 5rem;
            }
            
            .back-button {
                width: 450px;
                height: 180px;
                font-size: 2.5rem;
            }
            
            .back-button .button-icon {
                font-size: 4.5rem;
            }
        }
        
        @media (max-width: 768px) {
            .header-logo {
                height: 120px;
            }
            
            .glowing-text {
                font-size: 3.5rem;
            }
            
            .subtitle {
                font-size: 1.8rem;
            }
            
            .large-years {
                flex-direction: column;
                gap: 30px;
            }
            
            .large-year {
                width: 90%;
                max-width: 320px;
                height: 200px;
                flex-direction: row;
                justify-content: space-around;
            }
            
            .large-year .year-icon {
                margin-bottom: 0;
                font-size: 4rem;
            }
            
            .back-button {
                width: 90%;
                height: 150px;
                font-size: 2rem;
            }
            
            .back-button .button-icon {
                font-size: 3.5rem;
            }
            
            .section-title {
                font-size: 2.5rem;
            }
        }
        
        @media (max-width: 576px) {
            .header {
                padding: 80px 20px 60px;
            }
            
            .glowing-text {
                font-size: 2.8rem;
            }
            
            .subtitle {
                font-size: 1.5rem;
            }
            
            .large-year {
                height: 180px;
                font-size: 1.8rem;
            }
            
            .large-year .year-icon {
                font-size: 3.5rem;
            }
            
            .back-button {
                height: 130px;
                font-size: 1.8rem;
                padding: 20px;
            }
            
            .back-button .button-icon {
                font-size: 3rem;
            }
            
            .section-title {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Background Elements -->
    <div class="dynamic-bg"></div>
    <div class="particles" id="particles"></div>
    <div class="floating-elements" id="floatingElements"></div>
    <div class="spotlight"></div>
    
    <div class="container">
        <!-- Header Section -->
        <header>
            <img src="https://i.imgur.com/5X5p5p5.png" alt="Logo Trường" class="header-logo">
            <div class="header-content">
                <div class="header-icon">
                    <i class="fas fa-graduation-cap"></i>
                </div>
                <h1 class="glowing-text">VINH DANH</h1>
                <p class="subtitle">Học Sinh Xuất Sắc - 20 Năm Học</p>
                <p class="subtitle">Trường THPT Chuyên ABC</p>
                <div class="header-decoration"></div>
            </div>
        </header>
        
        <!-- Main Content -->
        <div class="main-content">
            <!-- Year Selection Section -->
            <div class="year-selection" id="yearSelection">
                <h2 class="section-title">
                    <i class="fas fa-calendar-alt"></i>CHỌN NĂM HỌC
                </h2>
                
                <div class="large-years">
                    <!-- Năm học 1 -->
                    <div class="large-year" onclick="redirectToWebsite('https://example.com/year1')">
                        <i class="fas fa-star year-icon"></i>
                        <div class="year-period">2020-2021</div>
                        <div class="year-label">Khóa 1</div>
                    </div>
                    
                    <!-- Năm học 2 -->
                    <div class="large-year" onclick="redirectToWebsite('https://example.com/year2')">
                        <i class="fas fa-trophy year-icon"></i>
                        <div class="year-period">2021-2022</div>
                        <div class="year-label">Khóa 2</div>
                    </div>
                    
                    <!-- Năm học 3 -->
                    <div class="large-year" onclick="redirectToWebsite('https://example.com/year3')">
                        <i class="fas fa-award year-icon"></i>
                        <div class="year-period">2022-2023</div>
                        <div class="year-label">Khóa 3</div>
                    </div>
                    
                    <!-- Năm học 4 -->
                    <div class="large-year" onclick="redirectToWebsite('https://example.com/year4')">
                        <i class="fas fa-medal year-icon"></i>
                        <div class="year-period">2023-2024</div>
                        <div class="year-label">Khóa 4</div>
                    </div>

                    <!-- Năm học 5-->
                    <div class="large-year" onclick="redirectToWebsite('https://example.com/year5')">
                        <i class="fas fa-crown year-icon"></i>
                        <div class="year-period">2024-2025</div>
                        <div class="year-label">Khóa 5</div>
                    </div>
                </div>
                
                <!-- Back Button -->
                <div class="back-section">
                    <div class="back-button" onclick="redirectToWebsite('https://example.com/back')">
                        <i class="fas fa-arrow-left button-icon"></i>
                        <div class="button-text">QUAY LẠI</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
        
    <script>
        // Tạo hiệu ứng hạt nền
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 50;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                
                // Kích thước ngẫu nhiên
                const size = Math.random() * 100 + 20;
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                
                // Vị trí ngẫu nhiên
                particle.style.left = `${Math.random() * 100}vw`;
                
                // Thời gian animation ngẫu nhiên
                const duration = Math.random() * 30 + 20;
                particle.style.animationDuration = `${duration}s`;
                
                // Độ trễ ngẫu nhiên
                const delay = Math.random() * 5;
                particle.style.animationDelay = `${delay}s`;
                
                particlesContainer.appendChild(particle);
            }
        }
        
        // Tạo các phần tử nổi
        function createFloatingElements() {
            const container = document.getElementById('floatingElements');
            const elementCount = 15;
            
            for (let i = 0; i < elementCount; i++) {
                const element = document.createElement('div');
                element.classList.add('floating-element');
                
                // Kích thước ngẫu nhiên
                const size = Math.random() * 150 + 50;
                element.style.width = `${size}px`;
                element.style.height = `${size}px`;
                
                // Vị trí ngẫu nhiên
                element.style.left = `${Math.random() * 100}vw`;
                
                // Thời gian animation ngẫu nhiên
                const duration = Math.random() * 40 + 30;
                element.style.animationDuration = `${duration}s`;
                
                // Độ trễ ngẫu nhiên
                const delay = Math.random() * 10;
                element.style.animationDelay = `${delay}s`;
                
                container.appendChild(element);
            }
        }
        
        // Hàm chuyển hướng đến website
        function redirectToWebsite(url) {
            window.open(url, '_blank');
        }
        
        // Khởi tạo khi trang được tải
        document.addEventListener('DOMContentLoaded', function() {
            createParticles();
            createFloatingElements();
        });
    </script>
</body>
</html>
