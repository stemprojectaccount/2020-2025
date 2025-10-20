<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vinh Danh Học Sinh Xuất Sắc - Trường THPT Chuyên ABC</title>
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
            --gradient-purple: linear-gradient(135deg, rgba(156, 39, 176, 0.9), rgba(123, 31, 162, 0.9));
            --gradient-teal: linear-gradient(135deg, rgba(0, 150, 136, 0.9), rgba(0, 121, 107, 0.9));
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
        
        .glowing-text {
            font-size: 7rem;
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
        
        /* ===== STUDENTS GRID STYLES ===== */
        .students-section {
            width: 100%;
            max-width: 1400px;
            margin: 0 auto;
            display: none;
        }
        
        .students-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .student-card {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.7), rgba(42, 77, 155, 0.8));
            border-radius: 20px;
            padding: 30px;
            border: 2px solid rgba(255, 215, 0, 0.4);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            cursor: pointer;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            position: relative;
            overflow: hidden;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3);
            min-height: 280px;
        }
        
        .student-card::before {
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
        
        .student-card:hover::before {
            transform: translateX(100%) skewX(-15deg);
        }
        
        .student-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.4), 0 0 30px rgba(255, 215, 0, 0.4);
        }
        
        .student-image {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid rgba(255, 215, 0, 0.5);
            margin-bottom: 20px;
            box-shadow: 0 0 20px rgba(255, 215, 0, 0.4);
        }
        
        .student-card h3 {
            font-size: 1.6rem;
            margin-bottom: 15px;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
            line-height: 1.3;
        }
        
        .student-card p {
            margin-bottom: 10px;
            font-size: 1.1rem;
            color: #e0e0ff;
            line-height: 1.5;
        }
        
        .student-icon {
            font-size: 2.5rem;
            margin-bottom: 15px;
            color: #FFD700;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.7);
            filter: drop-shadow(0 0 8px rgba(255, 215, 0, 0.5));
        }
        
        .achievement-badge {
            background: linear-gradient(135deg, rgba(255, 140, 66, 0.8), rgba(232, 106, 51, 0.8));
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 600;
            margin-top: 10px;
            border: 1px solid rgba(255, 215, 0, 0.5);
        }
        
        /* ===== BACK BUTTON STYLES ===== */
        .back-section {
            width: 100%;
            text-align: center;
            margin-top: 50px;
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
        
        /* ===== YEAR TITLE STYLES ===== */
        .year-title {
            font-size: 3rem;
            text-align: center;
            margin-bottom: 40px;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
            font-family: 'Playfair Display', serif;
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
            
            .students-grid {
                grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
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
            
            .students-grid {
                grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
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
            
            .students-grid {
                grid-template-columns: 1fr;
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
            
            .student-card {
                padding: 25px;
            }
            
            .student-card h3 {
                font-size: 1.4rem;
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
            <img src="https://i.postimg.cc/zGwcmPH1/image.png" alt="Logo Trường" class="header-logo">
            <div class="header-content">
                <div class="header-icon">
                    <i class="fas fa-graduation-cap"></i>
                </div>
                <h1 class="glowing-text">VINH DANH</h1>
                <p class="subtitle">Học Sinh Xuất Sắc - Nhiều Năm Học</p>
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
                    <!-- Năm học 2020-2021 -->
                    <div class="large-year" onclick="showStudents('2020-2021')">
                        <i class="fas fa-star year-icon"></i>
                        <div class="year-period">2020-2021</div>
                        <div class="year-label">Năm học hiện tại</div>
                    </div>
                    
                    <!-- Năm học 2021-2022 -->
                    <div class="large-year" onclick="showStudents('2021-2022')">
                        <i class="fas fa-trophy year-icon"></i>
                        <div class="year-period">2021-2022</div>
                        <div class="year-label">Năm học trước</div>
                    </div>
                    
                    <!-- Năm học 2022-2023 -->
                    <div class="large-year" onclick="showStudents('2022-2023')">
                        <i class="fas fa-award year-icon"></i>
                        <div class="year-period">2022-2023</div>
                        <div class="year-label">Năm học trước</div>
                    </div>

                    <!-- Năm học 2023-2024 -->
                    <div class="large-year" onclick="showStudents('2023-2024')">
                        <i class="fas fa-medal year-icon"></i>
                        <div class="year-period">2023-2024</div>
                        <div class="year-label">Năm học trước</div>
                    </div>

                    <!-- Năm học 2024-2025 -->
                    <div class="large-year" onclick="showStudents('2024-2025')">
                        <i class="fas fa-crown year-icon"></i>
                        <div class="year-period">2024-2025</div>
                        <div class="year-label">Năm học trước</div>
                    </div>
                </div>
            </div>
            
            <!-- Students Section (Hidden by default) -->
            <div class="students-section" id="studentsSection">
                <h2 class="section-title">
                    <i class="fas fa-users"></i>DANH SÁCH HỌC SINH XUẤT SẮC
                </h2>
                
                <h3 class="year-title" id="selectedYearTitle">NĂM HỌC 2023-2024</h3>
                
                <div class="students-grid" id="studentsGrid">
                    <!-- Student cards will be generated here by JavaScript -->
                </div>
                
                <!-- Back Button -->
                <div class="back-section">
                    <div class="back-button" onclick="hideStudents()">
                        <i class="fas fa-arrow-left button-icon"></i>
                        <div class="button-text">QUAY LẠI TRANG CHÍNH</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
        
    <script>
        // ===== DỮ LIỆU HỌC SINH MẪU =====
        // Bạn có thể thêm dữ liệu thực tế vào đây sau
        const studentsData = {
            "2020-2021": [
                {
                    name: "NGUYỄN VĂN A",
                    class: "12A1",
                    achievement: "Huy chương Vàng Toán Quốc gia, Giải Nhất Tin học",
                },
                {
                    name: "TRẦN THỊ B",
                    class: "12A2", 
                    achievement: "Huy chương Bạc Vật lý, Giải Nhì Hóa học",

                }
            ],
            "2021-2022": [
                                {
                    name: "NGUYỄN TRỌNG QUANG MINH",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh, Huy chương Đồng Olympic Tiếng Anh Quốc gia",
                },
                {
                    name: "VÕ ANH SỰ",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "PHẠM NHẬT MINH",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "KHÚC ĐẶNG THIÊN KHÚC",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "PHẠM NGUYỄN HÀ NGÂN",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                    teacher: "",
                    score: ""
                },
                {
                    name: "NGUYỄN THUỲ DUNG",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "TRỊNH GIA HÂN",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "PHẠM ANH THÁI",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh, Giải Nhất Văn hoá đọc cấp Tỉnh, Khuyến khích Văn hoá đọc Quốc gia",
                },
                {
                    name: "HỒ THỊ THANH MỸ",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGUYỄN HỒNG LÂM",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGUYỄN LÊ MINH ĐỨC",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "TRẦN NGUYỄN MINH NHẬT",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "MAI BÁ TÙNG DƯƠNG",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGUYỄN VĂN THÀNH TIẾN",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "TRẦN NGUYỄN LINH NHƯ",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Vật lí cấp Tỉnh",
                },
                {
                    name: "ĐỖ HOÀNG DUY KHOA",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Vật lí cấp Tỉnh",
                },
                {
                    name: "NGUYỄN ĐỨC GIA BẢO",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Vật lí cấp Tỉnh",
                },
                {
                    name: "PHẠM ANH THƯ",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Vật lí cấp Tỉnh",
                },
                {
                    name: "NGUYỄN PHƯƠNG UYÊN",
                    class: "",
                    achievement: "Giải Nhất Văn hoá đọc cấp Tỉnh",
                },
                {
                    name: "NGUYỄN BÙI HÀ DƯƠNG",
                    class: "",
                    achievement: "Giải Nhì KHKT cấp Tỉnh",
                },
                {
                    name: "VÕ DƯƠNG HÀ MY",
                    class: "",
                    achievement: "Giải Nhì KHKT cấp Tỉnh",
                }
            ],
            "2022-2023": [
                         {
                    name: "NGUYỄN BÙI KHÔI NGUYÊN",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh, Huy chương Đồng Violympic Toán TV Quốc gia",
                },
                {
                    name: "PHẠM GIA VĨNH TƯỜNG",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGUYỄN NGỌC GIA NHI",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGUYỄN MINH DƯƠNG",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "LÊ ĐỨC MINH NHẬT",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "BÙI NGỌC ANH THƯ",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "CAO BẢO TRÂM",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "PHẠM THỊ KHÁNH LY",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "CAO TUYẾT TRINH",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGUYỄN LÊ MINH ĐỨC",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh, Huy chương Bạc Violympic Toán TV Quốc gia",
                },
                {
                    name: "NGUYỄN TRUNG PHONG",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh, Huy chương Đồng Violympic Toán TV Quốc gia",
                },
                {
                    name: "NGUYỄN HỒNG LÂM",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "PHẠM GIA QUỲNH HƯƠNG",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "TRẦN NGUYỄN LINH NHƯ",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh, Khuyến khích Văn hóa đọc Quốc gia",
                },
                {
                    name: "HÀ PHÚ ĐỨC",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "ĐẶNG NGỌC BÌNH AN",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGUYỄN NGỌC BẢO CHÂU",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "TRẦN VĂN KHANG",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "PHẠM ANH THƯ",
                    class: "",
                    achievement: "Huy chương Vàng Violympic Toán TV cấp Tỉnh, Huy chương Bạc Violympic Vật lý cấp Tỉnh, Khuyến khích Violympic Toán TV Quốc gia",
                },
                {
                    name: "PHẠM NGUYỄN TUẤN MINH",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh, Huy chương Bạc Violympic Vật lý cấp Tỉnh, Giải Nhất STEM cấp Tỉnh, Khuyến khích Violympic Toán TV Quốc gia",
                },
                {
                    name: "NGUYỄN ĐỨC GIA BẢO",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh, Giải Nhì STEM cấp Tỉnh",
                },
                {
                    name: "ĐỖ HOÀNG DUY KHOA",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "BÙI NHẬT LÂM",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGUYỄN THIỆN NHÂN",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGUYỄN PHƯƠNG UYÊN",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh, Giải Nhì STEM cấp Tỉnh, Giải Nhất Văn hóa đọc cấp Tỉnh, Khuyến khích Văn hóa đọc Quốc gia, Cây bút triển vọng UPU Quốc tế lần thứ 52",
                },
                {
                    name: "NGUYỄN HOÀNG VŨ",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "HỒ THỊ THANH MỸ",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh, Huy chương Bạc Violympic Toán TV Quốc gia",
                },
                {
                    name: "NGUYỄN THUỲ DUNG",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "MAI BÁ TÙNG DƯƠNG",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "TRỊNH GIA HÂN",
                    class: "",
                    achievement: "Huy chương Đồng Violympic Toán TV cấp Tỉnh",
                },
                {
                    name: "NGÔ NGỌC THẢO VIÊN",
                    class: "",
                    achievement: "Khuyến khích Violympic Toán TV Quốc gia",
                },
                {
                    name: "NGUYỄN KHỞI NGUYÊN",
                    class: "",
                    achievement: "Khuyến khích Violympic Toán TV Quốc gia",
                },
                {
                    name: "NGUYỄN THÀNH GIA BẢO",
                    class: "",
                    achievement: "Huy chương Bạc Violympic Vật lý cấp Tỉnh",
                },
                {
                    name: "NGUYỄN LƯƠNG CHÂU LONG",
                    class: "",
                    achievement: "Giải Nhì IOE cấp Tỉnh",
                },
                {
                    name: "NGUYỄN HÀ NGÂN",
                    class: "",
                    achievement: "Giải Ba IOE cấp Tỉnh",
                },
                {
                    name: "PHẠM NGUYỄN HÀ NGÂN",
                    class: "",
                    achievement: "Giải Ba IOE cấp Tỉnh, Giải Nhất HSG cấp Huyện",
                },
                {
                    name: "MAI ĐỨC HƯNG",
                    class: "",
                    achievement: "Giải Ba IOE cấp Tỉnh",
                },
                {
                    name: "PHẠM THỊ NHƯ QUỲNH",
                    class: "",
                    achievement: "Giải Nhất HSG cấp Huyện",
                },
                {
                    name: "NGUYỄN BÙI HÀ DƯƠNG",
                    class: "",
                    achievement: "Giải Nhì KHKT cấp Tỉnh, Giải Nhì STEM cấp Tỉnh, Công nhận Quốc gia STEM",
                },
                {
                    name: "ĐỖ THÀNH THÁI",
                    class: "",
                    achievement: "Giải Nhì KHKT cấp Tỉnh, Giải Nhì STEM cấp Tỉnh",
                },
                {
                    name: "NGUYỄN VĂN THÀNH TIẾN",
                    class: "",
                    achievement: "Giải Nhất STEM cấp Tỉnh",
                },
                {
                    name: "NGUYỄN HỮU TẤT ANH",
                    class: "",
                    achievement: "Giải Nhất STEM cấp Tỉnh",
                },
                {
                    name: "MAI NGUYỄN BẢO AN",
                    class: "",
                    achievement: "Giải Nhất STEM cấp Tỉnh",
                },
                {
                    name: "TRẦN QUỐC HÙNG",
                    class: "",
                    achievement: "Giải Nhất STEM cấp Tỉnh",
                },
                {
                    name: "LÊ TIẾN ĐẠT",
                    class: "",
                    achievement: "Giải Nhì STEM cấp Tỉnh",
                },
                {
                    name: "NGUYỄN THU GIANG",
                    class: "",
                    achievement: "Giải Nhì STEM cấp Tỉnh",
                },
                {
                    name: "NGUYỄN NGỌC NHƯ Ý",
                    class: "",
                    achievement: "Giải Nhì Viết về thầy cô và mái trường cấp Tỉnh",
                },
                {
                    name: "NGUYỄN VÕ NGỌC HÀ",
                    class: "",
                    achievement: "Giải Nhì Văn hóa đọc cấp Tỉnh",
                },
                {
                    name: "VÕ LÂM ĐOAN PHƯỢNG",
                    class: "",
                    achievement: "Giải Ba Văn hóa đọc Quốc gia",
                }
            ],
            "2023-2024": [
                   {
        name: "DƯƠNG KHẮC VIỆT ANH",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh, Đồng Vioedu cấp Tỉnh",
    },
    {
        name: "NGUYỄN NGỌC BẢO ANH",
        class: "",
        achievement: "giải ĐỒNG TỈNH Violympic Toán",
    },
    {
        name: "PHẠM TRÍ DŨNG",
        class: "",
        achievement: "Bạc Violympic Toán cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "LÊ NGUYỄN GIA HÂN",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh, Đồng Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "ĐỖ GIA HÂN",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM NGUYỄN GIA HUY",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh, Bạc Vioedu cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN NHẬT HUY",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM MINH NGỌC",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh, Vàng Vioedu cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN ĐÌNH MINH NHẬT",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN PHƯƠNG NHI",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN PHÚ QUÝ",
        class: "",
        achievement: "Khuyến khích Violympic Toán Quốc Gia, Đồng Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "LÊ NGUYỄN BẢO QUYÊN",
        class: "",
        achievement: "Bạc Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN TRỌNG SINH",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN CẨM TÚ",
        class: "",
        achievement: "Đồng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "ĐỖ PHAN KHÁNH THI",
        class: "",
        achievement: "Bạc Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM GIA VĨNH TƯỜNG",
        class: "",
        achievement: "Khuyến khích Violympic Toán Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN LÊ MINH ĐỨC",
        class: "",
        achievement: "Đồng Violympic Toán Quốc Gia, Bạc Vioedu cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN NỮ KHÁNH TRANG",
        class: "",
        achievement: "Khuyến khích Violympic Toán Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN NGỌC BẢO CHÂU",
        class: "",
        achievement: "Khuyến khích Violympic Toán Quốc Gia, Đồng Vioedu cấp Tỉnh, Hoàn thành tốt IOE Quốc Gia, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM GIA QUỲNH HƯƠNG",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh, Đồng Vioedu cấp Tỉnh, Hoàn thành tốt IOE Quốc Gia, Vàng Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN HỒNG LÂM",
        class: "",
        achievement: "Đồng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM NHẬT MINH",
        class: "",
        achievement: "Bạc Violympic Toán cấp Tỉnh, Hoàn thành tốt IOE Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "HOÀNG MINH HIẾU",
        class: "",
        achievement: "Đồng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "ĐOÀN KHÁNH NHI",
        class: "",
        achievement: "Đồng Violympic Toán cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "HÀ PHÚ ĐỨC",
        class: "",
        achievement: "Bạc Violympic Toán cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN TRUNG PHONG",
        class: "",
        achievement: "Đồng Violympic Toán cấp Tỉnh, Đồng Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM THÁI MINH PHÚC",
        class: "",
        achievement: "Bạc Violympic Toán cấp Tỉnh, Nhất IOE cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "TRẦN VĂN HOÀNG",
        class: "",
        achievement: "Đồng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "TRẦN VĂN KHANG",
        class: "",
        achievement: "Đồng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "HỒ VIẾT XUÂN",
        class: "",
        achievement: "Đồng Violympic Toán cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN THIỆN NHÂN",
        class: "",
        achievement: "Bạc Violympic Toán Quốc Gia, Khuyến khích Violympic KHTN Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM NGUYỄN TUẤN MINH",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh, Vàng Vioedu cấp Tỉnh, Khuyến khích Violympic KHTN Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN THẢO NGUYÊN",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh, Nhất IOE cấp Tỉnh, Khuyến khích Tiếng Anh cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "TRỊNH CÔNG ĐỨC",
        class: "",
        achievement: "Đồng Violympic Toán Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM ANH THƯ",
        class: "",
        achievement: "Đồng Violympic Toán Quốc Gia, Đồng Violympic KHTN Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "TRẦN MẠNH HÙNG",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh, Hoàn thành tốt IOE Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "TRẦN MẠNH DŨNG",
        class: "",
        achievement: "Khuyến khích Violympic Toán Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "ĐẶNG DUY BẢO",
        class: "",
        achievement: "Khuyến khích Violympic Toán Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM LÊ ANH THƯ",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "BÙI NHẬT LÂM",
        class: "",
        achievement: "Bạc Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "HỒ NGỌC TƯỜNG NHI",
        class: "",
        achievement: "Đồng Violympic Toán cấp Tỉnh, Khuyến khích Violympic KHTN Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "ĐỖ HOÀNG DUY KHOA",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh, Đồng Vioedu cấp Tỉnh, Khuyến khích Violympic KHTN Quốc Gia, Nhất Toán cấp Huyện",
        teacher: "",
        score: ""
    },
    {
        name: "LƯU GIA BẢO",
        class: "",
        achievement: "Vàng Violympic Toán cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN PHƯƠNG UYÊN",
        class: "",
        achievement: "Bạc Violympic Toán cấp Tỉnh, Đồng Violympic KHTN Quốc Gia, Cây bút triển vọng Viết thư UPU",
        teacher: "",
        score: ""
    },
    {
        name: "TRẦN NGUYỄN MINH NHẬT",
        class: "",
        achievement: "Khuyến khích Violympic Toán Quốc Gia",
        teacher: "",
        score: ""
    },

    // IOE
    {
        name: "NGUYỄN BÙI ĐÔNG PHƯƠNG",
        class: "9C",
        achievement: "Khuyến khích IOE Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "HÀ CHÂU NGỌC PHƯƠNG",
        class: "6A",
        achievement: "Nhì IOE cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "TRẦN NGUYỄN LINH NHƯ",
        class: "8A",
        achievement: "Hoàn thành tốt IOE Quốc Gia, Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "LÊ HOÀNG TUẤN",
        class: "8A",
        achievement: "Nhì IOE cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN HÀ NGÂN",
        class: "9D",
        achievement: "Hoàn thành tốt IOE Quốc Gia, Khuyến khích Tiếng Anh cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "VÕ NGỌC TRÂM ANH",
        class: "9D",
        achievement: "Hoàn thành tốt IOE Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN ÁNH CẦM",
        class: "9D",
        achievement: "Hoàn thành tốt IOE Quốc Gia",
        teacher: "",
        score: ""
    },

    // Violympic KHTN
    {
        name: "NGUYỄN ĐỨC GIA BẢO",
        class: "9D",
        achievement: "Khuyến khích Violympic KHTN Quốc Gia",
        teacher: "",
        score: ""
    },
    {
        name: "TRỊNH NHẬT MINH",
        class: "6A",
        achievement: "Đồng Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "LÊ NGỌC ĐÔNG NHI",
        class: "6A",
        achievement: "Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "TRƯƠNG BÙI HOÀNG NHI",
        class: "6A",
        achievement: "Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "DƯƠNG HOÀNG MINH PHÚC",
        class: "6A",
        achievement: "Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN BÙI MINH TUẤN",
        class: "6A",
        achievement: "Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN NGỌC ANH",
        class: "6B",
        achievement: "Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN NGỌC GIA NHI",
        class: "7A",
        achievement: "Vàng Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN TRẦN ĐÌNH QUÂN",
        class: "8A",
        achievement: "Đồng Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM VIẾT BẢO LONG",
        class: "8A",
        achievement: "Bạc Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN NGỌC HỒNG ÂN",
        class: "8A",
        achievement: "Đồng Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "TRẦN VÕ LÊ DŨNG",
        class: "8A",
        achievement: "Vàng Violympic KHTN cấp Tỉnh",
        teacher: "",
        score: ""
    },

    // Thể thao
    {
        name: "NGUYỄN BẢO TRUNG",
        class: "6A",
        achievement: "Cờ vua",
        teacher: "",
        score: ""
    },
    {
        name: "VŨ KHẮC ĐẠT",
        class: "9C",
        achievement: "Bóng đá",
        teacher: "",
        score: ""
    },
    {
        name: "BÙI THÀNH ĐẠT",
        class: "9C",
        achievement: "Bóng đá",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN TẤN HOÁ",
        class: "9C",
        achievement: "Bóng đá",
        teacher: "",
        score: ""
    },
    {
        name: "HOÀNG GIA HƯNG",
        class: "9C",
        achievement: "Bóng đá",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN TRỌNG AN",
        class: "9D",
        achievement: "Bóng đá",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN TRẦN MINH PHÚC",
        class: "9D",
        achievement: "Bóng đá",
        teacher: "",
        score: ""
    },
    {
        name: "CAO DUY QUÝ",
        class: "9A",
        achievement: "Bóng đá",
        teacher: "",
        score: ""
    },
    {
        name: "MAI NGUYỄN BẢO AN",
        class: "9D",
        achievement: "Bóng đá",
        teacher: "",
        score: ""
    },

    // Học sinh giỏi văn hóa
    {
        name: "NGUYỄN HOÀNG VŨ",
        class: "",
        achievement: "Nhất Hóa học cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "NGUYỄN NHẬT AN",
        class: "",
        achievement: "Ba GDCD cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "PHẠM PHƯƠNG VY",
        class: "",
        achievement: "Ba GDCD cấp Tỉnh",
        teacher: "",
        score: ""
    },
    {
        name: "VŨ PHAN ĐỨC BẢO",
        class: "",
        achievement: "Khuyến khích Tin học cấp Tỉnh",
        teacher: "",
        score: ""
    }
            ],
            "2024-2025": [
{
    name: "CHU TUẤN HẢI",
    class: "7B",
    achievement: "Vàng Violympic Toán cấp Tỉnh, Bạc Vioedu cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHẠM TRÍ DŨNG",
    class: "7A",
    achievement: "Vàng Violympic Toán cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN LÊ MINH ĐỨC",
    class: "9A",
    achievement: "Vàng Violympic Toán cấp Tỉnh, Đồng Violympic KHTN cấp Tỉnh, Ba Toán cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "TRẦN VĂN KHANG",
    class: "9A",
    achievement: "Vàng Violympic Toán cấp Tỉnh, Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN NGỌC HỒNG ÂN",
    class: "9A",
    achievement: "Vàng Violympic Toán cấp Tỉnh, Vàng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHẠM GIA VĨNH TƯỜNG",
    class: "8A",
    achievement: "Vàng Toán Tiếng Anh cấp Tỉnh, Đồng Violympic Toán cấp Tỉnh, Vàng Violympic KHTN cấp Tỉnh, Ba IOE cấp Tỉnh, Nhất Văn hóa đọc cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN BÙI KHÔI NGUYÊN",
    class: "8A",
    achievement: "Vàng Toán Tiếng Anh cấp Tỉnh, Ba Sản phẩm STEM cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN VIỆT KHANG",
    class: "9A",
    achievement: "Vàng Violympic Toán cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "BÙI KHẢ MY",
    class: "6A",
    achievement: "Bạc Violympic Toán cấp Tỉnh, Bạc Toán Tiếng Anh cấp Tỉnh, Bạc Violympic KHTN cấp Tỉnh, Ba IOE cấp Tỉnh, Đồng Vioedu cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "LÊ NGỌC ĐÔNG NHI",
    class: "7A",
    achievement: "Bạc Violympic Toán cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHẠM VIẾT BẢO LONG",
    class: "9A",
    achievement: "Bạc Violympic Toán cấp Tỉnh, Vàng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "CAO THỊ TUYẾT CHÂU",
    class: "9A",
    achievement: "Bạc Violympic Toán cấp Tỉnh, Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN HỒNG LÂM",
    class: "9A",
    achievement: "Bạc Violympic Toán cấp Tỉnh, Vàng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHẠM THÁI MINH PHÚC",
    class: "9A",
    achievement: "Bạc Violympic Toán cấp Tỉnh, Nhì IOE cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHẠM MINH NGỌC",
    class: "7A",
    achievement: "Đồng Violympic Toán cấp Tỉnh, Ba IOE cấp Tỉnh, Đồng Vioedu cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN LÊ NHƯ Ý",
    class: "6A",
    achievement: "Vàng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "ĐỖ TRẦN THẢO NHI",
    class: "6A",
    achievement: "Vàng Violympic KHTN cấp Tỉnh, Đồng Vioedu cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "HOÀNG LÂM",
    class: "7A",
    achievement: "Vàng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN BÙI MINH TUẤN",
    class: "7A",
    achievement: "Vàng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "HOÀNG NHẬT VŨ",
    class: "9A",
    achievement: "Vàng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN NỮ KHÁNH TRANG",
    class: "9A",
    achievement: "Vàng Violympic KHTN cấp Tỉnh, Ba Lịch sử cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "TRẦN VĂN HOÀNG",
    class: "9A",
    achievement: "Vàng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHAN NGUYỄN NHÃ UYÊN",
    class: "6A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN YẾN NHI",
    class: "6A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "HUỲNH NGUYÊN PHÚC",
    class: "7A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN NHẬT HUY",
    class: "7A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHẠM NGUYỄN GIA HUY",
    class: "7A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "LÊ NGUYỄN GIA HÂN",
    class: "7A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN CẨM TÚ",
    class: "7A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN TRÍ DŨNG",
    class: "7A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN MINH DƯƠNG",
    class: "8A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "TRẦN VÕ LÊ DŨNG",
    class: "9A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "ĐỖ CHUỲ CHI",
    class: "9A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "HỒ BÙI QUANG VINH",
    class: "9A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHẠM NHẬT MINH",
    class: "9A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh, Nhì IOE cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHẠM GIA QUỲNH HƯƠNG",
    class: "9A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh, Nhì IOE cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "ĐOÀN KHÁNH NHI",
    class: "9A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh, Ba GDCD cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN TRẦN ĐÌNH QUÂN",
    class: "9A",
    achievement: "Bạc Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN HOÀNG NGỌC ÁNH",
    class: "6B",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHẠM NGUYỄN HIỀN NHI",
    class: "6A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh, Nhất Sản phẩm STEM cấp Huyện",
    teacher: "",
    score: ""
},
{
    name: "ĐÀO NGUYỄN ĐĂNG KHOA",
    class: "6A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "ĐẶNG BẢO TRÂM",
    class: "6A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "VÕ NGỌC VŨ",
    class: "6A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN VŨ LÂM LY",
    class: "6A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN TRỌNG SINH",
    class: "7A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "PHAN NGUYỄN BẢO HÂN",
    class: "7A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "HOÀNG NGÂN HÀ",
    class: "7A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "DƯƠNG KHẮC VIỆT ANH",
    class: "7A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh, Đồng Vioedu cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "ĐẶNG THỊ THANH HUYỀN",
    class: "8A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "CAO BẢO TRÂM",
    class: "8A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh, Ba IOE cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "ĐỖ TRẦN ĐĂNG KHOA",
    class: "8B",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "HÀ PHÚ ĐỨC",
    class: "9A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGÔ NGỌC THẢO VIÊN",
    class: "9A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN NGỌC BẢO CHÂU",
    class: "9A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "LÊ HOÀNG TUẤN",
    class: "9A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh, Ba IOE cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "LÊ PHẠM NGUYÊN PHÚC",
    class: "9A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "ĐẶNG NGỌC BÌNH AN",
    class: "9A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "LÊ NGUYỄN MINH THƯ",
    class: "9A",
    achievement: "Đồng Violympic KHTN cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "HÀ CHÂU NGỌC PHƯƠNG",
    class: "7A",
    achievement: "Nhì IOE cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN NGỌC GIA NHI",
    class: "8A",
    achievement: "Nhì IOE cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "VÕ PHẠM KHÁNH THY",
    class: "8A",
    achievement: "Ba IOE cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "TRẦN NGUYỄN LINH NHƯ",
    class: "9A",
    achievement: "Nhì Ngữ văn cấp Tỉnh, Ba Văn hóa đọc cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "ĐÀO DIỆU CHI",
    class: "9C",
    achievement: "Ba Lịch sử cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "TRẦN THÀNH ĐẠT",
    class: "6A",
    achievement: "Ba Sản phẩm STEM cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN VÕ NGỌC HÀ",
    class: "9A",
    achievement: "Nhất Sản phẩm STEM cấp Huyện, Khuyến khích Văn hóa đọc cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "TRƯƠNG CÔNG HOÀNG LONG",
    class: "6A",
    achievement: "Nhất Sản phẩm STEM cấp Huyện",
    teacher: "",
    score: ""
},
{
    name: "NGUYỄN THỊ HỒNG PHÚC",
    class: "8A",
    achievement: "Khuyến khích Văn hóa đọc cấp Tỉnh",
    teacher: "",
    score: ""
},
{
    name: "LÊ BẢO NGỌC",
    class: "8A",
    achievement: "Vàng Violympic KHTN cấp Quốc gia",
    teacher: "",
    score: ""
}
            ]
        };

        // ===== HÀM HIỂN THỊ DANH SÁCH HỌC SINH =====
        function showStudents(year) {
            // Ẩn phần chọn năm học
            document.getElementById('yearSelection').style.display = 'none';
            
            // Hiển thị phần danh sách học sinh
            const studentsSection = document.getElementById('studentsSection');
            studentsSection.style.display = 'block';
            
            // Cập nhật tiêu đề năm học
            document.getElementById('selectedYearTitle').textContent = `NĂM HỌC ${year}`;
            
            // Tạo các card học sinh
            const studentsGrid = document.getElementById('studentsGrid');
            studentsGrid.innerHTML = '';
            
            const students = studentsData[year] || [];
            
            students.forEach((student, index) => {
                const card = document.createElement('div');
                card.classList.add('student-card');
                
                // Tạo hình ảnh ngẫu nhiên dựa trên index
                const gender = index % 2 === 0 ? 'men' : 'women';
                const imgIndex = (index % 50) + 1;
                
                // Lấy thành tích đầu tiên để hiển thị badge
                const firstAchievement = student.achievement.split(',')[0];
                
                card.innerHTML = `
                    <i class="fas fa-user-graduate student-icon"></i>
                    <img src="https://randomuser.me/api/portraits/${gender}/${imgIndex}.jpg" alt="${student.name}" class="student-image">
                    <h3>${student.name}</h3>
                    <p><strong>Lớp:</strong> ${student.class}</p>
                    <div class="achievement-badge">${firstAchievement}</div>
                `;
                
                studentsGrid.appendChild(card);
            });
        }

        // ===== HÀM ẨN DANH SÁCH HỌC SINH =====
        function hideStudents() {
            // Ẩn phần danh sách học sinh
            document.getElementById('studentsSection').style.display = 'none';
            
            // Hiển thị phần chọn năm học
            document.getElementById('yearSelection').style.display = 'block';
        }

        // ===== TẠO HIỆU ỨNG NỀN =====
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 50;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                
                const size = Math.random() * 100 + 20;
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                particle.style.left = `${Math.random() * 100}vw`;
                particle.style.animationDuration = `${Math.random() * 30 + 20}s`;
                particle.style.animationDelay = `${Math.random() * 5}s`;
                
                particlesContainer.appendChild(particle);
            }
        }
        
        function createFloatingElements() {
            const container = document.getElementById('floatingElements');
            const elementCount = 15;
            
            for (let i = 0; i < elementCount; i++) {
                const element = document.createElement('div');
                element.classList.add('floating-element');
                
                const size = Math.random() * 150 + 50;
                element.style.width = `${size}px`;
                element.style.height = `${size}px`;
                element.style.left = `${Math.random() * 100}vw`;
                element.style.animationDuration = `${Math.random() * 40 + 30}s`;
                element.style.animationDelay = `${Math.random() * 10}s`;
                
                container.appendChild(element);
            }
        }

        // ===== KHỞI TẠO TRANG =====
        document.addEventListener('DOMContentLoaded', function() {
            createParticles();
            createFloatingElements();
            
            console.log("=== TRANG CHÍNH HỌC SINH XUẤT SẮC ===");
            console.log("Có 5 năm học để lựa chọn:");
            console.log("- 2023-2024 (Năm học hiện tại)");
            console.log("- 2022-2023");
            console.log("- 2021-2022"); 
            console.log("- 2020-2021");
            console.log("- 2019-2020");
            console.log("Mỗi năm học đều có nút QUAY LẠI TRANG CHÍNH");
        });
    </script>
