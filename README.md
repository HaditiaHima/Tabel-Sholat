# Tabel-Sholat
Pengingat Diri
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tabel Evaluasi Salat</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    body {
      background: linear-gradient(to right, #6EE7B7, #3B82F6);
      font-family: 'Inter', sans-serif;
      color: #333;
      padding: 20px;
    }
    .checkbox:checked + .check-label {
      background-color: #10B981;
      color: white;
      border-color: #10B981;
      transition: all 0.3s ease;
    }
    .check-label {
      display: inline-block;
      padding: 6px 12px;
      background-color: #F3F4F6;
      border: 2px solid #E5E7EB;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease, transform 0.3s ease;
    }
    .check-label:hover {
      background-color: #E5E7EB;
      transform: scale(1.1);
    }
    .table-row:hover {
      background-color: #E5E7EB;
      transition: background-color 0.3s ease;
    }
    .total-bounce {
      animation: bounce 1s infinite;
    }
    @keyframes bounce {
      0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
      40% { transform: translateY(-10px); }
      60% { transform: translateY(-5px); }
    }
    .btn {
      padding: 10px 20px;
      background-color: #4CAF50;
      color: white;
      border-radius: 8px;
      font-weight: bold;
      transition: all 0.3s ease;
    }
    .btn:hover {
      background-color: #45A049;
      transform: scale(1.05);
    }
    .btn-secondary {
      background-color: #FFDD57;
    }
    .btn-secondary:hover {
      background-color: #FFCC33;
    }
    .btn-tertiary {
      background-color: #3B82F6;
    }
    .btn-tertiary:hover {
      background-color: #2563EB;
    }
    .card {
      padding: 20px;
      background: white;
      border-radius: 10px;
      box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.2);
    }
  </style>
</head>
<body>

  <div class="max-w-4xl mx-auto space-y-6">
    <h1 class="text-4xl font-semibold text-center text-white mb-4">Tabel Evaluasi Salat</h1>
    <p class="text-center text-lg text-white mb-6">Mari kita merenung sejenak, apakah kita sudah menunaikan kewajiban yang telah diperintahkan-Nya? Salat adalah bentuk pengingat yang tak terbatas, yang harus senantiasa menjadi bagian dari hidup kita.</p>

    <!-- Tabel Salat Wajib -->
    <div class="card">
      <h2 class="text-2xl text-center text-blue-600 mb-4">Salat Wajib</h2>
      <table class="w-full table-auto text-center text-gray-700">
        <thead class="bg-gradient-to-r from-blue-500 to-blue-700 text-white">
          <tr>
            <th class="py-3 px-6">Waktu Salat</th>
            <th class="py-3 px-6">Apakah Anda Melaksanakannya?</th>
          </tr>
        </thead>
        <tbody>
          <tr class="table-row">
            <td class="py-4 px-6 border-b">Subuh</td>
            <td class="py-4 px-6 border-b">
              <input type="checkbox" id="subuh" class="checkbox hidden" />
              <label for="subuh" class="check-label">Tidak Salat</label>
            </td>
          </tr>
          <tr class="table-row">
            <td class="py-4 px-6 border-b">Dzuhur</td>
            <td class="py-4 px-6 border-b">
              <input type="checkbox" id="dzuhur" class="checkbox hidden" />
              <label for="dzuhur" class="check-label">Tidak Salat</label>
            </td>
          </tr>
          <tr class="table-row">
            <td class="py-4 px-6 border-b">Ashar</td>
            <td class="py-4 px-6 border-b">
              <input type="checkbox" id="ashar" class="checkbox hidden" />
              <label for="ashar" class="check-label">Tidak Salat</label>
            </td>
          </tr>
          <tr class="table-row">
            <td class="py-4 px-6 border-b">Maghrib</td>
            <td class="py-4 px-6 border-b">
              <input type="checkbox" id="maghrib" class="checkbox hidden" />
              <label for="maghrib" class="check-label">Tidak Salat</label>
            </td>
          </tr>
          <tr class="table-row">
            <td class="py-4 px-6 border-b">Isya</td>
            <td class="py-4 px-6 border-b">
              <input type="checkbox" id="isya" class="checkbox hidden" />
              <label for="isya" class="check-label">Tidak Salat</label>
            </td>
          </tr>
        </tbody>
      </table>
    </div>

    <!-- Tabel Salat Sunnah -->
    <div class="card mt-6">
      <h2 class="text-2xl text-center text-green-600 mb-4">Salat Sunnah</h2>
      <table class="w-full table-auto text-center text-gray-700">
        <thead class="bg-gradient-to-r from-green-500 to-green-700 text-white">
          <tr>
            <th class="py-3 px-6">Waktu Salat</th>
            <th class="py-3 px-6">Apakah Anda Melaksanakannya?</th>
          </tr>
        </thead>
        <tbody>
          <tr class="table-row">
            <td class="py-4 px-6 border-b">Dhuha</td>
            <td class="py-4 px-6 border-b">
              <input type="checkbox" id="dhuha" class="checkbox hidden" />
              <label for="dhuha" class="check-label">Tidak Salat</label>
            </td>
          </tr>
          <tr class="table-row">
            <td class="py-4 px-6 border-b">Tahajud</td>
            <td class="py-4 px-6 border-b">
              <input type="checkbox" id="tahajud" class="checkbox hidden" />
              <label for="tahajud" class="check-label">Tidak Salat</label>
            </td>
          </tr>
        </tbody>
      </table>
    </div>

    <!-- Tabel Tadarus -->
    <div class="card mt-6">
      <h2 class="text-2xl text-center text-purple-600 mb-4">Tadarus</h2>
      <table class="w-full table-auto text-center text-gray-700">
        <thead class="bg-gradient-to-r from-purple-500 to-purple-700 text-white">
          <tr>
            <th class="py-3 px-6">Apakah Anda Membaca Al-Qur'an Hari Ini?</th>
            <th class="py-3 px-6">Jumlah Halaman yang Dibaca</th>
          </tr>
        </thead>
        <tbody>
          <tr class="table-row">
            <td class="py-4 px-6 border-b">Tadarus</td>
            <td class="py-4 px-6 border-b">
              <input type="number" id="tadarus-pages" class="w-20 text-center border-2 rounded-lg" min="0" placeholder="Jumlah Halaman" />
            </td>
          </tr>
        </tbody>
      </table>
    </div>

    <!-- Total Salat yang Tidak Dikerjakan -->
    <div class="text-center mt-6">
      <p class="text-sm text-gray-600">Mari kita berhenti sejenak dan introspeksi diri. Berapa kali kita mengabaikan kewajiban kita hari ini?</p>
      <p id="total" class="text-2xl font-bold text-red-600 total-bounce">0</p>
    </div>

    <!-- Tombol Reset -->
    <div class="text-center mt-6">
      <button id="reset" class="btn mb-4">Reset Tabel</button>
    </div>

    <!-- Tombol untuk Ayat, Hadist dan Cerita -->
    <div class="text-center">
      <button onclick="showAyat()" class="btn btn-tertiary mb-2">Ayat Pendukung</button>
      <button onclick="showHadist()" class="btn btn-secondary mb-2">Hadist Pendukung</button>
      <button onclick="showCerita()" class="btn btn-secondary">Cerita Inspiratif</button>
    </div>

  </div>

  <script>
    const checkboxes = document.querySelectorAll('.checkbox');
    const totalElement = document.getElementById('total');

    checkboxes.forEach(checkbox => {
      checkbox.addEventListener('change', () => {
        let total = 0;
        checkboxes.forEach(cb => {
          if (cb.checked) total++;
        });
        totalElement.textContent = total;
      });
    });

    document.getElementById('reset').addEventListener('click', () => {
      checkboxes.forEach(cb => cb.checked = false);
      totalElement.textContent = "0";
    });

    function showAyat() {
      alert("Ayat tentang Salat: 'Sesungguhnya salat itu adalah kewajiban yang ditentukan waktunya atas orang-orang yang beriman.' (QS. An-Nisa: 103)");
    }

    function showHadist() {
      alert("Hadist tentang Salat: 'Solat itu adalah tiang agama, barang siapa yang mendirikannya maka ia mendirikan agama, dan barang siapa yang meninggalkannya maka ia meruntuhkan agama.' (HR. Bukhari dan Muslim)");
    }

    function showCerita() {
      alert("Cerita tentang Salat: Dalam kisah seorang sahabat Nabi, Abu Hurairah RA, yang selalu melaksanakan salat sunnah meskipun ia seorang yang miskin dan lemah. Ia berkata, 'Tidak ada yang lebih aku sukai setelah melaksanakan salat wajib, selain melaksanakan salat sunnah.'");
    }
  </script>
</body>
</html>
