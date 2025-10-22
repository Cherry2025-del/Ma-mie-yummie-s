# Ma-mie-yummie-s
Menu
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ma Mie Yummies - Menu Restaurant</title>
  
  <!-- Favicon -->
  <link rel="icon" href="images/Ma_Mie_Yummies_LOGO.png" type="image/png" />

  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- Feather Icons -->
  <script src="https://unpkg.com/feather-icons"></script>

  <!-- Configuration Tailwind -->
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primary: '#A020F0', // Violet doux inspiré du logo
            secondary: '#FF6B6B',
          },
        },
      },
    };
  </script>

  <style>
    /* Pour une transition fluide du menu mobile */
    .menu-active {
      display: block !important;
    }
  </style>
</head>

<body class="bg-gray-50 font-sans">

  <!-- ✅ NAVBAR avec logo -->
  <nav class="bg-white shadow-md fixed top-0 left-0 w-full z-50">
    <div class="container mx-auto flex justify-between items-center px-4 py-3">
      <!-- Logo -->
      <div class="flex items-center space-x-3">
        <img src="images/Ma_Mie_Yummies_LOGO.png" alt="Logo Ma Mie Yummies" class="w-12 h-12 rounded-full object-contain" />
        <h1 class="text-xl font-semibold text-primary">Ma Mie Yummies</h1>
      </div>

      <!-- Menu Desktop -->
      <ul class="hidden md:flex space-x-6 text-gray-700 font-medium">
        <li><a href="index.html" class="hover:text-primary">Accueil</a></li>
        <li><a href="plats-du-jour.html" class="hover:text-primary">Plats du Jour</a></li>
        <li><a href="sandwich.html" class="hover:text-primary">Sandwichs</a></li>
        <li><a href="shawarma.html" class="hover:text-primary">Shawarmas</a></li>
        <li><a href="tacos.html" class="hover:text-primary">Tacos</a></li>
        <li><a href="burger.html" class="hover:text-primary">Burgers</a></li>
      </ul>

      <!-- Bouton Menu Mobile -->
      <button id="menu-toggle" class="md:hidden text-primary">
        <i data-feather="menu" class="w-6 h-6"></i>
      </button>
    </div>

    <!-- Menu Mobile -->
    <div id="mobile-menu" class="hidden bg-white border-t border-gray-200 md:hidden">
      <ul class="flex flex-col items-center py-4 space-y-2 text-gray-700 font-medium">
        <li><a href="index.html" class="hover:text-primary">Accueil</a></li>
        <li><a href="plats-du-jour.html" class="hover:text-primary">Plats du Jour</a></li>
        <li><a href="sandwich.html" class="hover:text-primary">Sandwichs</a></li>
        <li><a href="shawarma.html" class="hover:text-primary">Shawarmas</a></li>
        <li><a href="tacos.html" class="hover:text-primary">Tacos</a></li>
        <li><a href="burger.html" class="hover:text-primary">Burgers</a></li>
      </ul>
    </div>
  </nav>

  <!-- Contenu principal -->
  <main class="container mx-auto px-4 py-24">
    <div class="text-center mb-12">
      <h1 class="text-4xl font-bold text-primary mb-4">Notre Menu Délicieux</h1>
      <p class="text-gray-600 max-w-2xl mx-auto">
        Découvrez nos plats savoureux et commandez en un clic !
      </p>
    </div>

    <!-- Grille des catégories -->
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">

      <!-- Plats du Jour -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105">
        <div class="bg-primary p-6">
          <h2 class="text-white text-xl font-bold">Plats du Jour</h2>
        </div>
        <div class="p-6">
          <p class="text-gray-600 mb-4">Découvrez nos spécialités quotidiennes</p>
          <a href="plats-du-jour.html" class="inline-flex items-center px-4 py-2 bg-secondary text-white rounded-lg hover:bg-opacity-90 transition">
            <span>Voir les plats</span>
            <i data-feather="arrow-right" class="ml-2"></i>
          </a>
        </div>
      </div>

      <!-- Sandwich -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105">
        <div class="bg-primary p-6">
          <h2 class="text-white text-xl font-bold">Nos Sandwichs</h2>
        </div>
        <div class="p-6">
          <p class="text-gray-600 mb-4">Des sandwichs frais et savoureux</p>
          <a href="sandwich.html" class="inline-flex items-center px-4 py-2 bg-secondary text-white rounded-lg hover:bg-opacity-90 transition">
            <span>Voir les options</span>
            <i data-feather="arrow-right" class="ml-2"></i>
          </a>
        </div>
      </div>

      <!-- Shawarmas -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105">
        <div class="bg-primary p-6">
          <h2 class="text-white text-xl font-bold">Nos Shawarmas</h2>
        </div>
        <div class="p-6">
          <p class="text-gray-600 mb-4">Shawarmas préparés avec soin</p>
          <a href="shawarma.html" class="inline-flex items-center px-4 py-2 bg-secondary text-white rounded-lg hover:bg-opacity-90 transition">
            <span>Voir les options</span>
            <i data-feather="arrow-right" class="ml-2"></i>
          </a>
        </div>
      </div>

      <!-- Tacos -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105">
        <div class="bg-primary p-6">
          <h2 class="text-white text-xl font-bold">Nos Tacos</h2>
        </div>
        <div class="p-6">
          <p class="text-gray-600 mb-4">Tacos gourmands à savourer</p>
          <a href="tacos.html" class="inline-flex items-center px-4 py-2 bg-secondary text-white rounded-lg hover:bg-opacity-90 transition">
            <span>Voir les options</span>
            <i data-feather="arrow-right" class="ml-2"></i>
          </a>
        </div>
      </div>

      <!-- Burgers -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105">
        <div class="bg-primary p-6">
          <h2 class="text-white text-xl font-bold">Nos Burgers</h2>
        </div>
        <div class="p-6">
          <p class="text-gray-600 mb-4">Burgers juteux et copieux</p>
          <a href="burger.html" class="inline-flex items-center px-4 py-2 bg-secondary text-white rounded-lg hover:bg-opacity-90 transition">
            <span>Voir les options</span>
            <i data-feather="arrow-right" class="ml-2"></i>
          </a>
        </div>
      </div>

    </div>
  </main>

  <!-- Footer simple -->
  <footer class="bg-white border-t py-6 text-center text-gray-600 text-sm">
    © 2025 Ma Mie Yummies — Tous droits réservés.
  </footer>

  <!-- Script menu mobile -->
  <script>
    feather.replace();
    const menuToggle = document.getElementById('menu-toggle');
    const mobileMenu = document.getElementById('mobile-menu');
    menuToggle.addEventListener('click', () => {
      mobileMenu.classList.toggle('menu-active');
    });
  </script>
</body>
</html>
