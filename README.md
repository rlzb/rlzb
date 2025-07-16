<!-- README Matrix Hacker Turbo -->

<!-- Título Hacker com efeito de digitação -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=00FF00&center=true&vCenter=true&width=435&lines=Inicializando+Terminal+Hacker...;Carregando+arquivos+do+GitHub...;Bem-vindo+ao+Sistema+Operacional+do+Dev!" alt="Typing SVG" />
</p>

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>rlzb - Portfólio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #1a0633, #0d1117, #1a1a2e);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            color: #f0f0f0;
            overflow-x: hidden;
            position: relative;
        }

        /* Partículas de fundo */
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
        }

        .particle {
            position: absolute;
            border-radius: 50%;
            background: rgba(0, 255, 195, 0.3);
            animation: float 15s infinite linear;
        }

        @keyframes float {
            0% { transform: translateY(0) translateX(0) rotate(0deg); }
            100% { transform: translateY(-100vh) translateX(100px) rotate(360deg); }
        }

        /* Container principal com efeito glass */
        .glass-container {
            width: 100%;
            max-width: 1000px;
            padding: 40px;
            border-radius: 25px;
            background: rgba(255, 255, 255, 0.08);
            backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 
                0 15px 35px rgba(0, 0, 0, 0.5),
                inset 0 5px 15px rgba(255, 255, 255, 0.1);
            position: relative;
            overflow: hidden;
            z-index: 1;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .glass-container:hover {
            transform: translateY(-5px);
            box-shadow: 
                0 20px 40px rgba(0, 0, 0, 0.6),
                inset 0 5px 15px rgba(255, 255, 255, 0.15);
        }

        /* Efeito de brilho */
        .glow-effect {
            position: absolute;
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, rgba(0, 255, 195, 0.2), transparent 70%);
            top: -150px;
            right: -150px;
            z-index: -1;
            animation: pulse 4s infinite alternate;
        }

        @keyframes pulse {
            0% { opacity: 0.3; }
            100% { opacity: 0.7; }
        }

        /* Header com animação */
        .header {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }

        .name {
            font-family: 'Montserrat', sans-serif;
            font-size: 3.5rem;
            background: linear-gradient(45deg, #00FFC3, #00B3FF);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 15px;
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { text-shadow: 0 0 5px rgba(0, 255, 195, 0.5); }
            to { text-shadow: 0 0 20px rgba(0, 255, 195, 0.8), 0 0 30px rgba(0, 179, 255, 0.6); }
        }

        .tagline {
            font-size: 1.4rem;
            color: #ccc;
            margin-bottom: 30px;
            font-weight: 300;
        }

        /* Typing animation */
        .typing-container {
            margin: 30px 0;
            min-height: 90px;
        }

        .typing-text {
            font-family: 'Fira Code', monospace;
            font-size: 1.8rem;
            text-align: center;
            background: rgba(0, 0, 0, 0.2);
            padding: 15px 25px;
            border-radius: 15px;
            display: inline-block;
            border-left: 3px solid #00FFC3;
        }

        /* Stats container */
        .stats-container {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
            margin: 40px 0;
        }

        .stat-card {
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s ease;
            height: 200px;
        }

        .stat-card:hover {
            transform: translateY(-10px);
        }

        /* Conecte-se */
        .connect-section {
            text-align: center;
            margin: 40px 0;
        }

        .section-title {
            font-size: 2.2rem;
            margin-bottom: 25px;
            background: linear-gradient(45deg, #00FFC3, #00B3FF);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            display: inline-block;
        }

        .social-badges {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 20px;
        }

        .social-badge {
            display: inline-flex;
            align-items: center;
            padding: 12px 25px;
            border-radius: 50px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.15);
            text-decoration: none;
            color: white;
            font-weight: 500;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .social-badge i {
            margin-right: 10px;
            font-size: 1.4rem;
        }

        .social-badge:hover {
            background: rgba(0, 255, 195, 0.2);
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 255, 195, 0.3);
        }

        /* Tecnologias */
        .tech-section {
            margin: 40px 0;
            text-align: center;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
            gap: 20px;
            max-width: 700px;
            margin: 30px auto;
        }

        .tech-card {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            padding: 20px 15px;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.08);
        }

        .tech-card:hover {
            background: rgba(0, 255, 195, 0.1);
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 255, 195, 0.1);
        }

        .tech-icon {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        .tech-name {
            font-size: 0.9rem;
            font-weight: 500;
        }

        /* Footer */
        .footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 1.1rem;
            color: #aaa;
        }

        .coffee-icon {
            color: #00FFC3;
            animation: bounce 2s infinite;
            display: inline-block;
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        /* Responsividade */
        @media (max-width: 768px) {
            .glass-container {
                padding: 30px 20px;
            }
            
            .name {
                font-size: 2.8rem;
            }
            
            .tagline {
                font-size: 1.2rem;
            }
            
            .typing-text {
                font-size: 1.4rem;
            }
            
            .stats-container {
                flex-direction: column;
                align-items: center;
            }
            
            .stat-card {
                width: 100%;
                max-width: 350px;
            }
            
            .tech-grid {
                grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
            }
        }
    </style>
</head>
<body>
    <!-- Partículas de fundo -->
    <div class="particles" id="particles"></div>
    
    <div class="glass-container">
        <div class="glow-effect"></div>
        
        <div class="header">
            <h1 class="name">✨ Olá! Eu sou <span>rlzb</span> ✨</h1>
            <p class="tagline">🚀 Programador iniciante explorando o mundo do código com estilo</p>
            
            <div class="typing-container">
                <div class="typing-text" id="typing-text">
                    Codando com estilo...
                </div>
            </div>
        </div>
        
        <div class="stats-container">
            <img class="stat-card" src="https://github-readme-stats.vercel.app/api?username=rlzb&show_icons=true&theme=tokyonight&border_radius=15&hide_border=false&bg_color=0d1117&title_color=00FFC3&icon_color=00FFC3" alt="GitHub stats">
            <img class="stat-card" src="https://github-readme-stats.vercel.app/api/top-langs/?username=rlzb&layout=compact&theme=tokyonight&border_radius=15&hide_border=false&bg_color=0d1117&title_color=00FFC3" alt="Top langs">
        </div>
        
        <div class="connect-section">
            <h2 class="section-title">🌐 Conecte-se comigo</h2>
            <div class="social-badges">
                <a href="https://youtube.com/@ynqx" target="_blank" class="social-badge">
                    <i class="fab fa-youtube"></i> YouTube
                </a>
                <a href="https://instagram.com/rlzy_" target="_blank" class="social-badge">
                    <i class="fab fa-instagram"></i> Instagram
                </a>
                <a href="mailto:kalyeltonvieira@gmail.com" class="social-badge">
                    <i class="fas fa-envelope"></i> Gmail
                </a>
                <a href="https://linkedin.com/in/SEULINKEDIN" target="_blank" class="social-badge">
                    <i class="fab fa-linkedin"></i> LinkedIn
                </a>
            </div>
        </div>
        
        <div class="tech-section">
            <h2 class="section-title">🛠️ Tecnologias</h2>
            <div class="tech-grid">
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-html5"></i>
                    </div>
                    <div class="tech-name">HTML5</div>
                </div>
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-css3-alt"></i>
                    </div>
                    <div class="tech-name">CSS3</div>
                </div>
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-js"></i>
                    </div>
                    <div class="tech-name">JavaScript</div>
                </div>
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-python"></i>
                    </div>
                    <div class="tech-name">Python</div>
                </div>
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-react"></i>
                    </div>
                    <div class="tech-name">React</div>
                </div>
            </div>
        </div>
        
        <div class="footer">
            <p>Feito com muito <i class="fas fa-coffee coffee-icon"></i> e <i class="fas fa-heart" style="color: #ff4d94;"></i></p>
        </div>
    </div>

    <script>
        // Criar partículas de fundo
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 30;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                
                // Tamanho e posição aleatórias
                const size = Math.random() * 15 + 5;
                const posX = Math.random() * 100;
                const posY = Math.random() * 100;
                
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                particle.style.left = `${posX}%`;
                particle.style.top = `${posY}%`;
                
                // Atraso de animação aleatório
                particle.style.animationDelay = `${Math.random() * 15}s`;
                
                particlesContainer.appendChild(particle);
            }
        }
        
        // Animações de texto
        const phrases = [
            "Codando com estilo...",
            "Apaixonado por tecnologia e design",
            "Aprendendo todo dia!",
            "Transformando café em código ☕"
        ];
        
        let currentPhrase = 0;
        let currentChar = 0;
        let isDeleting = false;
        let typingSpeed = 100;
        
        function typeText() {
            const textElement = document.getElementById('typing-text');
            const fullText = phrases[currentPhrase];
            
            if (isDeleting) {
                textElement.textContent = fullText.substring(0, currentChar - 1);
                currentChar--;
                typingSpeed = 50;
            } else {
                textElement.textContent = fullText.substring(0, currentChar + 1);
                currentChar++;
                typingSpeed = 100;
            }
            
            if (!isDeleting && currentChar === fullText.length) {
                typingSpeed = 1500;
                isDeleting = true;
            } else if (isDeleting && currentChar === 0) {
                isDeleting = false;
                currentPhrase = (currentPhrase + 1) % phrases.length;
                typingSpeed = 500;
            }
            
            setTimeout(typeText, typingSpeed);
        }
        
        // Inicializar
        document.addEventListener('DOMContentLoaded', () => {
            createParticles();
            setTimeout(typeText, 1000);
        });
    </script>
</body>
</html>
