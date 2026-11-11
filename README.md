<!DOCTYPE html>
<html lang="en" class="scroll-smooth">

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>SP Creation & Pahari Printers</title>

<script src="https://cdn.tailwindcss.com"></script>

<link rel="preconnect" href="https://fonts.googleapis.com">

<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet">

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>

<script>
tailwind.config = {
  darkMode: 'class',
  theme: {
    extend: {
      fontFamily: {
        sans: ['"Plus Jakarta Sans"', 'sans-serif'],
        serif: ['"Playfair Display"', 'serif']
      },
      colors: {
        brand: {
          gold: '#E5A93C',
          goldLight: '#F5C968',
          goldDark: '#BF8420',
          midnight: '#0B1120',
          slateCard: '#131B2E',
          borderSlate: '#1E293B',
          accentCyan: '#06B6D4'
        }
      }
    }
  }
}
</script>

<style>

body {
  background: #0B1120;
  color: white;
  font-family: "Plus Jakarta Sans", sans-serif;
}

.glass-card {
  background: rgba(15, 23, 42, 0.72);
  backdrop-filter: blur(16px);
  border: 1px solid rgba(229, 169, 60, 0.22);
  box-shadow: 0 10px 30px -10px rgba(0,0,0,0.5);
  transition: 0.3s;
}

.gold-gradient-text {
  background: linear-gradient(
    135deg,
    #FDE68A,
    #E5A93C,
    #B45309
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.tilt-card {
  transform-style: preserve-3d;
  perspective: 1000px;
}

</style>
</head>

<body class="bg-brand-midnight text-white">

<canvas id="webgl-canvas"></canvas>