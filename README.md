[New Text Document.html](https://github.com/user-attachments/files/30873479/New.Text.Document.html)
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HUT SMKN 1 Leles & Reuni Akbar 2026</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        *{margin:0;padding:0;box-sizing:border-box}
        :root{--navy:#092C55;--teal:#0B8F88;--white:#fff;--light-gray:#F4F7FA;--gray:#6B7280;--dark-gray:#374151;--gold:#D4AF37;--shadow:0 4px 20px rgba(0,0,0,0.1);--shadow-hover:0 8px 30px rgba(0,0,0,0.15);--radius:16px;--transition:all 0.3s ease}
        body{font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,Arial,sans-serif;background:var(--white);color:var(--dark-gray);line-height:1.6}
        a{text-decoration:none}
        .container{max-width:1200px;margin:0 auto;padding:0 20px}
        .btn{display:inline-flex;align-items:center;gap:10px;padding:12px 28px;border:none;border-radius:50px;font-size:16px;font-weight:600;cursor:pointer;transition:var(--transition);text-decoration:none;font-family:inherit}
        .btn-primary{background:var(--teal);color:var(--white)}.btn-primary:hover{background:#0a7a74;transform:translateY(-2px);box-shadow:var(--shadow-hover)}
        .btn-secondary{background:var(--navy);color:var(--white)}.btn-secondary:hover{background:#072144;transform:translateY(-2px);box-shadow:var(--shadow-hover)}
        .btn-gold{background:var(--gold);color:var(--navy)}.btn-gold:hover{background:#c4a035;transform:translateY(-2px);box-shadow:var(--shadow-hover)}
        .btn-outline{background:transparent;border:2px solid var(--teal);color:var(--teal)}.btn-outline:hover{background:var(--teal);color:var(--white)}
        .btn-sm{padding:8px 16px;font-size:14px}
        .btn-danger{background:#dc3545;color:var(--white)}.btn-danger:hover{background:#c82333}
        .btn-success{background:#28a745;color:var(--white)}.btn-success:hover{background:#1e7e34}
        .btn-warning{background:#ffc107;color:#000}.btn-warning:hover{background:#e0a800}
        .btn-edit{background:#ffc107;color:#000}.btn-edit:hover{background:#e0a800}
        .btn-delete{background:#dc3545;color:#fff}.btn-delete:hover{background:#c82333}
        .btn-status{background:#17a2b8;color:#fff}.btn-status:hover{background:#138496}
        .header{background:var(--navy);color:var(--white);padding:15px 0;position:sticky;top:0;z-index:1000;box-shadow:0 2px 10px rgba(0,0,0,0.2)}
        .header-content{display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:15px}
        .logo-wrapper{display:flex;align-items:center;gap:15px}
        .logo-image{width:50px;height:50px;object-fit:contain;border-radius:8px;background:var(--white);padding:4px;display:none}
        .logo-text h1{font-size:22px;color:var(--teal)}.logo-text small{display:block;font-size:12px;opacity:0.8}
        .nav-menu{display:flex;gap:20px;list-style:none;flex-wrap:wrap;align-items:center}
        .nav-menu a{color:var(--white);text-decoration:none;font-size:14px;padding:5px 10px;border-radius:5px;transition:var(--transition)}
        .nav-menu a:hover{background:rgba(11,143,136,0.3)}
        .nav-menu .btn-login{background:var(--teal);padding:5px 20px;border-radius:20px}.nav-menu .btn-login:hover{background:#0a7a74}
        .menu-toggle{display:none;background:none;border:none;color:var(--white);font-size:24px;cursor:pointer}

        /* ===== HERO DENGAN BACKGROUND GAMBAR ===== */
        .hero{
            position:relative;
            min-height:100vh;
            display:flex;
            align-items:center;
            justify-content:center;
            text-align:center;
            color:var(--white);
            overflow:hidden;
            padding:120px 0 80px;
        }
        
        /* Background Gambar dengan efek blur & transparansi */
        .hero-bg{
            position:absolute;
            top:0;
            left:0;
            right:0;
            bottom:0;
            background-image:url('data:image/svg+xml,%3Csvg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"%3E%3Crect width="100" height="100" fill="%23092C55"/%3E%3Ctext x="50" y="50" font-size="20" text-anchor="middle" fill="%230B8F88" font-family="Arial"%3ESMK%3C/text%3E%3C/svg%3E');
            background-size:cover;
            background-position:center;
            background-repeat:no-repeat;
            filter:blur(8px) brightness(0.4);
            transform:scale(1.05);
            z-index:0;
            transition:all 0.5s ease;
        }
        
        /* Overlay gelap untuk membuat teks lebih terbaca */
        .hero-overlay{
            position:absolute;
            top:0;
            left:0;
            right:0;
            bottom:0;
            background:rgba(9,44,85,0.6);
            z-index:1;
        }
        
        .hero-content{
            position:relative;
            z-index:2;
        }
        
        .hero-badge{
            display:inline-block;
            padding:8px 24px;
            background:rgba(212,175,55,0.2);
            border:1px solid rgba(212,175,55,0.3);
            border-radius:50px;
            font-size:14px;
            font-weight:500;
            color:var(--gold);
            margin-bottom:20px;
        }
        .hero h1{font-size:52px;font-weight:800;margin-bottom:15px;line-height:1.2;text-shadow:0 2px 20px rgba(0,0,0,0.5)}
        .hero .slogan{font-size:24px;font-weight:300;opacity:0.95;font-style:italic;margin-bottom:30px;text-shadow:0 2px 10px rgba(0,0,0,0.5)}
        .hero-info{display:flex;justify-content:center;gap:40px;flex-wrap:wrap;margin-bottom:30px}
        .hero-info span{display:flex;align-items:center;gap:8px;font-size:18px;opacity:0.95;text-shadow:0 2px 10px rgba(0,0,0,0.5)}
        .hero-info i{color:var(--gold)}
        .hero-buttons{display:flex;justify-content:center;gap:20px;flex-wrap:wrap;margin-top:20px}
        .countdown-wrapper{margin:30px 0}
        .countdown{display:flex;justify-content:center;gap:20px;flex-wrap:wrap}
        .countdown-item{background:rgba(255,255,255,0.1);backdrop-filter:blur(10px);padding:16px 28px;border-radius:12px;border:1px solid rgba(255,255,255,0.1);min-width:80px;text-align:center}
        .countdown-item .number{font-size:36px;font-weight:700;color:var(--gold);display:block}
        .countdown-item .label{font-size:14px;opacity:0.7}

        .stats-section{padding:60px 0;background:var(--light-gray)}
        .stats-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:24px;margin-bottom:40px}
        .stat-card{background:var(--white);padding:24px;border-radius:var(--radius);box-shadow:var(--shadow);text-align:center;transition:var(--transition)}
        .stat-card:hover{transform:translateY(-4px);box-shadow:var(--shadow-hover)}
        .stat-card .icon{font-size:32px;color:var(--teal);margin-bottom:10px}
        .stat-card .label{font-size:14px;color:var(--gray);font-weight:500}
        .stat-card .value{font-size:24px;font-weight:700;color:var(--navy);margin-top:5px}
        .stat-card .value.teal{color:var(--teal)}.stat-card .value.gold{color:var(--gold)}
        .progress-section{background:var(--white);padding:32px;border-radius:var(--radius);box-shadow:var(--shadow)}
        .progress-header{display:flex;justify-content:space-between;align-items:center;margin-bottom:12px}
        .progress-header .label{font-weight:600;font-size:18px;color:var(--navy)}
        .progress-header .percentage{font-weight:700;font-size:18px;color:var(--teal)}
        .progress-bar{width:100%;height:12px;background:var(--light-gray);border-radius:50px;overflow:hidden}
        .progress-bar .fill{height:100%;background:linear-gradient(90deg,var(--gold),var(--teal));border-radius:50px;transition:width 1.5s ease;width:0%}
        .progress-details{display:flex;justify-content:space-between;margin-top:12px;font-size:14px;color:var(--gray)}
        .dana-details{display:grid;grid-template-columns:repeat(3,1fr);gap:15px;margin-top:20px}
        .dana-item{background:var(--white);padding:15px;border-radius:10px;text-align:center;box-shadow:0 2px 8px rgba(0,0,0,0.05);border-left:4px solid var(--teal);transition:var(--transition)}
        .dana-item:hover{transform:translateY(-2px);box-shadow:var(--shadow-hover)}
        .dana-item .label{font-size:13px;color:var(--gray)}
        .dana-item .value{font-size:20px;font-weight:700;margin-top:4px}
        .dana-item .value.teal{color:var(--teal)}.dana-item .value.gold{color:var(--gold)}
        .dana-item .count{font-size:11px;color:var(--gray);margin-top:3px}
        .total-ringkasan{margin-top:15px;padding:12px;background:var(--navy);border-radius:10px;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:10px}
        .total-ringkasan .label{font-size:13px;opacity:0.8;color:var(--white)}
        .total-ringkasan .value{font-size:20px;font-weight:700}
        .total-ringkasan .value.gold{color:var(--gold)}
        .total-ringkasan .value.red{color:#ff6b6b}
        .section{padding:60px 0}
        .section-gray{background:var(--light-gray)}
        .section-title{font-size:32px;font-weight:700;text-align:center;color:var(--navy);margin-bottom:40px}
        .section-title i{color:var(--gold);margin-right:10px}
        .section-title .highlight{color:var(--gold)}
        .table-wrapper{background:var(--white);border-radius:var(--radius);box-shadow:var(--shadow);padding:20px;overflow-x:auto}
        .table-wrapper table{width:100%;border-collapse:collapse}
        .table-wrapper thead{background:var(--navy);color:var(--white)}
        .table-wrapper th{padding:14px 18px;text-align:left;font-weight:600}
        .table-wrapper td{padding:12px 18px;border-bottom:1px solid #eee}
        .table-wrapper tbody tr:hover{background:var(--light-gray)}
        .table-wrapper .highlight-row{background:rgba(212,175,55,0.1)}
        .badge-acara{display:inline-block;padding:2px 12px;border-radius:50px;font-size:11px;font-weight:600;background:var(--gold);color:var(--navy)}
        .sponsor-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:25px}
        .sponsor-card{background:var(--white);padding:25px;border-radius:var(--radius);box-shadow:var(--shadow);transition:var(--transition);border-left:4px solid var(--teal);text-align:center}
        .sponsor-card:hover{transform:translateY(-5px);box-shadow:var(--shadow-hover)}
        .sponsor-card .logo-container{width:100px;height:100px;margin:0 auto 15px;display:flex;align-items:center;justify-content:center;background:var(--light-gray);border-radius:50%;overflow:hidden;border:3px solid var(--teal)}
        .sponsor-card .logo-container img{width:100%;height:100%;object-fit:cover}
        .sponsor-card .logo-container .no-logo{font-size:40px;opacity:0.3}
        .sponsor-card .name{font-size:18px;font-weight:600;color:var(--navy)}
        .sponsor-card .amount{font-size:22px;font-weight:700;color:var(--teal);margin:8px 0}
        .sponsor-card .date{font-size:13px;color:var(--gray)}
        .sponsor-card .status{display:inline-block;padding:4px 14px;border-radius:50px;font-size:12px;font-weight:600;margin-top:8px}
        .status-diterima{background:#d4edda;color:#155724}
        .status-menunggu{background:#fff3cd;color:#856404}
        .sponsor-card .description{font-size:13px;color:var(--gray);margin-top:8px;font-style:italic}
        .sponsor-card .category-tag{display:inline-block;padding:2px 12px;border-radius:50px;font-size:11px;font-weight:600;background:var(--navy);color:var(--white);margin-top:5px}
        .kaos-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:20px}
        .kaos-card{background:var(--white);border-radius:var(--radius);box-shadow:var(--shadow);overflow:hidden;transition:var(--transition);cursor:pointer}
        .kaos-card:hover{transform:translateY(-5px);box-shadow:var(--shadow-hover)}
        .kaos-card .kaos-image{height:180px;display:flex;align-items:center;justify-content:center;font-size:72px;background:var(--light-gray)}
        .kaos-card .kaos-info{padding:15px}
        .kaos-card .kaos-info h4{color:var(--navy);font-size:16px}
        .kaos-card .kaos-info .harga{font-size:20px;font-weight:700;color:var(--teal)}
        .kaos-card .kaos-info .detail{font-size:13px;color:var(--gray);margin:4px 0}
        .badge-status{display:inline-block;padding:2px 12px;border-radius:50px;font-size:11px;font-weight:600}
        .badge-tersedia{background:#d4edda;color:#155724}
        .badge-habis{background:#f8d7da;color:#721c24}
        .badge-pesanan{background:#cce5ff;color:#004085}
        .kontak-box{background:var(--white);padding:40px;border-radius:var(--radius);box-shadow:var(--shadow);text-align:center;max-width:600px;margin:0 auto}
        .kontak-box .icon{font-size:48px;color:var(--teal);margin-bottom:15px}
        .kontak-box h3{font-size:24px;color:var(--navy);margin-bottom:15px}
        .kontak-item{display:flex;align-items:center;justify-content:center;gap:12px;padding:10px 0;font-size:16px;border-bottom:1px solid var(--light-gray)}
        .kontak-item:last-child{border-bottom:none}
        .kontak-item i{color:var(--teal);width:24px}
        .kontak-item a{color:var(--navy);text-decoration:none;transition:var(--transition)}
        .kontak-item a:hover{color:var(--teal)}
        .kontak-item .wa-name{font-weight:600;color:var(--teal)}
        .footer{background:var(--navy);color:var(--white);padding:40px 0;text-align:center}
        .footer .footer-logo{display:flex;align-items:center;justify-content:center;gap:15px;margin-bottom:10px}
        .footer .footer-logo img{width:40px;height:40px;object-fit:contain;background:var(--white);border-radius:8px;padding:4px;display:none}
        .footer h3{color:var(--gold)}
        .footer .slogan-footer{font-style:italic;opacity:0.8;margin:5px 0}
        .footer .copyright{font-size:12px;opacity:0.6;margin-top:15px}
        .loading{text-align:center;padding:40px}
        .spinner{border:4px solid var(--light-gray);border-top:4px solid var(--teal);border-radius:50%;width:40px;height:40px;animation:spin 1s linear infinite;margin:0 auto 15px}
        @keyframes spin{0%{transform:rotate(0deg)}100%{transform:rotate(360deg)}}
        .modal-overlay{display:none;position:fixed;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,0.5);backdrop-filter:blur(4px);z-index:2000;align-items:center;justify-content:center}
        .modal-overlay.show{display:flex}
        .modal{background:var(--white);border-radius:var(--radius);padding:32px;max-width:700px;width:90%;max-height:90vh;overflow-y:auto;animation:slideUp 0.3s ease}
        @keyframes slideUp{from{transform:translateY(20px);opacity:0}to{transform:translateY(0);opacity:1}}
        .modal-header{display:flex;justify-content:space-between;align-items:center;margin-bottom:20px}
        .modal-header h2{color:var(--navy);font-size:22px}
        .modal-close{background:none;border:none;font-size:28px;cursor:pointer;color:var(--gray);transition:var(--transition)}
        .modal-close:hover{color:var(--navy)}
        .form-group{margin-bottom:18px}
        .form-group label{display:block;font-weight:500;margin-bottom:6px;color:var(--navy)}
        .form-group input,.form-group select,.form-group textarea{width:100%;padding:10px 14px;border:2px solid #e2e8f0;border-radius:8px;font-size:15px;transition:var(--transition);font-family:inherit}
        .form-group input:focus,.form-group select:focus,.form-group textarea:focus{outline:none;border-color:var(--teal);box-shadow:0 0 0 3px rgba(11,143,136,0.1)}
        .form-group textarea{resize:vertical;min-height:80px}
        .form-row{display:grid;grid-template-columns:1fr 1fr;gap:15px}
        @media(max-width:600px){.form-row{grid-template-columns:1fr}}
        .file-upload-wrapper{position:relative}
        .file-upload-wrapper input[type="file"]{position:absolute;opacity:0;width:100%;height:100%;cursor:pointer}
        .file-upload-wrapper .file-label{display:block;padding:12px 16px;border:2px dashed #e2e8f0;border-radius:8px;text-align:center;color:var(--gray);transition:var(--transition);cursor:pointer}
        .file-upload-wrapper .file-label:hover{border-color:var(--teal);color:var(--teal)}
        .file-upload-wrapper .file-label i{font-size:24px;display:block;margin-bottom:5px}
        .image-preview{margin-top:10px;text-align:center}
        .image-preview img{max-width:100px;max-height:100px;border-radius:8px;border:2px solid #e2e8f0;padding:4px;object-fit:cover}
        .admin-table-wrap{overflow-x:auto;margin-top:10px}
        .admin-table{width:100%;border-collapse:collapse;font-size:14px}
        .admin-table th{background:var(--navy);color:var(--white);padding:10px 12px;text-align:left;white-space:nowrap}
        .admin-table td{padding:10px 12px;border-bottom:1px solid #eee;vertical-align:middle}
        .admin-table tr:hover{background:var(--light-gray)}
        .admin-table .actions{display:flex;gap:5px;flex-wrap:wrap}
        .admin-table .actions button{padding:4px 10px;border:none;border-radius:4px;font-size:12px;cursor:pointer;transition:var(--transition)}
        .admin-tabs{display:flex;gap:5px;flex-wrap:wrap;margin-bottom:20px;border-bottom:2px solid var(--light-gray);padding-bottom:10px}
        .admin-tabs button{padding:8px 20px;border:none;border-radius:8px;cursor:pointer;font-weight:600;transition:var(--transition);background:var(--light-gray);color:var(--gray)}
        .admin-tabs button:hover{background:var(--teal);color:#fff}
        .admin-tabs button.active{background:var(--navy);color:#fff}
        .tab-content{display:none}
        .tab-content.active{display:block}
        .notification{position:fixed;top:20px;right:20px;padding:15px 25px;border-radius:10px;color:white;font-weight:500;z-index:3000;animation:slideIn 0.3s ease;box-shadow:var(--shadow-hover)}
        .notification.success{background:#28a745}
        .notification.error{background:#dc3545}
        .notification.info{background:var(--teal)}
        @keyframes slideIn{from{transform:translateX(100%);opacity:0}to{transform:translateX(0);opacity:1}}
        @media(max-width:1024px){.stats-grid{grid-template-columns:repeat(2,1fr)}.dana-details{grid-template-columns:repeat(2,1fr)}}
        @media(max-width:768px){.menu-toggle{display:block}.nav-menu{display:none;width:100%;flex-direction:column;align-items:center;padding:20px 0;gap:15px}.nav-menu.open{display:flex}.hero h1{font-size:32px}.hero .slogan{font-size:18px}.hero-info{flex-direction:column;gap:10px;align-items:center}.countdown{gap:12px}.countdown-item{padding:12px 18px;min-width:60px}.countdown-item .number{font-size:24px}.stats-grid{grid-template-columns:1fr}.dana-details{grid-template-columns:1fr}.sponsor-grid,.kaos-grid{grid-template-columns:1fr}.hero-buttons{flex-direction:column;align-items:center}.btn{width:100%;justify-content:center}.section-title{font-size:24px}.logo-image{width:40px;height:40px}.logo-text h1{font-size:18px}.modal{padding:20px}}
        @media(max-width:480px){.hero h1{font-size:24px}.logo-text h1{font-size:16px}.stat-card .value{font-size:20px}.admin-tabs button{font-size:12px;padding:6px 12px}}
        @media print{.header,.footer,.hero-buttons,.btn,.admin-actions,.menu-toggle{display:none!important}.hero{padding:40px 0!important;background:var(--navy)!important}.section{padding:30px 0!important}.table-wrapper{box-shadow:none!important;border:1px solid #ddd!important}}
        
        .rekening-info{background:var(--light-gray);padding:15px;border-radius:10px;margin:15px 0;text-align:center}
        .rekening-info .bank{font-weight:700;color:var(--teal);font-size:18px}
        .rekening-info .no-rek{font-size:24px;font-weight:700;color:var(--navy);margin:5px 0}
        .rekening-info .atas-nama{color:var(--gray)}
        .hidden{display:none}
        
        .folder-badge{display:inline-block;padding:2px 12px;border-radius:50px;font-size:10px;font-weight:600;background:var(--gold);color:var(--navy);margin-left:5px}
        
        /* Folder View */
        .folder-view{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:20px}
        .folder-card{background:var(--white);padding:30px;border-radius:var(--radius);box-shadow:var(--shadow);text-align:center;transition:var(--transition);cursor:pointer;border:2px solid var(--light-gray)}
        .folder-card:hover{transform:translateY(-5px);box-shadow:var(--shadow-hover);border-color:var(--teal)}
        .folder-card .folder-icon{font-size:64px;margin-bottom:10px}
        .folder-card .folder-name{font-size:18px;font-weight:600;color:var(--navy)}
        .folder-card .folder-count{font-size:13px;color:var(--gray)}
        .folder-card .folder-color{width:100%;height:4px;border-radius:4px;margin-top:10px}
        
        /* Background Preview di Admin */
        .bg-preview-box{width:100%;height:150px;border-radius:12px;background-size:cover;background-position:center;border:2px dashed #e2e8f0;display:flex;align-items:center;justify-content:center;color:var(--gray);font-size:14px;transition:all 0.3s}
        .bg-preview-box.has-bg{color:var(--white);text-shadow:0 2px 10px rgba(0,0,0,0.5)}
        .bg-preview-box .fa-image{font-size:40px;opacity:0.5}
    </style>
</head>
<body>
    <!-- ===== HEADER ===== -->
    <header class="header">
        <div class="container header-content">
            <div class="logo-wrapper">
                <img src="" alt="Logo SMKN 1 Leles" class="logo-image" id="schoolLogo">
                <div class="logo-text">
                    <h1>SMK NEGERI 1 LELES</h1>
                    <small>HUT ke-19 & Reuni Akbar 2026</small>
                </div>
            </div>
            <button class="menu-toggle" onclick="toggleMenu()"><i class="fas fa-bars"></i></button>
            <nav>
                <ul class="nav-menu" id="navMenu">
                    <li><a href="#home">Beranda</a></li>
                    <li><a href="#rundown">Rundown</a></li>
                    <li><a href="#anggaran">Anggaran</a></li>
                    <li><a href="#kaos">Kaos</a></li>
                    <li><a href="#donatur">Donatur</a></li>
                    <li><a href="#sponsor">Sponsor</a></li>
                    <li><a href="#galeri">Galeri</a></li>
                    <li><a href="#kontak">Kontak</a></li>
                    <li><a href="#" class="btn-login" onclick="openLogin()"><i class="fas fa-lock"></i> Login Admin</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- ===== HERO DENGAN BACKGROUND ===== -->
    <section class="hero" id="home">
        <div class="hero-bg" id="heroBg"></div>
        <div class="hero-overlay"></div>
        <div class="container hero-content">
            <div class="hero-badge"><i class="fas fa-star"></i> HUT ke-19 & Reuni Akbar</div>
            <h1>HUT ke-19 SMK Negeri 1 Leles<br>& Reuni Akbar 2026</h1>
            <p class="slogan" id="heroSlogan">"Bersama Mengenang, Berkarya, dan Menginspirasi"</p>
            <div class="hero-info">
                <span><i class="fas fa-calendar-alt"></i> <span id="heroDate">Senin, 24 Agustus 2026</span></span>
                <span><i class="fas fa-map-marker-alt"></i> <span id="heroLocation">SMK Negeri 1 Leles</span></span>
            </div>
            <div class="countdown-wrapper">
                <div class="countdown" id="countdown">
                    <div class="countdown-item"><span class="number" id="days">00</span><span class="label">Hari</span></div>
                    <div class="countdown-item"><span class="number" id="hours">00</span><span class="label">Jam</span></div>
                    <div class="countdown-item"><span class="number" id="minutes">00</span><span class="label">Menit</span></div>
                    <div class="countdown-item"><span class="number" id="seconds">00</span><span class="label">Detik</span></div>
                </div>
            </div>
            <div class="hero-buttons">
                <a href="#rundown" class="btn btn-gold"><i class="fas fa-clock"></i> Lihat Rundown</a>
                <a href="#kaos" class="btn btn-secondary"><i class="fas fa-tshirt"></i> Pesan Kaos</a>
            </div>
        </div>
    </section>

    <!-- ===== STATS ===== -->
    <section class="stats-section" id="stats">
        <div class="container">
            <div class="stats-grid" id="statsGrid">
                <div class="stat-card"><div class="icon"><i class="fas fa-bullseye"></i></div><div class="label">Target Dana</div><div class="value" id="targetFund">Rp 40.000.000</div></div>
                <div class="stat-card"><div class="icon"><i class="fas fa-money-bill-wave"></i></div><div class="label">Total Dana Masuk</div><div class="value teal" id="danaMasuk">Rp 2.050.000</div></div>
                <div class="stat-card"><div class="icon"><i class="fas fa-users"></i></div><div class="label">Total Donatur</div><div class="value" id="sponsorCount">3 Donatur</div></div>
                <div class="stat-card"><div class="icon"><i class="fas fa-tshirt"></i></div><div class="label">Kaos Terjual</div><div class="value gold" id="kaosCount">0 Kaos</div></div>
            </div>
            
            <div class="progress-section">
                <div class="progress-header"><span class="label"><i class="fas fa-chart-line"></i> Progress Dana</span><span class="percentage" id="progressPercent">5.1%</span></div>
                <div class="progress-bar"><div class="fill" id="progressFill" style="width:5.1%"></div></div>
                <div class="progress-details">
                    <span><i class="fas fa-coins"></i> Terkumpul: <strong id="progressTerkumpul">Rp 2.050.000</strong></span>
                    <span><i class="fas fa-flag-checkered"></i> Target: <strong id="progressTarget">Rp 40.000.000</strong></span>
                </div>
                <div class="dana-details">
                    <div class="dana-item" style="border-left-color:var(--teal);">
                        <div class="label">💝 Dari Donatur</div>
                        <div class="value teal" id="danaDonatur">Rp 2.050.000</div>
                        <div class="count" id="danaDonaturCount">3 Donatur</div>
                    </div>
                    <div class="dana-item" style="border-left-color:var(--gold);">
                        <div class="label">🏢 Dari Sponsor</div>
                        <div class="value gold" id="danaSponsor">Rp 0</div>
                        <div class="count" id="danaSponsorCount">0 Sponsor</div>
                    </div>
                    <div class="dana-item" style="border-left-color:#ff6b6b;">
                        <div class="label">👕 Dari Penjualan Kaos</div>
                        <div class="value" style="color:#ff6b6b;" id="danaKaos">Rp 0</div>
                        <div class="count" id="danaKaosCount">0 Kaos Terjual</div>
                    </div>
                </div>
                <div class="total-ringkasan">
                    <div><div class="label">Total Dana Masuk</div><div class="value gold" id="totalDanaMasuk">Rp 2.050.000</div></div>
                    <div style="text-align:center;"><div class="label">Kekurangan</div><div class="value red" id="totalKekurangan">Rp 37.950.000</div></div>
                    <div style="text-align:right;"><div class="label">Progress</div><div class="value gold" id="totalProgress">5.1%</div></div>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== RUNDOWN ===== -->
    <section class="section" id="rundown">
        <div class="container">
            <h2 class="section-title"><i class="fas fa-clock"></i> Rundown <span class="highlight">Acara</span></h2>
            <div class="table-wrapper" id="rundownContainer"><div class="loading"><div class="spinner"></div><p>Memuat data...</p></div></div>
        </div>
    </section>

    <!-- ===== ANGGARAN ===== -->
    <section class="section section-gray" id="anggaran">
        <div class="container">
            <h2 class="section-title"><i class="fas fa-calculator"></i> Anggaran <span class="highlight">Dana</span></h2>
            <div class="table-wrapper" id="anggaranContainer"><div class="loading"><div class="spinner"></div><p>Memuat data...</p></div></div>
        </div>
    </section>

    <!-- ===== KAOS ===== -->
    <section class="section" id="kaos">
        <div class="container">
            <h2 class="section-title"><i class="fas fa-tshirt"></i> Kaos <span class="highlight">HUT & Reuni</span></h2>
            <div class="kaos-grid" id="kaosContainer"><div class="loading"><div class="spinner"></div><p>Memuat data...</p></div></div>
        </div>
    </section>

    <!-- ===== DONATUR ===== -->
    <section class="section section-gray" id="donatur">
        <div class="container">
            <h2 class="section-title"><i class="fas fa-handshake"></i> Donatur & <span class="highlight">Alumni</span></h2>
            <div class="sponsor-grid" id="donaturContainer"><div class="loading"><div class="spinner"></div><p>Memuat data...</p></div></div>
        </div>
    </section>

    <!-- ===== SPONSOR ===== -->
    <section class="section" id="sponsor">
        <div class="container">
            <h2 class="section-title"><i class="fas fa-building"></i> Sponsor <span class="highlight">Acara</span></h2>
            <div class="sponsor-grid" id="sponsorContainer"><div class="loading"><div class="spinner"></div><p>Memuat data...</p></div></div>
        </div>
    </section>

    <!-- ===== GALERI ===== -->
    <section class="section section-gray" id="galeri">
        <div class="container">
            <h2 class="section-title"><i class="fas fa-images"></i> Galeri <span class="highlight">Kegiatan</span></h2>
            <div style="display:flex;gap:10px;flex-wrap:wrap;justify-content:center;margin-bottom:30px">
                <button class="btn btn-sm btn-primary" onclick="filterGallery('all')">📁 Semua</button>
                <button class="btn btn-sm btn-outline" onclick="filterGallery('persiapan')">📁 Persiapan Panggung</button>
                <button class="btn btn-sm btn-outline" onclick="filterGallery('dekorasi')">📁 Dekorasi Acara</button>
                <button class="btn btn-sm btn-outline" onclick="filterGallery('latihan')">📁 Latihan Siswa</button>
                <button class="btn btn-sm btn-outline" onclick="filterGallery('spot')">📁 Spot Foto</button>
                <button class="btn btn-sm btn-gold" onclick="filterGallery('alumni')">📁 Foto Alumni</button>
            </div>
            <div style="display:flex;gap:15px;flex-wrap:wrap;justify-content:center;margin-bottom:25px;font-size:13px;color:var(--gray)">
                <span>📁 Persiapan: <strong id="count-persiapan">0</strong> foto</span>
                <span>📁 Dekorasi: <strong id="count-dekorasi">0</strong> foto</span>
                <span>📁 Latihan: <strong id="count-latihan">0</strong> foto</span>
                <span>📁 Spot Foto: <strong id="count-spot">0</strong> foto</span>
                <span>📁 Alumni: <strong id="count-alumni">0</strong> foto</span>
            </div>
            <div id="galeriContainer"><div class="loading"><div class="spinner"></div><p>Memuat galeri...</p></div></div>
        </div>
    </section>

    <!-- ===== KONTAK ===== -->
    <section class="section" id="kontak">
        <div class="container">
            <h2 class="section-title"><i class="fas fa-phone-alt"></i> Hubungi <span class="highlight">Panitia</span></h2>
            <div class="kontak-box">
                <div class="icon"><i class="fas fa-headset"></i></div>
                <h3>Panitia HUT & Reuni Akbar</h3>
                <div class="kontak-item"><i class="fab fa-whatsapp"></i><div><span class="wa-name">Pirman</span><br><a href="https://wa.me/6281223913350" target="_blank">0812-2391-3350</a></div></div>
                <div class="kontak-item"><i class="fab fa-whatsapp"></i><div><span class="wa-name">Abdul Aris</span><br><a href="https://wa.me/6285794325300" target="_blank">0857-9432-5300</a></div></div>
                <div class="kontak-item"><i class="fas fa-envelope"></i><a href="mailto:panitia@smkn1leles.sch.id">panitia@smkn1leles.sch.id</a></div>
                <div class="kontak-item"><i class="fas fa-map-marker-alt"></i><span id="kontakLocation">SMK Negeri 1 Leles, Jawa Barat</span></div>
                <div style="display:flex;gap:10px;flex-wrap:wrap;justify-content:center;margin-top:20px">
                    <a href="https://wa.me/6281223913350" target="_blank" class="btn btn-primary"><i class="fab fa-whatsapp"></i> Hubungi Pirman</a>
                    <a href="https://wa.me/6285794325300" target="_blank" class="btn btn-secondary"><i class="fab fa-whatsapp"></i> Hubungi Abdul Aris</a>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== FOOTER ===== -->
    <footer class="footer">
        <div class="container">
            <div class="footer-logo"><img src="" alt="Logo" id="footerLogo"><h3>SMK NEGERI 1 LELES</h3></div>
            <p class="slogan-footer" id="footerSlogan">"Bersama Mengenang, Berkarya, dan Menginspirasi"</p>
            <p style="font-size:14px;opacity:0.8">HUT ke-19 & Reuni Akbar 2026</p>
            <p class="copyright">&copy; 2026 - All Rights Reserved</p>
        </div>
    </footer>

    <!-- ===== MODALS ===== -->

    <!-- LOGIN MODAL -->
    <div class="modal-overlay" id="loginModal">
        <div class="modal">
            <div class="modal-header"><h2><i class="fas fa-lock" style="color:var(--teal)"></i> Login Admin</h2><button class="modal-close" onclick="closeLogin()">&times;</button></div>
            <form id="loginForm" onsubmit="handleLogin(event)">
                <div class="form-group"><label>Email</label><input type="email" id="loginEmail" placeholder="admin@smkn1leles.sch.id" required></div>
                <div class="form-group"><label>Password</label><input type="password" id="loginPassword" placeholder="Masukkan password" required></div>
                <button type="submit" class="btn btn-primary" style="width:100%;justify-content:center"><i class="fas fa-sign-in-alt"></i> MASUK</button>
            </form>
        </div>
    </div>

    <!-- ADMIN DASHBOARD -->
    <div class="modal-overlay" id="adminModal">
        <div class="modal" style="max-width:950px">
            <div class="modal-header"><h2><i class="fas fa-tachometer-alt" style="color:var(--teal)"></i> Dashboard Admin</h2><button class="modal-close" onclick="closeAdmin()">&times;</button></div>
            <div id="adminContent">
                <div style="background:var(--light-gray);padding:15px;border-radius:12px;margin-bottom:15px">
                    <div style="display:flex;align-items:center;gap:15px;flex-wrap:wrap">
                        <div id="adminLogoPreview" style="width:60px;height:60px;background:#fff;border-radius:12px;display:flex;align-items:center;justify-content:center;border:2px dashed #ddd;overflow:hidden"><span style="color:#ccc;font-size:12px">Logo</span></div>
                        <div style="flex:1">
                            <div style="display:flex;gap:10px;flex-wrap:wrap;align-items:center">
                                <div style="flex:1"><input type="file" id="schoolLogoInput" accept="image/*" onchange="uploadSchoolLogo(event)" style="display:none"><button class="btn btn-sm btn-outline" onclick="document.getElementById('schoolLogoInput').click()"><i class="fas fa-cloud-upload-alt"></i> Upload Logo</button></div>
                                <button class="btn btn-sm btn-danger" onclick="removeSchoolLogo()"><i class="fas fa-trash"></i> Hapus</button>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- ===== UPLOAD BACKGROUND HERO ===== -->
                <div style="background:var(--light-gray);padding:15px;border-radius:12px;margin-bottom:15px">
                    <h4 style="color:var(--navy);margin-bottom:10px"><i class="fas fa-image"></i> Background Hero</h4>
                    <div style="display:flex;align-items:center;gap:15px;flex-wrap:wrap">
                        <div id="heroBgPreview" class="bg-preview-box" style="width:150px;height:100px;">
                            <i class="fas fa-image"></i>
                        </div>
                        <div style="flex:1">
                            <div style="display:flex;gap:10px;flex-wrap:wrap;align-items:center">
                                <div style="flex:1">
                                    <input type="file" id="heroBgInput" accept="image/*" onchange="uploadHeroBg(event)" style="display:none">
                                    <button class="btn btn-sm btn-outline" onclick="document.getElementById('heroBgInput').click()">
                                        <i class="fas fa-cloud-upload-alt"></i> Upload Background
                                    </button>
                                </div>
                                <button class="btn btn-sm btn-danger" onclick="removeHeroBg()">
                                    <i class="fas fa-trash"></i> Hapus
                                </button>
                            </div>
                            <small style="color:var(--gray);display:block;margin-top:5px">
                                <i class="fas fa-info-circle"></i> Gambar akan otomatis di-blur & transparan
                            </small>
                        </div>
                    </div>
                </div>
                
                <div class="admin-tabs">
                    <button class="active" onclick="switchTab('pesanan')"><i class="fas fa-shopping-cart"></i> Pesanan</button>
                    <button onclick="switchTab('donatur')"><i class="fas fa-handshake"></i> Donatur</button>
                    <button onclick="switchTab('sponsor')"><i class="fas fa-building"></i> Sponsor</button>
                    <button onclick="switchTab('kaos')"><i class="fas fa-tshirt"></i> Kaos</button>
                    <button onclick="switchTab('rundown')"><i class="fas fa-clock"></i> Rundown</button>
                    <button onclick="switchTab('anggaran')"><i class="fas fa-calculator"></i> Anggaran</button>
                    <button onclick="switchTab('galeri')"><i class="fas fa-images"></i> Galeri</button>
                    <button onclick="switchTab('pengaturan')"><i class="fas fa-cog"></i> Pengaturan</button>
                </div>
                
                <!-- Tab: Pesanan -->
                <div class="tab-content active" id="tab-pesanan">
                    <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;margin-bottom:15px">
                        <h4 style="color:var(--navy)"><i class="fas fa-list"></i> Daftar Pesanan Kaos</h4>
                        <button class="btn btn-success btn-sm" onclick="exportPesanan()"><i class="fas fa-file-excel"></i> Export Excel</button>
                    </div>
                    <div class="admin-table-wrap" id="adminPesananList"><p style="color:var(--gray)">Belum ada pesanan</p></div>
                </div>

                <!-- Tab: Donatur -->
                <div class="tab-content" id="tab-donatur">
                    <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;margin-bottom:15px">
                        <h4 style="color:var(--navy)"><i class="fas fa-list"></i> Daftar Donatur</h4>
                        <button class="btn btn-primary btn-sm" onclick="openAddDonatur()"><i class="fas fa-plus"></i> Tambah Donatur</button>
                    </div>
                    <div class="admin-table-wrap" id="adminDonaturList"><p style="color:var(--gray)">Loading...</p></div>
                </div>

                <!-- Tab: Sponsor -->
                <div class="tab-content" id="tab-sponsor">
                    <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;margin-bottom:15px">
                        <h4 style="color:var(--navy)"><i class="fas fa-list"></i> Daftar Sponsor</h4>
                        <button class="btn btn-primary btn-sm" onclick="openAddSponsor()"><i class="fas fa-plus"></i> Tambah Sponsor</button>
                    </div>
                    <div class="admin-table-wrap" id="adminSponsorList"><p style="color:var(--gray)">Loading...</p></div>
                </div>

                <!-- Tab: Kaos -->
                <div class="tab-content" id="tab-kaos">
                    <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;margin-bottom:15px">
                        <h4 style="color:var(--navy)"><i class="fas fa-list"></i> Daftar Kaos</h4>
                        <button class="btn btn-primary btn-sm" onclick="openAddKaos()"><i class="fas fa-plus"></i> Tambah Kaos</button>
                    </div>
                    <div class="admin-table-wrap" id="adminKaosList"><p style="color:var(--gray)">Loading...</p></div>
                </div>

                <!-- Tab: Rundown -->
                <div class="tab-content" id="tab-rundown">
                    <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;margin-bottom:15px">
                        <h4 style="color:var(--navy)"><i class="fas fa-list"></i> Daftar Rundown</h4>
                        <button class="btn btn-primary btn-sm" onclick="openAddRundown()"><i class="fas fa-plus"></i> Tambah Acara</button>
                    </div>
                    <div class="admin-table-wrap" id="adminRundownList"><p style="color:var(--gray)">Loading...</p></div>
                </div>

                <!-- Tab: Anggaran -->
                <div class="tab-content" id="tab-anggaran">
                    <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;margin-bottom:15px">
                        <h4 style="color:var(--navy)"><i class="fas fa-list"></i> Daftar Anggaran</h4>
                        <button class="btn btn-primary btn-sm" onclick="openAddAnggaran()"><i class="fas fa-plus"></i> Tambah Anggaran</button>
                    </div>
                    <div class="admin-table-wrap" id="adminAnggaranList"><p style="color:var(--gray)">Loading...</p></div>
                </div>

                <!-- Tab: Galeri -->
                <div class="tab-content" id="tab-galeri">
                    <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;margin-bottom:15px">
                        <h4 style="color:var(--navy)"><i class="fas fa-list"></i> Daftar Galeri</h4>
                        <button class="btn btn-primary btn-sm" onclick="openAddGaleri()"><i class="fas fa-plus"></i> Tambah Foto</button>
                    </div>
                    <div class="admin-table-wrap" id="adminGaleriList"><p style="color:var(--gray)">Loading...</p></div>
                </div>

                <!-- Tab: Pengaturan -->
                <div class="tab-content" id="tab-pengaturan">
                    <h4 style="color:var(--navy);margin-bottom:15px"><i class="fas fa-cog"></i> Pengaturan Acara</h4>
                    <form id="settingsForm" onsubmit="handleSettingsUpdate(event)">
                        <div class="form-group"><label>Nama Acara</label><input type="text" id="settEventName"></div>
                        <div class="form-row"><div class="form-group"><label>Tanggal Acara</label><input type="date" id="settEventDate"></div><div class="form-group"><label>Target Dana</label><input type="number" id="settTargetFund"></div></div>
                        <div class="form-group"><label>Slogan</label><input type="text" id="settSlogan"></div>
                        <div class="form-row"><div class="form-group"><label>Lokasi</label><input type="text" id="settLocation"></div><div class="form-group"><label>WhatsApp (utama)</label><input type="text" id="settWhatsapp"></div></div>
                        <button type="submit" class="btn btn-primary"><i class="fas fa-save"></i> Simpan Pengaturan</button>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <!-- FORM MODAL -->
    <div class="modal-overlay" id="formModal">
        <div class="modal">
            <div class="modal-header"><h2 id="formModalTitle"><i class="fas fa-plus-circle" style="color:var(--teal)"></i> Tambah Data</h2><button class="modal-close" onclick="closeFormModal()">&times;</button></div>
            <form id="formModalContent" onsubmit="handleFormSubmit(event)">
                <div id="formFields"></div>
                <button type="submit" class="btn btn-primary" style="width:100%;justify-content:center"><i class="fas fa-save"></i> SIMPAN</button>
            </form>
        </div>
    </div>

    <!-- PESAN KAOS MODAL -->
    <div class="modal-overlay" id="pesanKaosModal">
        <div class="modal">
            <div class="modal-header">
                <h2><i class="fas fa-tshirt" style="color:var(--teal)"></i> Pesan Kaos</h2>
                <button class="modal-close" onclick="closePesanKaos()">&times;</button>
            </div>
            <form id="pesanKaosForm" onsubmit="handlePesanKaos(event)">
                <div id="pesanKaosInfo" style="background:var(--light-gray);padding:10px;border-radius:8px;margin-bottom:15px;text-align:center">
                    <strong id="pesanKaosNama">Kaos HUT SMKN 1 Leles</strong><br>
                    <span style="color:var(--teal);font-size:20px;font-weight:700" id="pesanKaosHarga">Rp 75.000</span>
                </div>
                <div class="form-group"><label>Nama Lengkap *</label><input type="text" id="fPesanNama" placeholder="Nama pemesan" required></div>
                <div class="form-group"><label>Nomor WhatsApp *</label><input type="text" id="fPesanWa" placeholder="0812-3456-7890" required></div>
                <div class="form-row">
                    <div class="form-group"><label>Ukuran *</label><select id="fPesanUkuran" required><option value="">Pilih Ukuran</option><option value="S">S</option><option value="M">M</option><option value="L">L</option><option value="XL">XL</option><option value="XXL">XXL</option></select></div>
                    <div class="form-group"><label>Model *</label><select id="fPesanModel" required><option value="">Pilih Model</option><option value="Pendek">Pendek (Short)</option><option value="Panjang">Panjang (Long)</option></select></div>
                </div>
                <div class="form-group"><label>Jumlah *</label><input type="number" id="fPesanJumlah" value="1" min="1" required></div>
                <div class="form-group"><label>Pilihan Pengambilan *</label><select id="fPesanPengambilan" onchange="toggleAlamat()" required><option value="ambil">Ambil Sendiri (di SMKN 1 Leles)</option><option value="kirim">Kirim (JNE/Pos)</option></select></div>
                <div class="form-group hidden" id="alamatGroup"><label>Alamat Pengiriman *</label><textarea id="fPesanAlamat" placeholder="Alamat lengkap, RT/RW, Kecamatan, Kabupaten, Kode Pos"></textarea></div>
                <div class="form-group">
                    <label>Upload Bukti Pembayaran *</label>
                    <div class="file-upload-wrapper">
                        <input type="file" id="fPesanBukti" accept="image/*" onchange="previewImage(this,'buktiPreview')" required>
                        <div class="file-label"><i class="fas fa-cloud-upload-alt"></i><span>Upload bukti transfer (foto/ss)</span></div>
                    </div>
                    <div class="image-preview" id="buktiPreview"></div>
                    <small style="color:var(--gray);display:block;margin-top:5px">Upload bukti pembayaran untuk konfirmasi</small>
                </div>
                <div class="rekening-info">
                    <div class="bank">🏦 Sea Bank</div>
                    <div class="no-rek">901991056025</div>
                    <div class="atas-nama">a/n Reni Andriani</div>
                    <div style="font-size:12px;color:var(--gray);margin-top:5px">Transfer sesuai total harga, lalu upload bukti di atas</div>
                </div>
                <button type="submit" class="btn btn-primary" style="width:100%;justify-content:center"><i class="fas fa-shopping-cart"></i> PESAN SEKARANG</button>
            </form>
        </div>
    </div>

    <!-- NOTIFICATION -->
    <div id="notification" style="display:none"></div>

    <!-- ============================================================ -->
    <!-- JAVASCRIPT LENGKAP -->
    <!-- ============================================================ -->
    <script>
        // ============================================================
        // DATA
        // ============================================================
        const DATA = {
            targetFund: 40000000,
            eventDate: '2026-08-24',
            eventName: 'HUT ke-19 SMK Negeri 1 Leles & Reuni Akbar 2026',
            slogan: '"Bersama Mengenang, Berkarya, dan Menginspirasi"',
            location: 'SMK Negeri 1 Leles',
            whatsapp: '+6281223913350',
            schoolLogo: '',
            heroBg: '',
            pesanan: [],
            donatur: [
                {id:1,name:'Deny Saputra',amount:500000,date:'24 Agustus 2026',status:'diterima',description:'Sumbangan Alumni',photo:'https://ui-avatars.com/api/?name=Deny+Saputra&size=100&background=0B8F88&color=fff'},
                {id:2,name:'Pirman',amount:1400000,date:'24 Agustus 2026',status:'diterima',description:'Sumbangan Alumni',photo:'https://ui-avatars.com/api/?name=Pirman&size=100&background=0B8F88&color=fff'},
                {id:3,name:'Abdul Majid',amount:150000,date:'24 Agustus 2026',status:'diterima',description:'Sumbangan Alumni',photo:'https://ui-avatars.com/api/?name=Abdul+Majid&size=100&background=0B8F88&color=fff'}
            ],
            sponsor: [
                {id:1,name:'PT BIMA ABADI TEKNIK',amount:5000000,date:'20 Agustus 2026',status:'diterima',description:'Sponsor utama acara',logo:'https://ui-avatars.com/api/?name=PT+BIMA&size=100&background=092C55&color=fff'},
                {id:2,name:'CV MAJU BERSAMA',amount:3000000,date:'18 Agustus 2026',status:'diterima',description:'Sponsor perlengkapan',logo:'https://ui-avatars.com/api/?name=CV+MAJU&size=100&background=0B8F88&color=fff'}
            ],
            kaos: [
                {id:1,name:'Kaos HUT SMKN 1 Leles',size:'S, M, L, XL, XXL',price:75000,stock:50,sold:0,image:'👕',status:'tersedia'},
                {id:2,name:'Kaos Reuni Akbar 2026',size:'S, M, L, XL, XXL',price:85000,stock:30,sold:0,image:'👚',status:'tersedia'}
            ],
            rundown: [
                {id:1,time:'07.00 - 08.00',activity:'Registrasi Peserta & Alumni',pic:'Panitia',isHighlight:false},
                {id:2,time:'08.00 - 08.10',activity:'Pembukaan',pic:'MC',isHighlight:false},
                {id:3,time:'08.10 - 08.20',activity:'Pembacaan Ayat Suci Al-Qur\'an',pic:'Petugas',isHighlight:false},
                {id:4,time:'08.20 - 08.25',activity:'Indonesia Raya',pic:'Seluruh peserta',isHighlight:false},
                {id:5,time:'08.25 - 08.35',activity:'Doa',pic:'Petugas',isHighlight:false},
                {id:6,time:'08.35 - 08.50',activity:'Sambutan Ketua Panitia',pic:'Ketua Panitia',isHighlight:false},
                {id:7,time:'08.50 - 09.10',activity:'Sambutan Kepala Sekolah',pic:'Kepala SMK Negeri 1 Leles',isHighlight:false},
                {id:8,time:'09.10 - 09.25',activity:'Sambutan Perwakilan Alumni',pic:'Perwakilan Alumni',isHighlight:false},
                {id:9,time:'09.25 - 09.40',activity:'🎉 Puncak HUT ke-19 & Reuni Akbar',pic:'Potong tumpeng/kue & simbolis HUT',isHighlight:true},
                {id:10,time:'09.40 - 10.00',activity:'🤲 Bakti Sosial Anak Yatim/Piatu',pic:'Penyerahan santunan',isHighlight:true},
                {id:11,time:'10.00 - 10.20',activity:'Seni Tari Siswa',pic:'Penampilan siswa',isHighlight:false},
                {id:12,time:'10.20 - 10.45',activity:'🎭 Kabaret Guru',pic:'Penampilan guru',isHighlight:true},
                {id:13,time:'10.45 - 11.15',activity:'Hiburan',pic:'Siswa/Alumni',isHighlight:false},
                {id:14,time:'11.15 - 12.15',activity:'🕌 ISHOMA',pic:'Istirahat, Sholat & Makan',isHighlight:true},
                {id:15,time:'12.15 - 12.30',activity:'Hiburan Pembuka',pic:'MC/Performance',isHighlight:false},
                {id:16,time:'12.30 - 13.15',activity:'🎮 GAME ALUMNI – RETROPEKSI 19',pic:'Games nostalgia alumni',isHighlight:true},
                {id:17,time:'13.15 - 13.30',activity:'Pembagian Hadiah Game',pic:'Panitia',isHighlight:false},
                {id:18,time:'13.30 - 14.30',activity:'🎵 Hiburan oleh CS Musik',pic:'Live Music',isHighlight:true},
                {id:19,time:'14.30 - 14.50',activity:'Sesi Nostalgia & Cerita Alumni',pic:'Kenangan masa sekolah',isHighlight:false},
                {id:20,time:'14.50 - 15.10',activity:'📸 Foto Bersama',pic:'Guru, alumni & siswa',isHighlight:false},
                {id:21,time:'15.10 - 15.20',activity:'Pengumuman & Apresiasi',pic:'Panitia',isHighlight:false},
                {id:22,time:'15.20 - 15.30',activity:'Penutupan',pic:'MC',isHighlight:false}
            ],
            budgets: [
                {id:1,name:'Dekorasi & Panggung',amount:8000000},
                {id:2,name:'Sound System',amount:6000000},
                {id:3,name:'Konsumsi',amount:8000000},
                {id:4,name:'Dokumentasi',amount:3000000},
                {id:5,name:'Publikasi',amount:2500000},
                {id:6,name:'Perlengkapan Acara',amount:4500000},
                {id:7,name:'Lain-lain',amount:8000000}
            ],
            gallery: [
                {id:1,title:'Persiapan Panggung - Hari H-7',category:'persiapan',image:'https://ui-avatars.com/api/?name=Persiapan+Panggung&size=200&background=6c5ce7&color=fff'},
                {id:2,title:'Pemasangan Panggung Utama',category:'persiapan',image:'https://ui-avatars.com/api/?name=Pemasangan+Panggung&size=200&background=6c5ce7&color=fff'},
                {id:3,title:'Dekorasi Acara Mulai Dipasang',category:'dekorasi',image:'https://ui-avatars.com/api/?name=Dekorasi+Acara&size=200&background=00b894&color=fff'},
                {id:4,title:'Hiasan Panggung Selesai',category:'dekorasi',image:'https://ui-avatars.com/api/?name=Hiasan+Panggung&size=200&background=00b894&color=fff'},
                {id:5,title:'Latihan Tari Tradisional',category:'latihan',image:'https://ui-avatars.com/api/?name=Latihan+Tari&size=200&background=fdcb6e&color=fff'},
                {id:6,title:'Latihan Paduan Suara',category:'latihan',image:'https://ui-avatars.com/api/?name=Latihan+Suara&size=200&background=fdcb6e&color=fff'},
                {id:7,title:'Spot Foto HUT ke-19',category:'spot',image:'https://ui-avatars.com/api/?name=Spot+Foto&size=200&background=e17055&color=fff'},
                {id:8,title:'Booth Foto Alumni',category:'spot',image:'https://ui-avatars.com/api/?name=Booth+Alumni&size=200&background=e17055&color=fff'},
                {id:9,title:'Alumni Angkatan 2005 - Reuni',category:'alumni',image:'https://ui-avatars.com/api/?name=Alumni+2005&size=200&background=D4AF37&color=fff'},
                {id:10,title:'Alumni Angkatan 2010',category:'alumni',image:'https://ui-avatars.com/api/?name=Alumni+2010&size=200&background=D4AF37&color=fff'},
                {id:11,title:'Alumni Angkatan 2015',category:'alumni',image:'https://ui-avatars.com/api/?name=Alumni+2015&size=200&background=D4AF37&color=fff'},
                {id:12,title:'Alumni Angkatan 2022',category:'alumni',image:'https://ui-avatars.com/api/?name=Alumni+2022&size=200&background=D4AF37&color=fff'}
            ]
        };

        let nextId={donatur:4,sponsor:3,kaos:3,rundown:23,budget:8,gallery:13,pesanan:1};
        let isLoggedIn=false,currentFormType='',currentEditId=null,currentGalleryFilter='all';
        let pesanKaosId=null;

        // ============================================================
        // STORAGE
        // ============================================================
        function loadFromStorage(){try{const saved=localStorage.getItem('hutData');if(saved){const parsed=JSON.parse(saved);Object.assign(DATA,parsed);if(parsed.nextId)Object.assign(nextId,parsed.nextId)}}catch(e){}}
        function saveToStorage(){try{localStorage.setItem('hutData',JSON.stringify({...DATA,nextId}))}catch(e){}}

        // ============================================================
        // HERO BACKGROUND
        // ============================================================
        function updateHeroBg(){
            const bgUrl=DATA.heroBg||'';
            const heroBg=document.getElementById('heroBg');
            const preview=document.getElementById('heroBgPreview');
            
            if(bgUrl){
                heroBg.style.backgroundImage=`url('${bgUrl}')`;
                preview.style.backgroundImage=`url('${bgUrl}')`;
                preview.classList.add('has-bg');
                preview.innerHTML='';
            }else{
                heroBg.style.backgroundImage='';
                preview.style.backgroundImage='';
                preview.classList.remove('has-bg');
                preview.innerHTML='<i class="fas fa-image"></i>';
            }
            saveToStorage();
        }

        function uploadHeroBg(event){
            const file=event.target.files[0];
            if(!file)return;
            if(file.size>5*1024*1024){showNotification('File terlalu besar! Maks 5MB.','error');return}
            const reader=new FileReader();
            reader.onload=function(e){
                DATA.heroBg=e.target.result;
                updateHeroBg();
                showNotification('✅ Background hero berhasil diupload!','success');
            };
            reader.readAsDataURL(file);
        }

        function removeHeroBg(){
            if(confirm('Hapus background hero?')){
                DATA.heroBg='';
                updateHeroBg();
                showNotification('Background hero dihapus.','info');
            }
        }

        // ============================================================
        // HELPERS
        // ============================================================
        function formatRupiah(amount){return 'Rp '+new Intl.NumberFormat('id-ID').format(amount)}
        function getTotalDonaturDiterima(){return DATA.donatur.filter(s=>s.status==='diterima').reduce((sum,s)=>sum+s.amount,0)}
        function getTotalSponsorDiterima(){return DATA.sponsor.filter(s=>s.status==='diterima').reduce((sum,s)=>sum+s.amount,0)}
        function getTotalKaosTerjual(){return DATA.kaos.reduce((sum,k)=>sum+k.sold,0)}
        function getTotalKaosPendapatan(){return DATA.kaos.reduce((sum,k)=>sum+(k.sold*k.price),0)}
        function getTotalDanaMasuk(){return getTotalDonaturDiterima()+getTotalSponsorDiterima()+getTotalKaosPendapatan()}
        function getTotalDonatur(){return DATA.donatur.length}
        function getTotalSponsor(){return DATA.sponsor.length}
        function getKekurangan(){const total=getTotalDanaMasuk();return DATA.targetFund-total>0?DATA.targetFund-total:0}
        function getProgress(){const total=getTotalDanaMasuk();return DATA.targetFund>0?(total/DATA.targetFund)*100:0}
        function getTotalAnggaran(){return DATA.budgets.reduce((sum,b)=>sum+b.amount,0)}

        // ============================================================
        // LOGO
        // ============================================================
        function updateSchoolLogo(){const url=DATA.schoolLogo||'';['schoolLogo','footerLogo'].forEach(id=>{const el=document.getElementById(id);if(el){if(url){el.src=url;el.style.display='block'}else{el.style.display='none'}}});const preview=document.getElementById('adminLogoPreview');if(preview){preview.innerHTML=url?`<img src="${url}" style="width:100%;height:100%;object-fit:contain;">`:'<span style="color:#ccc;font-size:12px">Logo</span>'}saveToStorage()}
        function uploadSchoolLogo(event){const file=event.target.files[0];if(!file)return;if(file.size>2*1024*1024){showNotification('File terlalu besar! Maks 2MB.','error');return}const reader=new FileReader();reader.onload=function(e){DATA.schoolLogo=e.target.result;updateSchoolLogo();showNotification('✅ Logo berhasil diupload!','success')};reader.readAsDataURL(file)}
        function removeSchoolLogo(){if(confirm('Hapus logo sekolah?')){DATA.schoolLogo='';updateSchoolLogo();showNotification('Logo dihapus.','info')}}

        // ============================================================
        // COUNTDOWN
        // ============================================================
        function updateCountdown(){try{const target=new Date(DATA.eventDate+'T07:00:00').getTime();const now=new Date().getTime();const diff=target-now;if(diff<=0){['days','hours','minutes','seconds'].forEach(id=>document.getElementById(id).textContent='00');return}document.getElementById('days').textContent=String(Math.floor(diff/(1000*60*60*24))).padStart(2,'0');document.getElementById('hours').textContent=String(Math.floor((diff%(1000*60*60*24))/(1000*60*60))).padStart(2,'0');document.getElementById('minutes').textContent=String(Math.floor((diff%(1000*60*60))/(1000*60))).padStart(2,'0');document.getElementById('seconds').textContent=String(Math.floor((diff%(1000*60))/1000)).padStart(2,'0')}catch(e){}}

        // ============================================================
        // PESAN KAOS
        // ============================================================
        function openPesanKaos(id){
            pesanKaosId=id;
            const item=DATA.kaos.find(k=>k.id===id);
            if(!item){showNotification('Kaos tidak ditemukan!','error');return}
            document.getElementById('pesanKaosNama').textContent=item.name;
            document.getElementById('pesanKaosHarga').textContent=formatRupiah(item.price);
            document.getElementById('fPesanJumlah').value=1;
            document.getElementById('pesanKaosModal').classList.add('show');
            document.getElementById('alamatGroup').classList.add('hidden');
            document.getElementById('buktiPreview').innerHTML='';
        }

        function closePesanKaos(){document.getElementById('pesanKaosModal').classList.remove('show');document.getElementById('pesanKaosForm').reset();document.getElementById('buktiPreview').innerHTML=''}

        function toggleAlamat(){
            const val=document.getElementById('fPesanPengambilan').value;
            const alamatGroup=document.getElementById('alamatGroup');
            if(val==='kirim'){alamatGroup.classList.remove('hidden');document.getElementById('fPesanAlamat').required=true}
            else{alamatGroup.classList.add('hidden');document.getElementById('fPesanAlamat').required=false}
        }

        function previewImage(input,previewId){
            if(input.files&&input.files[0]){
                const reader=new FileReader();
                reader.onload=function(e){
                    const preview=document.getElementById(previewId);
                    if(preview){preview.innerHTML=`<img src="${e.target.result}">`}
                };
                reader.readAsDataURL(input.files[0])
            }
        }

        function handlePesanKaos(e){
            e.preventDefault();
            const nama=document.getElementById('fPesanNama').value;
            const wa=document.getElementById('fPesanWa').value;
            const ukuran=document.getElementById('fPesanUkuran').value;
            const model=document.getElementById('fPesanModel').value;
            const jumlah=parseInt(document.getElementById('fPesanJumlah').value);
            const pengambilan=document.getElementById('fPesanPengambilan').value;
            const alamat=document.getElementById('fPesanAlamat').value;
            const buktiFile=document.getElementById('fPesanBukti').files[0];
            
            if(!nama||!wa||!ukuran||!model||!jumlah){showNotification('Semua field wajib diisi!','error');return}
            if(!buktiFile){showNotification('Upload bukti pembayaran!','error');return}
            
            const item=DATA.kaos.find(k=>k.id===pesanKaosId);
            if(!item){showNotification('Kaos tidak ditemukan!','error');return}
            if(jumlah>item.stock){showNotification('Stok tidak mencukupi! Stok tersisa: '+item.stock,'error');return}
            
            const totalHarga=item.price*jumlah;
            const reader=new FileReader();
            reader.onload=function(e){
                const buktiData=e.target.result;
                const pesanan={
                    id:nextId.pesanan++,
                    kaosId:item.id,
                    kaosNama:item.name,
                    nama:nama,
                    wa:wa,
                    ukuran:ukuran,
                    model:model,
                    jumlah:jumlah,
                    totalHarga:totalHarga,
                    pengambilan:pengambilan,
                    alamat:pengambilan==='kirim'?alamat:'-',
                    bukti:buktiData,
                    status:'menunggu',
                    tanggal:new Date().toLocaleDateString('id-ID',{day:'numeric',month:'long',year:'numeric'}),
                    jam:new Date().toLocaleTimeString('id-ID',{hour:'2-digit',minute:'2-digit'})
                };
                DATA.pesanan.push(pesanan);
                item.stock-=jumlah;
                item.sold+=jumlah;
                if(item.stock===0)item.status='habis';
                saveToStorage();
                closePesanKaos();
                renderAll();
                renderAdminPesanan();
                const pesanWA=`Halo Kak ${nama},\n\n✅ Pesanan Kaos Anda telah kami terima!\n\n📋 Detail Pesanan:\n👕 Kaos: ${item.name}\n📏 Ukuran: ${ukuran}\n👕 Model: ${model}\n📦 Jumlah: ${jumlah} pcs\n💰 Total: ${formatRupiah(totalHarga)}\n📦 Pengambilan: ${pengambilan==='ambil'?'Ambil Sendiri (SMKN 1 Leles)':'Dikirim'}\n${pengambilan==='kirim'?'📍 Alamat: '+alamat:''}\n\n📸 Bukti pembayaran sudah kami terima.\n\n💳 Transfer ke:\n🏦 Sea Bank\n💳 901991056025\na/n Reni Andriani\n\n📱 Konfirmasi ke panitia:\nPirman: 0812-2391-3350\nAbdul Aris: 0857-9432-5300\n\nTerima kasih! 🙏`;
                window.open('https://wa.me/62'+wa.replace(/[^0-9]/g,'')+'?text='+encodeURIComponent(pesanWA),'_blank');
                showNotification('✅ Pesanan berhasil! Silakan cek WhatsApp untuk konfirmasi.','success');
            };
            reader.readAsDataURL(buktiFile);
        }

        // ============================================================
        // RENDER FUNCTIONS
        // ============================================================
        function renderStats(){
            try{
                const totalDana=getTotalDanaMasuk(),progress=getProgress(),danaDonatur=getTotalDonaturDiterima(),danaSponsor=getTotalSponsorDiterima(),danaKaos=getTotalKaosPendapatan(),jumlahDonatur=getTotalDonatur(),jumlahSponsor=getTotalSponsor(),jumlahKaos=getTotalKaosTerjual(),kekurangan=getKekurangan();
                document.getElementById('targetFund').textContent=formatRupiah(DATA.targetFund);
                document.getElementById('danaMasuk').textContent=formatRupiah(totalDana);
                document.getElementById('sponsorCount').textContent=jumlahDonatur+' Donatur';
                document.getElementById('kaosCount').textContent=jumlahKaos+' Kaos';
                document.getElementById('progressPercent').textContent=progress.toFixed(1)+'%';
                document.getElementById('progressFill').style.width=Math.min(progress,100)+'%';
                document.getElementById('progressTerkumpul').textContent=formatRupiah(totalDana);
                document.getElementById('progressTarget').textContent=formatRupiah(DATA.targetFund);
                document.getElementById('danaDonatur').textContent=formatRupiah(danaDonatur);
                document.getElementById('danaDonaturCount').textContent=jumlahDonatur+' Donatur';
                document.getElementById('danaSponsor').textContent=formatRupiah(danaSponsor);
                document.getElementById('danaSponsorCount').textContent=jumlahSponsor+' Sponsor';
                document.getElementById('danaKaos').textContent=formatRupiah(danaKaos);
                document.getElementById('danaKaosCount').textContent=jumlahKaos+' Kaos Terjual';
                document.getElementById('totalDanaMasuk').textContent=formatRupiah(totalDana);
                document.getElementById('totalKekurangan').textContent=formatRupiah(kekurangan);
                document.getElementById('totalProgress').textContent=progress.toFixed(1)+'%';
            }catch(e){console.log('Render stats error:',e)}
        }

        function renderRundown(){try{const container=document.getElementById('rundownContainer');if(!DATA.rundown.length){container.innerHTML='<p style="text-align:center;padding:30px;color:var(--gray)">Belum ada data</p>';return}let html='<table><thead><tr><th style="width:15%">Waktu</th><th style="width:55%">Acara</th><th style="width:30%">Keterangan</th></tr></thead><tbody>';DATA.rundown.forEach(item=>{const cls=item.isHighlight?'highlight-row':'';const badge=item.isHighlight?'<span class="badge-acara">⭐ Utama</span> ':'';html+=`<tr class="${cls}"><td><strong>${item.time}</strong></td><td>${badge}${item.activity}</td><td>${item.pic}</td></tr>`});html+='</tbody></table>';container.innerHTML=html}catch(e){}}

        function renderAnggaran(){try{const container=document.getElementById('anggaranContainer');if(!DATA.budgets.length){container.innerHTML='<p style="text-align:center;padding:30px;color:var(--gray)">Belum ada data</p>';return}const total=getTotalAnggaran();let html='<table><thead><tr><th>Kebutuhan</th><th style="text-align:right">Anggaran</th></tr></thead><tbody>';DATA.budgets.forEach(item=>{html+=`<tr><td>${item.name}</td><td style="text-align:right">${formatRupiah(item.amount)}</td></tr>`});html+=`</tbody><tfoot><tr><td><strong>TOTAL</strong></td><td style="text-align:right"><strong>${formatRupiah(total)}</strong></td></tr></tfoot></table>`;container.innerHTML=html}catch(e){}}

        function renderKaos(){try{const container=document.getElementById('kaosContainer');if(!DATA.kaos.length){container.innerHTML='<p style="text-align:center;padding:30px;color:var(--gray)">Belum ada kaos</p>';return}let html='';DATA.kaos.forEach(item=>{const statusClass=item.status==='tersedia'?'badge-tersedia':'badge-habis';html+=`<div class="kaos-card" onclick="openPesanKaos(${item.id})"><div class="kaos-image">${item.image||'👕'}</div><div class="kaos-info"><h4>${item.name}</h4><div class="harga">${formatRupiah(item.price)}</div><div class="detail">Size: ${item.size}</div><div class="detail">Stok: ${item.stock} | Terjual: ${item.sold}</div><div style="margin-top:8px"><span class="badge-status ${statusClass}">${item.status==='tersedia'?'✅ Tersedia':'❌ Habis'}</span></div><div style="margin-top:8px;font-size:12px;color:var(--teal)"><i class="fas fa-shopping-cart"></i> Klik untuk pesan</div></div></div>`});container.innerHTML=html}catch(e){}}

        function renderDonatur(){try{const container=document.getElementById('donaturContainer');if(!DATA.donatur.length){container.innerHTML='<p style="text-align:center;padding:30px;color:var(--gray)">Belum ada donatur</p>';return}let html='';DATA.donatur.forEach(item=>{const statusClass=item.status==='diterima'?'status-diterima':'status-menunggu';const statusText=item.status==='diterima'?'✅ Diterima':'⏳ Menunggu';html+=`<div class="sponsor-card"><div class="logo-container">${item.photo?`<img src="${item.photo}">`:'<span class="no-logo"><i class="fas fa-user"></i></span>'}</div><div class="name">${item.name}</div><div class="amount">${formatRupiah(item.amount)}</div><div class="date"><i class="fas fa-calendar-alt"></i> ${item.date}</div><div><span class="status ${statusClass}">${statusText}</span></div>${item.description?`<div class="description"><i class="fas fa-info-circle"></i> ${item.description}</div>`:''}<div><span class="category-tag"><i class="fas fa-user-graduate"></i> Donatur</span></div></div>`});container.innerHTML=html}catch(e){}}

        function renderSponsor(){try{const container=document.getElementById('sponsorContainer');if(!DATA.sponsor.length){container.innerHTML='<p style="text-align:center;padding:30px;color:var(--gray)">Belum ada sponsor</p>';return}let html='';DATA.sponsor.forEach(item=>{const statusClass=item.status==='diterima'?'status-diterima':'status-menunggu';const statusText=item.status==='diterima'?'✅ Diterima':'⏳ Menunggu';html+=`<div class="sponsor-card" style="border-left-color:var(--gold)"><div class="logo-container">${item.logo?`<img src="${item.logo}">`:'<span class="no-logo"><i class="fas fa-building"></i></span>'}</div><div class="name">${item.name}</div><div class="amount">${formatRupiah(item.amount)}</div><div class="date"><i class="fas fa-calendar-alt"></i> ${item.date}</div><div><span class="status ${statusClass}">${statusText}</span></div>${item.description?`<div class="description"><i class="fas fa-info-circle"></i> ${item.description}</div>`:''}<div><span class="category-tag"><i class="fas fa-building"></i> Sponsor</span></div></div>`});container.innerHTML=html}catch(e){}}

        function filterGallery(category){
            currentGalleryFilter=category;
            renderGaleri();
            document.querySelectorAll('#galeri .btn').forEach(btn=>{
                btn.classList.remove('btn-primary','btn-gold');
                btn.classList.add('btn-outline')
            });
            if(category==='all'){
                document.querySelector('#galeri .btn[onclick="filterGallery(\'all\')"]')?.classList.remove('btn-outline');
                document.querySelector('#galeri .btn[onclick="filterGallery(\'all\')"]')?.classList.add('btn-primary');
            }else{
                const btn=document.querySelector(`#galeri .btn[onclick="filterGallery('${category}')"]`);
                if(btn){
                    btn.classList.remove('btn-outline');
                    btn.classList.add(category==='alumni'?'btn-gold':'btn-primary');
                }
            }
        }

        function renderGaleri(){
            try{
                const container=document.getElementById('galeriContainer');
                const categories=['persiapan','dekorasi','latihan','spot','alumni'];
                const labels={'persiapan':'📁 Persiapan Panggung','dekorasi':'📁 Dekorasi Acara','latihan':'📁 Latihan Siswa','spot':'📁 Spot Foto','alumni':'📁 Foto Alumni'};
                const colors={'persiapan':'#6c5ce7','dekorasi':'#00b894','latihan':'#fdcb6e','spot':'#e17055','alumni':'var(--gold)'};
                const icons={'persiapan':'🎪','dekorasi':'🎨','latihan':'💃','spot':'📸','alumni':'🎓'};
                
                categories.forEach(cat=>{
                    const count=DATA.gallery.filter(g=>g.category===cat).length;
                    document.getElementById('count-'+cat).textContent=count;
                });
                
                if(currentGalleryFilter==='all'){
                    let html='<div class="folder-view">';
                    categories.forEach(cat=>{
                        const count=DATA.gallery.filter(g=>g.category===cat).length;
                        const color=colors[cat];
                        html+=`<div class="folder-card" onclick="filterGallery('${cat}')"><div class="folder-icon">${icons[cat]}</div><div class="folder-name">${labels[cat]}</div><div class="folder-count">${count} foto</div><div class="folder-color" style="background:${color};"></div></div>`;
                    });
                    html+='</div>';
                    container.innerHTML=html;
                    return;
                }
                
                const filtered=DATA.gallery.filter(g=>g.category===currentGalleryFilter);
                if(!filtered.length){
                    container.innerHTML=`<p style="text-align:center;padding:30px;color:var(--gray)">📁 Belum ada foto di ${labels[currentGalleryFilter]}</p>`;
                    return;
                }
                
                let html='<div class="sponsor-grid">';
                filtered.forEach(item=>{
                    const isImage=item.image&&(item.image.startsWith('http')||item.image.startsWith('data:'));
                    const color=colors[item.category]||'var(--teal)';
                    html+=`<div class="sponsor-card" style="border-left-color:${color};"><div style="height:150px;display:flex;align-items:center;justify-content:center;overflow:hidden;border-radius:8px;background:var(--light-gray)">${isImage?`<img src="${item.image}" style="width:100%;height:100%;object-fit:cover;">`:`<span style="font-size:64px">${item.image||'📸'}</span>`}</div><div class="name">${item.title}</div><div><span class="category-tag" style="background:${color};">${icons[item.category]} ${labels[item.category]}</span></div><div style="font-size:12px;color:var(--gray);margin-top:5px"><i class="fas fa-clock"></i> ${new Date().toLocaleDateString('id-ID')}</div></div>`;
                });
                html+='</div>';
                container.innerHTML=html;
            }catch(e){console.log('Render galeri error:',e)}
        }

        function renderAll(){renderStats();renderRundown();renderAnggaran();renderKaos();renderDonatur();renderSponsor();renderGaleri()}

        // ============================================================
        // ADMIN RENDER
        // ============================================================
        function renderAdminPesanan(){try{const container=document.getElementById('adminPesananList');if(!DATA.pesanan.length){container.innerHTML='<p style="color:var(--gray)">Belum ada pesanan</p>';return}let html='<table class="admin-table"><thead><tr><th>#</th><th>Nama</th><th>Kaos</th><th>Ukuran</th><th>Model</th><th>Jml</th><th>Total</th><th>Pengambilan</th><th>Bukti</th><th>Status</th><th>Aksi</th></tr></thead><tbody>';DATA.pesanan.forEach((p,i)=>{const statusBadge=p.status==='menunggu'?'badge-menunggu':'badge-tersedia';const bukti=p.bukti?`<img src="${p.bukti}" style="width:40px;height:40px;object-fit:cover;border-radius:4px;cursor:pointer" onclick="window.open('${p.bukti}','_blank')">`:'-';html+=`<tr><td>${i+1}</td><td>${p.nama}</td><td>${p.kaosNama}</td><td>${p.ukuran}</td><td>${p.model}</td><td>${p.jumlah}</td><td>${formatRupiah(p.totalHarga)}</td><td>${p.pengambilan==='ambil'?'📦 Ambil':'🚚 Kirim'}</td><td>${bukti}</td><td><span class="badge-status ${statusBadge}">${p.status==='menunggu'?'⏳ Menunggu':'✅ Selesai'}</span></td><td><div class="actions"><button class="btn-status" onclick="toggleStatusPesanan(${p.id})"><i class="fas fa-check"></i></button><button class="btn-delete" onclick="deletePesanan(${p.id})"><i class="fas fa-trash"></i></button></div></td></tr>`});html+='</tbody></table>';container.innerHTML=html}catch(e){}}

        function renderAdminDonatur(){try{const container=document.getElementById('adminDonaturList');if(!DATA.donatur.length){container.innerHTML='<p style="color:var(--gray)">Belum ada donatur</p>';return}let html='<table class="admin-table"><thead><tr><th>Foto</th><th>Nama</th><th>Nominal</th><th>Tanggal</th><th>Status</th><th>Aksi</th></tr></thead><tbody>';DATA.donatur.forEach(s=>{const photo=s.photo?`<img src="${s.photo}" style="width:30px;height:30px;border-radius:50%;object-fit:cover">`:'<i class="fas fa-user" style="color:#ccc"></i>';const statusBadge=s.status==='diterima'?'badge-diterima':'badge-menunggu';html+=`<tr><td>${photo}</td><td>${s.name}</td><td>${formatRupiah(s.amount)}</td><td>${s.date}</td><td><span class="badge-status ${statusBadge}">${s.status==='diterima'?'✅ Diterima':'⏳ Menunggu'}</span></td><td><div class="actions"><button class="btn-edit" onclick="editDonatur(${s.id})"><i class="fas fa-edit"></i></button><button class="btn-delete" onclick="deleteDonatur(${s.id})"><i class="fas fa-trash"></i></button><button class="btn-status" onclick="toggleStatusDonatur(${s.id})"><i class="fas fa-sync"></i></button></div></td></tr>`});html+='</tbody></table>';container.innerHTML=html}catch(e){}}

        function renderAdminSponsor(){try{const container=document.getElementById('adminSponsorList');if(!DATA.sponsor.length){container.innerHTML='<p style="color:var(--gray)">Belum ada sponsor</p>';return}let html='<table class="admin-table"><thead><tr><th>Logo</th><th>Nama</th><th>Nominal</th><th>Tanggal</th><th>Status</th><th>Aksi</th></tr></thead><tbody>';DATA.sponsor.forEach(s=>{const logo=s.logo?`<img src="${s.logo}" style="width:30px;height:30px;border-radius:50%;object-fit:cover">`:'<i class="fas fa-building" style="color:#ccc"></i>';const statusBadge=s.status==='diterima'?'badge-diterima':'badge-menunggu';html+=`<tr><td>${logo}</td><td>${s.name}</td><td>${formatRupiah(s.amount)}</td><td>${s.date}</td><td><span class="badge-status ${statusBadge}">${s.status==='diterima'?'✅ Diterima':'⏳ Menunggu'}</span></td><td><div class="actions"><button class="btn-edit" onclick="editSponsor(${s.id})"><i class="fas fa-edit"></i></button><button class="btn-delete" onclick="deleteSponsor(${s.id})"><i class="fas fa-trash"></i></button><button class="btn-status" onclick="toggleStatusSponsor(${s.id})"><i class="fas fa-sync"></i></button></div></td></tr>`});html+='</tbody></table>';container.innerHTML=html}catch(e){}}

        function renderAdminKaos(){try{const container=document.getElementById('adminKaosList');if(!DATA.kaos.length){container.innerHTML='<p style="color:var(--gray)">Belum ada kaos</p>';return}let html='<table class="admin-table"><thead><tr><th>Gambar</th><th>Nama</th><th>Harga</th><th>Size</th><th>Stok</th><th>Terjual</th><th>Status</th><th>Aksi</th></tr></thead><tbody>';DATA.kaos.forEach(k=>{const statusBadge=k.status==='tersedia'?'badge-tersedia':'badge-habis';html+=`<tr><td style="font-size:24px">${k.image||'👕'}</td><td>${k.name}</td><td>${formatRupiah(k.price)}</td><td>${k.size}</td><td>${k.stock}</td><td>${k.sold}</td><td><span class="badge-status ${statusBadge}">${k.status==='tersedia'?'✅ Tersedia':'❌ Habis'}</span></td><td><div class="actions"><button class="btn-edit" onclick="editKaos(${k.id})"><i class="fas fa-edit"></i></button><button class="btn-delete" onclick="deleteKaos(${k.id})"><i class="fas fa-trash"></i></button><button class="btn-status" onclick="toggleStatusKaos(${k.id})"><i class="fas fa-sync"></i></button></div></td></tr>`});html+='</tbody></table>';container.innerHTML=html}catch(e){}}

        function renderAdminRundown(){try{const container=document.getElementById('adminRundownList');if(!DATA.rundown.length){container.innerHTML='<p style="color:var(--gray)">Belum ada data</p>';return}let html='<table class="admin-table"><thead><tr><th>Waktu</th><th>Acara</th><th>Keterangan</th><th>Utama</th><th>Aksi</th></tr></thead><tbody>';DATA.rundown.forEach(r=>{html+=`<tr><td>${r.time}</td><td>${r.activity}</td><td>${r.pic}</td><td>${r.isHighlight?'⭐':''}</td><td><div class="actions"><button class="btn-edit" onclick="editRundown(${r.id})"><i class="fas fa-edit"></i></button><button class="btn-delete" onclick="deleteRundown(${r.id})"><i class="fas fa-trash"></i></button><button class="btn-status" onclick="toggleHighlightRundown(${r.id})"><i class="fas fa-star"></i></button></div></td></tr>`});html+='</tbody></table>';container.innerHTML=html}catch(e){}}

        function renderAdminAnggaran(){try{const container=document.getElementById('adminAnggaranList');if(!DATA.budgets.length){container.innerHTML='<p style="color:var(--gray)">Belum ada data</p>';return}const total=getTotalAnggaran();let html='<table class="admin-table"><thead><tr><th>Kebutuhan</th><th>Anggaran</th><th>Aksi</th></tr></thead><tbody>';DATA.budgets.forEach(b=>{html+=`<tr><td>${b.name}</td><td>${formatRupiah(b.amount)}</td><td><div class="actions"><button class="btn-edit" onclick="editAnggaran(${b.id})"><i class="fas fa-edit"></i></button><button class="btn-delete" onclick="deleteAnggaran(${b.id})"><i class="fas fa-trash"></i></button></div></td></tr>`});html+=`<tr style="font-weight:700;background:var(--navy);color:#fff"><td>TOTAL</td><td>${formatRupiah(total)}</td><td></td></tr></tbody></table>`;container.innerHTML=html}catch(e){}}

        function renderAdminGaleri(){try{const container=document.getElementById('adminGaleriList');if(!DATA.gallery.length){container.innerHTML='<p style="color:var(--gray)">Belum ada foto</p>';return}let html='<table class="admin-table"><thead><tr><th>Foto</th><th>Judul</th><th>📁 Folder</th><th>Aksi</th></tr></thead><tbody>';const labels={'persiapan':'📁 Persiapan Panggung','dekorasi':'📁 Dekorasi Acara','latihan':'📁 Latihan Siswa','spot':'📁 Spot Foto','alumni':'📁 Foto Alumni'};DATA.gallery.forEach(g=>{const isImage=g.image&&(g.image.startsWith('http')||g.image.startsWith('data:'));const img=isImage?`<img src="${g.image}" style="width:50px;height:50px;object-fit:cover;border-radius:8px">`:`<span style="font-size:30px">${g.image||'📸'}</span>`;html+=`<tr><td>${img}</td><td>${g.title}</td><td><span class="folder-badge">${labels[g.category]||g.category}</span></td><td><div class="actions"><button class="btn-delete" onclick="deleteGaleri(${g.id})"><i class="fas fa-trash"></i></button></div></td></tr>`});html+='</tbody></table>';container.innerHTML=html}catch(e){}}

        function renderAdminAll(){renderAdminPesanan();renderAdminDonatur();renderAdminSponsor();renderAdminKaos();renderAdminRundown();renderAdminAnggaran();renderAdminGaleri();document.getElementById('settEventName').value=DATA.eventName||'';document.getElementById('settEventDate').value=DATA.eventDate||'';document.getElementById('settTargetFund').value=DATA.targetFund||'';document.getElementById('settSlogan').value=DATA.slogan||'';document.getElementById('settLocation').value=DATA.location||'';document.getElementById('settWhatsapp').value=DATA.whatsapp||''}

        // ============================================================
        // TAB SWITCH
        // ============================================================
        function switchTab(tab){document.querySelectorAll('.tab-content').forEach(el=>el.classList.remove('active'));document.querySelectorAll('.admin-tabs button').forEach(el=>el.classList.remove('active'));document.getElementById('tab-'+tab).classList.add('active');document.querySelector(`.admin-tabs button[onclick="switchTab('${tab}')"]`).classList.add('active');if(tab==='pesanan')renderAdminPesanan();else if(tab==='donatur')renderAdminDonatur();else if(tab==='sponsor')renderAdminSponsor();else if(tab==='kaos')renderAdminKaos();else if(tab==='rundown')renderAdminRundown();else if(tab==='anggaran')renderAdminAnggaran();else if(tab==='galeri')renderAdminGaleri()}

        // ============================================================
        // CRUD FUNCTIONS
        // ============================================================
        function toggleStatusPesanan(id){const item=DATA.pesanan.find(p=>p.id===id);if(item){item.status=item.status==='menunggu'?'selesai':'menunggu';saveToStorage();renderAdminPesanan();showNotification('✅ Status pesanan diubah!','success')}}
        function deletePesanan(id){if(confirm('Hapus pesanan ini?')){DATA.pesanan=DATA.pesanan.filter(p=>p.id!==id);saveToStorage();renderAdminPesanan();showNotification('✅ Pesanan dihapus!','success')}}
        function exportPesanan(){if(!DATA.pesanan.length){showNotification('Belum ada data pesanan!','error');return}let csv='No,Nama,Kaos,Ukuran,Model,Jumlah,Total Harga,Pengambilan,Alamat,Status,Tanggal\n';DATA.pesanan.forEach((p,i)=>{csv+=`${i+1},${p.nama},${p.kaosNama},${p.ukuran},${p.model},${p.jumlah},${p.totalHarga},${p.pengambilan==='ambil'?'Ambil Sendiri':'Kirim'},${p.alamat||'-'},${p.status},${p.tanggal}\n`});const blob=new Blob([csv],{type:'text/csv;charset=utf-8;'});const url=window.URL.createObjectURL(blob);const a=document.createElement('a');a.href=url;a.download=`pesanan_kaos_${new Date().toISOString().split('T')[0]}.csv`;a.click();window.URL.revokeObjectURL(url);showNotification('✅ Data pesanan berhasil diexport!','success')}

        function openAddDonatur(){openForm('donatur',null,'Tambah Donatur')}
        function editDonatur(id){openForm('donatur',id,'Edit Donatur')}
        function deleteDonatur(id){if(confirm('Hapus donatur ini?')){DATA.donatur=DATA.donatur.filter(s=>s.id!==id);saveToStorage();renderAll();renderAdminDonatur();showNotification('✅ Donatur dihapus!','success')}}
        function toggleStatusDonatur(id){const item=DATA.donatur.find(s=>s.id===id);if(item){item.status=item.status==='diterima'?'menunggu':'diterima';saveToStorage();renderAll();renderAdminDonatur();showNotification('✅ Status diubah!','success')}}

        function openAddSponsor(){openForm('sponsor',null,'Tambah Sponsor')}
        function editSponsor(id){openForm('sponsor',id,'Edit Sponsor')}
        function deleteSponsor(id){if(confirm('Hapus sponsor ini?')){DATA.sponsor=DATA.sponsor.filter(s=>s.id!==id);saveToStorage();renderAll();renderAdminSponsor();showNotification('✅ Sponsor dihapus!','success')}}
        function toggleStatusSponsor(id){const item=DATA.sponsor.find(s=>s.id===id);if(item){item.status=item.status==='diterima'?'menunggu':'diterima';saveToStorage();renderAll();renderAdminSponsor();showNotification('✅ Status diubah!','success')}}

        function openAddKaos(){openForm('kaos',null,'Tambah Kaos')}
        function editKaos(id){openForm('kaos',id,'Edit Kaos')}
        function deleteKaos(id){if(confirm('Hapus kaos ini?')){DATA.kaos=DATA.kaos.filter(k=>k.id!==id);saveToStorage();renderAll();renderAdminKaos();showNotification('✅ Kaos dihapus!','success')}}
        function toggleStatusKaos(id){const item=DATA.kaos.find(k=>k.id===id);if(item){item.status=item.status==='tersedia'?'habis':'tersedia';saveToStorage();renderAll();renderAdminKaos();showNotification('✅ Status diubah!','success')}}

        function openAddRundown(){openForm('rundown',null,'Tambah Acara')}
        function editRundown(id){openForm('rundown',id,'Edit Acara')}
        function deleteRundown(id){if(confirm('Hapus acara ini?')){DATA.rundown=DATA.rundown.filter(r=>r.id!==id);saveToStorage();renderAll();renderAdminRundown();showNotification('✅ Acara dihapus!','success')}}
        function toggleHighlightRundown(id){const item=DATA.rundown.find(r=>r.id===id);if(item){item.isHighlight=!item.isHighlight;saveToStorage();renderAll();renderAdminRundown();showNotification('✅ Status utama diubah!','success')}}

        function openAddAnggaran(){openForm('anggaran',null,'Tambah Anggaran')}
        function editAnggaran(id){openForm('anggaran',id,'Edit Anggaran')}
        function deleteAnggaran(id){if(confirm('Hapus anggaran ini?')){DATA.budgets=DATA.budgets.filter(b=>b.id!==id);saveToStorage();renderAll();renderAdminAnggaran();showNotification('✅ Anggaran dihapus!','success')}}

        function openAddGaleri(){openForm('galeri',null,'Tambah Foto')}
        function deleteGaleri(id){if(confirm('Hapus foto ini?')){DATA.gallery=DATA.gallery.filter(g=>g.id!==id);saveToStorage();renderAll();renderAdminGaleri();showNotification('✅ Foto dihapus!','success')}}

        // ============================================================
        // FORM
        // ============================================================
        function openForm(type,id,title){
            currentFormType=type;currentEditId=id;const icon=id?'fa-edit':'fa-plus-circle';const color=id?'#ffc107':'var(--teal)';document.getElementById('formModalTitle').innerHTML=`<i class="fas ${icon}" style="color:${color}"></i> ${title}`;let fields='';
            if(type==='donatur'){const item=id?DATA.donatur.find(s=>s.id===id):null;fields=`<div class="form-group"><label>Nama Donatur *</label><input type="text" id="fDonaturName" value="${item?item.name:''}" required></div><div class="form-group"><label>Nominal *</label><input type="number" id="fDonaturAmount" value="${item?item.amount:''}" required></div><div class="form-group"><label>Foto Donatur</label><div class="file-upload-wrapper"><input type="file" id="fDonaturPhoto" accept="image/*" onchange="previewImage(this,'donaturPreview')"><div class="file-label"><i class="fas fa-cloud-upload-alt"></i> Pilih Foto</div></div><div class="image-preview" id="donaturPreview">${item&&item.photo?`<img src="${item.photo}">`:''}</div></div><div class="form-group"><label>Tanggal</label><input type="date" id="fDonaturDate" value="${item&&item.date?item.date:new Date().toISOString().split('T')[0]}"></div><div class="form-group"><label>Status</label><select id="fDonaturStatus"><option value="diterima" ${item&&item.status==='diterima'?'selected':''}>Diterima</option><option value="menunggu" ${item&&item.status==='menunggu'?'selected':''}>Menunggu</option></select></div><div class="form-group"><label>Keterangan</label><textarea id="fDonaturDescription">${item?item.description||'':''}</textarea></div>`}
            else if(type==='sponsor'){const item=id?DATA.sponsor.find(s=>s.id===id):null;fields=`<div class="form-group"><label>Nama Sponsor *</label><input type="text" id="fSponsorName" value="${item?item.name:''}" required></div><div class="form-group"><label>Nominal *</label><input type="number" id="fSponsorAmount" value="${item?item.amount:''}" required></div><div class="form-group"><label>Logo Sponsor</label><div class="file-upload-wrapper"><input type="file" id="fSponsorLogo" accept="image/*" onchange="previewImage(this,'sponsorPreview')"><div class="file-label"><i class="fas fa-cloud-upload-alt"></i> Pilih Logo</div></div><div class="image-preview" id="sponsorPreview">${item&&item.logo?`<img src="${item.logo}">`:''}</div></div><div class="form-group"><label>Tanggal</label><input type="date" id="fSponsorDate" value="${item&&item.date?item.date:new Date().toISOString().split('T')[0]}"></div><div class="form-group"><label>Status</label><select id="fSponsorStatus"><option value="diterima" ${item&&item.status==='diterima'?'selected':''}>Diterima</option><option value="menunggu" ${item&&item.status==='menunggu'?'selected':''}>Menunggu</option></select></div><div class="form-group"><label>Keterangan</label><textarea id="fSponsorDescription">${item?item.description||'':''}</textarea></div>`}
            else if(type==='galeri'){fields=`<div class="form-group"><label>Judul Foto *</label><input type="text" id="fGalleryTitle" placeholder="Contoh: Persiapan Panggung Hari ke-7" required></div><div class="form-group"><label>📁 Pilih Folder</label><select id="fGalleryCategory"><option value="persiapan">📁 Persiapan Panggung</option><option value="dekorasi">📁 Dekorasi Acara</option><option value="latihan">📁 Latihan Siswa</option><option value="spot">📁 Spot Foto</option><option value="alumni">📁 Foto Alumni</option></select></div><div class="form-group"><label>Upload Foto</label><div class="file-upload-wrapper"><input type="file" id="fGalleryImageFile" accept="image/*" onchange="previewImage(this,'galleryPreview')"><div class="file-label"><i class="fas fa-cloud-upload-alt"></i> Pilih Foto</div></div><div class="image-preview" id="galleryPreview"></div><small style="color:var(--gray);display:block;margin-top:5px">Atau bisa juga masukkan URL gambar di bawah</small><input type="text" id="fGalleryImageUrl" placeholder="https://... atau 🎭" style="margin-top:8px"></div>`}
            else if(type==='kaos'){const item=id?DATA.kaos.find(k=>k.id===id):null;fields=`<div class="form-group"><label>Nama Kaos *</label><input type="text" id="fKaosName" value="${item?item.name:''}" required></div><div class="form-row"><div class="form-group"><label>Harga *</label><input type="number" id="fKaosPrice" value="${item?item.price:''}" required></div><div class="form-group"><label>Stok</label><input type="number" id="fKaosStock" value="${item?item.stock:50}"></div></div><div class="form-group"><label>Size</label><input type="text" id="fKaosSize" value="${item?item.size:'S, M, L, XL, XXL'}"></div>${id?`<div class="form-group"><label>Terjual</label><input type="number" id="fKaosSold" value="${item?item.sold:0}"></div>`:''}<div class="form-group"><label>Emoji/Icon</label><input type="text" id="fKaosImage" value="${item?item.image||'👕':'👕'}"></div>`}
            else if(type==='rundown'){const item=id?DATA.rundown.find(r=>r.id===id):null;fields=`<div class="form-group"><label>Waktu *</label><input type="text" id="fRundownTime" value="${item?item.time:''}" placeholder="08.00 - 09.00" required></div><div class="form-group"><label>Acara *</label><input type="text" id="fRundownActivity" value="${item?item.activity:''}" required></div><div class="form-group"><label>Keterangan/PIC</label><input type="text" id="fRundownPic" value="${item?item.pic:''}"></div><div class="form-group"><label><input type="checkbox" id="fRundownHighlight" ${item&&item.isHighlight?'checked':''}> Acara Utama</label></div>`}
            else if(type==='anggaran'){const item=id?DATA.budgets.find(b=>b.id===id):null;fields=`<div class="form-group"><label>Kebutuhan *</label><input type="text" id="fBudgetName" value="${item?item.name:''}" required></div><div class="form-group"><label>Nominal *</label><input type="number" id="fBudgetAmount" value="${item?item.amount:''}" required></div>`}
            document.getElementById('formFields').innerHTML=fields;document.getElementById('formModal').classList.add('show')
        }

        function closeFormModal(){document.getElementById('formModal').classList.remove('show')}

        function handleFormSubmit(e){
            e.preventDefault();
            if(currentFormType==='donatur'){
                const name=document.getElementById('fDonaturName').value,amount=parseInt(document.getElementById('fDonaturAmount').value),date=document.getElementById('fDonaturDate').value,status=document.getElementById('fDonaturStatus').value,description=document.getElementById('fDonaturDescription').value,photoFile=document.getElementById('fDonaturPhoto').files[0];
                if(!name||!amount){showNotification('Nama dan nominal wajib diisi!','error');return}
                const processSave=(photoData)=>{if(currentEditId){const item=DATA.donatur.find(s=>s.id===currentEditId);if(item){item.name=name;item.amount=amount;item.date=date||new Date().toLocaleDateString('id-ID',{day:'numeric',month:'long',year:'numeric'});item.status=status;item.description=description||'';if(photoData)item.photo=photoData}}else{DATA.donatur.push({id:nextId.donatur++,name:name,amount:amount,date:date||new Date().toLocaleDateString('id-ID',{day:'numeric',month:'long',year:'numeric'}),status:status,description:description||'',photo:photoData||`https://ui-avatars.com/api/?name=${encodeURIComponent(name)}&size=100&background=0B8F88&color=fff`})}saveToStorage();renderAll();renderAdminDonatur();closeFormModal();showNotification('✅ Donatur berhasil disimpan!','success')};
                if(photoFile){const reader=new FileReader();reader.onload=function(e){processSave(e.target.result)};reader.readAsDataURL(photoFile)}else{processSave(null)}}
            else if(currentFormType==='sponsor'){
                const name=document.getElementById('fSponsorName').value,amount=parseInt(document.getElementById('fSponsorAmount').value),date=document.getElementById('fSponsorDate').value,status=document.getElementById('fSponsorStatus').value,description=document.getElementById('fSponsorDescription').value,logoFile=document.getElementById('fSponsorLogo').files[0];
                if(!name||!amount){showNotification('Nama dan nominal wajib diisi!','error');return}
                const processSave=(logoData)=>{if(currentEditId){const item=DATA.sponsor.find(s=>s.id===currentEditId);if(item){item.name=name;item.amount=amount;item.date=date||new Date().toLocaleDateString('id-ID',{day:'numeric',month:'long',year:'numeric'});item.status=status;item.description=description||'';if(logoData)item.logo=logoData}}else{DATA.sponsor.push({id:nextId.sponsor++,name:name,amount:amount,date:date||new Date().toLocaleDateString('id-ID',{day:'numeric',month:'long',year:'numeric'}),status:status,description:description||'',logo:logoData||`https://ui-avatars.com/api/?name=${encodeURIComponent(name)}&size=100&background=092C55&color=fff`})}saveToStorage();renderAll();renderAdminSponsor();closeFormModal();showNotification('✅ Sponsor berhasil disimpan!','success')};
                if(logoFile){const reader=new FileReader();reader.onload=function(e){processSave(e.target.result)};reader.readAsDataURL(logoFile)}else{processSave(null)}}
            else if(currentFormType==='galeri'){
                const title=document.getElementById('fGalleryTitle').value,category=document.getElementById('fGalleryCategory').value,imageFile=document.getElementById('fGalleryImageFile').files[0],imageUrl=document.getElementById('fGalleryImageUrl').value;
                if(!title){showNotification('Judul wajib diisi!','error');return}if(!imageFile&&!imageUrl){showNotification('Upload foto atau masukkan URL gambar!','error');return}
                const processSave=(imageData)=>{DATA.gallery.push({id:nextId.gallery++,title:title,category:category,image:imageData||imageUrl||'📸'});saveToStorage();renderAll();renderAdminGaleri();closeFormModal();showNotification('✅ Foto berhasil ditambahkan ke folder '+category+'!','success')};
                if(imageFile){const reader=new FileReader();reader.onload=function(e){processSave(e.target.result)};reader.readAsDataURL(imageFile)}else{processSave(null)}}
            else if(currentFormType==='kaos'){
                const name=document.getElementById('fKaosName').value,price=parseInt(document.getElementById('fKaosPrice').value),stock=parseInt(document.getElementById('fKaosStock').value)||0,size=document.getElementById('fKaosSize').value||'S, M, L, XL, XXL',image=document.getElementById('fKaosImage').value||'👕',sold=parseInt(document.getElementById('fKaosSold')?.value)||0;
                if(!name||!price){showNotification('Nama dan harga wajib diisi!','error');return}
                if(currentEditId){const item=DATA.kaos.find(k=>k.id===currentEditId);if(item){item.name=name;item.price=price;item.stock=stock;item.size=size;item.image=image;item.sold=sold;item.status=stock>0?'tersedia':'habis'}}else{DATA.kaos.push({id:nextId.kaos++,name:name,price:price,stock:stock,size:size,image:image,sold:0,status:stock>0?'tersedia':'habis'})}saveToStorage();renderAll();renderAdminKaos();closeFormModal();showNotification('✅ Kaos berhasil disimpan!','success')}
            else if(currentFormType==='rundown'){
                const time=document.getElementById('fRundownTime').value,activity=document.getElementById('fRundownActivity').value,pic=document.getElementById('fRundownPic').value,isHighlight=document.getElementById('fRundownHighlight').checked;
                if(!time||!activity){showNotification('Waktu dan acara wajib diisi!','error');return}
                if(currentEditId){const item=DATA.rundown.find(r=>r.id===currentEditId);if(item){item.time=time;item.activity=activity;item.pic=pic||'';item.isHighlight=isHighlight}}else{DATA.rundown.push({id:nextId.rundown++,time:time,activity:activity,pic:pic||'',isHighlight:isHighlight})}saveToStorage();renderAll();renderAdminRundown();closeFormModal();showNotification('✅ Acara berhasil disimpan!','success')}
            else if(currentFormType==='anggaran'){
                const name=document.getElementById('fBudgetName').value,amount=parseInt(document.getElementById('fBudgetAmount').value);
                if(!name||!amount){showNotification('Nama dan nominal wajib diisi!','error');return}
                if(currentEditId){const item=DATA.budgets.find(b=>b.id===currentEditId);if(item){item.name=name;item.amount=amount}}else{DATA.budgets.push({id:nextId.budget++,name:name,amount:amount})}saveToStorage();renderAll();renderAdminAnggaran();closeFormModal();showNotification('✅ Anggaran berhasil disimpan!','success')}
        }

        // ============================================================
        // SETTINGS
        // ============================================================
        function handleSettingsUpdate(e){e.preventDefault();DATA.eventName=document.getElementById('settEventName').value;DATA.eventDate=document.getElementById('settEventDate').value;DATA.targetFund=parseInt(document.getElementById('settTargetFund').value);DATA.slogan=document.getElementById('settSlogan').value;DATA.location=document.getElementById('settLocation').value;DATA.whatsapp=document.getElementById('settWhatsapp').value;saveToStorage();renderAll();document.getElementById('heroSlogan').textContent=DATA.slogan;document.getElementById('heroLocation').textContent=DATA.location;document.getElementById('kontakLocation').textContent=DATA.location;document.getElementById('footerSlogan').textContent=DATA.slogan;showNotification('✅ Pengaturan berhasil diupdate!','success')}

        // ============================================================
        // LOGIN
        // ============================================================
        function openLogin(){document.getElementById('loginModal').classList.add('show')}
        function closeLogin(){document.getElementById('loginModal').classList.remove('show')}
        function handleLogin(e){e.preventDefault();const email=document.getElementById('loginEmail').value,password=document.getElementById('loginPassword').value;if((email==='admin@smkn1leles.sch.id'||email==='admin')&&password==='admin123'){isLoggedIn=true;closeLogin();showNotification('✅ Login berhasil!','success');openAdmin()}else{showNotification('❌ Email atau password salah!','error')}}
        function openAdmin(){if(!isLoggedIn){showNotification('Silakan login terlebih dahulu!','error');openLogin();return}document.getElementById('adminModal').classList.add('show');updateSchoolLogo();updateHeroBg();renderAdminAll()}
        function closeAdmin(){document.getElementById('adminModal').classList.remove('show')}

        // ============================================================
        // NOTIFICATION
        // ============================================================
        function showNotification(message,type='info'){const el=document.getElementById('notification');el.textContent=message;el.className=`notification ${type}`;el.style.display='block';setTimeout(()=>{el.style.display='none'},3000)}

        // ============================================================
        // MOBILE MENU
        // ============================================================
        function toggleMenu(){document.getElementById('navMenu').classList.toggle('open')}

        // ============================================================
        // INIT
        // ============================================================
        document.addEventListener('DOMContentLoaded',function(){try{loadFromStorage();updateHeroBg();renderAll();updateCountdown();setInterval(updateCountdown,1000);document.getElementById('heroSlogan').textContent=DATA.slogan||'"Bersama Mengenang, Berkarya, dan Menginspirasi"';document.getElementById('heroLocation').textContent=DATA.location||'SMK Negeri 1 Leles';document.getElementById('kontakLocation').textContent=DATA.location||'SMK Negeri 1 Leles, Jawa Barat';document.getElementById('footerSlogan').textContent=DATA.slogan||'"Bersama Mengenang, Berkarya, dan Menginspirasi"';console.log('✅ Website HUT SMKN 1 Leles & Reuni Akbar 2026 siap!');console.log('🎨 Admin bisa upload background hero dengan efek blur & transparan');console.log('🔑 Login Admin: admin@smkn1leles.sch.id / admin123')}catch(e){console.error('Error loading page:',e)}});
        document.getElementById('loginModal').addEventListener('click',function(e){if(e.target===this)closeLogin()});
        document.getElementById('adminModal').addEventListener('click',function(e){if(e.target===this)closeAdmin()});
        document.getElementById('formModal').addEventListener('click',function(e){if(e.target===this)closeFormModal()});
        document.getElementById('pesanKaosModal').addEventListener('click',function(e){if(e.target===this)closePesanKaos()});

        // ============================================================
        // EXPOSE GLOBALS
        // ============================================================
        window.toggleMenu=toggleMenu;
        window.openLogin=openLogin;window.closeLogin=closeLogin;window.handleLogin=handleLogin;
        window.openAdmin=openAdmin;window.closeAdmin=closeAdmin;
        window.switchTab=switchTab;
        window.uploadSchoolLogo=uploadSchoolLogo;window.removeSchoolLogo=removeSchoolLogo;
        window.uploadHeroBg=uploadHeroBg;window.removeHeroBg=removeHeroBg;
        window.openAddDonatur=openAddDonatur;window.editDonatur=editDonatur;window.deleteDonatur=deleteDonatur;window.toggleStatusDonatur=toggleStatusDonatur;
        window.openAddSponsor=openAddSponsor;window.editSponsor=editSponsor;window.deleteSponsor=deleteSponsor;window.toggleStatusSponsor=toggleStatusSponsor;
        window.openAddKaos=openAddKaos;window.editKaos=editKaos;window.deleteKaos=deleteKaos;window.toggleStatusKaos=toggleStatusKaos;
        window.openAddRundown=openAddRundown;window.editRundown=editRundown;window.deleteRundown=deleteRundown;window.toggleHighlightRundown=toggleHighlightRundown;
        window.openAddAnggaran=openAddAnggaran;window.editAnggaran=editAnggaran;window.deleteAnggaran=deleteAnggaran;
        window.openAddGaleri=openAddGaleri;window.deleteGaleri=deleteGaleri;
        window.closeFormModal=closeFormModal;window.handleFormSubmit=handleFormSubmit;
        window.handleSettingsUpdate=handleSettingsUpdate;window.showNotification=showNotification;
        window.filterGallery=filterGallery;window.previewImage=previewImage;
        window.openPesanKaos=openPesanKaos;window.closePesanKaos=closePesanKaos;window.handlePesanKaos=handlePesanKaos;window.toggleAlamat=toggleAlamat;
        window.toggleStatusPesanan=toggleStatusPesanan;window.deletePesanan=deletePesanan;window.exportPesanan=exportPesanan;
    </script>
</body>
</html>
