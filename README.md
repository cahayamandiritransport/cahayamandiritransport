<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cahaya Mandiri Transport</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Bebas+Neue&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #ffffff;
            color: #333;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        .header {
            background: linear-gradient(to right, #0033A0, #FF0000);
            padding: 20px;
            color: white;
            font-family: 'Bebas Neue', cursive;
            font-size: 32px;
        }
        .container {
            padding: 50px;
        }
        .btn {
            background-color: #0033A0;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
        }
        .dashboard {
            display: none;
            padding: 20px;
        }
        .dashboard h2 {
            color: #0033A0;
        }
        .dashboard-content {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
        }
        .card {
            background: #f8f8f8;
            padding: 20px;
            margin: 10px;
            border-radius: 10px;
            width: 250px;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
        }
        .about {
            background-color: #f4f4f4;
            padding: 40px;
            margin: 20px;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Cahaya Mandiri Transport</h1>
    </div>
    <div class="container">
        <h2>Selamat Datang di CMT</h2>
        <p>Penyedia layanan transportasi terbaik untuk kebutuhan bisnis dan personal Anda.</p>
        <a href="#" class="btn" onclick="showDashboard()">Masuk ke Dashboard</a>
    </div>
    
    <div class="about">
        <h2>Tentang Cahaya Mandiri Transport</h2>
        <p>Cahaya Mandiri Transport (CMT) adalah perusahaan yang bergerak di bidang transportasi dan logistik, menyediakan solusi pengiriman yang efisien dan andal untuk berbagai kebutuhan bisnis maupun personal. Dengan armada yang modern dan sistem pelacakan GPS real-time, kami memastikan keamanan dan ketepatan waktu dalam setiap pengiriman.</p>
        <p>Kami berkomitmen untuk memberikan pelayanan terbaik dengan standar profesionalisme tinggi. Tim kami yang berpengalaman siap membantu Anda dalam setiap perjalanan dan pengiriman barang dengan kecepatan dan ketepatan yang optimal.</p>
    </div>
    
    <div class="dashboard" id="dashboard">
        <h2>Dashboard</h2>
        <div class="dashboard-content">
            <div class="card">
                <h3>Tracking GPS</h3>
                <p>Lacak lokasi real-time kendaraan.</p>
            </div>
            <div class="card">
                <h3>Daftar Kendaraan</h3>
                <p>Kelola dan lihat data armada.</p>
            </div>
            <div class="card">
                <h3>Manajemen Pengguna</h3>
                <p>Atur akun pengguna berdasarkan role.</p>
            </div>
            <div class="card">
                <h3>Ringkasan Pengiriman</h3>
                <p>Lihat data aktivitas pengiriman terbaru.</p>
            </div>
        </div>
    </div>

    <script>
        function showDashboard() {
            document.querySelector('.container').style.display = 'none';
            document.querySelector('.about').style.display = 'none';
            document.getElementById('dashboard').style.display = 'block';
        }
    </script>
</body>
</html>
