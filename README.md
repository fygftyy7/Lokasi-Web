# Lokasi-Web
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Deteksi Lokasi Kamu</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 30px;
      text-align: center;
    }
    #alamat {
      margin-top: 20px;
      font-size: 1.2em;
    }
  </style>
</head>
<body>
  <h1>Website Deteksi Lokasi</h1>
  <p>Website ini akan mengetahui lokasi atau alamatmu saat dibuka.</p>
  <div id="alamat">Mendeteksi lokasi...</div>

  <script>
    function getAlamat(lat, lon) {
      // Ganti dengan API key kamu dari OpenCage (gratis signup di https://opencagedata.com/)
      const apiKey = 'd2fa48541c7547d19620eff70dc943c6';
      const url = https://api.opencagedata.com/geocode/v1/json?q=${lat}+${lon}&key=${apiKey}`https://api.opencagedata.com/geocode/v1/json?q=${lat}+${lon}&key=${apiKey}`;

      fetch(url)
        .then(response => response
