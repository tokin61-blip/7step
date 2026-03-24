<!DOCTYPE html>
<html lang="ru" data-theme="dark">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>7 шагов к изобилию — Александр Токин</title>
<meta name="description" content="3 месяца совместной работы по проверенному алгоритму — и у вас есть бизнес, блог и первые клиенты. Или возврат денег без вопросов.">
<meta property="og:title" content="7 шагов к изобилию — Александр Токин">
<meta property="og:description" content="Для экспертов и предпринимателей, которые делали всё правильно — но не в том порядке.">
<meta property="og:type" content="website">

<!-- Google Fonts -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;0,700;1,400;1,600&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
/* ===== DESIGN TOKENS ===== */
:root {
  /* Gold / Silver Palette */
  --gold-bright:    #FFD700;
  --gold-warm:      #E8B84B;
  --gold-deep:      #C8960C;
  --gold-muted:     #A87832;
  --silver-bright:  #E8E8F0;
  --silver-mid:     #C0C4D0;
  --silver-muted:   #8A8FA0;
  --silver-dark:    #5A5F70;

  /* Base dark palette — black stays */
  --black-pure:     #000000;
  --black-rich:     #0A0A0C;
  --black-deep:     #0F0F14;
  --black-surface:  #141418;
  --black-card:     #1A1A22;
  --black-elevated: #20202A;
  --black-border:   #2A2A38;
  --black-separator:#333345;

  /* Text */
  --text-primary:   #F0EEE8;
  --text-secondary: #B8B4A8;
  --text-muted:     #6A6860;
  --text-inverse:   #0A0A0C;

  /* Gradient accents */
  --grad-gold:      linear-gradient(135deg, #FFD700 0%, #E8B84B 40%, #C8960C 70%, #FFD700 100%);
  --grad-silver:    linear-gradient(135deg, #E8E8F0 0%, #C0C4D0 40%, #8A8FA0 70%, #E8E8F0 100%);
  --grad-gold-silver: linear-gradient(135deg, #FFD700 0%, #C0C4D0 50%, #E8B84B 100%);
  --grad-hero-bg:   radial-gradient(ellipse at top, #1A1A26 0%, #0A0A0C 60%);
  --grad-section:   linear-gradient(180deg, #0F0F14 0%, #141418 100%);
  --grad-cta:       linear-gradient(135deg, #C8960C 0%, #FFD700 50%, #E8B84B 100%);

  /* Type Scale */
  --text-xs:   clamp(0.75rem,  0.7rem  + 0.25vw, 0.875rem);
  --text-sm:   clamp(0.875rem, 0.8rem  + 0.35vw, 1rem);
  --text-base: clamp(1rem,     0.95rem + 0.25vw, 1.125rem);
  --text-lg:   clamp(1.125rem, 1rem    + 0.75vw, 1.5rem);
  --text-xl:   clamp(1.5rem,   1.2rem  + 1.25vw, 2.25rem);
  --text-2xl:  clamp(2rem,     1.2rem  + 2.5vw,  3.5rem);
  --text-3xl:  clamp(2.5rem,   1rem    + 4vw,    5rem);
  --text-hero: clamp(2.8rem,   0.5rem  + 7vw,    7rem);

  /* Spacing */
  --s1: 0.25rem; --s2: 0.5rem; --s3: 0.75rem; --s4: 1rem;
  --s5: 1.25rem; --s6: 1.5rem; --s8: 2rem;    --s10: 2.5rem;
  --s12: 3rem;   --s16: 4rem;  --s20: 5rem;   --s24: 6rem;

  /* Fonts */
  --font-display: 'Cormorant Garamond', Georgia, serif;
  --font-body:    'Inter', system-ui, sans-serif;

  /* Radius */
  --r-sm: 0.5rem;  --r-md: 0.75rem;
  --r-lg: 1.25rem; --r-xl: 2rem;  --r-pill: 9999px;

  /* Shadows */
  --shadow-gold-sm: 0 2px 16px rgba(200, 150, 12, 0.25);
  --shadow-gold-md: 0 4px 32px rgba(200, 150, 12, 0.35);
  --shadow-gold-lg: 0 8px 64px rgba(200, 150, 12, 0.45);
  --shadow-card:    0 4px 24px rgba(0,0,0,0.5);

  /* Transitions */
  --ease: 0.22s cubic-bezier(0.16, 1, 0.3, 1);
}

/* ===== RESET ===== */
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
html {
  scroll-behavior: smooth;
  -webkit-text-size-adjust: none;
  text-size-adjust: none;
  -webkit-font-smoothing: antialiased;
  scroll-padding-top: 70px;
}
body {
  min-height: 100dvh;
  font-family: var(--font-body);
  font-size: var(--text-base);
  line-height: 1.65;
  color: var(--text-primary);
  background-color: var(--black-rich);
  overflow-x: hidden;
}
img { display: block; max-width: 100%; height: auto; }
button { cursor: pointer; border: none; background: none; font: inherit; color: inherit; }
ul[role="list"] { list-style: none; }
h1, h2, h3, h4 { text-wrap: balance; line-height: 1.15; font-family: var(--font-display); }
p, li { text-wrap: pretty; }

/* ===== SHIMMER ANIMATION ===== */
@keyframes shimmer-gold {
  0%   { background-position: -200% center; }
  100% { background-position:  200% center; }
}
@keyframes shimmer-silver {
  0%   { background-position: -200% center; }
  100% { background-position:  200% center; }
}
@keyframes float-up {
  0%   { opacity: 0; transform: translateY(32px); }
  100% { opacity: 1; transform: translateY(0); }
}
@keyframes pulse-glow {
  0%, 100% { box-shadow: 0 0 20px rgba(200,150,12,0.3); }
  50%       { box-shadow: 0 0 50px rgba(200,150,12,0.7), 0 0 100px rgba(200,150,12,0.2); }
}
@keyframes border-spin {
  to { --angle: 360deg; }
}
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to   { opacity: 1; transform: translateY(0); }
}
@keyframes countUp {
  from { opacity: 0; }
  to   { opacity: 1; }
}
@keyframes scroll-indicator {
  0%   { transform: translateY(0); opacity: 1; }
  100% { transform: translateY(8px); opacity: 0; }
}
@keyframes sparkle {
  0%, 100% { opacity: 0; transform: scale(0); }
  50%       { opacity: 1; transform: scale(1); }
}

/* ===== UTILITY CLASSES ===== */
.gold-text {
  background: linear-gradient(90deg, #FFD700 0%, #E8B84B 25%, #FFFFFF 50%, #E8B84B 75%, #FFD700 100%);
  background-size: 200% auto;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: shimmer-gold 4s linear infinite;
}
.silver-text {
  background: linear-gradient(90deg, #C0C4D0 0%, #E8E8F0 25%, #FFFFFF 50%, #C0C4D0 75%, #8A8FA0 100%);
  background-size: 200% auto;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: shimmer-silver 3.5s linear infinite;
}
.gold-silver-text {
  background: linear-gradient(90deg, #FFD700 0%, #E8E8F0 30%, #FFD700 60%, #C0C4D0 80%, #FFD700 100%);
  background-size: 300% auto;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: shimmer-gold 5s linear infinite;
}
.section-pad {
  padding-block: clamp(var(--s12), 8vw, var(--s24));
  padding-inline: var(--s5);
}
.container {
  max-width: 500px;
  margin-inline: auto;
  width: 100%;
}
.container-wide {
  max-width: 600px;
  margin-inline: auto;
  width: 100%;
}
.reveal {
  opacity: 0;
  transform: translateY(28px);
  transition: opacity 0.7s cubic-bezier(0.16, 1, 0.3, 1),
              transform 0.7s cubic-bezier(0.16, 1, 0.3, 1);
}
.reveal.visible {
  opacity: 1;
  transform: translateY(0);
}
.reveal-delay-1 { transition-delay: 0.1s; }
.reveal-delay-2 { transition-delay: 0.2s; }
.reveal-delay-3 { transition-delay: 0.3s; }
.reveal-delay-4 { transition-delay: 0.4s; }

/* ===== HEADER ===== */
.site-header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;
  padding: var(--s3) var(--s5);
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: rgba(10,10,12,0.85);
  backdrop-filter: blur(16px);
  -webkit-backdrop-filter: blur(16px);
  border-bottom: 1px solid rgba(200,150,12,0.15);
  transition: background var(--ease), border-color var(--ease);
}
.site-header.scrolled {
  background: rgba(10,10,12,0.97);
  border-color: rgba(200,150,12,0.3);
}
.logo {
  display: flex;
  align-items: center;
  gap: var(--s2);
  text-decoration: none;
}
.logo-mark {
  width: 36px;
  height: 36px;
  flex-shrink: 0;
}
.logo-text {
  font-family: var(--font-display);
  font-size: 1.1rem;
  font-weight: 600;
  letter-spacing: 0.02em;
  line-height: 1.2;
}
.logo-text .num {
  display: block;
  font-size: 1.4rem;
  font-weight: 700;
}
.nav-cta {
  display: inline-flex;
  align-items: center;
  gap: var(--s2);
  padding: var(--s2) var(--s5);
  border-radius: var(--r-pill);
  background: var(--grad-cta);
  color: #0A0A0C;
  font-size: var(--text-sm);
  font-weight: 700;
  text-decoration: none;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  box-shadow: var(--shadow-gold-sm);
  transition: box-shadow var(--ease), transform var(--ease);
}
.nav-cta:hover {
  box-shadow: var(--shadow-gold-md);
  transform: translateY(-1px);
}

/* ===== PROGRESS BAR ===== */
#progress-bar {
  position: fixed;
  top: 0;
  left: 0;
  height: 3px;
  width: 0%;
  background: linear-gradient(90deg, #C8960C, #FFD700, #E8E8F0, #FFD700, #C8960C);
  background-size: 200% auto;
  animation: shimmer-gold 2s linear infinite;
  z-index: 200;
  transition: width 0.1s linear;
}

/* ===== HERO SECTION ===== */
.hero {
  min-height: 100dvh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  position: relative;
  overflow: hidden;
  padding: calc(70px + var(--s12)) var(--s5) var(--s16);
  background: var(--grad-hero-bg);
}
.hero-bg-particles {
  position: absolute;
  inset: 0;
  pointer-events: none;
  overflow: hidden;
}
.particle {
  position: absolute;
  border-radius: 50%;
  opacity: 0;
}
.hero-badge {
  display: inline-flex;
  align-items: center;
  gap: var(--s2);
  padding: var(--s2) var(--s5);
  border-radius: var(--r-pill);
  border: 1px solid rgba(200,150,12,0.4);
  background: rgba(200,150,12,0.08);
  font-size: var(--text-xs);
  font-weight: 600;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--gold-warm);
  margin-bottom: var(--s6);
  animation: float-up 0.8s 0.2s both;
}
.hero-badge::before {
  content: '';
  display: inline-block;
  width: 6px;
  height: 6px;
  border-radius: 50%;
  background: var(--gold-bright);
  box-shadow: 0 0 8px var(--gold-bright);
  animation: pulse-glow 2s infinite;
}
.hero-title {
  font-family: var(--font-display);
  font-size: var(--text-hero);
  font-weight: 700;
  line-height: 1.05;
  letter-spacing: -0.02em;
  margin-bottom: var(--s6);
  animation: float-up 0.8s 0.35s both;
}
.hero-subtitle {
  font-family: var(--font-display);
  font-size: var(--text-xl);
  font-weight: 400;
  font-style: italic;
  color: var(--text-secondary);
  max-width: 520px;
  margin-inline: auto;
  margin-bottom: var(--s8);
  animation: float-up 0.8s 0.5s both;
}
.hero-body {
  font-size: var(--text-base);
  color: var(--text-secondary);
  max-width: 460px;
  margin-inline: auto;
  margin-bottom: var(--s10);
  animation: float-up 0.8s 0.65s both;
}
.hero-body strong {
  color: var(--text-primary);
  font-weight: 600;
}
.hero-cta-group {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: var(--s4);
  animation: float-up 0.8s 0.8s both;
}
.btn-primary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: var(--s2);
  padding: var(--s4) var(--s10);
  border-radius: var(--r-pill);
  background: var(--grad-cta);
  color: #0A0A0C;
  font-size: var(--text-sm);
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  text-decoration: none;
  box-shadow: var(--shadow-gold-md);
  transition: transform var(--ease), box-shadow var(--ease);
  width: 100%;
  max-width: 340px;
  min-height: 54px;
}
.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-gold-lg);
}
.btn-primary:active { transform: translateY(0); }
.btn-secondary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: var(--s2);
  padding: var(--s3) var(--s8);
  border-radius: var(--r-pill);
  border: 1px solid rgba(192,196,208,0.4);
  background: rgba(192,196,208,0.06);
  color: var(--silver-mid);
  font-size: var(--text-sm);
  font-weight: 500;
  letter-spacing: 0.04em;
  text-decoration: none;
  text-transform: uppercase;
  transition: border-color var(--ease), background var(--ease), color var(--ease);
  width: 100%;
  max-width: 340px;
  min-height: 50px;
}
.btn-secondary:hover {
  border-color: rgba(192,196,208,0.7);
  background: rgba(192,196,208,0.12);
  color: var(--silver-bright);
}
.hero-cta-hint {
  font-size: var(--text-xs);
  color: var(--text-muted);
  text-align: center;
}
.hero-scroll {
  position: absolute;
  bottom: var(--s8);
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: var(--s2);
  font-size: var(--text-xs);
  color: var(--text-muted);
  letter-spacing: 0.08em;
  animation: float-up 1s 1.2s both;
}
.scroll-icon {
  width: 24px;
  height: 38px;
  border: 1px solid rgba(200,150,12,0.35);
  border-radius: var(--r-pill);
  display: flex;
  align-items: flex-start;
  justify-content: center;
  padding-top: 6px;
}
.scroll-dot {
  width: 4px;
  height: 8px;
  border-radius: var(--r-pill);
  background: var(--gold-warm);
  animation: scroll-indicator 1.6s infinite;
}

/* ===== HERO DECORATIVE ===== */
.hero-orb {
  position: absolute;
  border-radius: 50%;
  pointer-events: none;
  filter: blur(80px);
  opacity: 0.18;
}
.hero-orb-1 {
  width: 300px; height: 300px;
  background: radial-gradient(circle, #C8960C, transparent);
  top: 10%; left: -80px;
}
.hero-orb-2 {
  width: 250px; height: 250px;
  background: radial-gradient(circle, #8A8FA0, transparent);
  bottom: 15%; right: -60px;
}
.hero-orb-3 {
  width: 200px; height: 200px;
  background: radial-gradient(circle, #FFD700, transparent);
  top: 50%; left: 50%;
  transform: translate(-50%, -50%);
  opacity: 0.06;
}
/* Decorative lines */
.hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 59px,
      rgba(200,150,12,0.04) 60px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 59px,
      rgba(200,150,12,0.04) 60px
    );
  pointer-events: none;
}

/* ===== SECTION LABEL ===== */
.section-label {
  display: inline-flex;
  align-items: center;
  gap: var(--s2);
  font-size: var(--text-xs);
  font-weight: 700;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  margin-bottom: var(--s4);
  color: var(--gold-warm);
}
.section-label::before {
  content: '';
  display: block;
  width: 20px;
  height: 1px;
  background: var(--gold-warm);
}
.section-title {
  font-family: var(--font-display);
  font-size: var(--text-2xl);
  font-weight: 700;
  line-height: 1.1;
  margin-bottom: var(--s4);
}
.section-body {
  font-size: var(--text-base);
  color: var(--text-secondary);
  line-height: 1.7;
}

/* ===== DIVIDER ===== */
.gold-divider {
  width: 60px;
  height: 2px;
  background: var(--grad-gold);
  border-radius: var(--r-pill);
  margin-block: var(--s6);
}
.silver-divider {
  width: 100%;
  height: 1px;
  background: linear-gradient(90deg, transparent, rgba(192,196,208,0.2), transparent);
  margin-block: 0;
}

/* ===== PAIN SECTION ===== */
.pain-section {
  background: var(--black-surface);
  position: relative;
}
.pain-section::before {
  content: '';
  position: absolute;
  top: 0; left: 50%; transform: translateX(-50%);
  width: 1px;
  height: 60px;
  background: linear-gradient(180deg, rgba(200,150,12,0.5), transparent);
}
.pain-list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: var(--s5);
  margin-top: var(--s8);
}
.pain-item {
  display: flex;
  align-items: flex-start;
  gap: var(--s4);
  padding: var(--s5);
  border-radius: var(--r-md);
  background: var(--black-card);
  border: 1px solid var(--black-border);
  transition: border-color var(--ease), transform var(--ease);
}
.pain-item:hover {
  border-color: rgba(200,150,12,0.25);
  transform: translateX(4px);
}
.pain-icon {
  width: 36px;
  height: 36px;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: var(--r-sm);
  background: rgba(200,150,12,0.1);
  font-size: 1.1rem;
}
.pain-text {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.6;
}
.pain-answer {
  margin-top: var(--s10);
  padding: var(--s6);
  border-radius: var(--r-lg);
  background: linear-gradient(135deg, rgba(200,150,12,0.08) 0%, rgba(10,10,12,0) 100%);
  border: 1px solid rgba(200,150,12,0.25);
  text-align: center;
}
.pain-answer p {
  font-family: var(--font-display);
  font-size: var(--text-lg);
  font-style: italic;
  color: var(--text-primary);
  line-height: 1.5;
}

/* ===== CONTRAST SECTION ===== */
.contrast-section {
  background: var(--black-rich);
}
.contrast-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: var(--s5);
  margin-top: var(--s8);
}
.contrast-card {
  border-radius: var(--r-lg);
  padding: var(--s6);
  position: relative;
  overflow: hidden;
}
.contrast-card.bad {
  background: rgba(26,26,34,0.8);
  border: 1px solid rgba(90,95,112,0.3);
}
.contrast-card.good {
  background: linear-gradient(135deg, rgba(200,150,12,0.08), rgba(10,10,12,0));
  border: 1px solid rgba(200,150,12,0.3);
}
.contrast-card.good::after {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 2px;
  background: var(--grad-gold);
}
.contrast-label {
  display: inline-flex;
  align-items: center;
  gap: var(--s2);
  font-size: var(--text-xs);
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  padding: var(--s1) var(--s3);
  border-radius: var(--r-pill);
  margin-bottom: var(--s4);
}
.contrast-label.bad { color: var(--silver-muted); background: rgba(90,95,112,0.15); }
.contrast-label.good { color: var(--gold-warm); background: rgba(200,150,12,0.15); }
.contrast-title {
  font-family: var(--font-display);
  font-size: var(--text-xl);
  font-weight: 600;
  margin-bottom: var(--s4);
  color: var(--text-primary);
}
.contrast-body {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.7;
}
.contrast-body p + p { margin-top: var(--s3); }

/* ===== AUTHOR SECTION ===== */
.author-section {
  background: var(--black-surface);
  position: relative;
  overflow: hidden;
}
.author-section::after {
  content: '';
  position: absolute;
  bottom: 0; right: -100px;
  width: 300px; height: 300px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(200,150,12,0.06), transparent);
  pointer-events: none;
}
.author-avatar {
  width: 90px;
  height: 90px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--black-elevated), var(--black-card));
  border: 2px solid rgba(200,150,12,0.4);
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: var(--font-display);
  font-size: 2.5rem;
  font-weight: 700;
  margin-bottom: var(--s5);
  position: relative;
  box-shadow: var(--shadow-gold-sm);
  margin-inline: auto;
}
.author-avatar::after {
  content: '';
  position: absolute;
  inset: -4px;
  border-radius: 50%;
  border: 1px solid rgba(200,150,12,0.2);
}
.author-name {
  font-family: var(--font-display);
  font-size: var(--text-xl);
  font-weight: 700;
  text-align: center;
  margin-bottom: var(--s2);
}
.author-role {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  text-align: center;
  margin-bottom: var(--s8);
}
.author-story {
  display: flex;
  flex-direction: column;
  gap: var(--s5);
}
.author-block {
  padding: var(--s5);
  border-radius: var(--r-md);
  background: var(--black-card);
  border-left: 3px solid rgba(200,150,12,0.4);
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.7;
}
.author-block strong { color: var(--text-primary); }
.guarantee-pill {
  display: flex;
  align-items: center;
  gap: var(--s3);
  padding: var(--s4) var(--s5);
  border-radius: var(--r-lg);
  background: linear-gradient(135deg, rgba(200,150,12,0.12), rgba(10,10,12,0));
  border: 1px solid rgba(200,150,12,0.35);
  margin-top: var(--s8);
}
.guarantee-icon {
  font-size: 1.8rem;
  flex-shrink: 0;
}
.guarantee-text {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.5;
}
.guarantee-text strong {
  display: block;
  color: var(--text-primary);
  font-weight: 600;
  margin-bottom: var(--s1);
}

/* ===== WHAT IS THIS ===== */
.what-section {
  background: var(--black-rich);
}
.outcome-list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: var(--s4);
  margin-top: var(--s8);
  margin-bottom: var(--s8);
}
.outcome-item {
  display: flex;
  align-items: flex-start;
  gap: var(--s4);
  padding: var(--s4) var(--s5);
  border-radius: var(--r-md);
  background: var(--black-card);
  border: 1px solid var(--black-border);
}
.outcome-icon {
  width: 32px;
  height: 32px;
  border-radius: var(--r-sm);
  background: var(--grad-cta);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  color: var(--black-pure);
  font-size: 0.9rem;
}
.outcome-text {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.6;
}
.outcome-text strong { color: var(--text-primary); }

/* ===== 7 STEPS ===== */
.steps-section {
  background: var(--black-surface);
  position: relative;
}
.steps-intro {
  font-family: var(--font-display);
  font-size: var(--text-lg);
  font-style: italic;
  color: var(--text-secondary);
  text-align: center;
  margin-bottom: var(--s10);
  line-height: 1.6;
}
.steps-list {
  display: flex;
  flex-direction: column;
  gap: 0;
  position: relative;
}
.steps-list::before {
  content: '';
  position: absolute;
  left: 23px;
  top: 0;
  bottom: 0;
  width: 1px;
  background: linear-gradient(180deg, transparent, rgba(200,150,12,0.3) 10%, rgba(200,150,12,0.3) 90%, transparent);
}
.step-item {
  display: flex;
  gap: var(--s4);
  padding: var(--s6) 0;
  position: relative;
}
.step-item + .step-item {
  border-top: 1px solid var(--black-border);
}
.step-num-wrap {
  flex-shrink: 0;
  width: 46px;
  height: 46px;
  border-radius: 50%;
  background: var(--black-elevated);
  border: 1px solid rgba(200,150,12,0.4);
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  z-index: 1;
  flex-direction: column;
  box-shadow: var(--shadow-gold-sm);
}
.step-letter {
  font-family: var(--font-display);
  font-size: 1.3rem;
  font-weight: 700;
  background: var(--grad-gold);
  background-size: 200% auto;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: shimmer-gold 3s linear infinite;
  line-height: 1;
}
.step-content { flex: 1; padding-top: var(--s1); }
.step-title {
  font-family: var(--font-display);
  font-size: var(--text-lg);
  font-weight: 700;
  color: var(--text-primary);
  margin-bottom: var(--s2);
}
.step-kpi {
  font-size: var(--text-xs);
  font-weight: 700;
  letter-spacing: 0.06em;
  color: var(--gold-warm);
  margin-bottom: var(--s3);
  font-style: italic;
}
.step-body {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.7;
}
.step-secret {
  background: linear-gradient(135deg, rgba(200,150,12,0.1), rgba(192,196,208,0.05));
  border: 1px solid rgba(200,150,12,0.3);
  border-radius: var(--r-lg);
  padding: var(--s6);
  text-align: center;
  margin-top: var(--s6);
}
.step-secret .section-title { font-size: var(--text-xl); }
.step-secret .section-body { margin-top: var(--s3); }

/* ===== AI BLOCK ===== */
.ai-section {
  background: var(--black-rich);
}
.ai-card {
  border-radius: var(--r-xl);
  padding: var(--s8) var(--s6);
  background: linear-gradient(135deg,
    rgba(192,196,208,0.06) 0%,
    rgba(10,10,12,0) 60%,
    rgba(200,150,12,0.06) 100%
  );
  border: 1px solid rgba(192,196,208,0.2);
  text-align: center;
  position: relative;
  overflow: hidden;
}
.ai-card::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 2px;
  background: var(--grad-silver);
}
.ai-icon {
  font-size: 3rem;
  margin-bottom: var(--s4);
}
.ai-title {
  font-family: var(--font-display);
  font-size: var(--text-xl);
  font-weight: 700;
  margin-bottom: var(--s4);
}
.ai-body {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.7;
  max-width: 400px;
  margin-inline: auto;
}
.ai-badge {
  display: inline-flex;
  align-items: center;
  gap: var(--s2);
  margin-top: var(--s5);
  padding: var(--s2) var(--s4);
  border-radius: var(--r-pill);
  background: rgba(192,196,208,0.1);
  border: 1px solid rgba(192,196,208,0.2);
  font-size: var(--text-xs);
  color: var(--silver-mid);
  font-weight: 600;
  letter-spacing: 0.08em;
}

/* ===== VALUE STACK ===== */
.value-section {
  background: var(--black-surface);
}
.value-table {
  width: 100%;
  border-collapse: collapse;
  margin-top: var(--s8);
  border-radius: var(--r-lg);
  overflow: hidden;
}
.value-table thead tr {
  background: rgba(200,150,12,0.12);
  border-bottom: 1px solid rgba(200,150,12,0.25);
}
.value-table th {
  padding: var(--s3) var(--s4);
  font-size: var(--text-xs);
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--gold-warm);
  text-align: left;
}
.value-table td {
  padding: var(--s3) var(--s4);
  font-size: var(--text-sm);
  color: var(--text-secondary);
  border-bottom: 1px solid var(--black-border);
  vertical-align: top;
}
.value-table td:last-child {
  color: var(--gold-warm);
  font-weight: 600;
  text-align: right;
  white-space: nowrap;
}
.value-table tr:last-child td { border-bottom: none; }
.value-total {
  margin-top: var(--s4);
  padding: var(--s4) var(--s5);
  border-radius: var(--r-md);
  background: rgba(200,150,12,0.1);
  border: 1px solid rgba(200,150,12,0.3);
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: var(--s4);
}
.value-total .label {
  font-size: var(--text-sm);
  color: var(--text-secondary);
}
.value-total .amount {
  font-family: var(--font-display);
  font-size: var(--text-lg);
  font-weight: 700;
  color: var(--gold-warm);
}

/* ===== GUARANTEE SECTION ===== */
.guarantee-section {
  background: var(--black-rich);
}
.guarantee-card {
  border-radius: var(--r-xl);
  padding: var(--s8) var(--s6);
  background: linear-gradient(160deg,
    rgba(200,150,12,0.1) 0%,
    rgba(10,10,12,0) 50%,
    rgba(200,150,12,0.05) 100%
  );
  border: 1px solid rgba(200,150,12,0.35);
  position: relative;
  overflow: hidden;
  text-align: center;
}
.guarantee-card::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 3px;
  background: var(--grad-gold);
}
.guarantee-card::after {
  content: '';
  position: absolute;
  bottom: 0; left: 0; right: 0;
  height: 1px;
  background: var(--grad-silver);
}
.guarantee-big-icon {
  font-size: 3.5rem;
  margin-bottom: var(--s4);
}
.guarantee-quote {
  font-family: var(--font-display);
  font-size: var(--text-lg);
  font-style: italic;
  color: var(--text-primary);
  line-height: 1.5;
  margin-bottom: var(--s6);
}
.guarantee-options {
  display: flex;
  flex-direction: column;
  gap: var(--s3);
  margin-top: var(--s6);
}
.guarantee-opt {
  display: flex;
  align-items: center;
  gap: var(--s3);
  padding: var(--s3) var(--s4);
  border-radius: var(--r-md);
  background: rgba(200,150,12,0.06);
  border: 1px solid rgba(200,150,12,0.2);
  font-size: var(--text-sm);
  color: var(--text-secondary);
  text-align: left;
}
.guarantee-opt-icon { font-size: 1.2rem; flex-shrink: 0; }

/* ===== TARIFFS ===== */
.tariffs-section {
  background: var(--black-surface);
}
.tariff-urgency {
  text-align: center;
  padding: var(--s4);
  border-radius: var(--r-md);
  background: rgba(200,150,12,0.08);
  border: 1px solid rgba(200,150,12,0.25);
  margin-bottom: var(--s8);
  font-size: var(--text-sm);
  color: var(--text-secondary);
}
.tariff-urgency strong {
  color: var(--gold-warm);
  display: block;
  font-size: var(--text-base);
  margin-bottom: var(--s1);
}
.tariff-grid {
  display: flex;
  flex-direction: column;
  gap: var(--s5);
}
.tariff-card {
  border-radius: var(--r-xl);
  padding: var(--s7, 1.75rem) var(--s6);
  position: relative;
  overflow: hidden;
  transition: transform var(--ease), box-shadow var(--ease);
}
.tariff-card:hover { transform: translateY(-3px); }
.tariff-card.standard {
  background: var(--black-card);
  border: 1px solid var(--black-separator);
}
.tariff-card.supervip {
  background: linear-gradient(160deg, rgba(200,150,12,0.1) 0%, rgba(10,10,12,0) 60%);
  border: 1px solid rgba(200,150,12,0.4);
  box-shadow: var(--shadow-gold-sm);
}
.tariff-card.supervip:hover { box-shadow: var(--shadow-gold-md); }
.tariff-badge {
  position: absolute;
  top: var(--s4);
  right: var(--s4);
  padding: var(--s1) var(--s3);
  border-radius: var(--r-pill);
  font-size: 0.65rem;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}
.tariff-badge.popular {
  background: var(--grad-cta);
  color: var(--black-pure);
}
.tariff-badge.entry {
  background: rgba(192,196,208,0.12);
  color: var(--silver-mid);
  border: 1px solid rgba(192,196,208,0.2);
}
.tariff-name {
  font-size: var(--text-xs);
  font-weight: 700;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  margin-bottom: var(--s2);
  color: var(--text-muted);
}
.tariff-card.supervip .tariff-name { color: var(--gold-warm); }
.tariff-icon { font-size: 2rem; margin-bottom: var(--s3); }
.tariff-card-title {
  font-family: var(--font-display);
  font-size: var(--text-xl);
  font-weight: 700;
  margin-bottom: var(--s2);
}
.tariff-tagline {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  font-style: italic;
  margin-bottom: var(--s5);
  line-height: 1.5;
}
.tariff-price-block {
  display: flex;
  align-items: baseline;
  gap: var(--s2);
  margin-bottom: var(--s1);
}
.tariff-price {
  font-family: var(--font-display);
  font-size: var(--text-2xl);
  font-weight: 700;
  line-height: 1;
}
.tariff-card.supervip .tariff-price { color: var(--gold-warm); }
.tariff-card.standard .tariff-price { color: var(--silver-mid); }
.tariff-period {
  font-size: var(--text-sm);
  color: var(--text-muted);
}
.tariff-total {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  margin-bottom: var(--s6);
}
.tariff-total strong {
  color: var(--text-primary);
}
.tariff-divider {
  height: 1px;
  background: var(--black-border);
  margin-block: var(--s5);
}
.tariff-features {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: var(--s3);
  margin-bottom: var(--s6);
}
.tariff-feature {
  display: flex;
  align-items: flex-start;
  gap: var(--s3);
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.5;
}
.feature-check {
  width: 18px;
  height: 18px;
  border-radius: 50%;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 0.65rem;
  margin-top: 2px;
}
.tariff-card.supervip .feature-check {
  background: rgba(200,150,12,0.2);
  color: var(--gold-warm);
}
.tariff-card.standard .feature-check {
  background: rgba(192,196,208,0.1);
  color: var(--silver-mid);
}
.tariff-bonus {
  padding: var(--s4);
  border-radius: var(--r-md);
  background: rgba(200,150,12,0.06);
  border: 1px solid rgba(200,150,12,0.2);
  font-size: var(--text-xs);
  color: var(--text-secondary);
  line-height: 1.6;
  margin-bottom: var(--s5);
}
.tariff-bonus strong { color: var(--gold-warm); }
.tariff-note {
  font-size: var(--text-xs);
  color: var(--text-muted);
  text-align: center;
  margin-top: var(--s4);
  font-style: italic;
}
.why-supervip {
  margin-top: var(--s6);
  padding: var(--s5) var(--s5);
  border-radius: var(--r-lg);
  background: linear-gradient(135deg, rgba(200,150,12,0.06), rgba(10,10,12,0));
  border: 1px solid rgba(200,150,12,0.2);
}
.why-supervip h3 {
  font-family: var(--font-display);
  font-size: var(--text-lg);
  font-weight: 700;
  margin-bottom: var(--s4);
}
.why-supervip p {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.7;
  margin-bottom: var(--s3);
}
.why-supervip p:last-child { margin-bottom: 0; }
.process-note {
  margin-top: var(--s6);
  padding: var(--s5);
  border-radius: var(--r-lg);
  background: var(--black-card);
  border: 1px solid var(--black-border);
}
.process-note h4 {
  font-family: var(--font-display);
  font-size: var(--text-lg);
  font-weight: 600;
  margin-bottom: var(--s3);
  color: var(--silver-mid);
}
.process-note p {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.7;
}

/* ===== REVIEWS ===== */
.reviews-section {
  background: var(--black-rich);
}
.reviews-list {
  display: flex;
  flex-direction: column;
  gap: var(--s4);
  margin-top: var(--s8);
}
.review-card {
  border-radius: var(--r-lg);
  padding: var(--s5);
  background: var(--black-card);
  border: 1px solid var(--black-border);
  position: relative;
}
.review-card::before {
  content: '"';
  position: absolute;
  top: var(--s2);
  left: var(--s4);
  font-family: var(--font-display);
  font-size: 3rem;
  line-height: 1;
  color: rgba(200,150,12,0.2);
  pointer-events: none;
}
.review-stars {
  display: flex;
  gap: 2px;
  margin-bottom: var(--s3);
}
.star {
  color: var(--gold-warm);
  font-size: 0.85rem;
}
.review-text {
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.7;
  font-style: italic;
  margin-bottom: var(--s4);
}
.review-author {
  display: flex;
  align-items: center;
  gap: var(--s3);
}
.review-avatar {
  width: 36px;
  height: 36px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--black-elevated), var(--black-card));
  border: 1px solid rgba(200,150,12,0.3);
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 0.85rem;
  color: var(--gold-warm);
  flex-shrink: 0;
}
.review-name {
  font-size: var(--text-sm);
  font-weight: 600;
  color: var(--text-primary);
}

/* ===== NOT FOR YOU ===== */
.notforyou-section {
  background: var(--black-surface);
}
.not-for-grid, .for-grid {
  display: flex;
  flex-direction: column;
  gap: var(--s3);
  margin-top: var(--s5);
}
.not-item, .for-item {
  display: flex;
  align-items: flex-start;
  gap: var(--s3);
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.6;
  padding: var(--s3) var(--s4);
  border-radius: var(--r-md);
}
.not-item { background: rgba(90,95,112,0.08); border: 1px solid rgba(90,95,112,0.2); }
.for-item { background: rgba(200,150,12,0.06); border: 1px solid rgba(200,150,12,0.2); }
.not-icon { color: var(--silver-muted); font-size: 1rem; flex-shrink: 0; line-height: 1.6; }
.for-icon { color: var(--gold-warm); font-size: 1rem; flex-shrink: 0; line-height: 1.6; }
.not-divider-title {
  font-family: var(--font-display);
  font-size: var(--text-xl);
  font-weight: 700;
  text-align: center;
  margin: var(--s8) 0 var(--s5);
}

/* ===== FAQ ===== */
.faq-section {
  background: var(--black-rich);
}
.faq-list {
  display: flex;
  flex-direction: column;
  gap: var(--s3);
  margin-top: var(--s8);
}
.faq-item {
  border-radius: var(--r-md);
  background: var(--black-card);
  border: 1px solid var(--black-border);
  overflow: hidden;
  transition: border-color var(--ease);
}
.faq-item.open { border-color: rgba(200,150,12,0.3); }
.faq-question {
  width: 100%;
  text-align: left;
  padding: var(--s4) var(--s5);
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: var(--s3);
  font-size: var(--text-sm);
  font-weight: 600;
  color: var(--text-primary);
  line-height: 1.4;
  background: none;
  border: none;
  cursor: pointer;
  transition: color var(--ease);
}
.faq-item.open .faq-question { color: var(--gold-warm); }
.faq-chevron {
  flex-shrink: 0;
  width: 20px;
  height: 20px;
  border-radius: 50%;
  border: 1px solid rgba(200,150,12,0.3);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 0.7rem;
  transition: transform var(--ease), background var(--ease);
  color: var(--gold-warm);
}
.faq-item.open .faq-chevron {
  transform: rotate(180deg);
  background: rgba(200,150,12,0.1);
}
.faq-answer {
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.4s cubic-bezier(0.16, 1, 0.3, 1);
}
.faq-answer-inner {
  padding: 0 var(--s5) var(--s4);
  font-size: var(--text-sm);
  color: var(--text-secondary);
  line-height: 1.7;
}

/* ===== FINAL CTA ===== */
.final-cta-section {
  background: var(--black-surface);
  text-align: center;
  position: relative;
  overflow: hidden;
}
.final-cta-section::before {
  content: '';
  position: absolute;
  top: 50%; left: 50%;
  transform: translate(-50%, -50%);
  width: 400px; height: 400px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(200,150,12,0.08), transparent 70%);
  pointer-events: none;
}
.final-cta-title {
  font-family: var(--font-display);
  font-size: var(--text-2xl);
  font-weight: 700;
  line-height: 1.1;
  margin-bottom: var(--s4);
}
.final-cta-body {
  font-size: var(--text-base);
  color: var(--text-secondary);
  line-height: 1.7;
  max-width: 440px;
  margin-inline: auto;
  margin-bottom: var(--s8);
}
.final-cta-deadline {
  display: inline-flex;
  align-items: center;
  gap: var(--s2);
  padding: var(--s2) var(--s5);
  border-radius: var(--r-pill);
  background: rgba(200,150,12,0.1);
  border: 1px solid rgba(200,150,12,0.3);
  font-size: var(--text-sm);
  color: var(--gold-warm);
  font-weight: 600;
  margin-bottom: var(--s8);
}
.final-cta-buttons {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: var(--s4);
}
.final-hint {
  font-size: var(--text-xs);
  color: var(--text-muted);
  margin-top: var(--s2);
}
.deadline-counter {
  display: flex;
  justify-content: center;
  gap: var(--s4);
  margin-bottom: var(--s8);
}
.counter-unit {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: var(--s1);
}
.counter-num {
  font-family: var(--font-display);
  font-size: var(--text-2xl);
  font-weight: 700;
  color: var(--gold-warm);
  line-height: 1;
  min-width: 60px;
  text-align: center;
  padding: var(--s3) var(--s2);
  border-radius: var(--r-md);
  background: rgba(200,150,12,0.08);
  border: 1px solid rgba(200,150,12,0.25);
}
.counter-label {
  font-size: var(--text-xs);
  color: var(--text-muted);
  letter-spacing: 0.06em;
}

/* ===== FOOTER ===== */
.site-footer {
  background: var(--black-pure);
  padding: var(--s10) var(--s5);
  text-align: center;
  border-top: 1px solid rgba(200,150,12,0.15);
}
.footer-logo {
  font-family: var(--font-display);
  font-size: var(--text-xl);
  font-weight: 700;
  margin-bottom: var(--s3);
}
.footer-tagline {
  font-size: var(--text-xs);
  color: var(--text-muted);
  margin-bottom: var(--s6);
  letter-spacing: 0.06em;
}
.footer-links {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: var(--s5);
  margin-bottom: var(--s6);
}
.footer-links a {
  font-size: var(--text-xs);
  color: var(--text-muted);
  text-decoration: none;
  letter-spacing: 0.06em;
  transition: color var(--ease);
}
.footer-links a:hover { color: var(--gold-warm); }
.footer-copy {
  font-size: var(--text-xs);
  color: var(--text-muted);
  margin-top: var(--s4);
}
.footer-pplx {
  display: inline-flex;
  align-items: center;
  gap: var(--s1);
  font-size: var(--text-xs);
  color: var(--text-muted);
  text-decoration: none;
  margin-top: var(--s3);
  transition: color var(--ease);
}
.footer-pplx:hover { color: var(--silver-mid); }

/* ===== MOBILE OVERRIDES ===== */
@media (max-width: 480px) {
  .container { padding-inline: var(--s4); }
  .tariff-price { font-size: var(--text-xl); }
}
</style>
</head>
<body>

<!-- ===== PROGRESS BAR ===== -->
<div id="progress-bar"></div>

<!-- ===== HEADER ===== -->
<header class="site-header" id="site-header">
  <a href="#" class="logo" aria-label="7 шагов к изобилию">
    <svg class="logo-mark" viewBox="0 0 36 36" fill="none" aria-hidden="true">
      <circle cx="18" cy="18" r="17" stroke="url(#lg1)" stroke-width="1.5"/>
      <text x="18" y="24" text-anchor="middle" font-family="Cormorant Garamond, serif"
            font-size="18" font-weight="700" fill="url(#lg2)">7</text>
      <defs>
        <linearGradient id="lg1" x1="0" y1="0" x2="36" y2="36">
          <stop offset="0%" stop-color="#FFD700"/>
          <stop offset="50%" stop-color="#E8E8F0"/>
          <stop offset="100%" stop-color="#C8960C"/>
        </linearGradient>
        <linearGradient id="lg2" x1="0" y1="0" x2="36" y2="36">
          <stop offset="0%" stop-color="#FFD700"/>
          <stop offset="100%" stop-color="#E8B84B"/>
        </linearGradient>
      </defs>
    </svg>
    <span class="logo-text">
      <span class="gold-text">7 шагов</span>
    </span>
  </a>
  <a href="#tariffs" class="nav-cta">Оставить заявку</a>
</header>

<!-- ===== HERO ===== -->
<section class="hero" id="hero" aria-label="Главная">
  <!-- Decorative orbs -->
  <div class="hero-orb hero-orb-1" aria-hidden="true"></div>
  <div class="hero-orb hero-orb-2" aria-hidden="true"></div>
  <div class="hero-orb hero-orb-3" aria-hidden="true"></div>

  <div class="container">
    <div class="hero-badge" role="text">
      Программа наставничества · 3 месяца
    </div>

    <h1 class="hero-title">
      <span class="gold-silver-text">7 шагов<br>к изобилию</span>
    </h1>

    <p class="hero-subtitle">
      Для экспертов и предпринимателей, которые делали всё правильно — но не в том порядке
    </p>

    <p class="hero-body">
      Дело не в ваших знаниях. Не в нише. И точно не в лени.<br><br>
      <strong>Дело в последовательности.</strong>
    </p>

    <div class="hero-cta-group">
      <a href="#tariffs" class="btn-primary" aria-label="Оставить заявку — SUPERVIP">
        Оставить заявку →
      </a>
      <a href="#steps" class="btn-secondary">
        Узнать о программе
      </a>
      <p class="hero-cta-hint">Гарантия возврата · Александр ответит в течение 24 часов</p>
    </div>
  </div>

  <!-- Scroll indicator -->
  <div class="hero-scroll" aria-hidden="true">
    <div class="scroll-icon"><div class="scroll-dot"></div></div>
  </div>
</section>

<!-- ===== DIVIDER ===== -->
<div class="silver-divider" aria-hidden="true"></div>

<!-- ===== PAIN SECTION ===== -->
<section class="pain-section section-pad" id="pain" aria-label="Боль">
  <div class="container">
    <p class="section-label reveal">Узнаёте себя?</p>
    <h2 class="section-title reveal reveal-delay-1">
      Вы эксперт. У вас есть знания, которые реально <span class="silver-text">меняют жизни</span> людей.
    </h2>
    <p class="section-body reveal reveal-delay-2">
      Но каждый вечер вы возвращаетесь к одному и тому же.
    </p>

    <ul class="pain-list" role="list">
      <li class="pain-item reveal reveal-delay-1">
        <div class="pain-icon" aria-hidden="true">🤔</div>
        <p class="pain-text">Почему у коллеги, которая стартовала на год позже вас, — уже очередь из клиентов, а у вас лайки и «подумаю»?</p>
      </li>
      <li class="pain-item reveal reveal-delay-2">
        <div class="pain-icon" aria-hidden="true">⏰</div>
        <p class="pain-text">Почему вы работаете с девяти до десяти вечера, а деньги не сдвигаются — хотя вы делаете всё «правильно»?</p>
      </li>
      <li class="pain-item reveal reveal-delay-3">
        <div class="pain-icon" aria-hidden="true">💸</div>
        <p class="pain-text">Почему пять курсов по продажам не научили вас называть цену без внутреннего ступора?</p>
      </li>
      <li class="pain-item reveal reveal-delay-4">
        <div class="pain-icon" aria-hidden="true">📱</div>
        <p class="pain-text">Почему ваш блог есть, контент выходит — а заявок нет?</p>
      </li>
      <li class="pain-item reveal">
        <div class="pain-icon" aria-hidden="true">🔄</div>
        <p class="pain-text">Почему каждый раз, когда вы думаете «всё, запускаю» — что-то снова останавливает?</p>
      </li>
    </ul>

    <div class="pain-answer reveal">
      <div class="gold-divider" style="margin-inline: auto;"></div>
      <p>
        Ответ на все эти вопросы один.<br>
        <strong>Вам нужна последовательность шагов — и кто-то рядом, кто не даст сбиться с пути.</strong>
      </p>
    </div>
  </div>
</section>

<!-- ===== CONTRAST ===== -->
<section class="contrast-section section-pad" id="contrast" aria-label="Два сценария">
  <div class="container">
    <p class="section-label reveal">Выбор за вами</p>
    <h2 class="section-title reveal reveal-delay-1">
      Зачем работать больше,<br>если можно работать <span class="gold-text">правильно</span>?
    </h2>

    <div class="contrast-grid">
      <div class="contrast-card bad reveal">
        <div class="contrast-label bad">✖ Сценарий первый. Вы ничего не меняете</div>
        <div class="contrast-body">
          <p>Через год вы снова откроете свой блог и увидите того же человека, который стартовал позже вас — теперь он продаёт программу за 150 000 рублей.</p>
          <p>Деньги — те же. Клиентов — мало. Уверенности — меньше, чем год назад. Всё серое. Безопасное — и именно поэтому невыносимое.</p>
        </div>
      </div>

      <div class="contrast-card good reveal reveal-delay-1">
        <div class="contrast-label good">✦ Сценарий второй. Вы входите в программу</div>
        <div class="contrast-body">
          <p>Через три месяца вы открываете телефон — и видите заявки от людей, которые нашли вас сами. Потому, что ваш бизнес выстроен как алгоритм — и он работает, пока вы пьёте кофе.</p>
          <p>Вы знаете, кто вы. Что продаёте. Кому. И что делать завтра без тревоги.</p>
          <p style="font-family: var(--font-display); font-style: italic; font-size: 1.1rem; margin-top: var(--s4); color: var(--text-primary);">
            Вы просыпаетесь с ощущением, которое давно забыли: <span class="gold-text">я иду туда, куда хочу.</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ===== AUTHOR ===== -->
<section class="author-section section-pad" id="author" aria-label="Об авторе">
  <div class="container">
    <p class="section-label reveal">Кто за этим стоит</p>

    <div class="author-avatar reveal" aria-hidden="true">АТ</div>
    <h2 class="author-name reveal reveal-delay-1">Александр Токин</h2>
    <p class="author-role reveal reveal-delay-2">Бизнес-тренер · Эксперт по воронкам · Технолог</p>

    <div class="author-story">
      <div class="author-block reveal">
        Меня зовут Александр Токин. По образованию я <strong>технолог</strong>. Это значит, что меня учили мыслить алгоритмами: есть входные данные, есть последовательность шагов, есть предсказуемый результат на выходе.
      </div>
      <div class="author-block reveal reveal-delay-1">
        Когда я пришёл в инфобизнес — увидел парадокс. Люди с блестящими знаниями зарабатывали копейки. Люди с посредственными — миллионы. <strong>Разница была не в знаниях. Разница была в последовательности шагов.</strong>
      </div>
      <div class="author-block reveal reveal-delay-2">
        Я потратил годы на то, чтобы разобрать этот алгоритм до уровня инструкции. Сегодня утром я проснулся — а в это время моя воронка продаж сделала три заявки. <strong>Не потому, что я везунчик. Потому, что систему, которую я преподаю, я сначала выстроил в собственной жизни.</strong>
      </div>
    </div>

    <div class="guarantee-pill reveal">
      <div class="guarantee-icon" aria-hidden="true">🏅</div>
      <div class="guarantee-text">
        <strong>Единственный наставник в нише с тройной гарантией</strong>
        Результат — или деньги назад, без оговорок и без вопросов. Или продолжаю работать бесплатно до результата.
      </div>
    </div>
  </div>
</section>

<!-- ===== WHAT IS THIS ===== -->
<section class="what-section section-pad" id="what" aria-label="Что вы получите">
  <div class="container">
    <p class="section-label reveal">Программа</p>
    <h2 class="section-title reveal reveal-delay-1">
      Не курс с теорией —<br><span class="silver-text">три месяца совместной работы</span>
    </h2>
    <p class="section-body reveal reveal-delay-2">
      Большинство программ устроены так: вам дают знания — вы сами разбираетесь, как их применить. Мы идём по шагам — вы делаете, я рядом. Каждый шаг заканчивается не «понял теорию», а конкретным результатом в вашем бизнесе.
    </p>

    <div class="gold-divider reveal"></div>

    <p style="font-family: var(--font-display); font-size: var(--text-lg); font-weight: 600; margin-bottom: var(--s4);" class="reveal">
      В конце трёх месяцев у вас будет:
    </p>
    <ul class="outcome-list" role="list">
      <li class="outcome-item reveal">
        <div class="outcome-icon" aria-hidden="true">✦</div>
        <p class="outcome-text"><strong>Работающий бизнес</strong>, выстроенный под ваши сильные стороны</p>
      </li>
      <li class="outcome-item reveal reveal-delay-1">
        <div class="outcome-icon" aria-hidden="true">✦</div>
        <p class="outcome-text"><strong>Блог, который привлекает клиентов</strong> без ежедневного контента на износ</p>
      </li>
      <li class="outcome-item reveal reveal-delay-2">
        <div class="outcome-icon" aria-hidden="true">✦</div>
        <p class="outcome-text"><strong>Первые платящие клиенты</strong> — реальные люди, реальные деньги</p>
      </li>
      <li class="outcome-item reveal reveal-delay-3">
        <div class="outcome-icon" aria-hidden="true">✦</div>
        <p class="outcome-text"><strong>Воронка продаж</strong>, которая работает без вас</p>
      </li>
      <li class="outcome-item reveal reveal-delay-4">
        <div class="outcome-icon" aria-hidden="true">✦</div>
        <p class="outcome-text">Ответы на три главных вопроса: <strong>кто вы, что продаёте, кому</strong> — и куда идти дальше</p>
      </li>
    </ul>
  </div>
</section>

<!-- ===== 7 STEPS ===== -->
<section class="steps-section section-pad" id="steps" aria-label="7 шагов — алгоритм">
  <div class="container">
    <p class="section-label reveal">РЕЦЕПТ изобилия</p>
    <h2 class="section-title reveal reveal-delay-1">
      Алгоритм из <span class="gold-text">7 шагов</span>
    </h2>
    <p class="steps-intro reveal reveal-delay-2">
      Случайность, что первые буквы складываются в слово РЕЦЕПТ?<br>
      Нет. Это проверенный алгоритм технолога.
    </p>

    <div class="steps-list" role="list">
      <div class="step-item reveal" role="listitem">
        <div class="step-num-wrap" aria-hidden="true">
          <span class="step-letter">Р</span>
        </div>
        <div class="step-content">
          <h3 class="step-title">Раскрытие ценности</h3>
          <p class="step-kpi">«Одна фраза из 7 слов — и клиент сам напишет первым»</p>
          <p class="step-body">После этого шага у вас будет формулировка, от которой люди говорят: «Боже, именно это мне и нужно» — и сами тянутся написать вам первыми.</p>
        </div>
      </div>

      <div class="step-item reveal" role="listitem">
        <div class="step-num-wrap" aria-hidden="true">
          <span class="step-letter">Е</span>
        </div>
        <div class="step-content">
          <h3 class="step-title">Естественное позиционирование</h3>
          <p class="step-kpi">«9 из 10 экспертов выбирают нишу, которая гарантирует им невидимость»</p>
          <p class="step-body">После этого шага вы займёте позицию, в которой нет конкурентов — потому что это ваше место, и только ваше.</p>
        </div>
      </div>

      <div class="step-item reveal" role="listitem">
        <div class="step-num-wrap" aria-hidden="true">
          <span class="step-letter">Ц</span>
        </div>
        <div class="step-content">
          <h3 class="step-title">Целевая аудитория</h3>
          <p class="step-kpi">«3 типа клиентов. Вы будете работать только с одним»</p>
          <p class="step-body">После этого шага вы будете знать, где живут те, кто платит без вопросов и возвращается сам — и как сделать так, чтобы они находили вас, а не вы их.</p>
        </div>
      </div>

      <div class="step-item reveal" role="listitem">
        <div class="step-num-wrap" aria-hidden="true">
          <span class="step-letter">Е</span>
        </div>
        <div class="step-content">
          <h3 class="step-title">Естественная воронка</h3>
          <p class="step-kpi">«Контент, который продаёт, пока вы спите»</p>
          <p class="step-body">После этого шага ваш блог перестанет быть обязанностью и станет продавцом, который работает круглосуточно.</p>
        </div>
      </div>

      <div class="step-item reveal" role="listitem">
        <div class="step-num-wrap" aria-hidden="true">
          <span class="step-letter">П</span>
        </div>
        <div class="step-content">
          <h3 class="step-title">Продажи</h3>
          <p class="step-kpi">«7 слов, которые превращают "подумаю" в "куда оплатить"»</p>
          <p class="step-body">После этого шага вы никогда больше не будете чувствовать неловкость, называя цену — потому, что к этому моменту человек уже купил. Внутри.</p>
        </div>
      </div>

      <div class="step-item reveal" role="listitem">
        <div class="step-num-wrap" aria-hidden="true">
          <span class="step-letter">Т</span>
        </div>
        <div class="step-content">
          <h3 class="step-title">Тестирование и масштабирование</h3>
          <p class="step-kpi">«80% экспертов выгорают именно в момент роста»</p>
          <p class="step-body">После этого шага вы будете знать, что именно масштабировать, в какой момент — и что никогда не трогать.</p>
        </div>
      </div>
    </div>

    <div class="step-secret reveal">
      <div class="gold-divider" style="margin-inline: auto; margin-bottom: var(--s5);"></div>
      <p class="section-label" style="justify-content: center;">Седьмой шаг</p>
      <h3 class="section-title">
        <span class="gold-silver-text">А — Секретный</span>
      </h3>
      <p class="section-body" style="margin-top: var(--s3);">
        Я намеренно не раскрываю его здесь.<br>
        Скажу только одно: без него первые шесть работают на 40% своей мощности.<br>
        Это про то, без чего ни один алгоритм не запускается. И я сам прошёл этот шаг — именно он изменил всё.
      </p>
    </div>
  </div>
</section>

<!-- ===== AI BLOCK ===== -->
<section class="ai-section section-pad" id="ai" aria-label="Блок про ИИ">
  <div class="container">
    <div class="ai-card reveal">
      <div class="ai-icon" aria-hidden="true">🤖</div>
      <h2 class="ai-title">
        <span class="silver-text">И ещё кое-что</span>
      </h2>
      <p class="ai-body">
        В программе есть блок, о котором я не рассказываю заранее. Потому что если я скажу, что именно вы получите — вы не поверите. Пока не увидите своими глазами.
        <br><br>
        Это касается нейросетей. Конкретное применение ИИ для вашего бизнеса — такое, которое освобождает <strong>3–4 часа рабочего времени в день</strong> и при этом делает контент, продажи и воронку лучше.
        <br><br>
        Участники, которые уже это видели, спрашивают одно: <em>«Почему никто раньше не показывал это вот так?»</em>
      </p>
      <div class="ai-badge">✦ Эксклюзивно для участников программы</div>
    </div>
  </div>
</section>

<!-- ===== VALUE STACK ===== -->
<section class="value-section section-pad" id="value" aria-label="Ценностный стек">
  <div class="container">
    <p class="section-label reveal">Прежде чем увидите цену</p>
    <h2 class="section-title reveal reveal-delay-1">
      Личная сессия с Александром Токиным — <span class="gold-text">15 000 ₽/час</span>
    </h2>
    <p class="section-body reveal reveal-delay-2">Запомните эту цифру. За три месяца программы вы получаете:</p>

    <div class="reveal">
      <table class="value-table" aria-label="Что входит в программу">
        <thead>
          <tr>
            <th>Что входит</th>
            <th>Стоимость отдельно</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>7 модулей — каждый заканчивается конкретным результатом</td>
            <td>105 000 ₽</td>
          </tr>
          <tr>
            <td>Личное подключение Александра к вашим задачам</td>
            <td>от 90 000 ₽</td>
          </tr>
          <tr>
            <td>Мозговые штурмы и разборы в группе</td>
            <td>36 000 ₽</td>
          </tr>
          <tr>
            <td>Готовая воронка, блог и первые клиенты</td>
            <td>Бесценно</td>
          </tr>
          <tr>
            <td>ИИ-блок — такого применения нет в других программах</td>
            <td>Не продаётся отдельно</td>
          </tr>
        </tbody>
      </table>

      <div class="value-total">
        <span class="label">Итого, если собирать по частям:</span>
        <span class="amount gold-text">от 231 000 ₽</span>
      </div>
    </div>
  </div>
</section>

<!-- ===== GUARANTEE ===== -->
<section class="guarantee-section section-pad" id="guarantee" aria-label="Гарантия">
  <div class="container">
    <div class="guarantee-card reveal">
      <div class="guarantee-big-icon" aria-hidden="true">🛡️</div>
      <p class="section-label" style="justify-content: center; margin-bottom: var(--s4);">Гарантия технолога</p>
      <blockquote class="guarantee-quote">
        «Если вы пройдёте все 7 шагов вместе со мной и в конце трёх месяцев у вас не будет работающего бизнеса, первых платящих клиентов и ясного понимания своего пути — я верну вам деньги полностью.»
      </blockquote>

      <p style="font-size: var(--text-sm); color: var(--text-muted); margin-bottom: var(--s5);">
        Без переговоров. Без «ну вы же не всё сделали». Без вопросов.
      </p>

      <div class="guarantee-options" role="list">
        <div class="guarantee-opt" role="listitem">
          <span class="guarantee-opt-icon" aria-hidden="true">💰</span>
          <span>Возврат денег полностью — на ваши реквизиты</span>
        </div>
        <div class="guarantee-opt" role="listitem">
          <span class="guarantee-opt-icon" aria-hidden="true">🤝</span>
          <span>Или продолжаю работать с вами бесплатно до результата</span>
        </div>
      </div>

      <p style="font-family: var(--font-display); font-size: var(--text-lg); font-weight: 700; margin-top: var(--s6); color: var(--gold-warm);">
        Точка.
      </p>
    </div>
  </div>
</section>

<!-- ===== TARIFFS ===== -->
<section class="tariffs-section section-pad" id="tariffs" aria-label="Тарифы">
  <div class="container">
    <p class="section-label reveal">Следующий поток</p>
    <h2 class="section-title reveal reveal-delay-1">
      Старт <span class="gold-text">1 апреля</span>
    </h2>

    <div class="tariff-urgency reveal reveal-delay-2">
      <strong>⚡ Осталось мест: SUPERVIP — 5, STANDART — 5</strong>
      Когда места заполнены — набор закрывается до следующего потока
    </div>

    <div class="tariff-grid">
      <!-- SUPERVIP -->
      <div class="tariff-card supervip reveal">
        <div class="tariff-badge popular">Рекомендуем</div>
        <div class="tariff-name">SUPERVIP</div>
        <div class="tariff-icon" aria-hidden="true">💎</div>
        <h3 class="tariff-card-title">
          <span class="gold-text">SuperVIP</span>
        </h3>
        <p class="tariff-tagline">Александр Токин не только показывает — но и делает вместе с вами</p>

        <div class="tariff-price-block">
          <span class="tariff-price gold-text">50 000 ₽</span>
          <span class="tariff-period">/месяц</span>
        </div>
        <p class="tariff-total">Итого за 3 месяца: <strong>150 000 ₽</strong> (в стек входит от 231 000 ₽)</p>

        <div class="tariff-divider"></div>

        <ul class="tariff-features" role="list">
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✦</span>
            <span>Все 7 модулей с живой практикой</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✦</span>
            <span>Александр лично смотрит ваш блог и <strong>правит сам</strong> — не объясняет «подумайте над этим»</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✦</span>
            <span>Проверяет офферы и тексты — конкретные правки в ваш документ</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✦</span>
            <span>Подключается к техническим задачам — решает, а не рассказывает как</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✦</span>
            <span>Моделирует разговор с клиентом под вашу нишу и ваш голос</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✦</span>
            <span>Мозговые штурмы и разборы в группе</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✦</span>
            <span>ИИ-блок — эксклюзивно</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✦</span>
            <span>Приоритетный доступ к Александру на всё время программы</span>
          </li>
        </ul>

        <div class="tariff-bonus">
          <strong>🏆 Быстрый вызов.</strong> Первый, кто заработает больше, чем заплатил за программу — получает персональную стратегическую сессию с Александром на 3 часа (45 000 ₽). Нужно просто быть первым, кто окупился.<br><br>
          <strong>🥇 Главный вызов.</strong> Участник с наибольшим результатом за три месяца — совместная работа по созданию личного флагманского оффера.
        </div>

        <a href="https://t.me/m/iEsQljsMOTdi" class="btn-primary" style="max-width: 100%;" aria-label="Оставить заявку на SUPERVIP">
          Оставить заявку на SUPERVIP →
        </a>
        <p class="tariff-note">Гарантия возврата · Александр ответит в течение 24 часов</p>
      </div>

      <!-- STANDART -->
      <div class="tariff-card standard reveal reveal-delay-1">
        <div class="tariff-badge entry">Доступный старт</div>
        <div class="tariff-name">STANDART</div>
        <div class="tariff-icon" aria-hidden="true">🔷</div>
        <h3 class="tariff-card-title">
          <span class="silver-text">Standart</span>
        </h3>
        <p class="tariff-tagline">Александр Токин передаёт точные техники — вы применяете сами и получаете результат быстро</p>

        <div class="tariff-price-block">
          <span class="tariff-price" style="color: var(--silver-mid);">25 000 ₽</span>
          <span class="tariff-period">/месяц</span>
        </div>
        <p class="tariff-total">Итого за 3 месяца: <strong>75 000 ₽</strong> (в стек входит от 141 000 ₽)</p>

        <div class="tariff-divider"></div>

        <ul class="tariff-features" role="list">
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✓</span>
            <span>Все 7 модулей с практикой</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✓</span>
            <span>Александр показывает как проверять и улучшать блог, офферы, воронку — вы делаете сами по чёткой системе</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✓</span>
            <span>Шаблоны и техники с конкретными инструкциями применения</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✓</span>
            <span>Групповые разборы задач</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✓</span>
            <span>Мозговые штурмы в группе</span>
          </li>
          <li class="tariff-feature">
            <span class="feature-check" aria-hidden="true">✓</span>
            <span>ИИ-блок — эксклюзивно</span>
          </li>
        </ul>

        <a href="https://t.me/m/MuP4-QmSZTMy" class="btn-secondary" style="max-width: 100%; text-align: center;" aria-label="Оставить заявку на STANDART">
          Оставить заявку на STANDART →
        </a>
        <p class="tariff-note">Гарантия возврата · 25 000 ₽/месяц — это вложение, которое возвращается с умножением</p>
      </div>
    </div>

    <div class="why-supervip reveal">
      <h3>Почему большинство выбирают SUPERVIP?</h3>
      <p>Разница между тарифами — 75 000 рублей за три месяца. Это стоимость одного клиента. В формате SUPERVIP Александр лично правит ваши тексты, офферы и разборы — руками, а не объяснениями. Именно это приносит первого клиента быстрее.</p>
      <p>Человек, который выбирает лучшее для своего дела с самого старта — это уже другой тип решений. Другая скорость. Другой знак, который вы посылаете себе: <em>я серьёзно.</em></p>
    </div>

    <div class="process-note reveal">
      <h4>Как проходит заявка</h4>
      <p>Вы нажимаете кнопку → отвечаете на 5 коротких вопросов (последний: <em>«Напишите одним предложением, почему именно сейчас»</em>) → Александр Токин лично читает ваши ответы и пишет вам в Telegram в течение 24 часов. Не автоматическое письмо — живое общение.</p>
    </div>
  </div>
</section>

<!-- ===== REVIEWS ===== -->
<section class="reviews-section section-pad" id="reviews" aria-label="Отзывы">
  <div class="container">
    <p class="section-label reveal">Голоса участников</p>
    <h2 class="section-title reveal reveal-delay-1">
      Я не буду просить вас <span class="silver-text">верить мне на слово</span>
    </h2>

    <div class="reviews-list">
      <div class="review-card reveal">
        <div class="review-stars" aria-label="5 звёзд">
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
        </div>
        <p class="review-text">
          «Я часами пыталась разобраться сама — безрезультатно. Александр Токин посмотрел один скриншот, мгновенно увидел ошибку и провёл меня по всем шагам. Теперь всё работает. Невероятный профессионализм.»
        </p>
        <div class="review-author">
          <div class="review-avatar" aria-hidden="true">И</div>
          <span class="review-name">Ирина</span>
        </div>
      </div>

      <div class="review-card reveal reveal-delay-1">
        <div class="review-stars" aria-label="5 звёзд">
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
        </div>
        <p class="review-text">
          «Я запуталась в инструкциях — он нашёл ошибку, объяснил спокойно и по порядку, и результат получен.»
        </p>
        <div class="review-author">
          <div class="review-avatar" aria-hidden="true">Е</div>
          <span class="review-name">Елена</span>
        </div>
      </div>

      <div class="review-card reveal reveal-delay-2">
        <div class="review-stars" aria-label="5 звёзд">
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
          <span class="star" aria-hidden="true">★</span>
        </div>
        <p class="review-text">
          «Когда рядом такие мастера — те, кто был полным чайником, превращаются в специалистов. А потом и в экспертов.»
        </p>
        <div class="review-author">
          <div class="review-avatar" aria-hidden="true">Т</div>
          <span class="review-name">Татьяна</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ===== NOT FOR YOU ===== -->
<section class="notforyou-section section-pad" id="notforyou" aria-label="Для кого программа">
  <div class="container">
    <p class="section-label reveal">Фильтр</p>
    <h2 class="section-title reveal reveal-delay-1">Эта программа <span class="silver-text">не для вас</span>, если:</h2>

    <div class="not-for-grid">
      <div class="not-item reveal"><span class="not-icon" aria-hidden="true">✕</span>Вы ищете курс, который можно посмотреть когда-нибудь потом</div>
      <div class="not-item reveal reveal-delay-1"><span class="not-icon" aria-hidden="true">✕</span>Вы хотите знания без действий</div>
      <div class="not-item reveal reveal-delay-2"><span class="not-icon" aria-hidden="true">✕</span>Вы не готовы выделять время на шаги — даже небольшое</div>
      <div class="not-item reveal reveal-delay-3"><span class="not-icon" aria-hidden="true">✕</span>Вы уже знаете всё и вам нужно просто «добавить приёмов»</div>
      <div class="not-item reveal reveal-delay-4"><span class="not-icon" aria-hidden="true">✕</span>Вы ищете результат без собственного участия</div>
    </div>

    <h2 class="not-divider-title reveal">
      Программа <span class="gold-text">для вас</span>, если:
    </h2>

    <div class="for-grid">
      <div class="for-item reveal"><span class="for-icon" aria-hidden="true">✦</span>Вы из тех, кто не умеет «просто смириться с тем, как есть»</div>
      <div class="for-item reveal reveal-delay-1"><span class="for-icon" aria-hidden="true">✦</span>Вы готовы работать системно, не хаотично</div>
      <div class="for-item reveal reveal-delay-2"><span class="for-icon" aria-hidden="true">✦</span>Вы хотите результат — бизнес, клиентов, деньги — а не ещё одну папку материалов</div>
      <div class="for-item reveal reveal-delay-3"><span class="for-icon" aria-hidden="true">✦</span>Вы понимаете, что «позже» — самая дорогая стратегия из всех</div>
    </div>

    <p style="font-family: var(--font-display); font-size: var(--text-base); font-style: italic; color: var(--text-secondary); text-align: center; margin-top: var(--s8); line-height: 1.6;" class="reveal">
      Александр Токин лично смотрит каждую заявку. Три месяца совместной работы — это отношения, и он выбирает тех, с кем они дадут максимум.
    </p>
  </div>
</section>

<!-- ===== FAQ ===== -->
<section class="faq-section section-pad" id="faq" aria-label="Часто задаваемые вопросы">
  <div class="container">
    <p class="section-label reveal">FAQ</p>
    <h2 class="section-title reveal reveal-delay-1">
      Вы, скорее всего, уже задаёте себе <span class="silver-text">эти вопросы</span>
    </h2>

    <div class="faq-list reveal">
      <div class="faq-item">
        <button class="faq-question" aria-expanded="false">
          «50 000 рублей в месяц — это очень много»
          <span class="faq-chevron" aria-hidden="true">▾</span>
        </button>
        <div class="faq-answer" role="region">
          <div class="faq-answer-inner">
            Личная сессия со мной стоит 15 000 рублей за час. Три месяца программы — это эквивалент 15 личных сессий плюс всё остальное. Главное — это единственный формат, где я даю гарантию результата. Ваш реальный риск — ноль.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" aria-expanded="false">
          «Я уже вкладывал деньги в программы. Ни одна не дала результата»
          <span class="faq-chevron" aria-hidden="true">▾</span>
        </button>
        <div class="faq-answer" role="region">
          <div class="faq-answer-inner">
            Именно поэтому этот формат существует. В обычных программах вы платите за знания — а дальше сами. Здесь вы платите за результат, и я за него отвечаю личной гарантией. Если результата не будет — деньги вернутся к вам полностью.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" aria-expanded="false">
          «У меня нет времени ещё на одну программу»
          <span class="faq-chevron" aria-hidden="true">▾</span>
        </button>
        <div class="faq-answer" role="region">
          <div class="faq-answer-inner">
            Нет уроков, которые накапливаются и давят. Мы работаем в вашем ритме — шаг за шагом. Плюс: ИИ-блок возвращает вам 3–4 часа каждый день уже в первые недели. Большинство участников говорят, что в программе у них стало больше свободного времени, а не меньше.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" aria-expanded="false">
          «Сейчас не лучший момент — начну позже»
          <span class="faq-chevron" aria-hidden="true">▾</span>
        </button>
        <div class="faq-answer" role="region">
          <div class="faq-answer-inner">
            «Позже» — самая дорогая стратегия из всех. Каждый месяц без системы — это месяц, когда деньги не приходят, хотя вы работаете. Набор этого потока закрывается 31 марта. Лучший момент — это тот, в котором вы стоите прямо сейчас.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" aria-expanded="false">
          «А вдруг у меня не получится?»
          <span class="faq-chevron" aria-hidden="true">▾</span>
        </button>
        <div class="faq-answer" role="region">
          <div class="faq-answer-inner">
            Если не получится при соблюдении алгоритма — я верну вам деньги. Это убирает финансовый риск полностью. Страх «не получится» — это не сигнал отступить. Это сигнал, что для вас это по-настоящему важно. Значит, ресурс есть. Методология тоже. Осталось запустить.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" aria-expanded="false">
          «Что если я пропущу занятие?»
          <span class="faq-chevron" aria-hidden="true">▾</span>
        </button>
        <div class="faq-answer" role="region">
          <div class="faq-answer-inner">
            Все занятия записываются. Запись остаётся у вас навсегда — можно вернуться в любой момент. Ни одно место в алгоритме не закрывается.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" aria-expanded="false">
          «Как технически всё устроено?»
          <span class="faq-chevron" aria-hidden="true">▾</span>
        </button>
        <div class="faq-answer" role="region">
          <div class="faq-answer-inner">
            В Telegram. Живые встречи, групповые разборы, личная связь со мной — всё там. Никаких сложных платформ, личных кабинетов с паролями. Один канал, один чат, один алгоритм — и вы всегда знаете, что делать следующим.
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ===== FINAL CTA ===== -->
<section class="final-cta-section section-pad" id="final-cta" aria-label="Финальный призыв к действию">
  <div class="container">
    <h2 class="final-cta-title reveal">
      Сейчас вы стоите в точке<br>
      <span class="gold-silver-text">выбора</span>
    </h2>
    <p class="final-cta-body reveal reveal-delay-1">
      Не между двумя тарифами. Между двумя жизнями.<br><br>
      В одной — через год вы снова читаете подобный лендинг. В другой — через три месяца у вас уже есть клиенты, которые платят. Бизнес, который работает. Ощущение, что вы наконец-то идёте туда, куда хотите.
    </p>

    <div class="final-cta-deadline reveal reveal-delay-2">
      ⏰ Набор закрывается 31 марта или когда заполнятся последние места
    </div>

    <!-- Countdown timer -->
    <div class="deadline-counter reveal reveal-delay-3" id="countdown" aria-live="polite" aria-label="Обратный отсчёт до конца набора">
      <div class="counter-unit">
        <span class="counter-num" id="days">--</span>
        <span class="counter-label">Дней</span>
      </div>
      <div class="counter-unit">
        <span class="counter-num" id="hours">--</span>
        <span class="counter-label">Часов</span>
      </div>
      <div class="counter-unit">
        <span class="counter-num" id="minutes">--</span>
        <span class="counter-label">Минут</span>
      </div>
    </div>

    <div class="final-cta-buttons reveal reveal-delay-4">
      <a href="https://t.me/m/iEsQljsMOTdi" class="btn-primary" aria-label="Оставить заявку SUPERVIP — 50 000 руб./мес">
        Оставить заявку на SUPERVIP — 50 000 ₽/мес →
      </a>
      <a href="https://t.me/m/MuP4-QmSZTMy" class="btn-secondary" aria-label="Оставить заявку STANDART — 25 000 руб./мес">
        Оставить заявку на STANDART — 25 000 ₽/мес →
      </a>
      <p class="final-hint">Александр ответит лично в течение 24 часов</p>
    </div>
  </div>
</section>

<!-- ===== FOOTER ===== -->
<footer class="site-footer" role="contentinfo">
  <div class="container">
    <div class="footer-logo gold-silver-text">7 шагов к изобилию</div>
    <p class="footer-tagline">Александр Токин · Программа наставничества</p>

    <nav class="footer-links" aria-label="Навигация в подвале">
      <a href="#steps">Программа</a>
      <a href="#tariffs">Тарифы</a>
      <a href="#guarantee">Гарантия</a>
      <a href="#faq">FAQ</a>
      <a href="#reviews">Отзывы</a>
    </nav>

    <p class="footer-copy">© Александр Токин. Все права защищены.</p>
    </a>
  </div>
</footer>

<!-- ===== SCRIPTS ===== -->
<script>
// Header scroll behavior
const header = document.getElementById('site-header');
window.addEventListener('scroll', () => {
  header.classList.toggle('scrolled', window.scrollY > 50);
}, { passive: true });

// Progress bar
const progressBar = document.getElementById('progress-bar');
window.addEventListener('scroll', () => {
  const scrolled = (window.scrollY / (document.documentElement.scrollHeight - window.innerHeight)) * 100;
  progressBar.style.width = Math.min(scrolled, 100) + '%';
}, { passive: true });

// Scroll reveal
const revealObserver = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('visible');
      revealObserver.unobserve(entry.target);
    }
  });
}, { threshold: 0.12, rootMargin: '0px 0px -40px 0px' });

document.querySelectorAll('.reveal').forEach(el => revealObserver.observe(el));

// FAQ accordion
document.querySelectorAll('.faq-question').forEach(btn => {
  btn.addEventListener('click', () => {
    const item = btn.closest('.faq-item');
    const answer = item.querySelector('.faq-answer');
    const isOpen = item.classList.contains('open');

    // Close all
    document.querySelectorAll('.faq-item').forEach(i => {
      i.classList.remove('open');
      i.querySelector('.faq-answer').style.maxHeight = '0';
      i.querySelector('.faq-question').setAttribute('aria-expanded', 'false');
    });

    // Open clicked if wasn't open
    if (!isOpen) {
      item.classList.add('open');
      answer.style.maxHeight = answer.scrollHeight + 'px';
      btn.setAttribute('aria-expanded', 'true');
    }
  });
});

// Countdown to March 31
function updateCountdown() {
  const deadline = new Date('2026-03-31T23:59:59');
  const now = new Date();
  const diff = deadline - now;

  if (diff <= 0) {
    document.getElementById('days').textContent = '00';
    document.getElementById('hours').textContent = '00';
    document.getElementById('minutes').textContent = '00';
    return;
  }

  const days    = Math.floor(diff / (1000 * 60 * 60 * 24));
  const hours   = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));

  document.getElementById('days').textContent    = String(days).padStart(2, '0');
  document.getElementById('hours').textContent   = String(hours).padStart(2, '0');
  document.getElementById('minutes').textContent = String(minutes).padStart(2, '0');
}

updateCountdown();
setInterval(updateCountdown, 60000);

// Simple sparkle particles in hero
const heroBg = document.querySelector('.hero-bg-particles') || document.querySelector('.hero');
if (heroBg) {
  const colors = ['rgba(255,215,0,0.6)', 'rgba(232,232,240,0.5)', 'rgba(200,150,12,0.5)'];
  for (let i = 0; i < 18; i++) {
    const p = document.createElement('div');
    p.className = 'particle';
    const size = Math.random() * 4 + 2;
    const color = colors[Math.floor(Math.random() * colors.length)];
    p.style.cssText = `
      width: ${size}px; height: ${size}px;
      background: ${color};
      top: ${Math.random() * 100}%;
      left: ${Math.random() * 100}%;
      animation: sparkle ${Math.random() * 4 + 3}s ${Math.random() * 5}s ease-in-out infinite;
      box-shadow: 0 0 ${size * 2}px ${color};
    `;
    heroBg.appendChild(p);
  }
}
</script>

<script data-pplx-inline-edit>
(function(){
  if(window===window.top)return;
  function inlineAll(orig,clone){
    if(orig.nodeType!==1)return;
    try{
      var cs=getComputedStyle(orig);
      var t='';
      for(var i=0;i<cs.length;i++){t+=cs[i]+':'+cs.getPropertyValue(cs[i])+';';}
      clone.style.cssText=t;
    }catch(e){}
    var oc=orig.children,cc=clone.children;
    for(var j=0;j<oc.length&&j<cc.length;j++){inlineAll(oc[j],cc[j]);}
  }
  function stripExternal(clone){
    var imgs=clone.querySelectorAll('img');
    for(var i=0;i<imgs.length;i++){
      var s=imgs[i].getAttribute('src');
      if(s&&!s.startsWith('data:'))imgs[i].removeAttribute('src');
    }
    var all=clone.querySelectorAll('*');
    for(var i=0;i<all.length;i++){
      var st=all[i].style.cssText;
      if(st&&st.indexOf('url(')>=0){
        all[i].style.cssText=st.replace(/url\(["']?(?!data:)[^)"']*["']?\)/gi,'none');
      }
    }
  }
  window.addEventListener('message',function(e){
    if(!e.data||e.data.type!=='INLINE_EDIT_CAPTURE_REQUEST')return;
    var scrollX=window.scrollX||window.pageXOffset||0;
    var scrollY=window.scrollY||window.pageYOffset||0;
    var w=window.innerWidth,h=window.innerHeight;
    try{
      var clone=document.documentElement.cloneNode(true);
      var rm=clone.querySelectorAll('script,link[rel="stylesheet"],style');
      for(var i=0;i<rm.length;i++){rm[i].remove();}
      inlineAll(document.documentElement,clone);
      stripExternal(clone);
      var html=new XMLSerializer().serializeToString(clone);
      var svg='<svg xmlns="http://www.w3.org/2000/svg" width="'+w+'" height="'+h+'">'
        +'<foreignObject width="100%" height="100%">'
        +'<div xmlns="http://www.w3.org/1999/xhtml" style="width:'+w+'px;height:'+h+'px;overflow:hidden">'
        +'<div style="transform:translate(-'+scrollX+'px,-'+scrollY+'px);transform-origin:top left">'
        +html+'</div></div></foreignObject></svg>';
      var svgUrl='data:image/svg+xml;charset=utf-8,'+encodeURIComponent(svg);
      var img=new Image();
      img.onload=function(){
        var c=document.createElement('canvas');c.width=w;c.height=h;
        c.getContext('2d').drawImage(img,0,0);
        window.parent.postMessage({type:'INLINE_EDIT_SCREENSHOT_RESULT',dataUrl:c.toDataURL('image/png'),scrollX:scrollX,scrollY:scrollY},'*');
      };
      img.onerror=function(){
        window.parent.postMessage({type:'INLINE_EDIT_SCREENSHOT_RESULT',dataUrl:null,scrollX:scrollX,scrollY:scrollY},'*');
      };
      img.src=svgUrl;
    }catch(err){
      window.parent.postMessage({type:'INLINE_EDIT_SCREENSHOT_RESULT',dataUrl:null,scrollX:scrollX,scrollY:scrollY},'*');
    }
  });
})();
</script></body>
</html>
