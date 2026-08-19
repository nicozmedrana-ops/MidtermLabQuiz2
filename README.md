# MidtermLabQuiz2
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KAINAN | Filipino Food &amp; Restaurant Showcase</title>

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.css" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,500;0,9..144,700;0,9..144,900;1,9..144,600&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">

<link href="style.css" rel="stylesheet">
</head>
<body>

<nav class="navbar navbar-expand-lg navbar-kainan sticky-top py-3">
  <div class="container">
    <a class="navbar-brand" href="#home"><i class="bi bi-egg-fried me-1"></i>KAINAN</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#mainNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="mainNav">
      <ul class="navbar-nav ms-auto align-items-lg-center">
        <li class="nav-item"><a class="nav-link" href="#home">Home</a></li>
        <li class="nav-item"><a class="nav-link" href="#gallery">Gallery</a></li>
        <li class="nav-item"><a class="nav-link" href="#categories">Categories</a></li>
        <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
        <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
        <li class="nav-item ms-lg-3 mt-2 mt-lg-0">
          <button class="btn btn-reserve btn-sm px-3 rounded-pill" data-bs-toggle="offcanvas" data-bs-target="#reserveCanvas">
            Reserve a Table
          </button>
        </li>
      </ul>
    </div>
  </div>
</nav>

<header id="home" class="hero-carousel position-relative">
  <div id="heroCarousel" class="carousel slide carousel-fade" data-bs-ride="carousel">
    <div class="carousel-inner h-100">
      <div class="carousel-item active">
        <img src="sinigang.jpg" alt="Filipino feast spread">
      </div>
      <div class="carousel-item">
        <img src="adobo.jpg" alt="Restaurant kitchen">
      </div>
      <div class="carousel-item">
        <img src="halohalo.jpg" alt="Dining table setting">
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#heroCarousel" data-bs-slide="prev">
      <span class="carousel-control-prev-icon"></span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#heroCarousel" data-bs-slide="next">
      <span class="carousel-control-next-icon"></span>
    </button>
  </div>
  <div class="hero-caption px-3">
    <span class="ticket">Table for one · Est. 2026</span>
    <h1>Sarap ng Bahay,<br>Serve sa Bawat Plato</h1>
    <p class="lead">A photo showcase of the dishes we grew up on — from sizzling sisig to sweet halo-halo — plated with a little extra flair.</p>
    <a href="#gallery" class="btn btn-lg rounded-pill btn-reserve px-4">View the Gallery</a>
  </div>
</header>

<section id="featured">
  <div class="container">
    <span class="ticket">Chef's Picks</span>
    <h2 class="mb-4">Tonight's Featured Plates</h2>
    <div class="row g-4">
      <div class="col-12 col-md-6 col-lg-4">
        <div class="featured-card">
          <img src="sisig.jpg">
          <div class="featured-overlay">
            <h5 class="mb-0">Crispy Pork Sisig</h5>
            <small>Sizzling plate, calamansi &amp; egg</small>
          </div>
        </div>
      </div>
      <div class="col-12 col-md-6 col-lg-4">
        <div class="featured-card">
          <img src="kare kare.jpg" alt="Featured dish two">
          <div class="featured-overlay">
            <h5 class="mb-0">Kare-Kare</h5>
            <small>Oxtail stew, peanut sauce</small>
          </div>
        </div>
      </div>
      <div class="col-12 col-md-6 col-lg-4">
        <div class="featured-card">
          <img src="halohalo.jpg" alt="Featured dish three">
          <div class="featured-overlay">
            <h5 class="mb-0">Halo-Halo</h5>
            <small>Shaved ice, ube, leche flan</small>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="bg-charcoal py-5">
  <div class="container">
    <div class="row text-center g-4">
      <div class="col-6 col-md-3">
        <div class="stat-num">12+</div>
        <div>Signature Dishes</div>
      </div>
      <div class="col-6 col-md-3">
        <div class="stat-num">4</div>
        <div>Menu Categories</div>
      </div>
      <div class="col-6 col-md-3">
        <div class="stat-num">8</div>
        <div>Years Serving</div>
      </div>
      <div class="col-6 col-md-3">
        <div class="stat-num">100%</div>
        <div>Homestyle Recipes</div>
      </div>
    </div>
  </div>
</section>

<section id="gallery">
  <div class="container">
    <span class="ticket">The Full Menu</span>
    <h2 class="mb-2">Gallery of Dishes</h2>
    <p class="text-muted mb-4">Tap any photo for the full plate description. Filter by category below.</p>

    <ul class="nav cat-pills mb-4" id="categories">
      <li class="nav-item"><button class="nav-link active" data-filter="all">All</button></li>
      <li class="nav-item"><button class="nav-link" data-filter="appetizers">Appetizers</button></li>
      <li class="nav-item"><button class="nav-link" data-filter="mains">Mains</button></li>
      <li class="nav-item"><button class="nav-link" data-filter="desserts">Desserts</button></li>
      <li class="nav-item"><button class="nav-link" data-filter="drinks">Drinks</button></li>
    </ul>

    <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-lg-4 g-4" id="dishGrid">

            <div class="col dish-item" data-category="appetizers">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="lumpia.webp" alt="Lumpiang Shanghai"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Lumpiang Shanghai" data-price="₱150"
                 data-desc="Crispy fried spring rolls packed with seasoned ground pork and vegetables, served with a sweet-sour dipping sauce."
                 data-img="lumpia.webp">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Appetizers</span>
            <h5 class="card-title mb-1">Lumpiang Shanghai</h5>
            <p class="small text-muted mb-1">Crispy pork &amp; veggie spring rolls</p>
            <span class="price-tag">₱150</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="appetizers">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="leischon.webp" alt="Lechon Kawali"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Lechon Kawali" data-price="₱280"
                 data-desc="Deep-fried pork belly, shatteringly crisp on the outside and tender within, served with spiced vinegar."
                 data-img="leischon.webp">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Appetizers</span>
            <h5 class="card-title mb-1">Lechon Kawali</h5>
            <p class="small text-muted mb-1">Crispy fried pork belly</p>
            <span class="price-tag">₱280</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="appetizers">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="Kinilaw.jpg" alt="Kinilaw na Tanigue"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Kinilaw na Tanigue" data-price="₱260"
                 data-desc="Fresh mackerel 'cooked' in calamansi and vinegar, tossed with ginger, onions, and chili."
                 data-img="kinilaw.jpg">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Appetizers</span>
            <h5 class="card-title mb-1">Kinilaw na Tanigue</h5>
            <p class="small text-muted mb-1">Filipino-style ceviche</p>
            <span class="price-tag">₱260</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="mains">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="ado.jpg" alt="Chicken Adobo"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Chicken Adobo" data-price="₱220"
                 data-desc="Chicken slow-braised in soy sauce, vinegar, garlic, and bay leaf — the Philippines' most iconic dish."
                 data-img="ado.jpg">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Mains</span>
            <h5 class="card-title mb-1">Chicken Adobo</h5>
            <p class="small text-muted mb-1">Soy-vinegar braised chicken</p>
            <span class="price-tag">₱220</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="mains">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="sini.webp" alt="Sinigang na Baboy"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Sinigang na Baboy" data-price="₱260"
                 data-desc="Pork simmered in a sour tamarind broth with kangkong, radish, and okra. Comfort in a bowl."
                 data-img="sini.webp">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Mains</span>
            <h5 class="card-title mb-1">Sinigang na Baboy</h5>
            <p class="small text-muted mb-1">Sour pork &amp; vegetable stew</p>
            <span class="price-tag">₱260</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="mains">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="kare kare.jpg" alt="Kare-Kare"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Kare-Kare" data-price="₱320"
                 data-desc="Oxtail and vegetables in a rich, roasted peanut sauce, served with shrimp paste on the side."
                 data-img="kare kare.jpg">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Mains</span>
            <h5 class="card-title mb-1">Kare-Kare</h5>
            <p class="small text-muted mb-1">Oxtail peanut stew</p>
            <span class="price-tag">₱320</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="mains">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="canton.jpg" alt="Pancit Canton"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Pancit Canton" data-price="₱190"
                 data-desc="Stir-fried egg noodles with pork, shrimp, and vegetables — a birthday-table staple for long life."
                 data-img="canton.jpg">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Mains</span>
            <h5 class="card-title mb-1">Pancit Canton</h5>
            <p class="small text-muted mb-1">Stir-fried noodles</p>
            <span class="price-tag">₱190</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="mains">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="bulalo.webp" alt="Bulalo"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Bulalo" data-price="₱340"
                 data-desc="Beef shank and bone marrow simmered for hours into a clear, deeply savory broth with corn and cabbage."
                 data-img="bulalo.webp">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Mains</span>
            <h5 class="card-title mb-1">Bulalo</h5>
            <p class="small text-muted mb-1">Beef shank marrow soup</p>
            <span class="price-tag">₱340</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="desserts">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="halohalo.jpg" alt="Halo-Halo"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Halo-Halo" data-price="₱165"
                 data-desc="Shaved ice mixed with sweet beans, jellies, ube halaya, leche flan, and a scoop of ube ice cream."
                 data-img="halohalo.jpg">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Desserts</span>
            <h5 class="card-title mb-1">Halo-Halo</h5>
            <p class="small text-muted mb-1">Mixed shaved-ice dessert</p>
            <span class="price-tag">₱165</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="desserts">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="leche.webp" alt="Leche Flan"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Leche Flan" data-price="₱95"
                 data-desc="Silky steamed egg custard topped with caramelized sugar syrup — a Filipino party essential."
                 data-img="leche.webp">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Desserts</span>
            <h5 class="card-title mb-1">Leche Flan</h5>
            <p class="small text-muted mb-1">Caramel egg custard</p>
            <span class="price-tag">₱95</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="desserts">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="turon.webp" alt="Turon"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Turon" data-price="₱80"
                 data-desc="Caramelized saba banana and jackfruit rolled in a crisp lumpia wrapper, fried to a golden crunch."
                 data-img="turon.webp">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Desserts</span>
            <h5 class="card-title mb-1">Turon</h5>
            <p class="small text-muted mb-1">Caramelized banana roll</p>
            <span class="price-tag">₱80</span>
          </div>
        </div>
      </div>

            <div class="col dish-item" data-category="drinks">
        <div class="dish-card">
          <div class="dish-img-wrap">
            <img src="calamansi.jpg" alt="Calamansi Juice"
                 data-bs-toggle="modal" data-bs-target="#dishModal"
                 data-title="Calamansi Juice" data-price="₱70"
                 data-desc="Freshly squeezed Philippine lime, lightly sweetened and served over ice. Bright and refreshing."
                 data-img="calamansi.jpg">
          </div>
          <div class="card-body">
            <span class="badge badge-cat mb-2">Drinks</span>
            <h5 class="card-title mb-1">Calamansi Juice</h5>
            <p class="small text-muted mb-1">Fresh Philippine lime cooler</p>
            <span class="price-tag">₱70</span>
          </div>
        </div>
      </div>

    </div>
  </div>
</section>

<section id="about" class="bg-white">
  <div class="container">
    <div class="row align-items-center g-5">
      <div class="col-12 col-lg-6">
        <span class="ticket">Our Story</span>
        <h2 class="mb-3">From a Family Kitchen to Your Table</h2>
        <p>KAINAN started as a weekend karinderya run out of a home kitchen. Every recipe on this menu has been passed down, tweaked, and taste-tested by three generations — no shortcuts, just patience and a heavy hand with garlic.</p>
        <p class="mb-4">Every dish here is plated the way we'd serve it at our own table: generous, a little rustic, and meant to be shared.</p>
        <div class="d-flex flex-wrap gap-2">
          <span class="badge bg-dark">Homestyle</span>
          <span class="badge bg-dark">Locally Sourced</span>
          <span class="badge bg-dark">Family Recipes</span>
        </div>
      </div>
      <div class="col-12 col-lg-6">
        <img src="asd.jpg" class="img-fluid rounded-4 shadow" alt="Restaurant kitchen team">
      </div>
    </div>
  </div>
</section>

<section id="contact" class="bg-charcoal">
  <div class="container">
    <div class="row">
      <div class="col-12 col-md-8 col-lg-6 mx-auto text-center">
        <span class="ticket">Get in Touch</span>
        <h2 class="mb-3">Visit or Message Us</h2>
        <p class="mb-4">Katapatan Mutual Homes, Brgy. Banay-banay, City of Cabuyao, Laguna &nbsp;·&nbsp; Open daily, 10AM–9PM</p>
        <form class="text-start" onsubmit="return false;">
          <div class="form-floating mb-3">
            <input type="text" class="form-control" id="cName" placeholder="Your name">
            <label for="cName">Your name</label>
          </div>
          <div class="form-floating mb-3">
            <input type="email" class="form-control" id="cEmail" placeholder="you@email.com">
            <label for="cEmail">Email address</label>
          </div>
          <div class="form-floating mb-3">
            <textarea class="form-control" id="cMsg" style="height:100px" placeholder="Message"></textarea>
            <label for="cMsg">Message</label>
          </div>
          <button type="submit" class="btn btn-reserve w-100 rounded-pill py-2">Send Message</button>
        </form>
      </div>
    </div>
  </div>
</section>

<footer class="bg-charcoal border-top border-secondary-subtle py-4">
  <div class="container d-flex flex-column flex-md-row justify-content-between align-items-center gap-3">
    <span class="text-cream" style="color:var(--cream)">&copy; 2026 KAINAN Restaurant &amp; Showcase. All rights reserved.</span>
    <div>
      <a href="#" class="social-icon" data-bs-toggle="tooltip" title="Facebook"><i class="bi bi-facebook"></i></a>
      <a href="#" class="social-icon" data-bs-toggle="tooltip" title="Instagram"><i class="bi bi-instagram"></i></a>
      <a href="#" class="social-icon" data-bs-toggle="tooltip" title="TikTok"><i class="bi bi-tiktok"></i></a>
      <a href="#" class="social-icon" data-bs-toggle="tooltip" title="Call us"><i class="bi bi-telephone-fill"></i></a>
    </div>
  </div>
</footer>

<div class="modal fade" id="dishModal" tabindex="-1" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered modal-lg">
    <div class="modal-content" style="border-radius:14px;overflow:hidden;">
      <div class="modal-header border-0">
        <h5 class="modal-title" id="modalDishTitle">Dish name</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <img id="modalDishImg" src="" alt="" class="w-100" style="max-height:420px;object-fit:cover;">
      <div class="modal-body">
        <p id="modalDishDesc" class="mb-2"></p>
        <span id="modalDishPrice" class="price-tag fs-5"></span>
      </div>
    </div>
  </div>
</div>

<div class="offcanvas offcanvas-end" tabindex="-1" id="reserveCanvas">
  <div class="offcanvas-header">
    <h5 class="offcanvas-title">Reserve a Table</h5>
    <button type="button" class="btn-close" data-bs-dismiss="offcanvas"></button>
  </div>
  <div class="offcanvas-body">
    <form onsubmit="return false;">
      <div class="mb-3">
        <label class="form-label">Full name</label>
        <input type="text" class="form-control">
      </div>
      <div class="mb-3">
        <label class="form-label">Party size</label>
        <select class="form-select">
          <option>1–2 guests</option>
          <option>3–4 guests</option>
          <option>5+ guests</option>
        </select>
      </div>
      <div class="mb-3">
        <label class="form-label">Date &amp; time</label>
        <input type="datetime-local" class="form-control">
      </div>
      <button class="btn btn-reserve w-100 rounded-pill">Confirm Reservation</button>
    </form>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
<script>
  const dishModal = document.getElementById('dishModal');
  dishModal.addEventListener('show.bs.modal', (event) => {
    const trigger = event.relatedTarget;
    document.getElementById('modalDishTitle').textContent = trigger.getAttribute('data-title');
    document.getElementById('modalDishDesc').textContent = trigger.getAttribute('data-desc');
    document.getElementById('modalDishPrice').textContent = trigger.getAttribute('data-price');
    const img = document.getElementById('modalDishImg');
    img.src = trigger.getAttribute('data-img');
    img.alt = trigger.getAttribute('data-title');
  });

  const filterButtons = document.querySelectorAll('.cat-pills .nav-link');
  const dishItems = document.querySelectorAll('.dish-item');
  filterButtons.forEach(btn => {
    btn.addEventListener('click', () => {
      filterButtons.forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      const filter = btn.getAttribute('data-filter');
      dishItems.forEach(item => {
        const match = filter === 'all' || item.getAttribute('data-category') === filter;
        item.style.display = match ? '' : 'none';
      });
    });
  });

  document.querySelectorAll('[data-bs-toggle="tooltip"]').forEach(el => new bootstrap.Tooltip(el));
</script>
</body>
</html>
