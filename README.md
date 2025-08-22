# My-HTML-CSS-Portofolio
This is my Portofolio in HTML/CSS that's contain the program what i know.
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Galeri Sertifikat Samuel Tegar</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            padding: 20px;
        }
        
        header {
            text-align: center;
            margin-bottom: 40px;
            padding: 20px;
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            color: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
        }
        
        .certificates-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
            max-width: 1400px;
            margin: 0 auto;
        }
        
        .certificate-card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
            cursor: pointer;
            position: relative;
        }
        
        .certificate-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }
        
        .certificate-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, #6a11cb, #2575fc);
            transform: scaleX(0);
            transform-origin: left;
            transition: transform 0.3s ease;
        }
        
        .certificate-card:hover::before {
            transform: scaleX(1);
        }
        
        .certificate-img {
            height: 200px;
            background-color: #f0f4ff;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            position: relative;
        }
        
        .certificate-img::after {
            content: 'Lihat Sertifikat';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(106, 17, 203, 0.8);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 1.2rem;
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        
        .certificate-card:hover .certificate-img::after {
            opacity: 1;
        }
        
        .certificate-img i {
            font-size: 60px;
            color: #6a11cb;
            opacity: 0.7;
        }
        
        .certificate-content {
            padding: 20px;
        }
        
        .certificate-title {
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 10px;
            color: #2c3e50;
        }
        
        .certificate-desc {
            font-size: 0.9rem;
            color: #7f8c8d;
            margin-bottom: 15px;
            line-height: 1.5;
        }
        
        .certificate-date {
            font-size: 0.85rem;
            color: #6a11cb;
            font-weight: 500;
        }
        
        .certificate-type {
            display: inline-block;
            padding: 4px 10px;
            background: #eef4ff;
            color: #2575fc;
            border-radius: 20px;
            font-size: 0.75rem;
            font-weight: 600;
            margin-top: 10px;
        }
        
        footer {
            text-align: center;
            margin-top: 50px;
            padding: 20px;
            color: #7f8c8d;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .certificates-container {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Galeri Sertifikat</h1>
        <p class="subtitle">Samuel Tegar Mardhika Ariadi</p>
    </header>
    
    <div class="certificates-container">
        <!-- Sertifikat 1 -->
        <div class="certificate-card">
            <div class="certificate-img">
                <i>📄</i>
            </div>
            <div class="certificate-content">
                <h3 class="certificate-title">Certificate of Appreciation - POSKO VISUAL 2024</h3>
                <p class="certificate-desc">For outstanding performance as Member of Sponsorship in POSKO VISUAL International Poster Exhibition 2024.</p>
                <p class="certificate-date">October 2024</p>
                <span class="certificate-type">Penghargaan</span>
            </div>
        </div>
        
        <!-- Sertifikat 2 -->
        <div class="certificate-card">
            <div class="certificate-img">
                <i>📄</i>
            </div>
            <div class="certificate-content">
                <h3 class="certificate-title">Sertifikat Pelatihan Bahasa Mandarin</h3>
                <p class="certificate-desc">Telah menyelesaikan 24 jam pelatihan bahasa Mandarin di Confucius Institute Universitas Negeri Malang.</p>
                <p class="certificate-date">Februari - Mei 2022</p>
                <span class="certificate-type">Bahasa</span>
            </div>
        </div>
        
        <!-- Sertifikat 3 -->
        <div class="certificate-card">
            <div class="certificate-img">
                <i>📄</i>
            </div>
            <div class="certificate-content">
                <h3 class="certificate-title">English Proficiency Test</h3>
                <p class="certificate-desc">Telah mengikuti tes kemampuan bahasa Inggris dengan tingkat Pre-Advanced dan total skor 447.</p>
                <p class="certificate-date">Agustus 2022</p>
                <span class="certificate-type">Bahasa</span>
            </div>
        </div>
        
        <!-- Sertifikat 4 -->
        <div class="certificate-card">
            <div class="certificate-img">
                <i>📄</i>
            </div>
            <div class="certificate-content">
                <h3 class="certificate-title">WP Pro Course Completion</h3>
                <p class="certificate-desc">Successfully completed WP Pro Course dengan topik "Design Thinking, Web Development and SEO".</p>
                <p class="certificate-date">September 2022</p>
                <span class="certificate-type">Teknologi</span>
            </div>
        </div>
        
        <!-- Sertifikat 5 -->
        <div class="certificate-card">
            <div class="certificate-img">
                <i>📄</i>
            </div>
            <div class="certificate-content">
                <h3 class="certificate-title">Pendanaan PKM-RSH 2023</h3>
                <p class="certificate-desc">Sebagai peraih pendanaan bidang PKM-RSH dengan judul "Telisik Ratu Adil di Indonesia".</p>
                <p class="certificate-date">November 2023</p>
                <span class="certificate-type">Penelitian</span>
            </div>
        </div>
        
        <!-- Sertifikat 6 -->
        <div class="certificate-card">
            <div class="certificate-img">
                <i>📄</i>
            </div>
            <div class="certificate-content">
                <h3 class="certificate-title">Certificate of Participation - POSKO VISUAL 2023</h3>
                <p class="certificate-desc">For being selected designer at Posko Visual 2023 International Exhibition.</p>
                <p class="certificate-date">Oktober 2023</p>
                <span class="certificate-type">Desain</span>
            </div>
        </div>
    </div>
    
    <footer>
        <p>© 2024 Galeri Sertifikat Samuel Tegar</p>
    </footer>
</body>
</html>
