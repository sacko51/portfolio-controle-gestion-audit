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
  <a href="index.html">Profil</a>
  <a href="projets.html">Projets</a>
  <a href="parcours.html" class="active">Parcours & Contact</a>
</div>

<h1 class="section-title">Mon Parcours</h1>
<div class="section-line"></div>

<div class="background-grid">

  <div class="timeline-col">
    <h3>Études</h3>

    <div class="timeline-item">
      <div class="timeline-date">2025 - 2027</div>
      <div class="timeline-title">Master Contrôle de Gestion et Audit Organisationnel</div>
      <div class="timeline-subtitle">URCA, Reims</div>
      <div class="timeline-desc">Focus : Contrôle de gestion, analyse des écarts, tableaux de bord et gestion financière.</div>
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2022 - 2025</div>
      <div class="timeline-title">Licence Finance, Comptabilité, Contrôle</div>
      <div class="timeline-subtitle">URCA, Troyes</div>
      <div class="timeline-desc">Focus : Comptabilité de gestion, systèmes d'information et analyse financière.</div>
    </div>
  </div>

  <div class="timeline-col">
    <h3>Expériences Professionnelles</h3>

    <div class="timeline-item">
      <div class="timeline-date">07/2026 - 08/2026</div>
      <div class="timeline-title">Assistant Comptable Stagiaire</div>
      <div class="timeline-subtitle">FCN Expertise Audit Conseil, Reims</div>
      <div class="timeline-desc">• Saisie de factures d'achat/vente sur Cegid Expert et Ingeneo, avec contrôle systématique des imputations et de la TVA.</div>
      <div class="timeline-desc">• Réalisation de rapprochements bancaires et lettrage des comptes clients/fournisseurs pour détecter et justifier les écarts.</div>
      <div class="timeline-desc">• Contrôle de cohérence des déclarations de TVA et participation au traitement d'opérations intracommunautaires (DEB).</div>
      <div class="timeline-desc">• Participation à des travaux de clôture et de révision comptable.</div>
      <div class="timeline-tools">Outils : Cegid Expert, Ingeneo, Excel</div>
    </div>

    <div class="timeline-item">
      <div class="timeline-date">01/2025 - 02/2025</div>
      <div class="timeline-title">Assistant Comptable Stagiaire</div>
      <div class="timeline-subtitle">Société Conseils Formalité, Paris</div>
      <div class="timeline-desc">• Saisie et contrôle des pièces comptables (factures d'achats et de ventes, relevés bancaires) dans le respect des procédures internes.</div>
      <div class="timeline-desc">• Contribution à la préparation des déclarations fiscales et à la fabrication de l'information comptable.</div>
      <div class="timeline-tools">Outils : Excel, Comptabilité</div>
    </div>

    <div class="timeline-item">
      <div class="timeline-date">05/2023 - 12/2023</div>
      <div class="timeline-title">Médiateur Numérique</div>
      <div class="timeline-subtitle">Préfecture de l'Aube, Troyes</div>
      <div class="timeline-desc">• Accompagnement des personnes en difficulté avec l'informatique dans la réalisation de leurs démarches administratives en ligne (cartes grises, titres de séjour, permis, etc.).</div>
      <div class="timeline-desc">• Information, orientation et explication des procédures administratives auprès des usagers.</div>
      <div class="timeline-desc">• Vérification des pièces justificatives et sécurisation des dossiers pour limiter les erreurs et les risques de rejet.</div>
      <div class="timeline-tools">Outil : Accompagnement administratif</div>
    </div>

  </div>

</div>

<div class="contact-section">
  <h2 class="section-title">Discutons de vos enjeux</h2>
  <div class="section-line"></div>
  <p>Besoin d'un regard analytique et rigoureux sur votre pilotage financier ?</p>

  <div class="contact-buttons">
    <a href="mailto:sackobaka604@gmail.com" class="btn-solid">Email</a>
    <a href="#" class="btn-solid" target="_blank">LinkedIn</a>
  </div>
</div>
