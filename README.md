<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Programlama Dilleri | GitHub Profili</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a2a6c, #2c3e50);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #fff;
            padding: 20px;
        }
        
        .container {
            max-width: 1200px;
            width: 100%;
            text-align: center;
        }
        
        header {
            margin-bottom: 50px;
            animation: fadeIn 1s ease;
        }
        
        h1 {
            font-size: 3.5rem;
            margin-bottom: 15px;
            text-shadow: 0 2px 10px rgba(0,0,0,0.3);
            background: linear-gradient(45deg, #00c9ff, #92fe9d);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .subtitle {
            font-size: 1.4rem;
            opacity: 0.9;
            max-width: 800px;
            margin: 0 auto;
            line-height: 1.6;
        }
        
        .languages-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 35px;
            padding: 30px;
        }
        
        .language-card {
            width: 150px;
            height: 200px;
            perspective: 1000px;
        }
        
        .language-inner {
            position: relative;
            width: 100%;
            height: 100%;
            text-align: center;
            transition: transform 0.6s;
            transform-style: preserve-3d;
        }
        
        .language-card:hover .language-inner {
            transform: rotateY(180deg);
        }
        
        .language-front, .language-back {
            position: absolute;
            width: 100%;
            height: 100%;
            -webkit-backface-visibility: hidden;
            backface-visibility: hidden;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            border-radius: 20px;
            padding: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        .language-front {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .language-back {
            background: linear-gradient(45deg, #6a11cb, #2575fc);
            transform: rotateY(180deg);
            justify-content: space-around;
        }
        
        .language-img {
            width: 80px;
            height: 80px;
            margin-bottom: 20px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.9);
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .language-img img {
            max-width: 100%;
            max-height: 100%;
        }
        
        .language-name {
            font-size: 1.4rem;
            font-weight: 600;
            letter-spacing: 1px;
        }
        
        .language-back .language-name {
            font-size: 1.8rem;
            font-weight: 700;
        }
        
        .language-desc {
            font-size: 0.9rem;
            opacity: 0.9;
            line-height: 1.5;
        }
        
        footer {
            margin-top: 50px;
            padding: 20px;
            font-size: 1.1rem;
            opacity: 0.8;
        }
        
        .github-link {
            color: #92fe9d;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            margin-top: 10px;
            transition: all 0.3s;
        }
        
        .github-link:hover {
            color: #00c9ff;
            transform: translateY(-3px);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        
        .floating {
            animation: float 4s ease-in-out infinite;
        }
        
        .delay-1 { animation-delay: 0.1s; }
        .delay-2 { animation-delay: 0.2s; }
        .delay-3 { animation-delay: 0.3s; }
        .delay-4 { animation-delay: 0.4s; }
        .delay-5 { animation-delay: 0.5s; }
        .delay-6 { animation-delay: 0.6s; }
        .delay-7 { animation-delay: 0.7s; }
        .delay-8 { animation-delay: 0.8s; }
        
        @media (max-width: 768px) {
            .languages-container {
                gap: 20px;
            }
            
            .language-card {
                width: 130px;
                height: 180px;
            }
            
            h1 {
                font-size: 2.5rem;
            }
            
            .subtitle {
                font-size: 1.1rem;
            }
        }
        
        @media (max-width: 480px) {
            .languages-container {
                gap: 15px;
            }
            
            .language-card {
                width: 110px;
                height: 150px;
            }
            
            .language-img {
                width: 60px;
                height: 60px;
            }
            
            .language-name {
                font-size: 1.1rem;
            }
            
            .language-back .language-name {
                font-size: 1.4rem;
            }
            
            h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1><i class="fas fa-code"></i> Programlama Dilleri</h1>
            <p class="subtitle">GitHub profiliniz için hazırlanmış özel simge koleksiyonu. Her simgenin altında ilgili dilin adı bulunmaktadır.</p>
        </header>
        
        <div class="languages-container">
            <!-- Python -->
            <div class="language-card floating delay-1">
                <div class="language-inner">
                    <div class="language-front">
                        <div class="language-img">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" alt="Python">
                        </div>
                        <div class="language-name">Python</div>
                    </div>
                    <div class="language-back">
                        <div class="language-name">Python</div>
                        <div class="language-desc">Yüksek seviyeli, genel amaçlı programlama dili</div>
                    </div>
                </div>
            </div>
            
            <!-- Java -->
            <div class="language-card floating delay-2">
                <div class="language-inner">
                    <div class="language-front">
                        <div class="language-img">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" alt="Java">
                        </div>
                        <div class="language-name">Java</div>
                    </div>
                    <div class="language-back">
                        <div class="language-name">Java</div>
                        <div class="language-desc">Nesne yönelimli, platform bağımsız dil</div>
                    </div>
                </div>
            </div>
            
            <!-- Flutter -->
            <div class="language-card floating delay-3">
                <div class="language-inner">
                    <div class="language-front">
                        <div class="language-img">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/flutter/flutter-original.svg" alt="Flutter">
                        </div>
                        <div class="language-name">Flutter</div>
                    </div>
                    <div class="language-back">
                        <div class="language-name">Flutter</div>
                        <div class="language-desc">Google'ın çoklu platform uygulama geliştirme SDK'sı</div>
                    </div>
                </div>
            </div>
            
            <!-- SQLite -->
            <div class="language-card floating delay-4">
                <div class="language-inner">
                    <div class="language-front">
                        <div class="language-img">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/sqlite/sqlite-original.svg" alt="SQLite">
                        </div>
                        <div class="language-name">SQLite</div>
                    </div>
                    <div class="language-back">
                        <div class="language-name">SQLite</div>
                        <div class="language-desc">Hafif, gömülü ilişkisel veritabanı motoru</div>
                    </div>
                </div>
            </div>
            
            <!-- MATLAB -->
            <div class="language-card floating delay-5">
                <div class="language-inner">
                    <div class="language-front">
                        <div class="language-img">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/matlab/matlab-original.svg" alt="MATLAB">
                        </div>
                        <div class="language-name">MATLAB</div>
                    </div>
                    <div class="language-back">
                        <div class="language-name">MATLAB</div>
                        <div class="language-desc">Sayısal hesaplama ve veri görselleştirme</div>
                    </div>
                </div>
            </div>
            
            <!-- Linux -->
            <div class="language-card floating delay-6">
                <div class="language-inner">
                    <div class="language-front">
                        <div class="language-img">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/linux/linux-original.svg" alt="Linux">
                        </div>
                        <div class="language-name">Linux</div>
                    </div>
                    <div class="language-back">
                        <div class="language-name">Linux</div>
                        <div class="language-desc">Açık kaynaklı işletim sistemi çekirdeği</div>
                    </div>
                </div>
            </div>
            
            <!-- .NET -->
            <div class="language-card floating delay-7">
                <div class="language-inner">
                    <div class="language-front">
                        <div class="language-img">
                            <img src="https://skillicons.dev/icons?i=dotnet" alt=".NET">
                        </div>
                        <div class="language-name">.NET</div>
                    </div>
                    <div class="language-back">
                        <div class="language-name">.NET</div>
                        <div class="language-desc">Microsoft'un yazılım geliştirme platformu</div>
                    </div>
                </div>
            </div>
            
            <!-- MSSQL -->
            <div class="language-card floating delay-8">
                <div class="language-inner">
                    <div class="language-front">
                        <div class="language-img">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/microsoftsqlserver/microsoftsqlserver-original.svg" alt="MSSQL">
                        </div>
                        <div class="language-name">MSSQL</div>
                    </div>
                    <div class="language-back">
                        <div class="language-name">MSSQL</div>
                        <div class="language-desc">Microsoft SQL Server</div>
                    </div>
                </div>
            </div>
            
            <!-- C++ -->
            <div class="language-card floating">
                <div class="language-inner">
                    <div class="language-front">
                        <div class="language-img">
                            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/cplusplus/cplusplus-original.svg" alt="C++">
                        </div>
                        <div class="language-name">C++</div>
                    </div>
                    <div class="language-back">
                        <div class="language-name">C++</div>
                        <div class="language-desc">Nesne yönelimli sistem programlama dili</div>
                    </div>
                </div>
            </div>
        </div>
        
        <footer>
            <p>GitHub README dosyanıza eklemek için hazırlanmıştır</p>
            <a href="https://github.com" class="github-link" target="_blank">
                <i class="fab fa-github"></i> GitHub Profilinize Ekleyin
            </a>
        </footer>
    </div>
    
    <script>
        // Basit hover efekti için ek JavaScript
        document.querySelectorAll('.language-card').forEach(card => {
            card.addEventListener('mouseenter', () => {
                card.style.transform = 'scale(1.05)';
            });
            
            card.addEventListener('mouseleave', () => {
                card.style.transform = 'scale(1)';
            });
        });
    </script>
</body>
</html>
