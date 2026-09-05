```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Sai Tej | Data Analyst Portfolio</title>

<meta name="description"
      content="Sai Tej - Aspiring Data Analyst Portfolio | SQL | Python | Excel | Power BI | Tableau">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:Arial, Helvetica, sans-serif;
    background:#07111f;
    color:#f5f7fa;
    line-height:1.6;
}

/* NAVBAR */

nav{
    position:fixed;
    top:0;
    width:100%;
    z-index:1000;
    background:rgba(7,17,31,.92);
    backdrop-filter:blur(12px);
    border-bottom:1px solid #1d2b3d;
}

.nav-container{
    max-width:1200px;
    margin:auto;
    padding:18px 25px;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    font-size:24px;
    font-weight:bold;
    color:#4cc9f0;
}

.nav-links{
    display:flex;
    gap:25px;
    list-style:none;
}

.nav-links a{
    color:#dce6f2;
    text-decoration:none;
    font-size:15px;
    transition:.3s;
}

.nav-links a:hover{
    color:#4cc9f0;
}

/* HERO */

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:120px 20px 80px;
    background:
    radial-gradient(circle at 50% 30%, #12365a 0%, #07111f 55%);
}

.hero-content{
    max-width:900px;
}

.profile-circle{
    width:130px;
    height:130px;
    border-radius:50%;
    margin:0 auto 25px;
    display:flex;
    align-items:center;
    justify-content:center;
    background:linear-gradient(135deg,#4cc9f0,#4361ee);
    font-size:48px;
    font-weight:bold;
    box-shadow:0 0 50px rgba(76,201,240,.25);
}

.hero h1{
    font-size:58px;
    margin-bottom:10px;
}

.hero h1 span{
    color:#4cc9f0;
}

.hero h2{
    font-size:25px;
    color:#b9c7d8;
    margin-bottom:20px;
}

.hero p{
    max-width:700px;
    margin:auto;
    color:#9fb0c3;
    font-size:18px;
}

.buttons{
    margin-top:30px;
    display:flex;
    justify-content:center;
    gap:15px;
    flex-wrap:wrap;
}

.btn{
    padding:13px 25px;
    border-radius:8px;
    text-decoration:none;
    font-weight:bold;
    transition:.3s;
}

.primary{
    background:#4cc9f0;
    color:#06101d;
}

.secondary{
    border:1px solid #4cc9f0;
    color:#4cc9f0;
}

.btn:hover{
    transform:translateY(-3px);
}

/* SECTION */

section{
    max-width:1200px;
    margin:auto;
    padding:90px 25px;
}

.section-title{
    text-align:center;
    font-size:38px;
    margin-bottom:15px;
}

.section-subtitle{
    text-align:center;
    color:#94a6b9;
    margin-bottom:50px;
}

/* ABOUT */

.about{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:40px;
}

.about-card{
    background:#0c1929;
    border:1px solid #1c3046;
    padding:30px;
    border-radius:15px;
}

.about-card h3{
    color:#4cc9f0;
    margin-bottom:15px;
}

.about-card p{
    color:#b3c0ce;
}

/* SKILLS */

.skills{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:20px;
}

.skill-card{
    background:#0c1929;
    border:1px solid #1c3046;
    padding:25px;
    border-radius:14px;
    text-align:center;
    transition:.3s;
}

.skill-card:hover{
    transform:translateY(-7px);
    border-color:#4cc9f0;
}

.skill-icon{
    font-size:40px;
    margin-bottom:12px;
}

.skill-card h3{
    margin-bottom:8px;
}

.skill-card p{
    color:#91a3b7;
    font-size:14px;
}

/* PROJECTS */

.projects{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
}

.project{
    background:#0c1929;
    border:1px solid #1c3046;
    border-radius:16px;
    overflow:hidden;
    transition:.35s;
}

.project:hover{
    transform:translateY(-8px);
    box-shadow:0 15px 40px rgba(0,0,0,.3);
    border-color:#4cc9f0;
}

.project-image{
    height:190px;
    background:#101f31;
    display:flex;
    align-items:center;
    justify-content:center;
    overflow:hidden;
}

.project-image img{
    width:100%;
    height:100%;
    object-fit:cover;
}

.placeholder{
    font-size:65px;
}

.project-content{
    padding:25px;
}

.project-content h3{
    font-size:22px;
    margin-bottom:8px;
}

.project-content .type{
    color:#4cc9f0;
    font-size:14px;
    font-weight:bold;
    margin-bottom:15px;
}

.project-content p{
    color:#9dafc1;
    font-size:14px;
    margin-bottom:18px;
}

.tags{
    display:flex;
    flex-wrap:wrap;
    gap:7px;
    margin-bottom:20px;
}

.tag{
    padding:5px 9px;
    background:#13253a;
    border-radius:5px;
    color:#bcd0e4;
    font-size:12px;
}

.project-btn{
    display:inline-block;
    padding:9px 15px;
    background:#4cc9f0;
    color:#06101d;
    text-decoration:none;
    border-radius:6px;
    font-weight:bold;
    font-size:13px;
}

/* WORKFLOW */

.workflow{
    display:flex;
    justify-content:center;
    align-items:center;
    flex-wrap:wrap;
    gap:12px;
}

.workflow-step{
    background:#0c1929;
    border:1px solid #1c3046;
    padding:18px 22px;
    border-radius:10px;
    color:#c5d2df;
}

.arrow{
    color:#4cc9f0;
    font-size:22px;
}

/* KPI */

.kpis{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:20px;
}

.kpi{
    text-align:center;
    background:#0c1929;
    border:1px solid #1c3046;
    padding:30px 15px;
    border-radius:12px;
}

.kpi-number{
    font-size:35px;
    color:#4cc9f0;
    font-weight:bold;
}

.kpi p{
    color:#93a5b8;
}

/* CONTACT */

.contact{
    text-align:center;
}

.contact p{
    max-width:650px;
    margin:15px auto;
    color:#9fb0c3;
}

.socials{
    margin-top:25px;
    display:flex;
    justify-content:center;
    gap:15px;
    flex-wrap:wrap;
}

.social{
    padding:12px 22px;
    border:1px solid #2a425c;
    border-radius:7px;
    color:#d7e2ee;
    text-decoration:none;
}

.social:hover{
    border-color:#4cc9f0;
    color:#4cc9f0;
}

/* FOOTER */

footer{
    text-align:center;
    border-top:1px solid #1c3046;
    padding:30px;
    color:#74869a;
}

/* RESPONSIVE */

@media(max-width:900px){

    .projects{
        grid-template-columns:repeat(2,1fr);
    }

    .skills{
        grid-template-columns:repeat(2,1fr);
    }

    .kpis{
        grid-template-columns:repeat(2,1fr);
    }

    .hero h1{
        font-size:45px;
    }

}

@media(max-width:600px){

    .nav-links{
        display:none;
    }

    .about{
        grid-template-columns:1fr;
    }

    .projects{
        grid-template-columns:1fr;
    }

    .skills{
        grid-template-columns:1fr;
    }

    .kpis{
        grid-template-columns:1fr;
    }

    .hero h1{
        font-size:38px;
    }

}

</style>
</head>

<body>

<!-- NAVBAR -->

<nav>
<div class="nav-container">

<div class="logo">SAI M</div>

<ul class="nav-links">
<li><a href="#about">About</a></li>
<li><a href="#skills">Skills</a></li>
<li><a href="#projects">Projects</a></li>
<li><a href="#workflow">Workflow</a></li>
<li><a href="#contact">Contact</a></li>
</ul>

</div>
</nav>


<!-- HERO -->

<header class="hero">

<div class="hero-content">

<div class="profile-circle">
SM
</div>

<h1>Hi, I'm <span>Sai Tej</span></h1>

<h2>📊 Aspiring Data Analyst</h2>

<p>
I transform raw data into meaningful insights using
SQL, Python, Excel, Power BI and Tableau.
I build real-world analytics projects focused on
business problems, KPIs and data-driven decisions.
</p>

<div class="buttons">

<a class="btn primary"
   href="https://github.com/stej07033"
   target="_blank">
View GitHub
</a>

<a class="btn secondary"
   href="https://www.linkedin.com/in/madanapalli-sai-19b835389"
   target="_blank">
LinkedIn
</a>

</div>

</div>

</header>


<!-- ABOUT -->

<section id="about">

<h2 class="section-title">About Me</h2>

<p class="section-subtitle">
Turning data into insights and insights into decisions.
</p>

<div class="about">

<div class="about-card">

<h3>👨‍💻 Who I Am</h3>

<p>
I am an aspiring Data Analyst with a background in
Mechanical Engineering and a strong interest in
data analytics and business intelligence.
</p>

<br>

<p>
I enjoy cleaning datasets, writing SQL queries,
performing exploratory analysis, developing KPIs
and building interactive dashboards.
</p>

</div>

<div class="about-card">

<h3>🎯 Career Goal</h3>

<p>
My goal is to work as a Data Analyst where I can
use analytical thinking and technical skills to
solve real-world business problems.
</p>

<br>

<p>
I am currently building practical projects using
SQL, Python, Excel and Power BI while continuously
improving my analytical skills.
</p>

</div>

</div>

</section>


<!-- SKILLS -->

<section id="skills">

<h2 class="section-title">Technical Skills</h2>

<p class="section-subtitle">
Tools I use to analyze, visualize and communicate data.
</p>

<div class="skills">

<div class="skill-card">
<div class="skill-icon">🐍</div>
<h3>Python</h3>
<p>Pandas • NumPy • Matplotlib • Seaborn • EDA</p>
</div>

<div class="skill-card">
<div class="skill-icon">🗄️</div>
<h3>SQL</h3>
<p>MySQL • PostgreSQL • MS SQL • Joins • CTEs • Windows</p>
</div>

<div class="skill-card">
<div class="skill-icon">📊</div>
<h3>Power BI</h3>
<p>Power Query • DAX • Data Modeling • KPIs • Dashboards</p>
</div>

<div class="skill-card">
<div class="skill-icon">📗</div>
<h3>Excel</h3>
<p>Pivot Tables • Charts • XLOOKUP • Dashboards</p>
</div>

<div class="skill-card">
<div class="skill-icon">📈</div>
<h3>Tableau</h3>
<p>Visualization • Dashboards • Business Analytics</p>
</div>

<div class="skill-card">
<div class="skill-icon">🧹</div>
<h3>Data Cleaning</h3>
<p>Missing Values • Duplicates • Transformation</p>
</div>

<div class="skill-card">
<div class="skill-icon">🔎</div>
<h3>EDA</h3>
<p>Patterns • Trends • Correlation • Insights</p>
</div>

<div class="skill-card">
<div class="skill-icon">💡</div>
<h3>Business Analysis</h3>
<p>KPI Development • Reporting • Decision Support</p>
</div>

</div>

</section>


<!-- PROJECTS -->

<section id="projects">

<h2 class="section-title">Featured Projects</h2>

<p class="section-subtitle">
Real-world projects demonstrating my data analytics skills.
</p>

<div class="projects">


<!-- PROJECT 1 -->

<div class="project">

<div class="project-image">

<div class="placeholder">🍔</div>

</div>

<div class="project-content">

<h3>Swiggy SQL Data Analysis</h3>

<div class="type">
PostgreSQL • SQL
</div>

<p>
Analyzed Swiggy restaurant data using SQL to
study ratings, prices, food types, cities and
delivery performance.
</p>

<div class="tags">
<span class="tag">PostgreSQL</span>
<span class="tag">SQL</span>
<span class="tag">Joins</span>
<span class="tag">CTE</span>
<span class="tag">Window Functions</span>
</div>

<a class="project-btn"
href="https://github.com/stej07033/Swiggy_project_sql1"
target="_blank">
View Project →
</a>

</div>
</div>


<!-- PROJECT 2 -->

<div class="project">

<div class="project-image">

<div class="placeholder">🍕</div>

</div>

<div class="project-content">

<h3>Pizza Sales Analysis</h3>

<div class="type">
MS SQL Server • Excel
</div>

<p>
Business intelligence project analyzing pizza
sales to identify revenue, order trends,
product performance and customer preferences.
</p>

<div class="tags">
<span class="tag">MS SQL</span>
<span class="tag">T-SQL</span>
<span class="tag">Excel</span>
<span class="tag">KPI</span>
</div>

<a class="project-btn"
href="https://github.com/stej07033/MSSQL-EXCEL_PROJECT1"
target="_blank">
View Project →
</a>

</div>
</div>


<!-- PROJECT 3 -->

<div class="project">

<div class="project-image">

<div class="placeholder">📱</div>

</div>

<div class="project-content">

<h3>PhonePe Dashboard</h3>

<div class="type">
Microsoft Excel
</div>

<p>
Interactive Excel dashboard analyzing PhonePe
transactions across states, transaction types
and years using Pivot Tables, Pivot Charts,
Slicers and KPI cards.
</p>

<div class="tags">
<span class="tag">Excel</span>
<span class="tag">Pivot Tables</span>
<span class="tag">Slicers</span>
<span class="tag">Dashboard</span>
</div>

<a class="project-btn"
href="https://github.com/stej07033/Phonepe_Dashboard"
target="_blank">
View Project →
</a>

</div>
</div>


<!-- PROJECT 4 -->

<div class="project">

<div class="project-image">

<div class="placeholder">🎵</div>

</div>

<div class="project-content">

<h3>Spotify & YouTube Analysis</h3>

<div class="type">
Data Analytics
</div>

<p>
Explored Spotify and YouTube data to understand
content performance, engagement and popularity
patterns.
</p>

<div class="tags">
<span class="tag">Data Analysis</span>
<span class="tag">Visualization</span>
<span class="tag">EDA</span>
</div>

<a class="project-btn"
href="https://github.com/stej07033/Spotify-Youtube-Project"
target="_blank">
View Project →
</a>

</div>
</div>


<!-- PROJECT 5 -->

<div class="project">

<div class="project-image">

<div class="placeholder">🍔</div>

</div>

<div class="project-content">

<h3>Swiggy SQL Server Analysis</h3>

<div class="type">
SQL Server • T-SQL
</div>

<p>
End-to-end Swiggy food-delivery analysis covering
data validation, duplicate handling, database
design, loading, joins and KPI analysis.
</p>

<div class="tags">
<span class="tag">SQL Server</span>
<span class="tag">T-SQL</span>
<span class="tag">Data Validation</span>
<span class="tag">KPI</span>
</div>

<a class="project-btn"
href="https://github.com/stej07033/Swiggy_Sql_Project"
target="_blank">
View Project →
</a>

</div>
</div>


<!-- PROJECT 6 -->

<div class="project">

<div class="project-image">

<div class="placeholder">📊</div>

</div>

<div class="project-content">

<h3>Swiggy Excel Dashboard</h3>

<div class="type">
Microsoft Excel
</div>

<p>
Interactive Excel analytics dashboard focused on
restaurant performance, customer ratings,
delivery time, pricing, cuisine distribution
and order trends.
</p>

<div class="tags">
<span class="tag">Excel</span>
<span class="tag">Dashboard</span>
<span class="tag">Pivot Charts</span>
<span class="tag">Analytics</span>
</div>

<a class="project-btn"
href="https://github.com/stej07033/Swiggy_Excel"
target="_blank">
View Project →
</a>

</div>
</div>


<!-- BANK LOAN -->

<div class="project">

<div class="project-image">

<div class="placeholder">🏦</div>

</div>

<div class="project-content">

<h3>Bank Loan Analysis</h3>

<div class="type">
Python • Pandas
</div>

<p>
Financial loan analysis focused on loan applications,
funded amounts, payments and important MTD and
business KPIs.
</p>

<div class="tags">
<span class="tag">Python</span>
<span class="tag">Pandas</span>
<span class="tag">KPI</span>
<span class="tag">EDA</span>
</div>

<a class="project-btn"
href="https://github.com/stej07033"
target="_blank">
View GitHub →
</a>

</div>
</div>


<!-- ECOMMERCE -->

<div class="project">

<div class="project-image">

<div class="placeholder">🛒</div>

</div>

<div class="project-content">

<h3>E-Commerce Sales Analysis</h3>

<div class="type">
SQL • Python • Excel • Power BI
</div>

<p>
End-to-end analytics workflow covering data
cleaning, exploratory analysis, SQL business
questions, KPI development and dashboard reporting.
</p>

<div class="tags">
<span class="tag">Python</span>
<span class="tag">SQL</span>
<span class="tag">Excel</span>
<span class="tag">Power BI</span>
</div>

<a class="project-btn"
href="https://github.com/stej07033"
target="_blank">
View GitHub →
</a>

</div>
</div>


<!-- HR -->

<div class="project">

<div class="project-image">

<div class="placeholder">👥</div>

</div>

<div class="project-content">

<h3>HR Analytics</h3>

<div class="type">
Python • Tableau
</div>

<p>
Analyzed employee data to understand attrition
patterns and identify important factors related
to employee turnover.
</p>

<div class="tags">
<span class="tag">Python</span>
<span class="tag">EDA</span>
<span class="tag">Tableau</span>
<span class="tag">HR Analytics</span>
</div>

<a class="project-btn"
href="https://github.com/stej07033"
target="_blank">
View GitHub →
</a>

</div>
</div>


</div>

</section>


<!-- WORKFLOW -->

<section id="workflow">

<h2 class="section-title">My Data Analytics Workflow</h2>

<p class="section-subtitle">
From raw data to actionable business insights.
</p>

<div class="workflow">

<div class="workflow-step">📥 Data Collection</div>
<div class="arrow">→</div>

<div class="workflow-step">🧹 Data Cleaning</div>
<div class="arrow">→</div>

<div class="workflow-step">🔎 EDA</div>
<div class="arrow">→</div>

<div class="workflow-step">🗄️ SQL Analysis</div>
<div class="arrow">→</div>

<div class="workflow-step">📊 KPI Creation</div>
<div class="arrow">→</div>

<div class="workflow-step">📈 Visualization</div>
<div class="arrow">→</div>

<div class="workflow-step">💡 Insights</div>

</div>

</section>


<!-- KPIs -->

<section>

<h2 class="section-title">What I Analyze</h2>

<p class="section-subtitle">
Business questions I solve with data.
</p>

<div class="kpis">

<div class="kpi">
<div class="kpi-number">01</div>
<p>Sales & Revenue</p>
</div>

<div class="kpi">
<div class="kpi-number">02</div>
<p>Customer Behavior</p>
</div>

<div class="kpi">
<div class="kpi-number">03</div>
<p>Product Performance</p>
</div>

<div class="kpi">
<div class="kpi-number">04</div>
<p>Business KPIs</p>
</div>

</div>

</section>


<!-- CONTACT -->

<section id="contact" class="contact">

<h2 class="section-title">Let's Connect</h2>

<p>
I'm currently looking for opportunities as a
Data Analyst / Junior Data Analyst / Business Analyst.
</p>

<div class="socials">

<a class="social"
href="https://github.com/stej07033"
target="_blank">
🐙 GitHub
</a>

<a class="social"
href="https://www.linkedin.com/in/madanapalli-sai-19b835389"
target="_blank">
💼 LinkedIn
</a>

</div>

</section>


<!-- FOOTER -->

<footer>

<p>
© 2026 Sai Tej • Aspiring Data Analyst
</p>

<p>
SQL • Python • Excel • Power BI • Tableau
</p>

</footer>

</body>
</html>
```
