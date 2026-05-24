# Pandas_intro_ex-2
Limpeza, Transformação e Agrupamento de dados


<div align="center">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 240" width="100%" style="max-width:800px; background:#0d1117; border-radius:12px; border: 1px solid #30363d;">
    <defs>
      <linearGradient id="pipeline-grad" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#ff5e62" />
        <stop offset="50%" stop-color="#ff9966" />
        <stop offset="100%" stop-color="#7f00ff" />
      </linearGradient>
    </defs>

  <path d="M 100 120 L 700 120" stroke="#30363d" stroke-width="4" />
  <path d="M 100 120 L 700 120" stroke="url(#pipeline-grad)" stroke-width="4" stroke-dasharray="30 150">
      <animate attributeName="stroke-dashoffset" values="360;0" dur="4s" repeatCount="indefinite" />
    </path>

   <circle cx="0" cy="0" r="6" fill="#ff5e62">
      <animateMotion path="M 100 120 L 700 120" dur="3s" repeatCount="indefinite" />
    </circle>
    <circle cx="0" cy="0" r="4" fill="#7f00ff">
      <animateMotion path="M 100 120 L 700 120" dur="2s" begin="0.5s" repeatCount="indefinite" />
    </circle>

  <g transform="translate(200, 120)">
      <circle cx="0" cy="0" r="24" fill="#1f2937" stroke="#ff5e62" stroke-width="3">
        <animate attributeName="r" values="24;28;24" dur="2s" repeatCount="indefinite" />
      </circle>
      <text x="0" y="5" font-family="Segoe UI, sans-serif" font-size="12" fill="#fff" font-weight="bold" text-anchor="middle">🧹</text>
    </g>

   <g transform="translate(400, 120)">
     <rect x="-20" y="-20" width="40" height="40" rx="6" fill="#1f2937" stroke="#ff9966" stroke-width="3">
        <animateTransform attributeName="transform" type="rotate" values="0;180;360" dur="6s" repeatCount="indefinite" />
      </rect>
      <text x="0" y="5" font-family="Segoe UI, sans-serif" font-size="12" fill="#fff" font-weight="bold" text-anchor="middle">⚙️</text>
    </g>

  <g transform="translate(600, 120)">
      <circle cx="0" cy="0" r="24" fill="#1f2937" stroke="#7f00ff" stroke-width="3" />
      <circle cx="-6" cy="-6" r="4" fill="#7f00ff"><animate attributeName="cx" values="-12;-6;-12" dur="1.5s" repeatCount="indefinite"/></circle>
      <circle cx="6" cy="6" r="4"
