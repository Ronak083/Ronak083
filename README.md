<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ronak Gupta - LinkedIn Cover</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        .cover-container {
            width: 1584px;
            height: 396px;
            background: linear-gradient(135deg, #0f1419 0%, #1a2332 50%, #2d3748 100%);
            position: relative;
            overflow: hidden;
            font-family: 'Arial', sans-serif;
        }

        .grid-pattern {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image:
                linear-gradient(rgba(59, 130, 246, 0.1) 1px, transparent 1px),
                linear-gradient(90deg, rgba(59, 130, 246, 0.1) 1px, transparent 1px);
            background-size: 50px 50px;
            animation: gridShift 20s linear infinite;
        }

        @keyframes gridShift {
            0% {
                transform: translate(0, 0);
            }

            100% {
                transform: translate(50px, 50px);
            }
        }

        .profile-space {
            position: absolute;
            left: 50px;
            bottom: 50px;
            width: 180px;
            height: 180px;
            border-radius: 50%;
            background: transparent;
            border: 3px solid rgba(59, 130, 246, 0.3);
            box-shadow: 0 0 30px rgba(59, 130, 246, 0.2);
        }

        .content-area {
            position: absolute;
            right: 80px;
            top: 50%;
            transform: translateY(-50%);
            color: white;
            text-align: right;
            max-width: 800px;
        }

        .name {
            font-size: 48px;
            font-weight: bold;
            margin-bottom: 15px;
            background: linear-gradient(135deg, #60a5fa, #3b82f6, #1d4ed8);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-shadow: 0 4px 15px rgba(59, 130, 246, 0.3);
        }

        .title {
            font-size: 24px;
            color: #e2e8f0;
            margin-bottom: 20px;
            font-weight: 300;
        }

        .skills-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: flex-end;
            gap: 12px;
            margin-bottom: 20px;
        }

        .skill-badge {
            background: rgba(59, 130, 246, 0.15);
            border: 1px solid rgba(59, 130, 246, 0.3);
            padding: 8px 16px;
            border-radius: 25px;
            font-size: 14px;
            color: #93c5fd;
            backdrop-filter: blur(10px);
            transition: all 0.3s ease;
            animation: fadeInUp 0.6s ease-out forwards;
            opacity: 0;
            transform: translateY(20px);
        }

        .skill-badge:nth-child(1) {
            animation-delay: 0.1s;
        }

        .skill-badge:nth-child(2) {
            animation-delay: 0.2s;
        }

        .skill-badge:nth-child(3) {
            animation-delay: 0.3s;
        }

        .skill-badge:nth-child(4) {
            animation-delay: 0.4s;
        }

        .skill-badge:nth-child(5) {
            animation-delay: 0.5s;
        }

        .skill-badge:nth-child(6) {
            animation-delay: 0.6s;
        }

        .skill-badge:nth-child(7) {
            animation-delay: 0.7s;
        }

        .skill-badge:nth-child(8) {
            animation-delay: 0.8s;
        }

        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .skill-badge:hover {
            background: rgba(59, 130, 246, 0.25);
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(59, 130, 246, 0.2);
        }

        .experience {
            font-size: 16px;
            color: #cbd5e1;
            font-weight: 300;
        }

        .highlight {
            color: #60a5fa;
            font-weight: 500;
        }

        .floating-icons {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }

        .floating-icon {
            position: absolute;
            font-size: 24px;
            color: rgba(59, 130, 246, 0.15);
            animation: float 6s ease-in-out infinite;
        }

        .icon-1 {
            top: 20%;
            left: 20%;
            animation-delay: 0s;
        }

        .icon-2 {
            top: 60%;
            left: 15%;
            animation-delay: 1s;
        }

        .icon-3 {
            top: 30%;
            left: 75%;
            animation-delay: 2s;
        }

        .icon-4 {
            top: 70%;
            left: 80%;
            animation-delay: 3s;
        }

        @keyframes float {

            0%,
            100% {
                transform: translateY(0px) rotate(0deg);
            }

            50% {
                transform: translateY(-20px) rotate(180deg);
            }
        }

        .location-contact {
            position: absolute;
            bottom: 25px;
            right: 80px;
            font-size: 14px;
            color: #94a3b8;
            display: flex;
            gap: 20px;
            align-items: center;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .pulse-dot {
            width: 8px;
            height: 8px;
            background: #10b981;
            border-radius: 50%;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% {
                box-shadow: 0 0 0 0 rgba(16, 185, 129, 0.7);
            }

            70% {
                box-shadow: 0 0 0 10px rgba(16, 185, 129, 0);
            }

            100% {
                box-shadow: 0 0 0 0 rgba(16, 185, 129, 0);
            }
        }
    </style>
</head>

<body>
    <div class="cover-container">
        <div class="grid-pattern"></div>

        <div class="floating-icons">
            <div class="floating-icon icon-1">☁️</div>
            <div class="floating-icon icon-2">⚙️</div>
            <div class="floating-icon icon-3">🚀</div>
            <div class="floating-icon icon-4">🔧</div>
        </div>

        <!-- Space reserved for profile picture -->
        <div class="profile-space"></div>

        <div class="content-area">
            <h1 class="name">Ronak Gupta</h1>
            <p class="title">DevOps Engineer | Cloud Infrastructure Specialist</p>

            <div class="skills-container">
                <span class="skill-badge">AWS</span>
                <span class="skill-badge">Kubernetes</span>
                <span class="skill-badge">Docker</span>
                <span class="skill-badge">Terraform</span>
                <span class="skill-badge">Jenkins</span>
                <span class="skill-badge">Python</span>
                <span class="skill-badge">CI/CD</span>
                <span class="skill-badge">Monitoring</span>
            </div>

            <p class="experience">
                <span class="highlight">1.5+ years</span> managing cloud infrastructure & production environments<br>
                Building scalable solutions at <span class="highlight">SS&C Technologies</span>
            </p>
        </div>

        <div class="location-contact">
            <div class="contact-item">
                <div class="pulse-dot"></div>
                <span>Available for opportunities</span>
            </div>
            <div class="contact-item">
                <span>📍</span>
                <span>Bengaluru, India</span>
            </div>
        </div>
    </div>
</body>

</html>
