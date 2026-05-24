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
      <circle cx="6" cy="6" r="4" fill="#7f00ff"><animate attributeName="cy" values="12;6;12" dur="1.5s" repeatCount="indefinite"/></circle>
      <circle cx="6" cy="-6" r="4" fill="#7f00ff"/>
    </g>

  <text x="50%" y="50" font-family="Segoe UI, sans-serif" font-size="26" font-weight="bold" fill="#ffffff" text-anchor="middle">
    DATA PIPELINE EXPERT
      <animate attributeName="opacity" values="0.6;1;0.6" dur="3s" repeatCount="indefinite" />
    </text>
    
   <text x="50%" y="205" font-family="Segoe UI, sans-serif" font-size="14" fill="#8b949e" text-anchor="middle" letter-spacing="2">
      LIMPEZA  •  TRANSFORMAÇÃO  •  AGRUPAMENTO
    </text>
  </svg>
</div>

<br>

<div align="center">
  <img src="https://img.shields.io/badge/Data_Engineering-Pipeline-blueviolet?style=for-the-badge&logo=apache-spark" alt="Data Pipeline">
  <img src="https://img.shields.io/badge/Python-Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/SQL-Tratamento-orange?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL">
</div>

---

## 📌 Visão Geral do Processo

A jornada dos dados brutos até a geração de inteligência passa por três fases críticas de refino. Clique nas seções interativas abaixo para explorar as mecânicas de cada etapa.

---

### 🧹 1. Limpeza de Dados (Data Cleaning)

<details>
<summary><b>📐 Clique aqui para ver como funciona a Limpeza de Dados</b></summary>
<br>

A limpeza elimina inconsistências, ruídos e erros estruturais presentes nas fontes originais.

#### Animação Conceitual: Filtragem e Remoção de Ruído
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 500 80" width="100%" style="background:#161b22; border-radius:8px;">
  <text x="30" y="45" fill="#ff5e62" font-size="12" font-family="monospace">[ERRO]</text>
  <text x="110" y="45" fill="#58a6ff" font-size="12" font-family="monospace">ID_402</text>
  <text x="190" y="45" fill="#ff5e62" font-size="12" font-family="monospace">NULL</text>
  
  <line x1="280" y1="10" x2="280" y2="70" stroke="#ff9966" stroke-width="3" stroke-dasharray="4" />
  
  <text x="340" y="45" fill="#58a6ff" font-size="12" font-family="monospace">ID_402</text>
  <text x="420" y="45" fill="#58a6ff" font-size="12" font-family="monospace">ID_403</text>
  
  <line x1="0" y1="0" x2="0" y2="80" stroke="#fff" stroke-width="2" opacity="0.4">
    <animate attributeName="x1" values="20;280;20" dur="4s" repeatCount="indefinite" />
    <animate attributeName="x2" values="20;280;20" dur="4s" repeatCount="indefinite" />
  </line>
</svg>

#### Operações Críticas:
* **Remoção de Duplicatas:** Elimina registros idênticos para não distorcer as métricas.
* **Imputação de Nulos:** Preenchimento inteligente (média, mediana ou moda) de dados ausentes.
* **Ajuste de Tipos (`Cast`):** Conversão de strings para formatos apropriados (`datetime`, `float`, `int`).
</details>

---

### ⚙️ 2. Transformação de Dados (Data Transformation)

<details>
<summary><b>📐 Clique aqui para ver como funciona a Transformação</b></summary>
<br>

Modifica o formato, escala ou a estrutura física dos dados para prepará-los para modelagem matemática.

#### Animação Conceitual: Normalização e Escalonamento (Min-Max)
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 500 100" width="100%" style="background:#161b22; border-radius:8px;">
  <text x="20" y="30" fill="#8b949e" font-size="11" font-family="sans-serif">Valores Originais (0 a 50.000)</text>
  <circle cx="50" cy="50" r="8" fill="#ff9966">
    <animate attributeName="cx" values="50;400;50" dur="3s" repeatCount="indefinite" />
  </circle>
  
  <text x="20" y="85" fill="#58a6ff" font-size="11" font-family="sans-serif">Dados Normalizados (Intervalo 0.0 a 1.0)</text>
  <line x1="50" y1="70" x2="200" y2="70" stroke="#30363d" stroke-width="4" />
  <circle cx="50" cy="70" r="5" fill="#58a6ff">
    <animate attributeName="cx" values="50;200;50" dur="3s" repeatCount="indefinite" />
  </circle>
</svg>

#### Técnicas Utilizadas:
1. **One-Hot Encoding:** Transforma categorias de texto em colunas binárias (`0` ou `1`).
2. **Padronização (Z-Score):** Ajusta os dados para possuírem média 0 e desvio padrão 1.
3. **Feature Engineering:** Criação de novas colunas de negócio (Ex: extrair o mês a partir de uma string de data).
</details>

---

### 📊 3. Agrupamento de Dados (Data Grouping)

<details>
<summary><b>📐 Clique aqui para ver como funciona o Agrupamento</b></summary>
<br>

Agrega os dados a fim de extrair resumos estatísticos através da estratégia clássica **Split-Apply-Combine**.

#### Animação Conceitual: Agregação por Categorias
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 500 120" width="100%" style="background:#161b22; border-radius:8px;">
  <g id="dispersos">
    <circle cx="40" cy="30" r="6" fill="#7f00ff" />
    <circle cx="60" cy="80" r="6" fill="#ff5e62" />
    <circle cx="80" cy="40" r="6" fill="#7f00ff" />
    <circle cx="40" cy="70" r="6" fill="#ff5e62" />
  </g>

  <path d="M 120 50 L 250 30" stroke="#30363d" stroke-width="2" stroke-dasharray="5 5">
    <animate attributeName="stroke-dashoffset" values="50;0" dur="2s" repeatCount="indefinite" />
  </path>
  <path d="M 120 70 L 250 90" stroke="#30363d" stroke-width="2" stroke-dasharray="5 5">
    <animate attributeName="stroke-dashoffset" values="50;0" dur="2s" repeatCount="indefinite" />
  </path>

  <g transform="translate(320, 35)">
    <rect x="-10" y="-15" width="120" height="30" rx="5" fill="#1f2937" stroke="#7f00ff" />
    <text x="10" y="5" fill="#fff" font-size="11" font-family="sans-serif">Grupo A: SUM(vendas)</text>
  </g>
  
  <g transform="translate(320, 85)">
    <rect x="-10" y="-15" width="120" height="30" rx="5" fill="#1f2937" stroke="#ff5e62" stroke-width="3">
      <animate attributeName="stroke" values="#ff5e62;#30363d;#ff5e62" dur="2s" repeatCount="indefinite" />
    </rect>
    <text x="10" y="5" fill="#fff" font-size="11" font-family="sans-serif">Grupo B: MEAN(idade)</text>
  </g>
</svg>

#### Funções de Agregação Comuns:
* `SUM()`: Consolidação de volumes econômicos e totais.
* `COUNT()`: Volumetria de transações ou cadastros ativos.
* `AVG()` / `MEAN()`: Identificação de comportamentos médios do ecossistema.
</details>

---

## 🛠️ Stack Tecnológica Recomendada

Abaixo estão as ferramentas líderes de mercado utilizadas para implementar este fluxo:

| Tecnologia | Função Principal | Tipo |
| :--- | :--- | :--- |
| **Python (Pandas / Polars)** | Limpeza em memória e transformações complexas | Code-based |
| **SQL (PostgreSQL / BigQuery)** | Agrupamentos massivos em Bancos de Dados | Query-based |
| **Apache Spark** | Pipelines distribuídos para Big Data | Cluster-based |

---

<div align="center">
  <sub>Desenvolvido para fins de documentação em Engenharia de Dados. Sinta-se livre para clonar e adaptar! 🚀</sub>
</div>
