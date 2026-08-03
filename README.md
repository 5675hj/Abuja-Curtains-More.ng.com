
<html lang="en" class="scroll-smooth">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Abuja Curtains & More | Luxury Curtains, Blinds & Window Treatments</title>
  
  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <!-- Lucide Icons -->
  <script src="https://unpkg.com/lucide@latest"></script>
  
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            cream: '#FAF8F5',
            warmBeige: '#F4EFEA',
            softBeige: '#EBE3DB',
            champagneGold: '#D4AF37',
            champagneLight: '#F3E5AB',
            darkCharcoal: '#1A1A1A',
            mutedGray: '#666666'
          },
          fontFamily: {
            serif: ['Playfair Display', 'serif'],
            sans: ['Poppins', 'sans-serif'],
          }
        }
      }
    }
  </script>

  <style>
    /* Glassmorphism Styles */
    .glass-card {
      background: rgba(255, 255, 255, 0.65);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border: 1px solid rgba(212, 175, 55, 0.18);
    }
    
    .glass-card-hover {
      transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
    }
    
    .glass-card-hover:hover {
      transform: translateY(-6px);
      background: rgba(255, 255, 255, 0.85);
      border-color: rgba(212, 175, 55, 0.4);
      box-shadow: 0 20px 40px -15px rgba(212, 175, 55, 0.15);
    }

    .hero-overlay {
      background: linear-gradient(180deg, rgba(26,26,26,0.4) 0%, rgba(250,248,245,0.95) 90%, #FAF8F5 100%);
    }

    /* Custom Scrollbar */
    ::-webkit-scrollbar {
      width: 8px;
    }
    ::-webkit-scrollbar-track {
      background: #FAF8F5;
    }
    ::-webkit-scrollbar-thumb {
      background: #D4AF37;
      border-radius: 4px;
    }

    /* Animation utility */
    .fade-in-section {
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.8s ease-out, transform 0.8s ease-out;
      will-change: opacity, transform;
    }
    .fade-in-section.is-visible {
      opacity: 1;
      transform: none;
    }
  </style>
</head>
<body class="bg-cream text-darkCharcoal font-sans antialiased selection:bg-champagneGold selection:text-white">

  <!-- Floating WhatsApp Button -->
  <a href="https://wa.me/2349086543309" target="_blank" rel="noopener noreferrer" class="fixed bottom-6 right-6 z-50 bg-[#25D366] text-white p-4 rounded-full shadow-2xl hover:scale-110 transition-transform duration-300 flex items-center justify-center group" aria-label="Chat on WhatsApp">
    <i data-lucide="message-circle" class="w-6 h-6"></i>
    <span class="max-w-0 overflow-hidden whitespace-nowrap group-hover:max-w-xs transition-all duration-500 ease-in-out ease-out font-medium text-sm pl-0 group-hover:pl-2">Chat with Us</span>
  </a>

  <!-- Header / Sticky Navigation -->
  <header id="navbar" class="fixed top-0 left-0 w-full z-40 transition-all duration-300">
    <div class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
      <a href="#" class="flex flex-col">
        <span class="font-serif text-xl md:text-2xl font-bold tracking-wider text-darkCharcoal">ABUJA CURTAINS</span>
        <span class="text-[10px] tracking-[0.3em] uppercase text-champagneGold font-semibold -mt-1">& More</span>
      </a>

      <!-- Desktop Nav -->
      <nav class="hidden md:flex items-center space-x-8 text-sm font-medium">
        <a href="#about" class="hover:text-champagneGold transition-colors">About Us</a>
        <a href="#why-us" class="hover:text-champagneGold transition-colors">Why Choose Us</a>
        <a href="#services" class="hover:text-champagneGold transition-colors">Services</a>
        <a href="#gallery" class="hover:text-champagneGold transition-colors">Gallery</a>
        <a href="#process" class="hover:text-champagneGold transition-colors">Process</a>
        <a href="#contact" class="hover:text-champagneGold transition-colors">Contact</a>
      </nav>

      <div class="hidden md:block">
        <a href="#contact" class="px-6 py-2.5 rounded-full border border-champagneGold text-darkCharcoal hover:bg-champagneGold hover:text-white transition-all duration-300 text-sm font-medium">
          Book Consultation
        </a>
      </div>

      <!-- Mobile Menu Button -->
      <button id="mobile-menu-btn" class="md:hidden text-darkCharcoal focus:outline-none">
        <i data-lucide="menu" class="w-7 h-7"></i>
      </button>
    </div>

    <!-- Mobile Navigation Drawer -->
    <div id="mobile-menu" class="hidden md:hidden bg-cream/95 backdrop-blur-md border-b border-champagneGold/20 px-6 py-6 transition-all">
      <nav class="flex flex-col space-y-4 text-base font-medium">
        <a href="#about" class="mobile-link">About Us</a>
        <a href="#why-us" class="mobile-link">Why Choose Us</a>
        <a href="#services" class="mobile-link">Services</a>
        <a href="#gallery" class="mobile-link">Gallery</a>
        <a href="#process" class="mobile-link">Process</a>
        <a href="#contact" class="mobile-link">Contact</a>
        <a href="#contact" class="inline-block text-center mt-2 px-6 py-3 rounded-full bg-champagneGold text-white font-medium">
          Book Consultation
        </a>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="relative min-h-screen flex items-center justify-center pt-24 pb-16 overflow-hidden">
    <!-- Hero Background Image -->
    <div class="absolute inset-0 z-0">
      <img src="https://i.ibb.co/LzgbJHxZ/Screenshot-20260803-144452-Whats-App-Business.jpg" alt="Luxury Living Room Window Treatments" class="w-full h-full object-cover object-center scale-105 animate-pulse" style="animation-duration: 10s;" />
      <div class="absolute inset-0 hero-overlay"></div>
    </div>

    <div class="relative z-10 max-w-5xl mx-auto px-6 text-center mt-12 fade-in-section">
      <span class="inline-block text-xs md:text-sm uppercase tracking-[0.4em] font-semibold text-champagneGold mb-4 px-4 py-1.5 rounded-full border border-champagneGold/30 bg-white/40 backdrop-blur-sm">
        Exquisite Window Styling
      </span>
      <h1 class="font-serif text-4xl md:text-6xl lg:text-7xl font-bold leading-tight text-darkCharcoal mb-6">
        Luxury Curtains & Window Treatments Designed for Elegant Living
      </h1>
      <p class="text-base md:text-lg text-mutedGray max-w-3xl mx-auto mb-10 leading-relaxed">
        Transform your home, office or hospitality space with expertly crafted curtains, blinds and window treatments. Abuja Curtains & More combines premium fabrics, flawless installation and timeless designs to create interiors that feel luxurious, comfortable and sophisticated.
      </p>
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <a href="#contact" class="w-full sm:w-auto px-8 py-4 rounded-full bg-champagneGold text-white font-medium hover:bg-amber-600 transition-all duration-300 shadow-lg shadow-champagneGold/20 hover:shadow-xl">
          Book a Consultation
        </a>
        <a href="#gallery" class="w-full sm:w-auto px-8 py-4 rounded-full border border-darkCharcoal/30 text-darkCharcoal bg-white/30 backdrop-blur-sm font-medium hover:bg-darkCharcoal hover:text-white transition-all duration-300">
          View Projects
        </a>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="py-24 bg-cream fade-in-section">
    <div class="max-w-7xl mx-auto px-6 grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
      <div class="lg:col-span-6 space-y-6">
        <div class="inline-block border-b-2 border-champagneGold pb-1">
          <span class="text-xs uppercase tracking-[0.3em] font-semibold text-champagneGold">Our Heritage</span>
        </div>
        <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl font-bold text-darkCharcoal">
          Bringing Luxury Into Every Window
        </h2>
        <p class="text-mutedGray leading-relaxed">
          At Abuja Curtains & More, we specialize in creating beautiful living and working spaces through premium window treatments. From luxurious curtains and modern blinds to complete window styling, every project is designed to enhance the beauty, comfort and value of your property.
        </p>
        <p class="text-mutedGray leading-relaxed">
          Our team works closely with homeowners, architects, interior designers, hotels and corporate offices to deliver customized window solutions that perfectly match each space.
        </p>
        <p class="text-mutedGray leading-relaxed">
          Whether you're furnishing a new home, renovating your office or upgrading a luxury apartment, we ensure every installation reflects elegance, quality and attention to detail. We believe curtains are more than window coverings—they define the atmosphere of a room, improve privacy, control natural lighting and complete the overall interior design.
        </p>
      </div>

      <div class="lg:col-span-6 relative">
        <div class="relative rounded-2xl overflow-hidden shadow-2xl">
          <img src="https://i.ibb.co/JWnrW2Q1/Screenshot-20260803-143741-Instagram.jpg" alt="Tailored Luxury Drapes" class="w-full h-[500px] object-cover hover:scale-105 transition-transform duration-700" />
        </div>
        <!-- Accent Glass Box -->
        <div class="absolute -bottom-6 -left-6 glass-card p-6 rounded-2xl hidden sm:block max-w-xs">
          <div class="flex items-center gap-4">
            <div class="p-3 bg-champagneGold/20 rounded-full text-champagneGold">
              <i data-lucide="sparkles" class="w-6 h-6"></i>
            </div>
            <div>
              <p class="font-serif font-bold text-darkCharcoal text-lg">Flawless Finish</p>
              <p class="text-xs text-mutedGray">Crafted with precision & care</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Why Choose Us Section -->
  <section id="why-us" class="py-24 bg-warmBeige/60 fade-in-section">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs uppercase tracking-[0.3em] font-semibold text-champagneGold">The Difference</span>
        <h2 class="font-serif text-3xl md:text-5xl font-bold text-darkCharcoal mt-2">Why Choose Us</h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Feature 1 -->
        <div class="glass-card p-8 rounded-2xl glass-card-hover">
          <div class="w-12 h-12 rounded-xl bg-champagneGold/15 flex items-center justify-center text-champagneGold mb-6">
            <i data-lucide="gem" class="w-6 h-6"></i>
          </div>
          <h3 class="font-serif text-xl font-bold mb-3">Premium Fabrics</h3>
          <p class="text-sm text-mutedGray leading-relaxed">Carefully selected high-quality materials available in elegant textures, colours and finishes.</p>
        </div>

        <!-- Feature 2 -->
        <div class="glass-card p-8 rounded-2xl glass-card-hover">
          <div class="w-12 h-12 rounded-xl bg-champagneGold/15 flex items-center justify-center text-champagneGold mb-6">
            <i data-lucide="pen-tool" class="w-6 h-6"></i>
          </div>
          <h3 class="font-serif text-xl font-bold mb-3">Custom Designs</h3>
          <p class="text-sm text-mutedGray leading-relaxed">Every curtain and blind is tailored specifically for your space and interior style.</p>
        </div>

        <!-- Feature 3 -->
        <div class="glass-card p-8 rounded-2xl glass-card-hover">
          <div class="w-12 h-12 rounded-xl bg-champagneGold/15 flex items-center justify-center text-champagneGold mb-6">
            <i data-lucide="check-circle-2" class="w-6 h-6"></i>
          </div>
          <h3 class="font-serif text-xl font-bold mb-3">Professional Installation</h3>
          <p class="text-sm text-mutedGray leading-relaxed">Neat, precise and flawless installation carried out by experienced professionals.</p>
        </div>

        <!-- Feature 4 -->
        <div class="glass-card p-8 rounded-2xl glass-card-hover">
          <div class="w-12 h-12 rounded-xl bg-champagneGold/15 flex items-center justify-center text-champagneGold mb-6">
            <i data-lucide="award" class="w-6 h-6"></i>
          </div>
          <h3 class="font-serif text-xl font-bold mb-3">Trusted Experience</h3>
          <p class="text-sm text-mutedGray leading-relaxed">Serving homeowners, luxury apartments, hotels, offices and commercial spaces across Abuja and beyond.</p>
        </div>

        <!-- Feature 5 -->
        <div class="glass-card p-8 rounded-2xl glass-card-hover">
          <div class="w-12 h-12 rounded-xl bg-champagneGold/15 flex items-center justify-center text-champagneGold mb-6">
            <i data-lucide="sliders" class="w-6 h-6"></i>
          </div>
          <h3 class="font-serif text-xl font-bold mb-3">Elegant Finishing</h3>
          <p class="text-sm text-mutedGray leading-relaxed">Attention to every detail ensures a refined and luxurious appearance.</p>
        </div>

        <!-- Feature 6 -->
        <div class="glass-card p-8 rounded-2xl glass-card-hover">
          <div class="w-12 h-12 rounded-xl bg-champagneGold/15 flex items-center justify-center text-champagneGold mb-6">
            <i data-lucide="user-check" class="w-6 h-6"></i>
          </div>
          <h3 class="font-serif text-xl font-bold mb-3">Consultation</h3>
          <p class="text-sm text-mutedGray leading-relaxed">Professional advice to help clients choose the perfect fabrics, colours and window treatment solutions.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section id="services" class="py-24 bg-cream fade-in-section">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs uppercase tracking-[0.3em] font-semibold text-champagneGold">Bespoke Offerings</span>
        <h2 class="font-serif text-3xl md:text-5xl font-bold text-darkCharcoal mt-2">Our Premium Services</h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Service Card 1 -->
        <div class="glass-card rounded-2xl p-8 glass-card-hover border-t-2 border-t-champagneGold/60">
          <div class="mb-4 text-champagneGold"><i data-lucide="layers" class="w-8 h-8"></i></div>
          <h3 class="font-serif text-2xl font-bold mb-3">Luxury Curtains</h3>
          <p class="text-mutedGray text-sm leading-relaxed">Beautiful custom-made curtains designed to elevate every room with elegant fabrics and tailored lengths.</p>
        </div>

        <!-- Service Card 2 -->
        <div class="glass-card rounded-2xl p-8 glass-card-hover border-t-2 border-t-champagneGold/60">
          <div class="mb-4 text-champagneGold"><i data-lucide="grid" class="w-8 h-8"></i></div>
          <h3 class="font-serif text-2xl font-bold mb-3">Modern Blinds</h3>
          <p class="text-mutedGray text-sm leading-relaxed">Elegant blinds combining style, functionality and privacy control for modern spaces.</p>
        </div>

        <!-- Service Card 3 -->
        <div class="glass-card rounded-2xl p-8 glass-card-hover border-t-2 border-t-champagneGold/60">
          <div class="mb-4 text-champagneGold"><i data-lucide="layout" class="w-8 h-8"></i></div>
          <h3 class="font-serif text-2xl font-bold mb-3">Window Treatment</h3>
          <p class="text-mutedGray text-sm leading-relaxed">Complete window styling solutions for homes and businesses tailored to complement your architecture.</p>
        </div>

        <!-- Service Card 4 -->
        <div class="glass-card rounded-2xl p-8 glass-card-hover border-t-2 border-t-champagneGold/60">
          <div class="mb-4 text-champagneGold"><i data-lucide="home" class="w-8 h-8"></i></div>
          <h3 class="font-serif text-2xl font-bold mb-3">Residential Installation</h3>
          <p class="text-mutedGray text-sm leading-relaxed">Luxury curtain installation for apartments, duplexes, estates, and private villas.</p>
        </div>

        <!-- Service Card 5 -->
        <div class="glass-card rounded-2xl p-8 glass-card-hover border-t-2 border-t-champagneGold/60">
          <div class="mb-4 text-champagneGold"><i data-lucide="building-2" class="w-8 h-8"></i></div>
          <h3 class="font-serif text-2xl font-bold mb-3">Commercial Projects</h3>
          <p class="text-mutedGray text-sm leading-relaxed">Curtain and blind solutions designed for hotels, corporate offices, restaurants and commercial buildings.</p>
        </div>

        <!-- Service Card 6 -->
        <div class="glass-card rounded-2xl p-8 glass-card-hover border-t-2 border-t-champagneGold/60">
          <div class="mb-4 text-champagneGold"><i data-lucide="palette" class="w-8 h-8"></i></div>
          <h3 class="font-serif text-2xl font-bold mb-3">Interior Consultation</h3>
          <p class="text-mutedGray text-sm leading-relaxed">Helping clients select colours, fabrics and overall window designs that complement their interiors.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Luxury Gallery -->
  <section id="gallery" class="py-24 bg-warmBeige/40 fade-in-section">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs uppercase tracking-[0.3em] font-semibold text-champagneGold">Portfolio</span>
        <h2 class="font-serif text-3xl md:text-5xl font-bold text-darkCharcoal mt-2">Luxury Gallery</h2>
      </div>

      <!-- Grid Gallery -->
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Item 1 -->
        <div class="group relative overflow-hidden rounded-2xl shadow-md cursor-pointer">
          <img src="https://i.ibb.co/LzgbJHxZ/Screenshot-20260803-144452-Whats-App-Business.jpg" alt="Luxury Living Room" class="w-full h-80 object-cover group-hover:scale-110 transition-transform duration-700" />
          <div class="absolute inset-0 bg-gradient-to-t from-darkCharcoal/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end p-6">
            <span class="font-serif text-xl font-bold text-white">Luxury Living Room</span>
          </div>
        </div>

        <!-- Item 2 -->
        <div class="group relative overflow-hidden rounded-2xl shadow-md cursor-pointer">
          <img src="https://i.ibb.co/rGzpcGFs/Screenshot-20260803-143735-Instagram.jpg" alt="Modern Sheer Curtains" class="w-full h-80 object-cover group-hover:scale-110 transition-transform duration-700" />
          <div class="absolute inset-0 bg-gradient-to-t from-darkCharcoal/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end p-6">
            <span class="font-serif text-xl font-bold text-white">Modern Sheer Curtains</span>
          </div>
        </div>

        <!-- Item 3 -->
        <div class="group relative overflow-hidden rounded-2xl shadow-md cursor-pointer">
          <img src="https://i.ibb.co/JWnrW2Q1/Screenshot-20260803-143741-Instagram.jpg" alt="Premium Fabric Collection" class="w-full h-80 object-cover group-hover:scale-110 transition-transform duration-700" />
          <div class="absolute inset-0 bg-gradient-to-t from-darkCharcoal/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end p-6">
            <span class="font-serif text-xl font-bold text-white">Premium Fabric Collection</span>
          </div>
        </div>

        <!-- Item 4 -->
        <div class="group relative overflow-hidden rounded-2xl shadow-md cursor-pointer">
          <img src="https://i.ibb.co/dJwjH0xT/Screenshot-20260803-143748-Instagram.jpg" alt="Office Installation" class="w-full h-80 object-cover group-hover:scale-110 transition-transform duration-700" />
          <div class="absolute inset-0 bg-gradient-to-t from-darkCharcoal/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end p-6">
            <span class="font-serif text-xl font-bold text-white">Office Installation</span>
          </div>
        </div>

        <!-- Item 5 -->
        <div class="group relative overflow-hidden rounded-2xl shadow-md cursor-pointer">
          <img src="https://i.ibb.co/nq1Kv5Y8/Screenshot-20260803-143752-Instagram.jpg" alt="Hotel Interior" class="w-full h-80 object-cover group-hover:scale-110 transition-transform duration-700" />
          <div class="absolute inset-0 bg-gradient-to-t from-darkCharcoal/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end p-6">
            <span class="font-serif text-xl font-bold text-white">Hotel Interior</span>
          </div>
        </div>

        <!-- Item 6 -->
        <div class="group relative overflow-hidden rounded-2xl shadow-md cursor-pointer">
          <img src="https://i.ibb.co/tS4whkz/Screenshot-20260803-143757-Instagram.jpg" alt="Elegant Window Design" class="w-full h-80 object-cover group-hover:scale-110 transition-transform duration-700" />
          <div class="absolute inset-0 bg-gradient-to-t from-darkCharcoal/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end p-6">
            <span class="font-serif text-xl font-bold text-white">Elegant Window Design</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Process Section -->
  <section id="process" class="py-24 bg-cream fade-in-section">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs uppercase tracking-[0.3em] font-semibold text-champagneGold">Seamless Journey</span>
        <h2 class="font-serif text-3xl md:text-5xl font-bold text-darkCharcoal mt-2">Our Process</h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
        <!-- Step 1 -->
        <div class="glass-card p-8 rounded-2xl text-center relative border border-champagneGold/20">
          <div class="w-12 h-12 mx-auto rounded-full bg-champagneGold text-white font-serif text-xl font-bold flex items-center justify-center mb-6 shadow-md">1</div>
          <h3 class="font-serif text-xl font-bold mb-3">Book a Consultation</h3>
          <p class="text-xs text-mutedGray leading-relaxed">Tell us about your project, window dimensions, and design requirements.</p>
        </div>

        <!-- Step 2 -->
        <div class="glass-card p-8 rounded-2xl text-center relative border border-champagneGold/20">
          <div class="w-12 h-12 mx-auto rounded-full bg-champagneGold text-white font-serif text-xl font-bold flex items-center justify-center mb-6 shadow-md">2</div>
          <h3 class="font-serif text-xl font-bold mb-3">Choose Your Design</h3>
          <p class="text-xs text-mutedGray leading-relaxed">Select fabrics, textures, colours, and window styles with our expert guidance.</p>
        </div>

        <!-- Step 3 -->
        <div class="glass-card p-8 rounded-2xl text-center relative border border-champagneGold/20">
          <div class="w-12 h-12 mx-auto rounded-full bg-champagneGold text-white font-serif text-xl font-bold flex items-center justify-center mb-6 shadow-md">3</div>
          <h3 class="font-serif text-xl font-bold mb-3">Professional Installation</h3>
          <p class="text-xs text-mutedGray leading-relaxed">Our experienced team installs everything with precision and utmost care.</p>
        </div>

        <!-- Step 4 -->
        <div class="glass-card p-8 rounded-2xl text-center relative border border-champagneGold/20">
          <div class="w-12 h-12 mx-auto rounded-full bg-champagneGold text-white font-serif text-xl font-bold flex items-center justify-center mb-6 shadow-md">4</div>
          <h3 class="font-serif text-xl font-bold mb-3">Enjoy Your New Space</h3>
          <p class="text-xs text-mutedGray leading-relaxed">Experience beautiful, elegant, and functional interiors customized for you.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonials Section -->
  <section class="py-24 bg-warmBeige/50 fade-in-section">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs uppercase tracking-[0.3em] font-semibold text-champagneGold">Client Satisfaction</span>
        <h2 class="font-serif text-3xl md:text-5xl font-bold text-darkCharcoal mt-2">What Our Clients Say</h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Testimonial 1 -->
        <div class="glass-card p-8 rounded-2xl relative">
          <div class="flex text-champagneGold mb-4">
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
          </div>
          <p class="text-sm italic text-mutedGray leading-relaxed mb-6">"Our living room feels completely transformed. The quality and finishing exceeded our expectations."</p>
          <div class="text-xs font-semibold text-darkCharcoal">Private Residence • Maitama, Abuja</div>
        </div>

        <!-- Testimonial 2 -->
        <div class="glass-card p-8 rounded-2xl relative">
          <div class="flex text-champagneGold mb-4">
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
          </div>
          <p class="text-sm italic text-mutedGray leading-relaxed mb-6">"The installation was professional, neat and completed on schedule. Truly exceptional work."</p>
          <div class="text-xs font-semibold text-darkCharcoal">Corporate Suite • Central Business District, Abuja</div>
        </div>

        <!-- Testimonial 3 -->
        <div class="glass-card p-8 rounded-2xl relative">
          <div class="flex text-champagneGold mb-4">
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
            <i data-lucide="star" class="w-4 h-4 fill-current"></i>
          </div>
          <p class="text-sm italic text-mutedGray leading-relaxed mb-6">"Excellent customer service and beautiful curtain designs. Highly recommended for luxury projects."</p>
          <div class="text-xs font-semibold text-darkCharcoal">Boutique Hotel • Guzape, Abuja</div>
        </div>
      </div>
    </div>
  </section>

  <!-- CEO / Founder Section -->
  <section class="py-24 bg-cream fade-in-section">
    <div class="max-w-5xl mx-auto px-6">
      <div class="glass-card rounded-3xl p-8 md:p-12 border border-champagneGold/20 shadow-xl flex flex-col md:flex-row items-center gap-10">
        <div class="w-48 h-48 md:w-64 md:h-64 rounded-full overflow-hidden flex-shrink-0 border-4 border-white shadow-lg">
          <img src="https://ibb.co/YBccc5kQ" alt="Founder of Abuja Curtains & More" class="w-full h-full object-cover" />
        </div>
        <div class="space-y-4 text-center md:text-left">
          <span class="text-xs uppercase tracking-[0.3em] font-semibold text-champagneGold">Leadership</span>
          <h2 class="font-serif text-3xl md:text-4xl font-bold text-darkCharcoal">Meet Our Founder</h2>
          <p class="text-sm text-mutedGray leading-relaxed">
            Driven by a passion for elegant interiors and customer satisfaction, the founder of Abuja Curtains & More has built a trusted brand known for quality craftsmanship, premium materials and exceptional service.
          </p>
          <p class="text-sm text-mutedGray leading-relaxed">
            Every project is approached with professionalism, creativity and attention to detail, ensuring clients receive window treatment solutions that combine beauty, durability and functionality.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="py-24 bg-warmBeige/60 fade-in-section">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs uppercase tracking-[0.3em] font-semibold text-champagneGold">Get In Touch</span>
        <h2 class="font-serif text-3xl md:text-5xl font-bold text-darkCharcoal mt-2">Connect With Us</h2>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
        <!-- Contact Details -->
        <div class="lg:col-span-6 space-y-8">
          <div class="glass-card p-8 rounded-2xl space-y-6">
            <h3 class="font-serif text-2xl font-bold text-darkCharcoal mb-4">Abuja Curtains & More</h3>
            
            <div class="flex items-center space-x-4 text-mutedGray">
              <div class="w-10 h-10 rounded-full bg-champagneGold/10 flex items-center justify-center text-champagneGold">
                <i data-lucide="phone" class="w-5 h-5"></i>
              </div>
              <div>
                <p class="text-xs text-mutedGray uppercase tracking-wider">Phone</p>
                <a href="tel:+2349086543309" class="font-medium text-darkCharcoal hover:text-champagneGold transition-colors">+234 908 654 3309</a>
              </div>
            </div>

            <div class="flex items-center space-x-4 text-mutedGray">
              <div class="w-10 h-10 rounded-full bg-champagneGold/10 flex items-center justify-center text-champagneGold">
                <i data-lucide="message-circle" class="w-5 h-5"></i>
              </div>
              <div>
                <p class="text-xs text-mutedGray uppercase tracking-wider">WhatsApp</p>
                <a href="https://wa.me/2349086543309" target="_blank" rel="noopener noreferrer" class="font-medium text-darkCharcoal hover:text-champagneGold transition-colors">+234 908 654 3309</a>
              </div>
            </div>

            <div class="flex items-center space-x-4 text-mutedGray">
              <div class="w-10 h-10 rounded-full bg-champagneGold/10 flex items-center justify-center text-champagneGold">
                <i data-lucide="mail" class="w-5 h-5"></i>
              </div>
              <div>
                <p class="text-xs text-mutedGray uppercase tracking-wider">Email</p>
                <a href="mailto:abujacurtainsmore@gmail.com" class="font-medium text-darkCharcoal hover:text-champagneGold transition-colors">abujacurtainsmore@gmail.com</a>
              </div>
            </div>

            <div class="flex items-center space-x-4 text-mutedGray">
              <div class="w-10 h-10 rounded-full bg-champagneGold/10 flex items-center justify-center text-champagneGold">
                <i data-lucide="map-pin" class="w-5 h-5"></i>
              </div>
              <div>
                <p class="text-xs text-mutedGray uppercase tracking-wider">Location</p>
                <p class="font-medium text-darkCharcoal">Abuja, Nigeria</p>
              </div>
            </div>
          </div>

          <!-- Quick Action Buttons -->
          <div class="flex flex-col sm:flex-row gap-4">
            <a href="tel:+2349086543309" class="flex-1 py-3.5 px-6 rounded-full bg-darkCharcoal text-white font-medium text-center hover:bg-black transition-colors">
              Call Now
            </a>
            <a href="https://wa.me/2349086543309" target="_blank" rel="noopener noreferrer" class="flex-1 py-3.5 px-6 rounded-full bg-[#25D366] text-white font-medium text-center hover:bg-emerald-600 transition-colors">
              Chat on WhatsApp
            </a>
          </div>
        </div>

        <!-- Interactive Consultation Form Card -->
        <div class="lg:col-span-6">
          <div class="glass-card p-8 md:p-10 rounded-3xl border border-champagneGold/30">
            <h3 class="font-serif text-2xl font-bold mb-2">Book Consultation</h3>
            <p class="text-xs text-mutedGray mb-6">Fill in your details below to schedule an expert window styling assessment.</p>

            <form onsubmit="event.preventDefault(); alert('Thank you for requesting a consultation. Our team will contact you shortly!');" class="space-y-4">
              <div>
                <label class="block text-xs font-semibold uppercase text-mutedGray mb-1">Your Name</label>
                <input type="text" placeholder="Full Name" required class="w-full px-4 py-3 rounded-xl bg-white/60 border border-champagneGold/20 focus:outline-none focus:border-champagneGold text-sm transition-all" />
              </div>
              <div>
                <label class="block text-xs font-semibold uppercase text-mutedGray mb-1">Phone / WhatsApp Number</label>
                <input type="tel" placeholder="+234..." required class="w-full px-4 py-3 rounded-xl bg-white/60 border border-champagneGold/20 focus:outline-none focus:border-champagneGold text-sm transition-all" />
              </div>
              <div>
                <label class="block text-xs font-semibold uppercase text-mutedGray mb-1">Project Type</label>
                <select class="w-full px-4 py-3 rounded-xl bg-white/60 border border-champagneGold/20 focus:outline-none focus:border-champagneGold text-sm transition-all text-darkCharcoal">
                  <option>Residential Space</option>
                  <option>Commercial Office</option>
                  <option>Hotel / Hospitality</option>
                  <option>Consultation & Design Selection</option>
                </select>
              </div>
              <button type="submit" class="w-full py-4 rounded-full bg-champagneGold text-white font-medium hover:bg-amber-600 transition-all shadow-md">
                Book Consultation
              </button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer Section -->
  <footer class="bg-darkCharcoal text-white py-16">
    <div class="max-w-7xl mx-auto px-6 text-center space-y-6">
      <a href="#" class="inline-block">
        <span class="font-serif text-2xl md:text-3xl font-bold tracking-wider text-white">ABUJA CURTAINS</span>
        <span class="block text-xs tracking-[0.4em] uppercase text-champagneGold font-semibold -mt-1">& More</span>
      </a>

      <p class="text-sm text-gray-400">Luxury Curtains • Blinds • Window Treatments</p>
      <p class="text-xs text-gray-500">Serving Abuja and clients across Nigeria.</p>

      <div class="pt-8 border-t border-gray-800 text-xs text-gray-500">
        &copy; <script>document.write(new Date().getFullYear())</script> Abuja Curtains & More. All rights reserved.
      </div>
    </div>
  </footer>

  <!-- Lucide Icons initialization & Custom JS -->
  <script>
    // Initialize icons
    lucide.createIcons();

    // Mobile Navbar Toggle
    const mobileMenuBtn = document.getElementById('mobile-menu-btn');
    const mobileMenu = document.getElementById('mobile-menu');
    const mobileLinks = document.querySelectorAll('.mobile-link');

    mobileMenuBtn.addEventListener('click', () => {
      mobileMenu.classList.toggle('hidden');
    });

    mobileLinks.forEach(link => {
      link.addEventListener('click', () => {
        mobileMenu.classList.add('hidden');
      });
    });

    // Header background change on scroll
    const navbar = document.getElementById('navbar');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 50) {
        navbar.classList.add('bg-cream/90', 'backdrop-blur-md', 'shadow-sm', 'py-3');
        navbar.classList.remove('py-4');
      } else {
        navbar.classList.remove('bg-cream/90', 'backdrop-blur-md', 'shadow-sm', 'py-3');
        navbar.classList.add('py-4');
      }
    });

    // Intersection Observer for Smooth Fade-In Animations
    const observerOptions = {
      root: null,
      rootMargin: '0px',
      threshold: 0.15
    };

    const observer = new IntersectionObserver((entries, observer) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('is-visible');
        }
      });
    }, observerOptions);

    document.querySelectorAll('.fade-in-section').forEach(section => {
      observer.observe(section);
    });
  </script>
</body>
</html>
