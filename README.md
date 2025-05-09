<!DOCTYPE html><html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Мини-курс: Growth Mindset</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap" rel="stylesheet">
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            cyber: ['Orbitron', 'sans-serif'],
          },
          colors: {
            neon: '#39FF14',
            matrix: '#00FF41',
            pinkish: '#FF00FF',
          },
        }
      }
    }
  </script>
</head>
<body class="bg-black text-white font-cyber min-h-screen flex items-center justify-center relative overflow-hidden">
  <div class="absolute inset-0 bg-gradient-to-br from-pinkish via-neon to-matrix opacity-10 animate-pulse"></div>  <section class="z-10 p-6 w-full max-w-md bg-gray-900 bg-opacity-80 rounded-2xl shadow-2xl backdrop-blur-lg">
    <div class="flex flex-col items-center mb-6">
      <img src="https://cdn-icons-png.flaticon.com/512/3522/3522094.png" alt="Логотип" class="w-20 h-20 mb-2" />
      <h1 class="text-3xl font-bold text-pinkish">Growth Mindset</h1>
      <p class="text-center text-gray-300 mt-2">Как прокачать мышление и выйти на новый уровень</p>
    </div><form class="space-y-4" onsubmit="handleSubmit(event)">
  <div>
    <label class="block text-sm font-medium mb-1">Имя</label>
    <div class="relative">
      <span class="absolute left-3 top-2.5 text-neon">
        <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"/></svg>
      </span>
      <input type="text" id="name" class="w-full pl-10 px-4 py-2 border border-matrix rounded-xl bg-black text-white focus:outline-none focus:ring-2 focus:ring-neon" required />
    </div>
  </div>
  <div>
    <label class="block text-sm font-medium mb-1">Телефон</label>
    <div class="relative">
      <span class="absolute left-3 top-2.5 text-neon">
        <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M6.62 10.79a15.053 15.053 0 006.59 6.59l2.2-2.2c.27-.27.67-.36 1.02-.24 1.12.37 2.33.57 3.57.57.55 0 1 .45 1 1v3.5c0 .55-.45 1-1 1C10.61 22 2 13.39 2 2c0-.55.45-1 1-1H6.5c.55 0 1 .45 1 1 0 1.24.2 2.45.57 3.57.11.35.03.74-.25 1.02l-2.2 2.2z"/></svg>
      </span>
      <input type="tel" id="phone" class="w-full pl-10 px-4 py-2 border border-matrix rounded-xl bg-black text-white focus:outline-none focus:ring-2 focus:ring-neon" required />
    </div>
  </div>
  <button type="submit" class="w-full bg-neon text-black py-2 font-bold rounded-xl hover:bg-matrix transition-colors duration-200">Получить доступ</button>
</form>

<p id="successMessage" class="text-neon text-center mt-4 hidden">Спасибо! Мы свяжемся с вами.</p>

  </section>  <script>
    function handleSubmit(event) {
      event.preventDefault();
      document.getElementById('successMessage').classList.remove('hidden');
    }
  </script></body>
</html>
