<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Sai | Data Analyst Portfolio</title>

<meta name="description"
content="Sai - Data Analyst Portfolio | SQL | Python | Excel | Business Analytics">

<style>

/* =========================================================
   RESET
========================================================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:Inter,Segoe UI,Arial,sans-serif;
    background:#050816;
    color:#fff;
    overflow-x:hidden;
    transition:background .5s,color .5s;
}

body.light{
    background:#f4f7fb;
    color:#111827;
}

a{
    color:inherit;
    text-decoration:none;
}

button{
    font-family:inherit;
}

/* =========================================================
   LOADING SCREEN
========================================================= */

.loader{
    position:fixed;
    inset:0;
    background:#03040b;
    z-index:99999;
    display:flex;
    align-items:center;
    justify-content:center;
    flex-direction:column;
    transition:opacity 1s,visibility 1s;
}

.loader.hide{
    opacity:0;
    visibility:hidden;
}

.loader-title{
    font-size:clamp(2rem,6vw,5rem);
    font-weight:900;
    letter-spacing:8px;
    background:linear-gradient(90deg,#fff,#7dd3fc,#a78bfa,#fff);
    background-size:300%;
    -webkit-background-clip:text;
    color:transparent;
    animation:gradient 3s infinite;
}

.loader-line{
    width:220px;
    height:3px;
    background:#222;
    margin-top:30px;
    overflow:hidden;
    border-radius:50px;
}

.loader-line span{
    display:block;
    height:100%;
    width:0;
    background:linear-gradient(90deg,#38bdf8,#8b5cf6);
    animation:load 2.2s forwards;
}

@keyframes load{
    to{width:100%}
}

@keyframes gradient{
    0%{background-position:0%}
    50%{background-position:100%}
    100%{background-position:0%}
}

/* =========================================================
   CANVAS
========================================================= */

#particles{
    position:fixed;
    inset:0;
    width:100%;
    height:100%;
    z-index:-5;
    pointer-events:none;
}

/* =========================================================
   CURSOR
========================================================= */

.cursor{
    position:fixed;
    width:280px;
    height:280px;
    border-radius:50%;
    background:radial-gradient(circle,
        rgba(56,189,248,.13),
        transparent 65%);
    pointer-events:none;
    transform:translate(-50%,-50%);
    z-index:0;
}

/* =========================================================
   NAVBAR
========================================================= */

nav{
    position:fixed;
    top:15px;
    left:50%;
    transform:translateX(-50%);
    width:min(1150px,94%);
    height:68px;
    padding:0 20px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    z-index:1000;

    background:rgba(8,12,30,.55);
    backdrop-filter:blur(20px);
    border:1px solid rgba(255,255,255,.1);
    border-radius:20px;

    box-shadow:
        0 20px 70px rgba(0,0,0,.35),
        inset 0 1px rgba(255,255,255,.08);
}

body.light nav{
    background:rgba(255,255,255,.7);
    color:#111827;
    border-color:rgba(0,0,0,.08);
}

.logo{
    font-size:24px;
    font-weight:900;
    letter-spacing:2px;
}

.logo span{
    color:#38bdf8;
}

.nav-links{
    display:flex;
    gap:25px;
    align-items:center;
}

.nav-links a{
    font-size:14px;
    opacity:.8;
    transition:.3s;
}

.nav-links a:hover{
    opacity:1;
    color:#38bdf8;
}

.theme-btn{
    width:42px;
    height:42px;
    border-radius:50%;
    border:1px solid rgba(255,255,255,.15);
    background:rgba(255,255,255,.06);
    color:white;
    cursor:pointer;
    font-size:18px;
}

body.light .theme-btn{
    color:#111;
}

.menu-btn{
    display:none;
    background:none;
    border:0;
    color:inherit;
    font-size:25px;
}

/* =========================================================
   GLOBAL
========================================================= */

section{
    width:min(1150px,92%);
    margin:auto;
    padding:120px 0;
}

.section-label{
    color:#38bdf8;
    text-transform:uppercase;
    letter-spacing:4px;
    font-size:12px;
    font-weight:800;
    margin-bottom:12px;
}

.section-title{
    font-size:clamp(2rem,5vw,4rem);
    font-weight:900;
    line-height:1;
    margin-bottom:20px;
}

.section-description{
    color:#94a3b8;
    max-width:700px;
    line-height:1.8;
}

body.light .section-description{
    color:#64748b;
}

/* =========================================================
   HERO
========================================================= */

.hero{
    min-height:100vh;
    display:grid;
    grid-template-columns:1.15fr .85fr;
    align-items:center;
    gap:50px;
    padding-top:150px;
}

.hero-badge{
    display:inline-flex;
    align-items:center;
    gap:8px;
    padding:9px 15px;
    border:1px solid rgba(56,189,248,.3);
    background:rgba(56,189,248,.08);
    border-radius:50px;
    color:#7dd3fc;
    font-size:13px;
    margin-bottom:25px;
}

.status-dot{
    width:8px;
    height:8px;
    border-radius:50%;
    background:#22c55e;
    box-shadow:0 0 15px #22c55e;
    animation:pulse 1.5s infinite;
}

@keyframes pulse{
    50%{transform:scale(1.5);opacity:.5}
}

.hero h1{
    font-size:clamp(3rem,7vw,7rem);
    line-height:.9;
    font-weight:950;
    letter-spacing:-5px;
}

.hero h1 .gradient{
    background:linear-gradient(110deg,#38bdf8,#818cf8,#c084fc);
    -webkit-background-clip:text;
    color:transparent;
}

.typing{
    min-height:42px;
    margin-top:25px;
    font-size:clamp(1.1rem,2vw,1.5rem);
    color:#cbd5e1;
}

body.light .typing{
    color:#475569;
}

.hero-text{
    margin-top:20px;
    max-width:650px;
    color:#94a3b8;
    line-height:1.8;
}

body.light .hero-text{
    color:#64748b;
}

.hero-buttons{
    display:flex;
    gap:15px;
    flex-wrap:wrap;
    margin-top:30px;
}

.btn{
    padding:14px 22px;
    border-radius:14px;
    border:1px solid rgba(255,255,255,.12);
    display:inline-flex;
    align-items:center;
    gap:9px;
    cursor:pointer;
    transition:.3s;
    font-weight:700;
}

.btn-primary{
    background:linear-gradient(135deg,#38bdf8,#6366f1);
    color:white;
    box-shadow:0 15px 35px rgba(56,189,248,.25);
}

.btn-secondary{
    background:rgba(255,255,255,.05);
}

.btn:hover{
    transform:translateY(-5px) scale(1.02);
}

/* =========================================================
   3D CUBE
========================================================= */

.hero-visual{
    display:flex;
    justify-content:center;
    align-items:center;
    perspective:1000px;
}

.cube-wrapper{
    width:260px;
    height:260px;
    position:relative;
    transform-style:preserve-3d;
    animation:floatCube 6s ease-in-out infinite;
}

.cube{
    position:absolute;
    width:180px;
    height:180px;
    left:40px;
    top:40px;
    transform-style:preserve-3d;
    animation:rotateCube 16s linear infinite;
}

.face{
    position:absolute;
    width:180px;
    height:180px;
    border:1px solid rgba(125,211,252,.45);
    background:linear-gradient(
        135deg,
        rgba(56,189,248,.12),
        rgba(139,92,246,.1)
    );
    backdrop-filter:blur(5px);
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:22px;
    font-weight:900;
    color:#7dd3fc;
    box-shadow:
        inset 0 0 50px rgba(56,189,248,.08),
        0 0 30px rgba(56,189,248,.08);
}

.front{transform:translateZ(90px)}
.back{transform:rotateY(180deg) translateZ(90px)}
.right{transform:rotateY(90deg) translateZ(90px)}
.left{transform:rotateY(-90deg) translateZ(90px)}
.top{transform:rotateX(90deg) translateZ(90px)}
.bottom{transform:rotateX(-90deg) translateZ(90px)}

@keyframes rotateCube{
    from{transform:rotateX(0) rotateY(0)}
    to{transform:rotateX(360deg) rotateY(360deg)}
}

@keyframes floatCube{
    50%{transform:translateY(-25px) rotateZ(3deg)}
}

/* =========================================================
   STATS
========================================================= */

.stats{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:18px;
    margin-top:60px;
}

.stat{
    padding:30px;
    border-radius:22px;
    border:1px solid rgba(255,255,255,.09);
    background:rgba(255,255,255,.035);
    backdrop-filter:blur(15px);
    position:relative;
    overflow:hidden;
    transition:.4s;
}

body.light .stat,
body.light .glass{
    background:rgba(255,255,255,.7);
    border-color:rgba(15,23,42,.08);
}

.stat:hover{
    transform:translateY(-10px) rotateX(4deg);
    box-shadow:0 25px 60px rgba(0,0,0,.25);
}

.stat-number{
    font-size:2.6rem;
    font-weight:950;
    color:#7dd3fc;
}

.stat-label{
    color:#94a3b8;
    margin-top:5px;
}

/* =========================================================
   ABOUT
========================================================= */

.about-grid{
    display:grid;
    grid-template-columns:.8fr 1.2fr;
    gap:60px;
    align-items:center;
}

.about-card{
    min-height:400px;
    border-radius:30px;
    border:1px solid rgba(255,255,255,.1);
    background:
        radial-gradient(circle at 30% 20%,rgba(56,189,248,.15),transparent 35%),
        rgba(255,255,255,.035);
    backdrop-filter:blur(15px);
    display:flex;
    align-items:center;
    justify-content:center;
    position:relative;
    overflow:hidden;
    transform-style:preserve-3d;
}

.about-orb{
    width:210px;
    height:210px;
    border-radius:50%;
    background:
        radial-gradient(circle at 35% 30%,#bae6fd,#38bdf8 35%,#6366f1 70%,#111827);
    box-shadow:
        0 0 80px rgba(56,189,248,.3),
        inset -30px -30px 60px rgba(0,0,0,.35);
    animation:orb 5s ease-in-out infinite;
}

@keyframes orb{
    50%{
        transform:translateY(-20px) scale(1.06);
    }
}

/* =========================================================
   SKILLS
========================================================= */

.skills-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:22px;
    margin-top:45px;
}

.skill{
    padding:25px;
    border-radius:20px;
    background:rgba(255,255,255,.035);
    border:1px solid rgba(255,255,255,.08);
}

.skill-top{
    display:flex;
    justify-content:space-between;
    margin-bottom:14px;
    font-weight:700;
}

.skill-bar{
    height:8px;
    background:rgba(255,255,255,.08);
    border-radius:50px;
    overflow:hidden;
}

.skill-progress{
    height:100%;
    width:0;
    border-radius:50px;
    background:linear-gradient(90deg,#38bdf8,#8b5cf6);
    transition:width 1.5s cubic-bezier(.2,.8,.2,1);
}

/* =========================================================
   PROJECTS
========================================================= */

.projects-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:25px;
    margin-top:45px;
}

.project{
    padding:30px;
    border-radius:25px;
    background:rgba(255,255,255,.035);
    border:1px solid rgba(255,255,255,.09);
    position:relative;
    overflow:hidden;
    transform-style:preserve-3d;
    transition:.4s;
}

.project:hover{
    transform:translateY(-12px);
    border-color:rgba(56,189,248,.35);
    box-shadow:0 30px 80px rgba(0,0,0,.25);
}

.project-number{
    font-size:60px;
    font-weight:950;
    color:rgba(56,189,248,.08);
    position:absolute;
    right:20px;
    top:10px;
}

.project-icon{
    font-size:35px;
    margin-bottom:20px;
}

.project h3{
    font-size:24px;
    margin-bottom:12px;
}

.project p{
    color:#94a3b8;
    line-height:1.7;
}

.tags{
    display:flex;
    flex-wrap:wrap;
    gap:8px;
    margin:20px 0;
}

.tag{
    font-size:11px;
    padding:7px 10px;
    border-radius:50px;
    background:rgba(56,189,248,.08);
    color:#7dd3fc;
    border:1px solid rgba(56,189,248,.12);
}

.project-link{
    color:#7dd3fc;
    font-weight:800;
}

/* =========================================================
   WORKFLOW
========================================================= */

.workflow{
    display:grid;
    grid-template-columns:repeat(6,1fr);
    gap:12px;
    margin-top:50px;
}

.workflow-item{
    padding:22px 12px;
    text-align:center;
    border-radius:18px;
    background:rgba(255,255,255,.035);
    border:1px solid rgba(255,255,255,.08);
    transition:.4s;
}

.workflow-item:hover{
    transform:translateY(-10px) scale(1.04);
    background:rgba(56,189,248,.08);
}

.workflow-icon{
    font-size:27px;
    margin-bottom:10px;
}

.workflow-item span{
    font-size:12px;
    color:#94a3b8;
}

/* =========================================================
   CERTIFICATIONS
========================================================= */

.cert-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
    margin-top:40px;
}

.cert{
    padding:25px;
    border-radius:20px;
    border:1px solid rgba(255,255,255,.08);
    background:rgba(255,255,255,.035);
    transition:.3s;
}

.cert:hover{
    transform:translateY(-7px);
}

.cert-icon{
    font-size:30px;
    margin-bottom:15px;
}

.cert p{
    margin-top:8px;
    color:#94a3b8;
    font-size:14px;
}

/* =========================================================
   CONTACT
========================================================= */

.contact{
    text-align:center;
    padding-bottom:80px;
}

.contact-box{
    padding:60px 30px;
    border-radius:35px;
    background:
        radial-gradient(circle at 20% 20%,rgba(56,189,248,.14),transparent 30%),
        radial-gradient(circle at 80% 80%,rgba(139,92,246,.14),transparent 30%),
        rgba(255,255,255,.035);
    border:1px solid rgba(255,255,255,.1);
    margin-top:45px;
}

.email{
    margin:25px 0;
    color:#7dd3fc;
    font-size:18px;
    word-break:break-word;
}

/* =========================================================
   FOOTER
========================================================= */

footer{
    text-align:center;
    padding:30px;
    color:#64748b;
    border-top:1px solid rgba(255,255,255,.06);
}

/* =========================================================
   REVEAL ANIMATION
========================================================= */

.reveal{
    opacity:0;
    transform:translateY(60px);
    transition:
        opacity .9s ease,
        transform .9s cubic-bezier(.2,.8,.2,1);
}

.reveal.active{
    opacity:1;
    transform:translateY(0);
}

/* =========================================================
   3D TILT
========================================================= */

.tilt{
    transform-style:preserve-3d;
}

/* =========================================================
   LIGHT MODE
========================================================= */

body.light .project,
body.light .skill,
body.light .workflow-item,
body.light .cert,
body.light .stat{
    background:rgba(255,255,255,.8);
    border-color:rgba(15,23,42,.08);
}

body.light .project p,
body.light .cert p,
body.light .stat-label,
body.light .workflow-item span{
    color:#64748b;
}

/* =========================================================
   RESPONSIVE
========================================================= */

@media(max-width:850px){

    .nav-links{
        position:absolute;
        top:78px;
        left:0;
        width:100%;
        padding:25px;
        border-radius:20px;
        background:rgba(8,12,30,.95);
        display:none;
        flex-direction:column;
    }

    body.light .nav-links{
        background:white;
    }

    .nav-links.open{
        display:flex;
    }

    .menu-btn{
        display:block;
    }

    .hero{
        grid-template-columns:1fr;
        text-align:center;
    }

    .hero-buttons{
        justify-content:center;
    }

    .hero-text{
        margin-left:auto;
        margin-right:auto;
    }

    .stats{
        grid-template-columns:repeat(2,1fr);
    }

    .about-grid{
        grid-template-columns:1fr;
    }

    .skills-grid,
    .projects-grid{
        grid-template-columns:1fr;
    }

    .workflow{
        grid-template-columns:repeat(3,1fr);
    }

    .cert-grid{
        grid-template-columns:1fr;
    }
}

@media(max-width:500px){

    section{
        padding:85px 0;
    }

    .hero h1{
        letter-spacing:-3px;
    }

    .stats{
        grid-template-columns:1fr;
    }

    .workflow{
        grid-template-columns:repeat(2,1fr);
    }

    .cube-wrapper{
        transform:scale(.8);
    }
}

</style>
</head>

<body>

<!-- =======================================================
     LOADER
======================================================= -->

<div class="loader" id="loader">

    <div class="loader-title">
        SAI
    </div>

    <div class="loader-line">
        <span></span>
    </div>

</div>

<!-- =======================================================
     PARTICLES
======================================================= -->

<canvas id="particles"></canvas>

<div class="cursor" id="cursor"></div>

<!-- =======================================================
     NAVBAR
======================================================= -->

<nav>

    <div class="logo">
        SAI<span>.</span>
    </div>

    <div class="nav-links" id="navLinks">

        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#certifications">Certifications</a>
        <a href="#contact">Contact</a>

    </div>

    <div style="display:flex;gap:10px;align-items:center">

        <button class="theme-btn" id="themeBtn">
            ☀️
        </button>

        <button class="menu-btn" id="menuBtn">
            ☰
        </button>

    </div>

</nav>

<!-- =======================================================
     HERO
======================================================= -->

<section class="hero" id="home">

    <div class="reveal">

        <div class="hero-badge">

            <span class="status-dot"></span>

            Data Analyst Intern • Open to Opportunities

        </div>

        <h1>

            Hi, I'm

            <span class="gradient">
                Sai
            </span>

        </h1>

        <div class="typing" id="typing"></div>

        <p class="hero-text">

            I transform raw data into meaningful business insights using
            SQL, Python, Excel and data visualization. I enjoy solving
            practical business problems through data-driven analysis.

        </p>

        <div class="hero-buttons">

            <a
                href="https://github.com/stej07033"
                target="_blank"
                class="btn btn-primary"
            >
                🐙 GitHub
            </a>

            <a
                href="https://www.linkedin.com/"
                target="_blank"
                class="btn btn-secondary"
            >
                💼 LinkedIn
            </a>

            <a
                href="#projects"
                class="btn btn-secondary"
            >
                🚀 View Projects
            </a>

        </div>

    </div>

    <div class="hero-visual reveal">

        <div class="cube-wrapper">

            <div class="cube">

                <div class="face front">SQL</div>
                <div class="face back">PYTHON</div>
                <div class="face right">EXCEL</div>
                <div class="face left">DATA</div>
                <div class="face top">BI</div>
                <div class="face bottom">EDA</div>

            </div>

        </div>

    </div>

</section>

<!-- =======================================================
     STATS
======================================================= -->

<section>

    <div class="stats">

        <div class="stat reveal">

            <div
                class="stat-number counter"
                data-target="394800"
            >
                0
            </div>

            <div class="stat-label">
                Swiggy Records
            </div>

        </div>

        <div class="stat reveal">

            <div
                class="stat-number counter"
                data-target="20"
            >
                0
            </div>

            <div class="stat-label">
                Business Questions
            </div>

        </div>

        <div class="stat reveal">

            <div
                class="stat-number counter"
                data-target="75"
            >
                0
            </div>

            <div class="stat-label">
                SQL Problems+
            </div>

        </div>

        <div class="stat reveal">

            <div
                class="stat-number counter"
                data-target="4"
            >
                0
            </div>

            <div class="stat-label">
                Core Analytics Tools
            </div>

        </div>

    </div>

</section>

<!-- =======================================================
     ABOUT
======================================================= -->

<section id="about">

    <div class="about-grid">

        <div class="about-card tilt reveal">

            <div class="about-orb"></div>

        </div>

        <div class="reveal">

            <div class="section-label">
                About Me
            </div>

            <h2 class="section-title">
                Data-driven.<br>
                Business-focused.
            </h2>

            <p class="section-description">

                I'm a Data Analyst Intern at Tap Academy, working with
                Python, SQL and Excel to analyze business datasets,
                perform data cleaning, develop reports and support
                data-driven decision-making.

                <br><br>

                My portfolio focuses on practical analytics projects
                rather than simply learning individual tools. I like
                connecting data preparation, SQL analysis, KPI tracking,
                visualization and business recommendations into one
                complete workflow.

            </p>

        </div>

    </div>

</section>

<!-- =======================================================
     SKILLS
======================================================= -->

<section id="skills">

    <div class="section-label reveal">
        Technical Skills
    </div>

    <h2 class="section-title reveal">
        My Analytics Stack
    </h2>

    <p class="section-description reveal">
        Tools I use to clean, analyze, visualize and communicate data.
    </p>

    <div class="skills-grid">

        <div class="skill reveal">

            <div class="skill-top">
                <span>SQL / T-SQL</span>
                <span>90%</span>
            </div>

            <div class="skill-bar">
                <div class="skill-progress" data-width="90%"></div>
            </div>

        </div>

        <div class="skill reveal">

            <div class="skill-top">
                <span>Python / Pandas</span>
                <span>88%</span>
            </div>

            <div class="skill-bar">
                <div class="skill-progress" data-width="88%"></div>
            </div>

        </div>

        <div class="skill reveal">

            <div class="skill-top">
                <span>Excel</span>
                <span>90%</span>
            </div>

            <div class="skill-bar">
                <div class="skill-progress" data-width="90%"></div>
            </div>

        </div>

        <div class="skill reveal">

            <div class="skill-top">
                <span>Data Visualization</span>
                <span>85%</span>
            </div>

            <div class="skill-bar">
                <div class="skill-progress" data-width="85%"></div>
            </div>

        </div>

        <div class="skill reveal">

            <div class="skill-top">
                <span>Data Cleaning</span>
                <span>88%</span>
            </div>

            <div class="skill-bar">
                <div class="skill-progress" data-width="88%"></div>
            </div>

        </div>

        <div class="skill reveal">

            <div class="skill-top">
                <span>Business Analytics</span>
                <span>82%</span>
            </div>

            <div class="skill-bar">
                <div class="skill-progress" data-width="82%"></div>
            </div>

        </div>

    </div>

</section>

<!-- =======================================================
     WORKFLOW
======================================================= -->

<section>

    <div class="section-label reveal">
        Workflow
    </div>

    <h2 class="section-title reveal">
        How I Work With Data
    </h2>

    <div class="workflow">

        <div class="workflow-item reveal">
            <div class="workflow-icon">📥</div>
            <b>Raw Data</b>
            <span>Collect</span>
        </div>

        <div class="workflow-item reveal">
            <div class="workflow-icon">🧹</div>
            <b>Cleaning</b>
            <span>Prepare</span>
        </div>

        <div class="workflow-item reveal">
            <div class="workflow-icon">🔍</div>
            <b>EDA</b>
            <span>Explore</span>
        </div>

        <div class="workflow-item reveal">
            <div class="workflow-icon">🗄️</div>
            <b>SQL</b>
            <span>Analyze</span>
        </div>

        <div class="workflow-item reveal">
            <div class="workflow-icon">📊</div>
            <b>KPIs</b>
            <span>Measure</span>
        </div>

        <div class="workflow-item reveal">
            <div class="workflow-icon">💡</div>
            <b>Insights</b>
            <span>Decide</span>
        </div>

    </div>

</section>

<!-- =======================================================
     PROJECTS
======================================================= -->

<section id="projects">

    <div class="section-label reveal">
        Featured Projects
    </div>

    <h2 class="section-title reveal">
        Selected Work
    </h2>

    <p class="section-description reveal">
        Practical analytics projects demonstrating data cleaning,
        SQL analysis, Python workflows and business reporting.
    </p>

    <div class="projects-grid">

        <!-- PROJECT 1 -->

        <article class="project tilt reveal">

            <div class="project-number">
                01
            </div>

            <div class="project-icon">
                🛵
            </div>

            <h3>
                Swiggy End-to-End Analytics
            </h3>

            <p>

                An end-to-end food-delivery analytics project using
                394,800+ records. The same dataset was analyzed through
                Python, SQL Server and Excel to answer 20+ business
                questions.

            </p>

            <div class="tags">

                <span class="tag">Python</span>
                <span class="tag">Pandas</span>
                <span class="tag">SQL Server</span>
                <span class="tag">T-SQL</span>
                <span class="tag">Excel</span>
                <span class="tag">KPI Analysis</span>

            </div>

            <a
                class="project-link"
                href="https://github.com/stej07033/Swiggy_Sql_Project"
                target="_blank"
            >
                Explore Project →
            </a>

        </article>

        <!-- PROJECT 2 -->

        <article class="project tilt reveal">

            <div class="project-number">
                02
            </div>

            <div class="project-icon">
                📊
            </div>

            <h3>
                HR Analytics Dashboard
            </h3>

            <p>

                Interactive Excel dashboard analyzing employee
                attrition, demographics, job satisfaction and
                department-level performance through KPI reporting.

            </p>

            <div class="tags">

                <span class="tag">Excel</span>
                <span class="tag">Pivot Tables</span>
                <span class="tag">Pivot Charts</span>
                <span class="tag">Slicers</span>
                <span class="tag">KPI Cards</span>

            </div>

            <a
                class="project-link"
                href="https://github.com/stej07033"
                target="_blank"
            >
                Explore Project →
            </a>

        </article>

        <!-- PROJECT 3 -->

        <article class="project tilt reveal">

            <div class="project-number">
                03
            </div>

            <div class="project-icon">
                🐍
            </div>

            <h3>
                Python Data Analytics
            </h3>

            <p>

                Python-based analytics workflows using Pandas,
                NumPy and visualization libraries to clean,
                explore and understand structured datasets.

            </p>

            <div class="tags">

                <span class="tag">Python</span>
                <span class="tag">Pandas</span>
                <span class="tag">NumPy</span>
                <span class="tag">Matplotlib</span>
                <span class="tag">Seaborn</span>

            </div>

            <a
                class="project-link"
                href="https://github.com/stej07033"
                target="_blank"
            >
                View GitHub →
            </a>

        </article>

        <!-- PROJECT 4 -->

        <article class="project tilt reveal">

            <div class="project-number">
                04
            </div>

            <div class="project-icon">
                🗄️
            </div>

            <h3>
                SQL Business Analysis
            </h3>

            <p>

                SQL analysis focused on business questions using
                joins, aggregations, CTEs, subqueries and window
                functions to generate actionable metrics.

            </p>

            <div class="tags">

                <span class="tag">SQL</span>
                <span class="tag">Joins</span>
                <span class="tag">CTEs</span>
                <span class="tag">Window Functions</span>
                <span class="tag">KPIs</span>

            </div>

            <a
                class="project-link"
                href="https://github.com/stej07033"
                target="_blank"
            >
                View GitHub →
            </a>

        </article>

    </div>

</section>

<!-- =======================================================
     ANALYTICS CAPABILITIES
======================================================= -->

<section>

    <div class="section-label reveal">
        Analytics Capabilities
    </div>

    <h2 class="section-title reveal">
        What I Bring
    </h2>

    <div class="stats">

        <div class="stat reveal">
            <div class="stat-number">SQL</div>
            <div class="stat-label">
                Analytical querying
            </div>
        </div>

        <div class="stat reveal">
            <div class="stat-number">PY</div>
            <div class="stat-label">
                Python analytics
            </div>
        </div>

        <div class="stat reveal">
            <div class="stat-number">XLS</div>
            <div class="stat-label">
                Excel reporting
            </div>
        </div>

        <div class="stat reveal">
            <div class="stat-number">BI</div>
            <div class="stat-label">
                Business intelligence
            </div>
        </div>

    </div>

</section>

<!-- =======================================================
     CERTIFICATIONS
======================================================= -->

<section id="certifications">

    <div class="section-label reveal">
        Certifications
    </div>

    <h2 class="section-title reveal">
        Learning & Credentials
    </h2>

    <div class="cert-grid">

        <div class="cert reveal">

            <div class="cert-icon">
                🏆
            </div>

            <h3>
                Google Data Analytics
            </h3>

            <p>
                Google / Coursera
            </p>

        </div>

        <div class="cert reveal">

            <div class="cert-icon">
                🐍
            </div>

            <h3>
                Python for Data Science
            </h3>

            <p>
                Coursera
            </p>

        </div>

        <div class="cert reveal">

            <div class="cert-icon">
                📊
            </div>

            <h3>
                Power BI Data Analyst
            </h3>

            <p>
                Microsoft Learn
            </p>

        </div>

        <div class="cert reveal">

            <div class="cert-icon">
                🗄️
            </div>

            <h3>
                SQL for Data Analysis
            </h3>

            <p>
                HackerRank
            </p>

        </div>

        <div class="cert reveal">

            <div class="cert-icon">
                📚
            </div>

            <h3>
                Introduction to Data Analytics
            </h3>

            <p>
                NPTEL
            </p>

        </div>

    </div>

</section>

<!-- =======================================================
     CAREER
======================================================= -->

<section>

    <div class="about-grid">

        <div class="reveal">

            <div class="section-label">
                Career Direction
            </div>

            <h2 class="section-title">
                From Data<br>
                to Decisions.
            </h2>

        </div>

        <div class="reveal">

            <p class="section-description">

                My goal is to build a career in data analytics where
                technical analysis is connected directly to business
                decision-making.

                <br><br>

                I'm particularly interested in:

                <br><br>

                <strong>
                    Data Analyst • Junior Data Analyst • Business Analyst
                    • BI Analyst • SQL Analyst
                </strong>

            </p>

        </div>

    </div>

</section>

<!-- =======================================================
     CONTACT
======================================================= -->

<section id="contact" class="contact">

    <div class="section-label reveal">
        Contact
    </div>

    <h2 class="section-title reveal">
        Let's Connect
    </h2>

    <div class="contact-box reveal">

        <p class="section-description" style="margin:auto">

            Interested in data analytics, SQL, Python,
            Excel or business intelligence?

            Let's connect.

        </p>

        <div class="email" id="email">
            stej07033@gmail.com
        </div>

        <div class="hero-buttons" style="justify-content:center">

            <button
                class="btn btn-primary"
                onclick="copyEmail()"
            >
                📋 Copy Email
            </button>

            <a
                href="mailto:stej07033@gmail.com"
                class="btn btn-secondary"
            >
                ✉️ Email Me
            </a>

            <a
                href="https://github.com/stej07033"
                target="_blank"
                class="btn btn-secondary"
            >
                🐙 GitHub
            </a>

        </div>

    </div>

</section>

<!-- =======================================================
     FOOTER
======================================================= -->

<footer>

    © <span id="year"></span> Sai.

    <br><br>

    Data Analyst • SQL • Python • Excel • Business Analytics

</footer>

<!-- =======================================================
     JAVASCRIPT
======================================================= -->

<script>

/* =========================================================
   LOADER
========================================================= */

window.addEventListener("load",()=>{

    setTimeout(()=>{

        document
        .getElementById("loader")
        .classList.add("hide");

    },2300);

});

/* =========================================================
   YEAR
========================================================= */

document.getElementById("year").textContent =
new Date().getFullYear();

/* =========================================================
   TYPING ANIMATION
========================================================= */

const typingElement =
document.getElementById("typing");

const words = [

    "Data Analyst",
    "SQL Analyst",
    "Python Analytics Enthusiast",
    "Business Analytics Aspirant",
    "Excel Dashboard Developer"

];

let wordIndex = 0;
let charIndex = 0;
let deleting = false;

function typeEffect(){

    const current = words[wordIndex];

    if(!deleting){

        typingElement.textContent =
        current.substring(0,charIndex++);

        if(charIndex > current.length){

            deleting = true;

            setTimeout(typeEffect,1200);

            return;
        }

    }else{

        typingElement.textContent =
        current.substring(0,charIndex--);

        if(charIndex === 0){

            deleting = false;

            wordIndex =
            (wordIndex + 1) % words.length;

        }

    }

    setTimeout(
        typeEffect,
        deleting ? 45 : 85
    );

}

typeEffect();

/* =========================================================
   THEME
========================================================= */

const themeBtn =
document.getElementById("themeBtn");

themeBtn.addEventListener("click",()=>{

    document.body.classList.toggle("light");

    themeBtn.textContent =
    document.body.classList.contains("light")
    ? "🌙"
    : "☀️";

});

/* =========================================================
   MOBILE MENU
========================================================= */

const menuBtn =
document.getElementById("menuBtn");

const navLinks =
document.getElementById("navLinks");

menuBtn.addEventListener("click",()=>{

    navLinks.classList.toggle("open");

});

document
.querySelectorAll(".nav-links a")
.forEach(link=>{

    link.addEventListener("click",()=>{

        navLinks.classList.remove("open");

    });

});

/* =========================================================
   SCROLL REVEAL
========================================================= */

const observer =
new IntersectionObserver(

    entries=>{

        entries.forEach(entry=>{

            if(entry.isIntersecting){

                entry.target
                .classList
                .add("active");

            }

        });

    },

    {
        threshold:.12
    }

);

document
.querySelectorAll(".reveal")
.forEach(el=>observer.observe(el));

/* =========================================================
   SKILL BARS
========================================================= */

const skillObserver =
new IntersectionObserver(

    entries=>{

        entries.forEach(entry=>{

            if(entry.isIntersecting){

                const progress =
                entry.target;

                progress.style.width =
                progress.dataset.width;

                skillObserver.unobserve(progress);

            }

        });

    },

    {
        threshold:.5
    }

);

document
.querySelectorAll(".skill-progress")
.forEach(el=>{

    skillObserver.observe(el);

});

/* =========================================================
   COUNTERS
========================================================= */

function animateCounter(element){

    const target =
    Number(element.dataset.target);

    let current = 0;

    const duration = 1800;

    const start =
    performance.now();

    function update(time){

        const progress =
        Math.min(
            (time-start)/duration,
            1
        );

        const eased =
        1-Math.pow(1-progress,4);

        current =
        Math.floor(target*eased);

        element.textContent =
        current.toLocaleString();

        if(progress < 1){

            requestAnimationFrame(update);

        }else{

            element.textContent =
            target.toLocaleString();

        }

    }

    requestAnimationFrame(update);

}

const counterObserver =
new IntersectionObserver(

    entries=>{

        entries.forEach(entry=>{

            if(entry.isIntersecting){

                animateCounter(entry.target);

                counterObserver
                .unobserve(entry.target);

            }

        });

    },

    {
        threshold:.6
    }

);

document
.querySelectorAll(".counter")
.forEach(el=>{

    counterObserver.observe(el);

});

/* =========================================================
   MOUSE CURSOR GLOW
========================================================= */

const cursor =
document.getElementById("cursor");

window.addEventListener("mousemove",e=>{

    cursor.style.left =
    e.clientX+"px";

    cursor.style.top =
    e.clientY+"px";

});

/* =========================================================
   3D TILT
========================================================= */

document
.querySelectorAll(".tilt")
.forEach(card=>{

    card.addEventListener("mousemove",e=>{

        const rect =
        card.getBoundingClientRect();

        const x =
        e.clientX-rect.left;

        const y =
        e.clientY-rect.top;

        const centerX =
        rect.width/2;

        const centerY =
        rect.height/2;

        const rotateX =
        ((y-centerY)/centerY)*-5;

        const rotateY =
        ((x-centerX)/centerX)*5;

        card.style.transform =
        `perspective(900px)
         rotateX(${rotateX}deg)
         rotateY(${rotateY}deg)
         translateY(-5px)`;

    });

    card.addEventListener("mouseleave",()=>{

        card.style.transform =
        "";

    });

});

/* =========================================================
   COPY EMAIL
========================================================= */

function copyEmail(){

    const email =
    document
    .getElementById("email")
    .textContent
    .trim();

    navigator.clipboard
    .writeText(email)
    .then(()=>{

        const btn =
        event.currentTarget;

        const old =
        btn.textContent;

        btn.textContent =
        "✓ Email Copied";

        setTimeout(()=>{

            btn.textContent =
            old;

        },1800);

    });

}

/* =========================================================
   PARTICLE SYSTEM
========================================================= */

const canvas =
document.getElementById("particles");

const ctx =
canvas.getContext("2d");

let particles = [];

function resizeCanvas(){

    canvas.width =
    window.innerWidth;

    canvas.height =
    window.innerHeight;

}

resizeCanvas();

window.addEventListener(
    "resize",
    resizeCanvas
);

class Particle{

    constructor(){

        this.x =
        Math.random()*canvas.width;

        this.y =
        Math.random()*canvas.height;

        this.vx =
        (Math.random()-.5)*.35;

        this.vy =
        (Math.random()-.5)*.35;

        this.size =
        Math.random()*1.7+.3;

    }

    update(){

        this.x += this.vx;
        this.y += this.vy;

        if(this.x < 0)
            this.x = canvas.width;

        if(this.x > canvas.width)
            this.x = 0;

        if(this.y < 0)
            this.y = canvas.height;

        if(this.y > canvas.height)
            this.y = 0;

    }

    draw(){

        ctx.beginPath();

        ctx.arc(
            this.x,
            this.y,
            this.size,
            0,
            Math.PI*2
        );

        ctx.fillStyle =
        "rgba(125,211,252,.45)";

        ctx.fill();

    }

}

for(let i=0;i<130;i++){

    particles.push(
        new Particle()
    );

}

function connectParticles(){

    for(let a=0;a<particles.length;a++){

        for(
            let b=a+1;
            b<particles.length;
            b++
        ){

            const dx =
            particles[a].x-particles[b].x;

            const dy =
            particles[a].y-particles[b].y;

            const distance =
            Math.sqrt(dx*dx+dy*dy);

            if(distance < 110){

                ctx.beginPath();

                ctx.moveTo(
                    particles[a].x,
                    particles[a].y
                );

                ctx.lineTo(
                    particles[b].x,
                    particles[b].y
                );

                ctx.strokeStyle =
                `rgba(
                    56,
                    189,
                    248,
                    ${1-distance/110}
                )`;

                ctx.lineWidth=.25;

                ctx.stroke();

            }

        }

    }

}

function animateParticles(){

    ctx.clearRect(
        0,
        0,
        canvas.width,
        canvas.height
    );

    particles.forEach(p=>{

        p.update();
        p.draw();

    });

    connectParticles();

    requestAnimationFrame(
        animateParticles
    );

}

animateParticles();

/* =========================================================
   PARALLAX HERO
========================================================= */

window.addEventListener("mousemove",e=>{

    const x =
    (e.clientX/window.innerWidth-.5);

    const y =
    (e.clientY/window.innerHeight-.5);

    const cube =
    document.querySelector(".cube-wrapper");

    if(cube){

        cube.style.transform =
        `translate(${x*18}px,${y*18}px)`;

    }

});

</script>

</body>
</html>
