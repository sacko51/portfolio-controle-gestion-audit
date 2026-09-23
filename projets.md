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
  <a href="projets.html" class="active">Projets</a>
  <a href="parcours.html">Parcours & Contact</a>
</div>

<h1 class="section-title">Projets</h1>
<div class="section-line"></div>
<p style="text-align: center; margin-bottom: 40px; color: #666;">Focus sur le pilotage de la performance, l'audit interne et la modélisation financière.</p>

<div class="projects-grid">

  <div class="project-card">
    <h3 class="project-title">Diagnostic & Pilotage de la Performance</h3>
    <div class="project-desc">
      <strong>Diagnostic financier et construction d'un modèle budgétaire pour le CHHS.</strong><br><br>
      Missions : Diagnostic financier sur 3 exercices et analyse de rentabilité par activité (comptabilité analytique, clés de répartition), révélant un effet de ciseaux masse salariale/CA de +4,8 points. Construction d'un modèle budgétaire avec décomposition des écarts (volume/coût), d'un tableau de bord de 18 KPI et d'un dashboard Power BI (4 pages, 24 mesures DAX).
    </div>
    <div class="btn-group">
      <a href="https://github.com/sacko51/chhs-controle-gestion" class="btn" target="_blank">Voir le projet</a>
    </div>
    <div class="project-tools">Outils : Excel avancé, Power BI, DAX.</div>
  </div>

  <div class="project-card">
    <h3 class="project-title">Audit Interne & Prévisions</h3>
    <div class="project-desc">
      <strong>Audit comptable et modélisation prévisionnelle pour le CHHS.</strong><br><br>
      Missions : Audit d'un journal comptable de 3 015 écritures via 9 tests de détection automatisés (doublons, TVA incohérente, anomalies), et cartographie des risques selon le référentiel COSO. Modélisation prévisionnelle N+1 à 3 scénarios avec analyse de sensibilité, débouchant sur un plan d'action chiffré à +1 850 k€ de gain potentiel annuel.
    </div>
    <div class="btn-group">
      <a href="https://github.com/sacko51/chhs-controle-gestion" class="btn" target="_blank">Voir le projet</a>
    </div>
    <div class="project-tools">Outils : Contrôle interne, Modélisation financière.</div>
  </div>
  <div class="project-card">
    <h3 class="project-title">Contrôle de Gestion Industriel</h3>
    <div class="project-desc">
      <strong>Comparaison des méthodes de calcul des coûts pour une PME industrielle fictive (Mécano-Est SAS).</strong><br><br>
      Missions : Comparaison coûts complets méthode traditionnelle vs méthode ABC (5 inducteurs d'activité) sur deux gammes de production, révélant un subventionnement croisé entre les gammes standard et sur-mesure. Valorisation des stocks selon les méthodes FIFO et PUMP, et analyse du seuil de rentabilité et du risque d'exploitation.
    </div>
    <div class="btn-group">
      <a href="https://github.com/sacko51/Mecano-Est" class="btn" target="_blank">Voir le projet</a>
    </div>
    <div class="project-tools">Outils : Excel avancé (modélisation formulée), comptabilité analytique.</div>
  </div>

  <div class="project-card">
    <h3 class="project-title">Gestion de Trésorerie & Pilotage du BFR</h3>
    <div class="project-desc">
      <strong>Plan de trésorerie prévisionnel et pilotage du BFR pour une PME fictive de négoce et distribution.</strong><br><br>
      Missions : Construction d'un plan de trésorerie glissant sur 12 mois (encaissements, décaissements, TVA), diagnostic d'une impasse de trésorerie liée à un effet de ciseau du BFR en phase de croissance, suivi des indicateurs DSO/DPO, et modélisation d'un scénario de financement corrigé neutralisant l'impasse.
    </div>
    <div class="btn-group">
      <a href="https://github.com/sacko51/Tresorerie-BFR" class="btn" target="_blank">Voir le projet</a>
    </div>
    <div class="project-tools">Outils : Excel avancé (modélisation formulée), gestion de trésorerie.</div>
  </div>
</div>
