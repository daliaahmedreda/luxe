# LUXE — مستحضرات تجميل فاخرة

Premium cosmetics e-commerce website with glassmorphism design, bilingual support (Arabic/English), and Supabase integration ready.

## Features

- **16 Products** across categories: Skincare, Makeup, Hair Care, Oils & Perfumes, Professional/Clinic
- **Product Images** from Unsplash with CSS fallback placeholders
- **Product Detail Modal** with gallery, ingredients, usage instructions
- **Shopping Cart** sidebar with quantity controls and WhatsApp checkout
- **Category Filters** and search functionality
- **Bilingual** full Arabic/English support with one-click toggle
- **Glassmorphism Design** with luxury color palette
- **WhatsApp Floating Button** with multiple quick-action options
- **Testimonials** and skincare tips sections
- **Responsive** for mobile, tablet, and desktop
- **Supabase Ready** — see integration notes in code

## Quick Start

1. Open `index.html` in any modern browser
2. No build step or server required

## Customization

### Change Products
Edit the `products` array in the `<script>` section. Each product has:
```js
{
  id: 1,
  nameEn: 'English Name',
  nameAr: 'الاسم العربي',
  descEn: 'English description',
  descAr: 'الوصف العربي',
  price: 1890,           // Price in EGP
  category: 'skincare',  // skincare|makeup|hair|perfume|clinic
  images: ['url1', 'url2'],
  forClinics: false       // true = professional/clinic product
}
```

### Change WhatsApp Number
Current number: `201023116065` (01023116065). Replace in all `wa.me/` links if needed.

### Change Colors
Edit CSS variables in `:root`:
- `--cream` — background
- `--rose-gold` — primary accent
- `--gold` — secondary accent
- `--soft-brown` — text color

## Supabase Integration

1. Create project at [supabase.com](https://supabase.com)
2. Add `<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>`
3. Init: `const sb = supabase.createClient('YOUR_URL','YOUR_ANON_KEY');`
4. Replace static `products` array with async fetch

## Deploy to Vercel

1. Push to GitHub
2. Import repository in Vercel
3. Framework: "Other" / "Static"
4. Deploy

## Tech Stack

- Vanilla HTML/CSS/JS (no frameworks)
- Google Fonts (Inter, Noto Sans Arabic, Playfair Display)
- Font Awesome 6.5 icons
- Unsplash product images
