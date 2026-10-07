<div align="center">

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--              SAI MADANAPALLI • DATA INTELLIGENCE               -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<svg width="100%" height="430" viewBox="0 0 1000 430"
     xmlns="http://www.w3.org/2000/svg">

<defs>

  <!-- Background -->
  <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%" stop-color="#030508"/>
    <stop offset="50%" stop-color="#07111c"/>
    <stop offset="100%" stop-color="#020406"/>
  </linearGradient>

  <!-- Cyan glow -->
  <filter id="glow">
    <feGaussianBlur stdDeviation="4" result="blur"/>
    <feMerge>
      <feMergeNode in="blur"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>

  <!-- Grid -->
  <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
    <path d="M40 0H0V40" fill="none" stroke="#00D9FF" stroke-opacity=".08"/>
  </pattern>

  <!-- Gradient -->
  <linearGradient id="cyan" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0%" stop-color="#00D9FF"/>
    <stop offset="100%" stop-color="#6EF3FF"/>
  </linearGradient>

</defs>

<!-- BACKGROUND -->
<rect width="1000" height="430" rx="25" fill="url(#bg)"/>
<rect width="1000" height="430" rx="25" fill="url(#grid)"/>

<!-- TOP BAR -->
<rect x="25" y="22" width="950" height="48" rx="12"
      fill="#08131E" stroke="#00D9FF" stroke-opacity=".35"/>

<circle cx="50" cy="46" r="6" fill="#00D9FF">
  <animate attributeName="opacity"
           values="1;.2;1" dur="1.5s" repeatCount="indefinite"/>
</circle>

<text x="70" y="51"
      fill="#FFFFFF"
      font-family="monospace"
      font-size="17"
      font-weight="bold">
DATA INTELLIGENCE LAB
</text>

<text x="945" y="51"
      fill="#00D9FF"
      text-anchor="end"
      font-family="monospace"
      font-size="13">
SYSTEM ONLINE
</text>

<!-- NAME -->
<text x="55" y="115"
      fill="#FFFFFF"
      font-family="monospace"
      font-size="34"
      font-weight="bold">
SAI MADANAPALLI
</text>

<text x="57" y="143"
      fill="#00D9FF"
      font-family="monospace"
      font-size="15">
DATA ANALYST • PYTHON • SQL • POWER BI • EXCEL
</text>

<!-- MOVING DATA PARTICLES -->

<g fill="#00D9FF" filter="url(#glow)">

<circle cx="160" cy="180" r="3">
  <animate attributeName="cx"
           values="160;850;160"
           dur="7s"
           repeatCount="indefinite"/>
</circle>

<circle cx="400" cy="210" r="2">
  <animate attributeName="cx"
           values="400;900;400"
           dur="5s"
           repeatCount="indefinite"/>
</circle>

<circle cx="700" cy="175" r="3">
  <animate attributeName="cx"
           values="700;100;700"
           dur="8s"
           repeatCount="indefinite"/>
</circle>

</g>

<!-- KPI 1 -->
<rect x="55" y="175" width="205" height="85" rx="14"
      fill="#08131E"
      stroke="#00D9FF"
      stroke-opacity=".35"/>

<text x="75" y="200"
      fill="#7D93A5"
      font-family="monospace"
      font-size="12">
ANALYTICS
</text>

<text x="75" y="232"
      fill="#FFFFFF"
      font-family="monospace"
      font-size="27"
      font-weight="bold">
DATA
</text>

<text x="75" y="250"
      fill="#00D9FF"
      font-family="monospace"
      font-size="11">
INSIGHT ENGINE
</text>

<!-- KPI 2 -->
<rect x="280" y="175" width="205" height="85" rx="14"
      fill="#08131E"
      stroke="#00D9FF"
      stroke-opacity=".35"/>

<text x="300" y="200"
      fill="#7D93A5"
      font-family="monospace"
      font-size="12">
CORE SKILL
</text>

<text x="300" y="232"
      fill="#FFFFFF"
      font-family="monospace"
      font-size="25"
      font-weight="bold">
SQL
</text>

<text x="300" y="250"
      fill="#00D9FF"
      font-family="monospace"
      font-size="11">
QUERY • ANALYZE
</text>

<!-- KPI 3 -->
<rect x="505" y="175" width="205" height="85" rx="14"
      fill="#08131E"
      stroke="#00D9FF"
      stroke-opacity=".35"/>

<text x="525" y="200"
      fill="#7D93A5"
      font-family="monospace"
      font-size="12">
PROGRAMMING
</text>

<text x="525" y="232"
      fill="#FFFFFF"
      font-family="monospace"
      font-size="25"
      font-weight="bold">
PYTHON
</text>

<text x="525" y="250"
      fill="#00D9FF"
      font-family="monospace"
      font-size="11">
CLEAN • ANALYZE
</text>

<!-- KPI 4 -->
<rect x="730" y="175" width="215" height="85" rx="14"
      fill="#08131E"
      stroke="#00D9FF"
      stroke-opacity=".35"/>

<text x="750" y="200"
      fill="#7D93A5"
      font-family="monospace"
      font-size="12">
BI ENGINE
</text>

<text x="750" y="232"
      fill="#FFFFFF"
      font-family="monospace"
      font-size="25"
      font-weight="bold">
POWER BI
</text>

<text x="750" y="250"
      fill="#00D9FF"
      font-family="monospace"
      font-size="11">
DASHBOARD • DAX
</text>

<!-- TERMINAL -->
<rect x="55" y="285" width="890" height="105" rx="15"
      fill="#03070B"
      stroke="#00D9FF"
      stroke-opacity=".3"/>

<circle cx="78" cy="307" r="5" fill="#00D9FF"/>
<circle cx="96" cy="307" r="5" fill="#31515F"/>
<circle cx="114" cy="307" r="5" fill="#31515F"/>

<text x="75" y="335"
      fill="#00D9FF"
      font-family="monospace"
      font-size="13">
$ sql.run()
</text>

<text x="75" y="357"
      fill="#FFFFFF"
      font-family="monospace"
      font-size="13">
SELECT insight FROM data
</text>

<text x="75" y="378"
      fill="#7D93A5"
      font-family="monospace"
      font-size="12">
&gt; cleaning...  analyzing...  visualizing...  ✓ insight ready
</text>

<!-- FOOTER LINE -->
<line x1="55" y1="407" x2="945" y2="407"
      stroke="#00D9FF"
      stroke-opacity=".25"/>

<text x="55" y="421"
      fill="#607684"
      font-family="monospace"
      font-size="10">
BUILD • ANALYZE • VISUALIZE • IMPROVE
</text>

<text x="945" y="421"
      fill="#00D9FF"
      text-anchor="end"
      font-family="monospace"
      font-size="10">
v2026
</text>

</svg>

<br>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2800&pause=700&color=00D9FF&center=true&vCenter=true&width=850&lines=Turning+Raw+Data+Into+Meaningful+Insights;Python+%7C+SQL+%7C+Power+BI+%7C+Excel;Clean+Data.+Find+Patterns.+Tell+Stories.;Building+My+Career+Around+Data." />

</div>

---

# 👨‍💻 `ABOUT_ME`

Hi, I'm **Sai Madanapalli**, an aspiring **Data Analyst** focused on transforming raw data into meaningful business insights.

I enjoy working with data, discovering patterns, building dashboards, and communicating insights through clear visualizations.

```text
╭────────────────────────────────────────────────────────╮
│                                                        │
│   DATA → QUESTIONS → ANALYSIS → VISUALIZATION         │
│                         ↓                              │
│                      INSIGHTS                          │
│                         ↓                              │
│                     DECISIONS                          │
│                                                        │
╰────────────────────────────────────────────────────────╯
```

---

# ⚡ `SKILL_MATRIX`

<div align="center">

| AREA | TECHNOLOGIES |
|:---:|:---|
| 🐍 **Programming** | Python • Pandas • NumPy |
| 🗄️ **Database** | SQL • MySQL • PostgreSQL |
| 📊 **BI** | Power BI • DAX |
| 📗 **Spreadsheet** | Microsoft Excel |
| 📈 **Analytics** | Data Cleaning • EDA • KPI Analysis |
| 📉 **Visualization** | Charts • Dashboards • Data Storytelling |
| 🛠️ **Tools** | Git • GitHub • Jupyter Notebook • VS Code |

</div>

---

# 🧠 `ANALYTICS_ENGINE`

```text
              ┌─────────────────┐
              │    RAW DATA     │
              └────────┬────────┘
                       ↓
              ┌─────────────────┐
              │  DATA CLEANING  │
              └────────┬────────┘
                       ↓
              ┌─────────────────┐
              │     PYTHON      │
              └────────┬────────┘
                       ↓
              ┌─────────────────┐
              │       SQL       │
              └────────┬────────┘
                       ↓
              ┌─────────────────┐
              │    POWER BI     │
              └────────┬────────┘
                       ↓
              ┌─────────────────┐
              │    INSIGHTS     │
              └─────────────────┘
```

---

# 🖥️ `SQL_TERMINAL`

```sql
-- DATA ANALYST MODE

SELECT
    skill,
    mindset,
    curiosity
FROM analyst
WHERE passion = 'DATA'
ORDER BY growth DESC;
```

```text
┌──────────────────────────────────────────────┐
│ QUERY STATUS                                 │
├──────────────────────────────────────────────┤
│ ✓ DATA CONNECTED                             │
│ ✓ QUERY EXECUTED                             │
│ ✓ PATTERNS FOUND                             │
│ ✓ INSIGHTS GENERATED                         │
└──────────────────────────────────────────────┘
```

---

# 📊 `DATA_TOOLKIT`

<div align="center">

<img src="https://skillicons.dev/icons?i=python,mysql,postgresql,git,github,vscode,jupyter&theme=dark"/>

<br><br>

<img src="https://img.shields.io/badge/Python-Analytics-00D9FF?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL-Querying-00D9FF?style=for-the-badge&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/Power%20BI-Business%20Intelligence-00D9FF?style=for-the-badge&logo=powerbi&logoColor=white"/>
<img src="https://img.shields.io/badge/Excel-Data%20Analysis-00D9FF?style=for-the-badge&logo=microsoftexcel&logoColor=white"/>

</div>

---

# 📈 `GITHUB_ANALYTICS`

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=stej07033&show_icons=true&hide_border=true&bg_color=050505&title_color=00D9FF&icon_color=00D9FF&text_color=FFFFFF&include_all_commits=true&count_private=true"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=stej07033&layout=compact&hide_border=true&bg_color=050505&title_color=00D9FF&text_color=FFFFFF&langs_count=8"/>

<br><br>

<img src="https://streak-stats.demolab.com?user=stej07033&hide_border=true&background=050505&ring=00D9FF&fire=00D9FF&currStreakLabel=00D9FF&sideLabels=FFFFFF&dates=888888&currStreakNum=FFFFFF&sideNums=FFFFFF"/>

</div>

---

# 🎯 `CURRENT_FOCUS`

```text
┌──────────────────────────────────────────────────┐
│                                                  │
│  ████████████████████░░  PYTHON                 │
│  █████████████████████░  SQL                    │
│  ███████████████████░░░  POWER BI               │
│  ████████████████████░░  EXCEL                  │
│  █████████████████░░░░░  DATA ANALYTICS         │
│                                                  │
└──────────────────────────────────────────────────┘
```

**Learning → Building → Analyzing → Improving**

---

# 💡 `MY_MINDSET`

> **Don't just look at the numbers. Understand the story behind them.**

```text
CURIOUS
   ↓
ASK
   ↓
ANALYZE
   ↓
DISCOVER
   ↓
VISUALIZE
   ↓
EXPLAIN
   ↓
IMPACT
```

---

# 🌐 `CONNECT`

<div align="center">

<a href="https://github.com/stej07033">
<img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=00D9FF"/>
</a>

<a href="https://www.linkedin.com/in/madanapalli-sai-19b835389/">
<img src="https://img.shields.io/badge/LinkedIn-000000?style=for-the-badge&logo=linkedin&logoColor=00D9FF"/>
</a>

<a href="mailto:stej07033@gmail.com">
<img src="https://img.shields.io/badge/Email-000000?style=for-the-badge&logo=gmail&logoColor=00D9FF"/>
</a>

<br><br>

### `OPEN TO DATA ANALYST OPPORTUNITIES`

**Python • SQL • Power BI • Excel • Data Analytics**

<br>

<img src="https://capsule-render.vercel.app/api?type=waving&height=120&color=0:00D9FF,50:07111f,100:050505&section=footer"/>

</div>
