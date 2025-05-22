/* PHOTOGRAPHY PORTFOLIO COLOR PALETTE */
:root {
    /* Primary Colors - Elegant & Professional */
    --primary-dark: #1a1a1a;           /* Deep charcoal for text */
    --primary-light: #f8f8f8;         /* Off-white background */
    --accent-gold: #d4af37;           /* Luxury gold accent */
    --accent-warm: #c9a96e;           /* Warm gold variation */
    
    /* Neutral Grays - Professional Photography Feel */
    --gray-100: #ffffff;              /* Pure white */
    --gray-200: #f5f5f5;              /* Light gray background */
    --gray-300: #e0e0e0;              /* Border gray */
    --gray-400: #bdbdbd;              /* Medium gray */
    --gray-500: #757575;              /* Text gray */
    --gray-600: #424242;              /* Dark text */
    --gray-700: #212121;              /* Very dark */
    --gray-800: #1a1a1a;              /* Almost black */
    
    /* Alternative Elegant Palette */
    --elegant-cream: #faf7f2;         /* Warm cream */
    --elegant-beige: #e8dcc0;         /* Soft beige */
    --elegant-brown: #8b7355;         /* Warm brown */
    --elegant-dark: #2c2c2c;          /* Sophisticated dark */
    
    /* Overlay & Effects */
    --overlay-dark: rgba(0, 0, 0, 0.7);
    --overlay-light: rgba(255, 255, 255, 0.9);
    --shadow-soft: rgba(0, 0, 0, 0.15);
    --shadow-medium: rgba(0, 0, 0, 0.25);
}

/* HOW TO APPLY TO YOUR EXISTING PORTFOLIO: */

/* 1. Update your existing color variables in your portfolio CSS */
/* Replace these lines in your portfolio's :root section: */

:root {
    /* Replace your current colors with photography theme */
    --primary-gradient-start: #1a1a1a;    /* Dark charcoal */
    --primary-gradient-end: #2c2c2c;      /* Sophisticated dark */
    --accent-gradient-start: #d4af37;     /* Luxury gold */
    --accent-gradient-end: #c9a96e;       /* Warm gold */
    
    /* Background Colors */
    --bg-primary: linear-gradient(135deg, var(--primary-gradient-start) 0%, var(--primary-gradient-end) 100%);
    --bg-accent: linear-gradient(135deg, var(--accent-gradient-start) 0%, var(--accent-gradient-end) 100%);
    --bg-glass: rgba(255, 255, 255, 0.1);
    --bg-white: #faf7f2;                  /* Warm cream instead of pure white */
    --bg-light: #f5f5f5;
    
    /* Text Colors */
    --text-primary: #1a1a1a;              /* Dark charcoal */
    --text-secondary: #424242;            /* Medium dark */
    --text-light: #757575;                /* Medium gray */
    --text-white: #ffffff;
    
    /* Interactive Colors */
    --focus-color: #d4af37;               /* Gold focus */
    --shadow-light: rgba(0, 0, 0, 0.15);
    --shadow-medium: rgba(0, 0, 0, 0.25);
    --shadow-dark: rgba(0, 0, 0, 0.35);
}

/* 2. SPECIFIC PHOTOGRAPHY WEBSITE STYLING */
/* Add these additional styles for photography theme: */

.hero {
    background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), 
                url('your-hero-image.jpg') center/cover;
    color: white;
    min-height: 100vh;
    display: flex;
    align-items: center;
}

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
    padding: 20px 0;
}

.gallery-item {
    position: relative;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 4px 15px var(--shadow-soft);
    transition: transform 0.3s ease;
}

.gallery-item:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 25px var(--shadow-medium);
}

.filter-btn {
    background: var(--gray-200);
    color: var(--gray-600);
    border: 2px solid transparent;
    padding: 8px 20px;
    margin: 0 5px;
    border-radius: 25px;
    transition: all 0.3s ease;
}

.filter-btn.active,
.filter-btn:hover {
    background: var(--accent-gold);
    color: white;
    border-color: var(--accent-gold);
}

.service-card {
    background: var(--gray-100);
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 5px 20px var(--shadow-soft);
    transition: transform 0.3s ease;
}

.service-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 15px 35px var(--shadow-medium);
}

/* 3. ALTERNATIVE COLOR SCHEMES YOU CAN TRY: */

/* Minimalist Black & White */
/*
--primary-gradient-start: #000000;
--primary-gradient-end: #333333;
--accent-gradient-start: #ffffff;
--accent-gradient-end: #f0f0f0;
*/

/* Warm Earth Tones */
/*
--primary-gradient-start: #8b4513;    -- Saddle brown
--primary-gradient-end: #a0522d;      -- Sienna
--accent-gradient-start: #daa520;     -- Goldenrod
--accent-gradient-end: #f4a460;       -- Sandy brown
*/

/* Cool Professional */
/*
--primary-gradient-start: #2c3e50;    -- Dark blue-gray
--primary-gradient-end: #34495e;      -- Blue-gray
--accent-gradient-start: #3498db;     -- Bright blue
--accent-gradient-end: #5dade2;       -- Light blue
*/

/* Vintage Film */
/*
--primary-gradient-start: #5d4037;    -- Brown
--primary-gradient-end: #6d4c41;      -- Dark brown
--accent-gradient-start: #ff8a65;     -- Deep orange
--accent-gradient-end: #ffab91;       -- Light orange
*/