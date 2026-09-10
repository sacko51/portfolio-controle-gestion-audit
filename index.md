---
layout: null
---
<style>
  body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; line-height: 1.6; color: #333; max-width: 1000px; margin: 0 auto; padding: 20px; background-color: #f9f9f9; }
  h1, h2, h3 { color: #111; text-align: center; }
  .section-title { font-size: 2em; margin-bottom: 5px; margin-top: 40px;}
  .section-line { width: 50px; height: 3px; background-color: #28a745; margin: 0 auto 30px auto; }

  /* Navigation */
  .navbar { display: flex; justify-content: center; gap: 15px; margin-bottom: 40px; flex-wrap: wrap; }
  .navbar a { color: #28a745; text-decoration: none; font-weight: 600; padding: 8px 20px; border: 2px solid #28a745; border-radius: 6px; transition: all 0.2s; }
  .navbar a:hover, .navbar a.active { background-color: #28a745; color: white; }

  /* Section Profil */
  .profile-container { display: flex; gap: 40px; background: white; padding: 40px; border-radius: 12px; box-shadow: 0 4px 6px rgba(0,0,0,0.05); margin-bottom: 50px; align-items: center; }

  .profile-image {
    flex: 0 0 200px;
    width: 200px;
    height: 200px;
    overflow: hidden;
    border-radius: 50%;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    border: 4px solid #fff;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .profile-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center 15%;
  }

  .profile-text { flex: 2; }
  .profile-title { font-size: 1.5em; color: #28a745; font-weight: bold; margin-bottom: 5px; margin-top: 0;}
  .profile-subtitle { color: #666; font-weight: bold; margin-bottom: 20px; font-size: 1.1em; }
  .tech-stack { color: #666; font-size: 0.9em; margin-top: 20px; padding-top: 15px; border-top: 1px dashed #eee; }

  /* Section Projets (Cartes) */
  .projects-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(350px, 1fr)); gap: 30px; margin-bottom: 50px; }
  .project-card { background: white; padding: 30px; border-radius: 12px; box-shadow: 0 4px 6px rgba(0,0,0,0.05); border: 1px solid #eee; display: flex; flex-direction: column; }
  .project-title { color: #28a745; font-size: 1.4em; margin-top: 0; margin-bottom: 15px; text-align: left;}
  .project-desc { flex-grow: 1; margin-bottom: 20px; color: #555; }
  .project-tools { color: #888; font-size: 0.85em; margin-top: 20px; border-top: 1px dashed #eee; padding-top: 15px; }

  /* Section Background (Timeline) */
  .background-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 40px; margin-bottom: 50px; }
  .timeline-col h3 { text-align: left; color: #111; margin-bottom: 30px; font-size: 1.5em;}
  .timeline-item { border-left: 3px solid #28a745; padding-left: 20px; margin-bottom: 30px; position: relative; }
  .timeline-item::before { content: ''; position: absolute; left: -9px; top: 0; width: 15px; height: 15px; background: white; border: 3px solid #28a745; border-radius: 50%; }
  .timeline-date { color: #888; font-size: 0.9em; margin-bottom: 5px; font-weight: bold;}
  .timeline-title { font-weight: bold; color: #333; font-size: 1.1em; margin-bottom: 2px;}
  .timeline-subtitle { color: #555; font-style: italic; margin-bottom: 10px; font-size: 0.95em;}
  .timeline-desc { color: #555; font-size: 0.95em; margin-bottom: 5px;}
  .timeline-tools { font-size: 0.85em; color: #888; margin-top: 5px; font-style: italic;}

  /* Boutons */
  .btn-group { display: flex; gap: 15px; margin-bottom: 10px; }
  .btn { display: inline-block; padding: 8px 20px; border: 2px solid #28a745; color: #28a745; text-decoration: none; border-radius: 6px; font-weight: 600; font-size: 0.9em; transition: all 0.2s; }
  .btn:hover { background-color: #28a745; color: white; }
  .btn-solid { background-color: #28a745; color: white; border: none; padding: 12px 25px; border-radius: 8px; font-size: 1em; text-decoration: none; font-weight: bold;}
  .btn-solid:hover { background-color: #218838; color: white; text-decoration: none;}

  /* Section Contact */
  .contact-section { text-align: center; margin-top: 60px; padding: 40px 0; }
  .contact-buttons { display: flex; justify-content: center; gap: 20px; margin-top: 20px; }

  @media (max-width: 768px) {
    .profile-container { flex-direction: column; text-align: center; }
    .projects-grid, .background-grid { grid-template-columns: 1fr; }
    .timeline-col h3 { text-align: center; }
  }
</style>

<div class="navbar">
  <a href="index.html" class="active">Profil</a>
  <a href="projets.html">Projets</a>
  <a href="parcours.html">Parcours & Contact</a>
</div>

<h1 class="section-title">Profil Professionel</h1>
<div class="section-line"></div>

<div class="profile-container">
  <div class="profile-image" style="background-color: #f0f0f0;">
    <svg width="100" height="100" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
      <circle cx="12" cy="8" r="4" fill="#28a745" opacity="0.6"/>
      <path d="M4 20c0-4.4 3.6-8 8-8s8 3.6 8 8" fill="#28a745" opacity="0.6"/>
    </svg>
  </div>
  <div class="profile-text">
    <p class="profile-title">Bakary SACKO</p>
    <p class="profile-subtitle">Contrôleur de Gestion — À la recherche d'un stage de fin d'études</p>
    <p>Je suis un futur contrôleur de gestion issu d'un parcours Contrôle de Gestion et Audit Organisationnel.</p>
    <p>J'apporte une vision transversale du pilotage de la performance, de l'analyse budgétaire au reporting stratégique, en passant par l'évaluation du contrôle interne, pour aider les entreprises à sécuriser leurs décisions sur des bases financières fiables.</p>
    <p><strong>+33 7 69 42 46 48 · sacko_bakary@outlook.com</strong></p>
    <div class="tech-stack"><strong>Stack Technique :</strong> Excel avancé, Power BI, DAX, Word, PowerPoint, Access, SAP, Ciel, Cegid, Ingeneo, Meg, Dext.</div>
  </div>
</div>
