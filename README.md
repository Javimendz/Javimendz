<!-- ============================================================
  README de perfil de GitHub (versión visual).
  Necesita en la raíz del repositorio: header.svg y divider.svg.
  Los comentarios "VERIFICA" no se ven en la página: confirma que
  esos datos son ciertos y que puedes defenderlos en una entrevista.
  La sección de proyectos está comentada: descoméntala al rellenarla.
============================================================ -->

<div align="center">

<svg xmlns="http://www.w3.org/2000/svg" width="1200" height="340" viewBox="0 0 1200 340" fill="none">
  <defs>
    <!-- Gradientes sólidos y profundos -->
    <linearGradient id="bgGrad" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0B1B33"/>
      <stop offset="55%" stop-color="#11294D"/>
      <stop offset="100%" stop-color="#0A1524"/>
    </linearGradient>

    <linearGradient id="accentGrad" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#3B82F6"/>
      <stop offset="50%" stop-color="#22D3EE"/>
      <stop offset="100%" stop-color="#6366F1"/>
    </linearGradient>

    <linearGradient id="textGrad" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#E6F0FF"/>
      <stop offset="100%" stop-color="#A9C7FF"/>
    </linearGradient>

    <!-- Resplandor -->
    <filter id="glow" x="-40%" y="-40%" width="180%" height="180%">
      <feGaussianBlur stdDeviation="6" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Máscara para barrido de línea -->
    <clipPath id="lineClip">
      <rect x="0" y="0" width="1200" height="340"/>
    </clipPath>
  </defs>

  <!-- Fondo -->
  <rect width="1200" height="340" rx="18" fill="url(#bgGrad)"/>

  <!-- Rejilla sutil animada (opcional, elegante) -->
  <g opacity="0.07" stroke="#9CC4FF" stroke-width="1">
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none"/>
    </pattern>
    <rect width="1200" height="340" fill="url(#grid)">
      <animate attributeName="x" from="0" to="40" dur="6s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- Borde luminoso animado -->
  <rect x="2" y="2" width="1196" height="336" rx="16" fill="none"
        stroke="url(#accentGrad)" stroke-width="2.5" opacity="0.9">
    <animate attributeName="opacity" values="0.55;1;0.55" dur="4s" repeatCount="indefinite"/>
  </rect>

  <!-- Barra lateral de acento con pulso -->
  <rect x="0" y="0" width="10" height="340" fill="url(#accentGrad)">
    <animate attributeName="height" values="340;340" dur="1s" repeatCount="indefinite"/>
  </rect>

  <!-- Avatar / Monograma -->
  <g transform="translate(90, 120)">
    <circle cx="50" cy="50" r="48" fill="#0F2444" stroke="url(#accentGrad)" stroke-width="3" filter="url(#glow)">
      <animate attributeName="r" values="48;50;48" dur="3.5s" repeatCount="indefinite"/>
    </circle>
    <text x="50" y="63" text-anchor="middle"
          font-family="'Fira Code', 'Segoe UI', monospace"
          font-size="34" font-weight="700" fill="url(#accentGrad)">JM</text>
  </g>

  <!-- Nombre -->
  <text x="200" y="140"
        font-family="'Inter', 'Segoe UI', 'Helvetica Neue', sans-serif"
        font-size="52" font-weight="800" fill="url(#textGrad)"
        letter-spacing="1.5">
    Javier Méndez
    <animate attributeName="opacity" values="0.92;1;0.92" dur="5s" repeatCount="indefinite"/>
  </text>

  <!-- Subtítulo -->
  <text x="202" y="182"
        font-family="'Fira Code', 'Segoe UI', monospace"
        font-size="21" font-weight="500" fill="#7FB3FF"
        letter-spacing="0.8">
    Junior Backend Developer
  </text>

  <!-- Stack: badges con aparición escalonada -->
  <g font-family="'Fira Code', monospace" font-size="15" font-weight="600" fill="#0B1B33">
    <g transform="translate(200, 218)">
      <rect width="98" height="34" rx="17" fill="#7FB3FF">
        <animate attributeName="opacity" values="0;1" begin="0.2s" dur="0.8s" fill="freeze"/>
      </rect>
      <text x="49" y="23" text-anchor="middle">Java</text>
    </g>
    <g transform="translate(310, 218)">
      <rect width="140" height="34" rx="17" fill="#8FD3FF">
        <animate attributeName="opacity" values="0;1" begin="0.45s" dur="0.8s" fill="freeze"/>
      </rect>
      <text x="70" y="23" text-anchor="middle">Spring Boot</text>
    </g>
    <g transform="translate(462, 218)">
      <rect width="130" height="34" rx="17" fill="#A7B7FF">
        <animate attributeName="opacity" values="0;1" begin="0.7s" dur="0.8s" fill="freeze"/>
      </rect>
      <text x="65" y="23" text-anchor="middle">TypeScript</text>
    </g>
    <g transform="translate(604, 218)">
      <rect width="96" height="34" rx="17" fill="#9EE6FF">
        <animate attributeName="opacity" values="0;1" begin="0.95s" dur="0.8s" fill="freeze"/>
      </rect>
      <text x="48" y="23" text-anchor="middle">Python</text>
    </g>
    <g transform="translate(712, 218)">
      <rect width="72" height="34" rx="17" fill="#C0C9FF">
        <animate attributeName="opacity" values="0;1" begin="1.2s" dur="0.8s" fill="freeze"/>
      </rect>
      <text x="36" y="23" text-anchor="middle">C#</text>
    </g>
    <g transform="translate(796, 218)">
      <rect width="150" height="34" rx="17" fill="#8FE6D2">
        <animate attributeName="opacity" values="0;1" begin="1.45s" dur="0.8s" fill="freeze"/>
      </rect>
      <text x="75" y="23" text-anchor="middle">IA · Big Data</text>
    </g>
  </g>

  <!-- Línea de barrido animada -->
  <g clip-path="url(#lineClip)" opacity="0.7">
    <rect x="-300" y="300" width="260" height="3" fill="url(#accentGrad)">
      <animate attributeName="x" from="-300" to="1200" dur="4.5s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- Puntos de acento animados (esquinas) -->
  <circle cx="1160" cy="40" r="4" fill="#22D3EE">
    <animate attributeName="opacity" values="0.3;1;0.3" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1130" cy="40" r="4" fill="#6366F1">
    <animate attributeName="opacity" values="1;0.3;1" dur="2.5s" repeatCount="indefinite"/>
  </circle>
</svg>
</div>
<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=500&size=22&pause=1200&color=36BCF7&center=true&vCenter=true&width=620&height=45&lines=Junior+Backend+Developer;Java+%C2%B7+Spring+Boot+%C2%B7+TypeScript+%C2%B7+Python+%C2%B7+C%23;IA+%26+Big+Data" alt="Typing SVG" />

<br><br>

<a href="https://www.linkedin.com/in/javiermendz/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:javiermendez.dev00@gmail.com" target="_blank"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://github.com/javimendz" target="_blank"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>

<br><br>

<img src="https://img.shields.io/badge/Disponible_para_trabajar-Backend-2ea44f?style=flat-square&logo=checkmarx&logoColor=white" alt="Disponible" />
<img src="https://img.shields.io/badge/Modalidad-Cualquiera-blue?style=flat-square" alt="Modalidad: cualquiera" />
<img src="https://img.shields.io/badge/Idiomas-Espa%C3%B1ol_%C2%B7_Ingl%C3%A9s-orange?style=flat-square" alt="Idiomas" />
<img src="https://komarev.com/ghpvc/?username=javimendz&label=Visitas&color=0e75b6&style=flat-square" alt="Visitas al perfil" />

</div>

<div align="center"><img src="divider.svg" alt="" width="100%" /></div>

## 👋 Sobre mí

Desarrollador backend junior, apasionado por las arquitecturas sólidas, las APIs bien diseñadas y los sistemas escalables. Busco un equipo donde aprender de perfiles con más experiencia, trabajar en proyectos reales y crecer.

| | |
|---|---|
| 🎓 **Formación** | Técnico Superior en DAM · Ingeniería Informática (UMU) · Especialización en IA & Big Data <!-- VERIFICA: título y estado de cada estudio --> |
| 💼 **Experiencia** | 1 año en desarrollo backend con Docker, despliegues cloud y pipelines CI/CD <!-- VERIFICA: cuánto fue prácticas y cuánto trabajo; sé preciso --> |
| 🎯 **Busco** | Mi próximo puesto como desarrollador backend |
| 🌱 **Aprendiendo ahora** | Go, y análisis de datos con pandas y NumPy |
| 📚 **Me interesa** | Arquitectura de software, optimización de rendimiento, procesamiento de datos e IA aplicada |
| 🗣️ **Idiomas** | Español · Inglés <!-- VERIFICA: añade tu nivel de inglés (por ejemplo B2) --> |
| ⚡ **Dato curioso** | El código limpio y la mejora continua son mi rutina, en la pantalla y en el gimnasio 🏋️‍♂️ |

<div align="center"><img src="divider.svg" alt="" width="100%" /></div>

## 🛠️ Stack

<div align="center">

**💻 Lenguajes**

<img src="https://skillicons.dev/icons?i=java,ts,js,py,cs&perline=10" alt="Lenguajes" />

**⚙️ Backend y bases de datos**

<img src="https://skillicons.dev/icons?i=spring,nestjs,nodejs,postgres&perline=10" alt="Backend y bases de datos" />

**🚢 DevOps y cloud**

<img src="https://skillicons.dev/icons?i=docker,git,githubactions&perline=10" alt="DevOps y cloud" />

**🧰 Herramientas**

<img src="https://skillicons.dev/icons?i=idea,vscode,postman,androidstudio&perline=10" alt="Herramientas" />

**🌱 Aprendiendo**

<img src="https://skillicons.dev/icons?i=go,pandas,numpy&perline=10" alt="Aprendiendo" />

</div>

<div align="center"><img src="divider.svg" alt="" width="100%" /></div>

<!-- ============================================================
## 🚀 Proyectos destacados

Con dos o tres bien explicados basta: qué hace, con qué tecnologías
y cómo ejecutarlo. Enlaza cada uno a su repositorio.

| Proyecto | Descripción | Tecnologías |
|---|---|---|
| [Nombre](https://github.com/javimendz/repo) | Qué problema resuelve, en una línea | Java, Spring Boot, PostgreSQL, Docker |
| [Nombre](https://github.com/javimendz/repo) | Qué problema resuelve, en una línea | Go, PostgreSQL |
| [Nombre](https://github.com/javimendz/repo) | Qué problema resuelve, en una línea | Python, pandas |
============================================================ -->

## 📊 Actividad en GitHub

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=javimendz&show_icons=true&theme=tokyonight&hide_border=true&locale=es" alt="Estadísticas de GitHub" height="170" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=javimendz&layout=compact&theme=tokyonight&hide_border=true&locale=es" alt="Lenguajes más usados" height="170" />

<br>

<img src="https://streak-stats.demolab.com/?user=javimendz&theme=tokyonight&hide_border=true" alt="Racha de GitHub" />

<br><br>

<img src="https://raw.githubusercontent.com/javimendz/javimendz/output/grid-snake.svg" alt="snake" />

</div>

<div align="center"><img src="divider.svg" alt="" width="100%" /></div>

## 🌍 In English

Junior backend developer with a background in multiplatform application development (DAM), computer engineering (UMU) and a specialization in AI and Big Data. I work with Java (Spring Boot), TypeScript (NestJS), Python and C#, and I am currently learning Go. I am looking for my next backend role.

<div align="center">

### 🤝 Conecta conmigo

¿Tienes un proyecto o una oferta backend? Escríbeme por [LinkedIn](https://www.linkedin.com/in/javiermendz/) o a [javiermendez.dev00@gmail.com](mailto:javiermendez.dev00@gmail.com).

<img src="divider.svg" alt="" width="100%" />

</div>
