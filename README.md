# Real-Suhani
Debugging life and deploying dreams . Open to opportunities that challenge me.

I'm Suhani Yadav — a software engineer in the making who genuinely believes the best way to learn is to build something that actually works.
I'm currently in my final year of B.Tech in Computer Science & AI at Netaji Subhas University of Technology, Delhi. Over the past two years I've interned as a MERN backend developer, trained ML models for medical imaging, and analysed business data — because I refuse to be just one thing.
My technical world spans React, Next.js, Node.js, and MongoDB on the web side, PyTorch, OpenCV, and Vision Transformers on the AI side, and LangChain and LangGraph on the GenAI side. I speak fluent C++ when DSA calls, and Python when the data does.
I've built a startup discovery platform, an ocular disease detector, a mood-based music recommender, and a Simon memory game — not because I had to, but because each one taught me something the classroom couldn't.
I'm not looking for easy. I'm looking for meaningful.

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Suhani Yadav — Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;0,700;1,300;1,400&family=DM+Sans:wght@300;400;500&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
<style>
:root{
  --pk1:#00695c;--pk2:#00897b;--pk3:#26a69a;--pk4:#4db6ac;--pk5:#80cbc4;
  --gold:#c9a84c;--gold2:#e8c96a;--cream:#f5f0e8;--dark:#0a1a18;
  --ink:#1a2e2a;--muted:#5a7a75;--border:rgba(0,137,123,0.25);
}
*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}

/* LOADER */
#loader{
  position:fixed;inset:0;z-index:9999;background:var(--dark);
  display:flex;flex-direction:column;align-items:center;justify-content:center;
  transition:opacity .7s ease,visibility .7s ease;
}
#loader.hide{opacity:0;visibility:hidden;pointer-events:none;}
.lp{font-size:90px;animation:lp-anim 1.1s ease-in-out infinite alternate;}
@keyframes lp-anim{0%{transform:scale(1) rotate(-6deg);}100%{transform:scale(1.12) rotate(6deg);filter:drop-shadow(0 0 30px rgba(0,137,123,0.7));}}
.lf{display:flex;gap:7px;margin-top:20px;align-items:flex-end;}
.lf span{
  width:5px;border-radius:8px;
  background:linear-gradient(180deg,var(--gold),var(--pk3));
  animation:lf-w .75s ease-in-out infinite alternate;
}
.lf span:nth-child(1){height:28px;}
.lf span:nth-child(2){height:44px;animation-delay:.1s;}
.lf span:nth-child(3){height:60px;animation-delay:.2s;}
.lf span:nth-child(4){height:44px;animation-delay:.3s;}
.lf span:nth-child(5){height:28px;animation-delay:.4s;}
@keyframes lf-w{0%{opacity:.4;transform:scaleY(.8);}100%{opacity:1;transform:scaleY(1.05);}}
.lt{
  margin-top:30px;font-family:'Space Mono',monospace;font-size:12px;
  color:var(--pk4);letter-spacing:5px;text-transform:uppercase;
  animation:lt-p 1.4s ease-in-out infinite;
}
@keyframes lt-p{0%,100%{opacity:.3;}50%{opacity:1;}}

/* BASE */
body{background:var(--dark);color:var(--cream);font-family:'DM Sans',sans-serif;overflow-x:hidden;}

/* BG */
.bg-m{position:fixed;inset:0;z-index:0;pointer-events:none;
  background:radial-gradient(ellipse 60% 50% at 15% 20%,rgba(0,105,92,.16) 0%,transparent 60%),
  radial-gradient(ellipse 50% 60% at 85% 80%,rgba(0,137,123,.12) 0%,transparent 60%),
  radial-gradient(ellipse 35% 35% at 50% 50%,rgba(201,168,76,.05) 0%,transparent 70%);}
.bg-g{position:fixed;inset:0;z-index:0;pointer-events:none;
  background-image:linear-gradient(rgba(0,137,123,.035) 1px,transparent 1px),linear-gradient(90deg,rgba(0,137,123,.035) 1px,transparent 1px);
  background-size:64px 64px;}

/* NAV */
nav{
  position:fixed;top:0;left:0;right:0;z-index:100;
  padding:14px 44px;display:flex;justify-content:space-between;align-items:center;
  background:rgba(10,26,24,.88);backdrop-filter:blur(22px);
  border-bottom:.5px solid var(--border);transition:box-shadow .3s;
}
.n-logo{
  font-family:'Cormorant Garamond',serif;font-size:21px;font-weight:600;letter-spacing:2px;
  background:linear-gradient(90deg,var(--gold),var(--pk4));-webkit-background-clip:text;-webkit-text-fill-color:transparent;
}
.n-links{display:flex;gap:30px;list-style:none;}
.n-links a{font-size:11px;letter-spacing:2px;text-transform:uppercase;color:rgba(245,240,232,.5);text-decoration:none;font-family:'Space Mono',monospace;transition:color .2s;}
.n-links a:hover{color:var(--gold2);}

/* HERO */
#hero{min-height:100vh;display:flex;align-items:center;padding-top:80px;}
.h-inner{display:grid;grid-template-columns:1fr 400px;gap:60px;align-items:center;width:100%;}
.h-tag{display:inline-block;border:.5px solid rgba(201,168,76,.35);border-radius:4px;padding:5px 16px;font-family:'Space Mono',monospace;font-size:10px;color:var(--gold);letter-spacing:3px;text-transform:uppercase;margin-bottom:22px;background:rgba(201,168,76,.07);}
.h-name{font-family:'Cormorant Garamond',serif;font-size:clamp(50px,8vw,82px);font-weight:700;line-height:1.02;margin-bottom:10px;background:linear-gradient(135deg,#fff 0%,var(--pk4) 50%,var(--gold) 100%);-webkit-background-clip:text;-webkit-text-fill-color:transparent;}
.h-role{font-family:'Cormorant Garamond',serif;font-size:21px;font-weight:300;font-style:italic;color:var(--pk4);letter-spacing:1px;margin-bottom:22px;}
.h-bio{font-size:14px;color:rgba(245,240,232,.52);line-height:1.85;max-width:480px;margin-bottom:34px;}
.h-btns{display:flex;gap:12px;flex-wrap:wrap;}
.bp{padding:12px 26px;border-radius:4px;background:linear-gradient(135deg,var(--pk2),var(--pk1));border:none;color:#fff;font-family:'Space Mono',monospace;font-size:10px;font-weight:700;letter-spacing:2px;text-transform:uppercase;cursor:pointer;text-decoration:none;transition:transform .2s,box-shadow .2s;display:inline-flex;align-items:center;gap:7px;}
.bp:hover{transform:translateY(-2px);box-shadow:0 8px 22px rgba(0,137,123,.35);}
.bo{padding:12px 26px;border-radius:4px;background:transparent;border:.5px solid rgba(201,168,76,.4);color:var(--gold);font-family:'Space Mono',monospace;font-size:10px;font-weight:700;letter-spacing:2px;text-transform:uppercase;cursor:pointer;text-decoration:none;transition:transform .2s,background .2s;display:inline-flex;align-items:center;gap:7px;}
.bo:hover{transform:translateY(-2px);background:rgba(201,168,76,.08);}

/* hero visual */
.h-vis{display:flex;flex-direction:column;align-items:center;}
.h-emoji{font-size:130px;filter:drop-shadow(0 0 40px rgba(0,137,123,.5));animation:hf 4s ease-in-out infinite;}
@keyframes hf{0%,100%{transform:translateY(0) rotate(-3deg);}50%{transform:translateY(-13px) rotate(3deg);}}
.h-stats{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:26px;width:100%;}
.hs{background:rgba(255,255,255,.04);border:.5px solid var(--border);border-radius:8px;padding:14px 10px;text-align:center;}
.hs-n{font-family:'Cormorant Garamond',serif;font-size:26px;font-weight:700;background:linear-gradient(90deg,var(--gold),var(--pk4));-webkit-background-clip:text;-webkit-text-fill-color:transparent;display:block;}
.hs-l{font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--muted);margin-top:2px;}

/* SECTION */
section{position:relative;z-index:1;}
.container{max-width:1050px;margin:0 auto;padding:0 28px;}
.sec-h{display:flex;align-items:center;gap:14px;margin-bottom:42px;}
.sec-h::after{content:'';flex:1;height:.5px;background:linear-gradient(90deg,rgba(0,137,123,.4),transparent);}
.sec-n{font-family:'Cormorant Garamond',serif;font-size:13px;color:var(--muted);}
.sec-l{font-family:'Space Mono',monospace;font-size:10px;letter-spacing:4px;text-transform:uppercase;color:var(--gold);}

/* SKILLS */
#skills{padding:100px 0;}
.sk-grid{display:flex;flex-direction:column;gap:22px;}
.sk-cat{font-family:'Cormorant Garamond',serif;font-size:15px;font-style:italic;color:var(--pk4);margin-bottom:9px;}
.pills{display:flex;flex-wrap:wrap;gap:7px;}
.pill{padding:6px 15px;border-radius:50px;border:.5px solid var(--border);font-size:12px;color:rgba(245,240,232,.72);background:rgba(0,137,123,.06);letter-spacing:1px;transition:all .2s;}
.pill:hover{border-color:var(--pk3);color:var(--pk4);background:rgba(0,137,123,.12);}
.pill.gp{border-color:rgba(201,168,76,.35);background:rgba(201,168,76,.06);color:var(--gold2);}
.pill.gp:hover{background:rgba(201,168,76,.12);}

/* EXPERIENCE */
#experience{padding:100px 0;}
.ex-card{background:rgba(255,255,255,.03);border:.5px solid var(--border);border-left:3px solid var(--pk3);border-radius:0 12px 12px 0;padding:26px 30px;margin-bottom:14px;transition:border-color .2s,transform .2s;}
.ex-card:hover{border-color:var(--pk3);transform:translateX(4px);}
.ex-hd{display:flex;justify-content:space-between;align-items:flex-start;gap:14px;flex-wrap:wrap;}
.ex-role{font-family:'Cormorant Garamond',serif;font-size:20px;font-weight:600;color:#fff;}
.ex-co{font-family:'Space Mono',monospace;font-size:11px;color:var(--pk4);letter-spacing:1px;margin-top:3px;}
.ex-date{font-family:'Space Mono',monospace;font-size:10px;color:var(--muted);border:.5px solid var(--border);border-radius:4px;padding:3px 10px;white-space:nowrap;}
.ex-ul{list-style:none;margin-top:13px;display:flex;flex-direction:column;gap:6px;}
.ex-ul li{font-size:13px;color:rgba(245,240,232,.48);padding-left:15px;position:relative;line-height:1.65;}
.ex-ul li::before{content:'›';position:absolute;left:0;color:var(--pk3);}
.ex-stk{display:flex;flex-wrap:wrap;gap:5px;margin-top:13px;}
.stk{font-size:10px;padding:2px 9px;border-radius:4px;background:rgba(0,137,123,.08);border:.5px solid rgba(0,137,123,.2);color:var(--pk5);letter-spacing:1px;}

/* PROJECTS */
#projects{padding:100px 0;}
.pr-grid{display:grid;grid-template-columns:1fr 1fr;gap:18px;}
.pr-card{background:rgba(255,255,255,.03);border:.5px solid rgba(255,255,255,.07);border-radius:14px;padding:24px;cursor:pointer;position:relative;overflow:hidden;transition:transform .2s,border-color .2s;text-decoration:none;color:inherit;display:block;}
.pr-card::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,var(--pk3),var(--gold));opacity:0;transition:opacity .3s;}
.pr-card:hover{transform:translateY(-5px);border-color:rgba(0,137,123,.35);}
.pr-card:hover::before{opacity:1;}
.pr-hd{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:11px;}
.pr-type{font-family:'Space Mono',monospace;font-size:10px;letter-spacing:2px;text-transform:uppercase;color:var(--pk4);}
.pr-ico{width:28px;height:28px;border-radius:6px;background:rgba(0,137,123,.1);border:.5px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:14px;transition:background .2s;}
.pr-card:hover .pr-ico{background:rgba(0,137,123,.22);}
.pr-name{font-family:'Cormorant Garamond',serif;font-size:21px;font-weight:600;color:#fff;margin-bottom:9px;line-height:1.2;}
.pr-desc{font-size:12px;color:rgba(245,240,232,.42);line-height:1.7;margin-bottom:13px;}
.pr-tags{display:flex;flex-wrap:wrap;gap:5px;}
.pr-tag{font-size:10px;padding:2px 8px;border-radius:4px;background:rgba(255,255,255,.04);border:.5px solid rgba(255,255,255,.1);color:rgba(245,240,232,.38);}

/* EDUCATION */
#education{padding:100px 0;}
.ed-grid{display:flex;flex-direction:column;gap:11px;}
.ed-card{background:rgba(255,255,255,.03);border:.5px solid rgba(255,255,255,.07);border-radius:10px;padding:18px 24px;display:flex;justify-content:space-between;align-items:center;transition:border-color .2s;}
.ed-card:hover{border-color:rgba(201,168,76,.3);}
.ed-crs{font-family:'Cormorant Garamond',serif;font-size:17px;font-weight:600;color:#fff;}
.ed-sc{font-size:12px;color:var(--muted);margin-top:3px;}
.ed-yr{font-family:'Space Mono',monospace;font-size:13px;color:var(--gold);}

/* CONTACT */
#contact{padding:100px 0 60px;}
.ct-wrap{background:rgba(255,255,255,.03);border:.5px solid var(--border);border-radius:20px;padding:50px;text-align:center;}
.ct-title{font-family:'Cormorant Garamond',serif;font-size:clamp(30px,5vw,50px);font-weight:700;background:linear-gradient(135deg,#fff,var(--pk4));-webkit-background-clip:text;-webkit-text-fill-color:transparent;margin-bottom:10px;}
.ct-sub{font-size:14px;color:var(--muted);margin-bottom:34px;font-style:italic;font-family:'Cormorant Garamond',serif;}
.ct-links{display:flex;gap:11px;justify-content:center;flex-wrap:wrap;}
.cl{display:flex;align-items:center;gap:8px;padding:11px 20px;border-radius:8px;border:.5px solid rgba(255,255,255,.1);color:rgba(245,240,232,.62);font-size:13px;background:rgba(255,255,255,.03);cursor:pointer;text-decoration:none;transition:all .2s;}
.cl:hover{border-color:rgba(0,137,123,.5);color:var(--pk4);transform:translateY(-2px);}
.cl.gl:hover{border-color:rgba(201,168,76,.5);color:var(--gold);}

/* FOOTER */
footer{text-align:center;padding:22px;font-family:'Space Mono',monospace;font-size:10px;color:rgba(245,240,232,.14);letter-spacing:2px;border-top:.5px solid var(--border);}

/* REVEAL */
.reveal{opacity:0;transform:translateY(28px);transition:opacity .7s ease,transform .7s ease;}
.reveal.v{opacity:1;transform:translateY(0);}

/* RESPONSIVE */
@media(max-width:768px){
  .h-inner{grid-template-columns:1fr;}
  .h-vis{order:-1;}
  .h-emoji{font-size:90px;}
  .pr-grid{grid-template-columns:1fr;}
  nav{padding:12px 18px;}
  .container{padding:0 16px;}
  .ct-wrap{padding:30px 18px;}
}
@media(max-width:480px){.n-links{display:none;}}
</style>
</head>
<body>

<div id="loader">
  <div class="lp">🦚</div>
  <div class="lf"><span></span><span></span><span></span><span></span><span></span></div>
  <div class="lt">Loading Portfolio</div>
</div>

<div class="bg-m"></div>
<div class="bg-g"></div>

<nav id="nav">
  <div class="n-logo">SY 🦚</div>
  <ul class="n-links">
    <li><a href="#hero">Home</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#education">Education</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<section id="hero">
  <div class="container">
    <div class="h-inner">
      <div class="reveal">
        <div class="h-tag">⚡ Open to Opportunities</div>
        <h1 class="h-name">Suhani<br>Yadav</h1>
        <div class="h-role">Full Stack Developer · AI/ML Engineer</div>
        <p class="h-bio">Final-year CSAI student at NSUT, Delhi. I build at the intersection of full-stack web and AI/ML — real-time chat apps, deep learning models with 94%+ accuracy, and GenAI-powered tools.</p>
        <div class="h-btns">
          <a href="https://github.com/suhani-yadav04" target="_blank" class="bp">🐙 GitHub</a>
          <a href="https://www.linkedin.com/in/suhani-yadav04" target="_blank" class="bp">💼 LinkedIn</a>
          <a href="mailto:suhani.yadav.ug22@nsut.ac.in" class="bo">📧 Email Me</a>
        </div>
      </div>
      <div class="h-vis reveal">
        <div class="h-emoji">🦚</div>
        <div class="h-stats">
          <div class="hs"><span class="hs-n">5+</span><div class="hs-l">Projects</div></div>
          <div class="hs"><span class="hs-n">3</span><div class="hs-l">Internships</div></div>
          <div class="hs"><span class="hs-n">94%</span><div class="hs-l">ML Accuracy</div></div>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="skills">
  <div class="container">
    <div class="sec-h reveal"><span class="sec-n">01</span><span class="sec-l">Technical Skills</span></div>
    <div class="sk-grid">
      <div class="reveal"><div class="sk-cat">Generative AI</div><div class="pills"><span class="pill gp">LangChain</span><span class="pill gp">LangGraph</span><span class="pill gp">RAG</span><span class="pill gp">Prompt Engineering</span></div></div>
      <div class="reveal"><div class="sk-cat">Languages</div><div class="pills"><span class="pill">C++ · DSA</span><span class="pill">Python</span><span class="pill">JavaScript</span><span class="pill">SQL</span></div></div>
      <div class="reveal"><div class="sk-cat">Web Development</div><div class="pills"><span class="pill">React.js</span><span class="pill">Next.js</span><span class="pill">Node.js</span><span class="pill">Express</span><span class="pill">MongoDB</span><span class="pill">Tailwind CSS</span><span class="pill">Socket.io</span><span class="pill">HTML · CSS</span></div></div>
      <div class="reveal"><div class="sk-cat">AI / ML</div><div class="pills"><span class="pill">PyTorch</span><span class="pill">OpenCV</span><span class="pill">Vision Transformers</span><span class="pill">Scikit-learn</span><span class="pill">NLTK</span><span class="pill">Matplotlib</span><span class="pill">Streamlit</span></div></div>
      <div class="reveal"><div class="sk-cat">Tools & Platforms</div><div class="pills"><span class="pill">Git · GitHub</span><span class="pill">Vercel</span><span class="pill">Jupyter</span><span class="pill">Sanity CMS</span><span class="pill">Power BI</span><span class="pill">Excel</span></div></div>
    </div>
  </div>
</section>

<section id="experience">
  <div class="container">
    <div class="sec-h reveal"><span class="sec-n">02</span><span class="sec-l">Experience</span></div>
    <div class="ex-card reveal">
      <div class="ex-hd">
        <div><div class="ex-role">MERN Backend Developer Intern</div><div class="ex-co">◈ Graduation · Remote</div></div>
        <div class="ex-date">Oct 2024 – Jan 2025</div>
      </div>
      <ul class="ex-ul">
        <li>Built a real-time chat app with MERN + Socket.io supporting hundreds of concurrent users</li>
        <li>Optimised API performance and backend scalability for multiple simultaneous sessions</li>
      </ul>
      <div class="ex-stk"><span class="stk">Node.js</span><span class="stk">Express</span><span class="stk">MongoDB</span><span class="stk">Socket.io</span></div>
    </div>
    <div class="ex-card reveal">
      <div class="ex-hd">
        <div><div class="ex-role">AI / ML Research Intern</div><div class="ex-co">◈ Dewtown · Remote</div></div>
        <div class="ex-date">Oct 2024 – Jan 2025</div>
      </div>
      <ul class="ex-ul">
        <li>Early brain tumor detection from MRI scans — achieved 94% accuracy</li>
        <li>Built visual tools to highlight affected regions for healthcare professionals</li>
      </ul>
      <div class="ex-stk"><span class="stk">Python</span><span class="stk">PyTorch</span><span class="stk">Medical Imaging</span></div>
    </div>
    <div class="ex-card reveal">
      <div class="ex-hd">
        <div><div class="ex-role">Business Analyst Intern</div><div class="ex-co">◈ CrackNonTech · Remote</div></div>
        <div class="ex-date">Oct 2025 – Present</div>
      </div>
      <ul class="ex-ul">
        <li>Industry analysis, profitability assessments and business case problem solving</li>
        <li>SQL & Python for data-driven analysis and insight communication</li>
      </ul>
      <div class="ex-stk"><span class="stk">SQL</span><span class="stk">Python</span><span class="stk">Power BI</span><span class="stk">Excel</span></div>
    </div>
  </div>
</section>

<section id="projects">
  <div class="container">
    <div class="sec-h reveal"><span class="sec-n">03</span><span class="sec-l">Projects</span></div>
    <div class="pr-grid">
      <a href="https://pitchbase-app.vercel.app/user/a87IKZMulbOquOhziLwsvy" target="_blank" class="pr-card reveal">
        <div class="pr-hd"><div class="pr-type">◈ Web App</div><div class="pr-ico">🔗</div></div>
        <div class="pr-name">PitchBase</div>
        <div class="pr-desc">Startup discovery & submission platform — founders showcase, editors spotlight. Auth + personalised profiles.</div>
        <div class="pr-tags"><span class="pr-tag">Next.js</span><span class="pr-tag">React</span><span class="pr-tag">Tailwind</span><span class="pr-tag">Sanity CMS</span></div>
      </a>
      <a href="https://github.com/suhani-yadav04/Ocular-disease-recognization-" target="_blank" class="pr-card reveal">
        <div class="pr-hd"><div class="pr-type">◈ Deep Learning</div><div class="pr-ico">🐙</div></div>
        <div class="pr-name">Ocular Disease Recognition</div>
        <div class="pr-desc">Retinal fundus classification using LBP-enhanced CNNs + Vision Transformers. 98%+ validation accuracy on ODIR dataset.</div>
        <div class="pr-tags"><span class="pr-tag">PyTorch</span><span class="pr-tag">OpenCV</span><span class="pr-tag">ViT</span><span class="pr-tag">ResNet50</span></div>
      </a>
      <a href="https://github.com/suhani-yadav04/Moody_Music_recommender-app.py" target="_blank" class="pr-card reveal">
        <div class="pr-hd"><div class="pr-type">◈ NLP · Python</div><div class="pr-ico">🐙</div></div>
        <div class="pr-name">Moody Music Recommender</div>
        <div class="pr-desc">Recommends songs from your mood using TF-IDF + cosine similarity. Album covers + quick play links.</div>
        <div class="pr-tags"><span class="pr-tag">Streamlit</span><span class="pr-tag">NLTK</span><span class="pr-tag">Python</span><span class="pr-tag">Matplotlib</span></div>
      </a>
      <a href="http://127.0.0.1:5500/index.html" target="_blank" class="pr-card reveal">
        <div class="pr-hd"><div class="pr-type">◈ Game · JS</div><div class="pr-ico">🎮</div></div>
        <div class="pr-name">Simon Game</div>
        <div class="pr-desc">Classic Simon memory game in vanilla JS — animated, interactive, with increasing difficulty levels.</div>
        <div class="pr-tags"><span class="pr-tag">JavaScript</span><span class="pr-tag">HTML</span><span class="pr-tag">CSS</span><span class="pr-tag">Game Logic</span></div>
      </a>
    </div>
  </div>
</section>

<section id="education">
  <div class="container">
    <div class="sec-h reveal"><span class="sec-n">04</span><span class="sec-l">Education</span></div>
    <div class="ed-grid">
      <div class="ed-card reveal">
        <div><div class="ed-crs">B.Tech — Computer Science & AI</div><div class="ed-sc">Netaji Subhas University of Technology (NSUT), New Delhi</div></div>
        <div class="ed-yr">2022 – 2026</div>
      </div>
      <div class="ed-card reveal">
        <div><div class="ed-crs">CBSE Class XII</div><div class="ed-sc">John Wesley Convent School</div></div>
        <div class="ed-yr">2022</div>
      </div>
      <div class="ed-card reveal">
        <div><div class="ed-crs">CBSE Class X</div><div class="ed-sc">D.G.V.SR SEC Public School</div></div>
        <div class="ed-yr">2020</div>
      </div>
    </div>
  </div>
</section>

<section id="contact">
  <div class="container">
    <div class="sec-h reveal"><span class="sec-n">05</span><span class="sec-l">Get In Touch</span></div>
    <div class="ct-wrap reveal">
      <div class="ct-title">Let's Build Together 🦚</div>
      <div class="ct-sub">Open to internships, collaborations & full-time roles</div>
      <div class="ct-links">
        <a class="cl" href="mailto:suhani.yadav.ug22@nsut.ac.in">📧 Email</a>
        <a class="cl" href="https://github.com/suhani-yadav04" target="_blank">🐙 GitHub</a>
        <a class="cl" href="https://www.linkedin.com/in" target="_blank">💼 LinkedIn</a>
        <a class="cl gl" href="tel:+918398023440">📱 +91-8398023440</a>
      </div>
    </div>
  </div>
</section>

<footer>© 2025 Suhani Yadav · NSUT CSAI · Built with 🦚 & lots of chai</footer>

<script>
// LOADER
window.addEventListener('load',()=>{
  setTimeout(()=>{
    document.getElementById('loader').classList.add('hide')
    setTimeout(checkReveal,200)
  },1900)
})

// REVEAL
function checkReveal(){
  document.querySelectorAll('.reveal').forEach(el=>{
    if(el.getBoundingClientRect().top<window.innerHeight-60)
      el.classList.add('v')
  })
}
window.addEventListener('scroll',checkReveal)

// NAV SHADOW
window.addEventListener('scroll',()=>{
  document.getElementById('nav').style.boxShadow=
    window.scrollY>40?'0 4px 30px rgba(0,0,0,.4)':'none'
})

// SMOOTH SCROLL
document.querySelectorAll('a[href^="#"]').forEach(a=>{
  a.addEventListener('click',e=>{
    e.preventDefault()
    const t=document.querySelector(a.getAttribute('href'))
    if(t)t.scrollIntoView({behavior:'smooth',block:'start'})
  })
})
</script>
</body>
</html>
