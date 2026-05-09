<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Script DM — Flux B · Réparateur du Peuple</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Manrope:wght@300;400;500;600;700;800&display=swap');

*,*::before,*::after{margin:0;padding:0;box-sizing:border-box;}

:root {
  --white:   #FFFFFF;
  --off:     #F7F9FC;
  --ice:     #EEF4FF;
  --blue-l:  #C7D9FF;
  --blue:    #3B6EF5;
  --navy:    #0D1B3E;
  --mid:     #8A96B0;
  --border:  #E4EBF8;
  --success: #34C77B;
  --warn:    #F59E0B;
  --red:     #EF4444;
  --purple:  #8B5CF6;
}

body { background: #F0F4FB; font-family: 'Manrope', sans-serif; color: var(--navy); }

@media print {
  header { position: relative; }
  body { background: white; }
}

/* HEADER */
header {
  background: var(--navy); padding: 16px 40px;
  display: flex; align-items: center; justify-content: space-between;
  position: sticky; top: 0; z-index: 100;
}
.h-left h1 { font-family: 'Plus Jakarta Sans', sans-serif; font-size: 16px; font-weight: 800; color: white; }
.h-left p { font-size: 11px; color: var(--mid); margin-top: 2px; }
.h-pills { display: flex; gap: 8px; }
.hpill { padding: 4px 12px; border-radius: 20px; font-size: 10px; font-weight: 700; letter-spacing: 0.5px; }
.hp-b { background: rgba(59,110,245,0.25); color: #7aaeff; border: 1px solid rgba(59,110,245,0.3); }
.hp-g { background: rgba(52,199,123,0.2); color: #5cdd9b; border: 1px solid rgba(52,199,123,0.3); }
.hp-p { background: rgba(139,92,246,0.2); color: #c4b5fd; border: 1px solid rgba(139,92,246,0.3); }
.hp-w { background: rgba(245,158,11,0.2); color: #fbbf24; border: 1px solid rgba(245,158,11,0.3); }

.wrap { max-width: 900px; margin: 0 auto; padding: 32px 24px 80px; }

/* SDIV */
.sdiv {
  display: flex; align-items: center; gap: 12px;
  margin: 36px 0 18px;
  font-size: 10px; font-weight: 800; letter-spacing: 2.5px;
  text-transform: uppercase; color: var(--mid);
}
.sdiv::before,.sdiv::after { content:''; flex:1; height:1px; background:var(--border); }

/* INTRO CARDS */
.intro-grid { display: grid; grid-template-columns: repeat(3,1fr); gap: 10px; margin-bottom: 24px; }
.ig-card { background: white; border: 1.5px solid var(--border); border-radius: 12px; padding: 14px 16px; }
.ig-label { font-size: 9px; font-weight: 800; letter-spacing: 2px; text-transform: uppercase; color: var(--mid); margin-bottom: 4px; }
.ig-val { font-family: 'Plus Jakarta Sans', sans-serif; font-size: 13px; font-weight: 700; color: var(--navy); }

/* FLOW DIAGRAM */
.flow {
  background: white; border: 1.5px solid var(--border);
  border-radius: 14px; padding: 20px 24px; margin-bottom: 28px;
}
.flow h3 {
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-size: 13px; font-weight: 800; color: var(--navy); margin-bottom: 14px;
}
.flow-steps { display: flex; align-items: center; gap: 0; flex-wrap: wrap; }
.flow-step {
  display: flex; flex-direction: column; align-items: center;
  gap: 5px; padding: 10px 14px; border-radius: 10px;
  font-size: 11px; font-weight: 700; text-align: center; min-width: 90px;
}
.fs-blue { background: var(--ice); color: var(--blue); border: 1.5px solid var(--blue-l); }
.fs-green { background: rgba(52,199,123,0.08); color: var(--success); border: 1.5px solid rgba(52,199,123,0.25); }
.fs-warn { background: rgba(245,158,11,0.08); color: var(--warn); border: 1.5px solid rgba(245,158,11,0.25); }
.fs-purple { background: rgba(139,92,246,0.08); color: var(--purple); border: 1.5px solid rgba(139,92,246,0.25); }
.fs-navy { background: rgba(13,27,62,0.06); color: var(--navy); border: 1.5px solid rgba(13,27,62,0.15); }
.flow-arrow { font-size: 16px; color: var(--mid); padding: 0 4px; }
.flow-step .icon { font-size: 18px; }

/* ENTRY TYPES */
.entry-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-bottom: 8px; }
.entry-card {
  background: white; border: 1.5px solid var(--border);
  border-radius: 12px; padding: 14px 16px;
  display: flex; gap: 12px; align-items: flex-start;
}
.entry-icon { font-size: 22px; flex-shrink: 0; }
.entry-tag {
  font-size: 9px; font-weight: 800; letter-spacing: 1.5px;
  text-transform: uppercase; padding: 2px 8px; border-radius: 4px;
  display: inline-block; margin-bottom: 5px;
}
.et-1 { background: var(--ice); color: var(--blue); }
.et-2 { background: rgba(52,199,123,0.1); color: var(--success); }
.et-3 { background: rgba(245,158,11,0.1); color: var(--warn); }
.et-4 { background: rgba(139,92,246,0.1); color: var(--purple); }
.entry-title { font-family: 'Plus Jakarta Sans', sans-serif; font-size: 13px; font-weight: 800; color: var(--navy); margin-bottom: 3px; }
.entry-examples { font-size: 11px; color: var(--mid); line-height: 1.6; font-style: italic; }

/* CONVERSATION BLOCK */
.conv-block {
  background: white; border: 1.5px solid var(--border);
  border-radius: 14px; overflow: hidden; margin-bottom: 12px;
}

.conv-header {
  padding: 12px 18px; border-bottom: 1.5px solid var(--border);
  display: flex; align-items: center; gap: 12px;
}
.conv-step-num {
  width: 28px; height: 28px; border-radius: 8px;
  display: flex; align-items: center; justify-content: center;
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-size: 12px; font-weight: 800; flex-shrink: 0;
}
.csn-blue { background: var(--ice); color: var(--blue); }
.csn-green { background: rgba(52,199,123,0.1); color: var(--success); }
.csn-warn { background: rgba(245,158,11,0.1); color: var(--warn); }
.csn-red { background: rgba(239,68,68,0.1); color: var(--red); }
.csn-purple { background: rgba(139,92,246,0.1); color: var(--purple); }
.csn-navy { background: rgba(13,27,62,0.08); color: var(--navy); }

.conv-title { font-family: 'Plus Jakarta Sans', sans-serif; font-size: 14px; font-weight: 800; color: var(--navy); }
.conv-sub { font-size: 11px; color: var(--mid); margin-top: 1px; }
.conv-tag {
  margin-left: auto; font-size: 9px; font-weight: 800;
  letter-spacing: 1px; text-transform: uppercase;
  padding: 3px 10px; border-radius: 5px;
}
.ct-obj { background: var(--ice); color: var(--blue); }
.ct-close { background: rgba(52,199,123,0.1); color: var(--success); }
.ct-obj2 { background: rgba(245,158,11,0.1); color: var(--warn); }
.ct-fall { background: rgba(139,92,246,0.1); color: var(--purple); }

.conv-body { padding: 18px 20px; display: flex; flex-direction: column; gap: 14px; }

/* MESSAGE BUBBLES */
.msg-row { display: flex; flex-direction: column; gap: 6px; }

.msg-label {
  font-size: 9px; font-weight: 800; letter-spacing: 1.5px;
  text-transform: uppercase;
}
.ml-prospect { color: var(--mid); }
.ml-us { color: var(--blue); }

.bubble {
  max-width: 82%; padding: 11px 16px;
  border-radius: 16px; font-size: 13.5px; line-height: 1.7;
}

.bubble-prospect {
  background: var(--off); border: 1.5px solid var(--border);
  border-radius: 16px 16px 16px 4px; color: #3a4a6b;
  align-self: flex-start;
}

.bubble-us {
  background: var(--blue); color: white;
  border-radius: 16px 16px 4px 16px;
  align-self: flex-end;
}

.bubble-us strong { font-weight: 700; }
.bubble-prospect strong { color: var(--navy); font-weight: 700; }

/* NOTE BOX */
.note {
  background: var(--ice); border: 1px solid var(--blue-l);
  border-radius: 10px; padding: 11px 15px;
  font-size: 11.5px; color: #2a3a6b; line-height: 1.6;
}
.note strong { font-weight: 700; }

.warn-note {
  background: rgba(245,158,11,0.06); border: 1px solid rgba(245,158,11,0.25);
  border-left: 3px solid var(--warn);
  border-radius: 0 10px 10px 0; padding: 11px 15px;
  font-size: 11.5px; color: #7a5000; line-height: 1.6;
}
.warn-note strong { font-weight: 700; }

.success-note {
  background: rgba(52,199,123,0.06); border: 1px solid rgba(52,199,123,0.25);
  border-radius: 10px; padding: 11px 15px;
  font-size: 11.5px; color: #1a6640; line-height: 1.6;
}
.success-note strong { font-weight: 700; }

/* VARIANTS */
.variants { display: flex; flex-direction: column; gap: 8px; margin-top: 4px; }
.variant {
  border: 1.5px solid var(--border); border-radius: 10px; overflow: hidden;
}
.variant-head {
  padding: 7px 12px; font-size: 10px; font-weight: 800;
  letter-spacing: 1px; text-transform: uppercase;
  border-bottom: 1.5px solid var(--border);
}
.vh-a { background: rgba(52,199,123,0.06); color: var(--success); }
.vh-b { background: rgba(245,158,11,0.06); color: var(--warn); }
.vh-c { background: rgba(239,68,68,0.06); color: var(--red); }
.variant-body { padding: 12px 16px; background: white; }
.variant-body .bubble-us { font-size: 13px; }

/* OBJECTION GRID */
.obj-grid { display: flex; flex-direction: column; gap: 10px; }
.obj-item { background: white; border: 1.5px solid var(--border); border-radius: 12px; overflow: hidden; }
.obj-item-head {
  padding: 11px 16px; border-bottom: 1.5px solid var(--border);
  display: flex; align-items: center; gap: 10px;
}
.obj-icon { font-size: 18px; }
.obj-title { font-family: 'Plus Jakarta Sans', sans-serif; font-size: 13px; font-weight: 800; color: var(--navy); }
.obj-body { display: grid; grid-template-columns: 1fr 1fr; gap: 0; }
.obj-col { padding: 14px 16px; }
.obj-col:first-child { border-right: 1.5px solid var(--border); }
.obj-col-label { font-size: 9px; font-weight: 800; letter-spacing: 1.5px; text-transform: uppercase; color: var(--mid); margin-bottom: 8px; }

/* ROUTE CARDS */
.routes { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 10px; }
.route-card { border-radius: 12px; padding: 16px; border: 1.5px solid; }
.rc-green { background: rgba(52,199,123,0.06); border-color: rgba(52,199,123,0.3); }
.rc-blue { background: var(--ice); border-color: var(--blue-l); }
.rc-warn { background: rgba(245,158,11,0.06); border-color: rgba(245,158,11,0.25); }
.rc-title { font-family: 'Plus Jakarta Sans', sans-serif; font-size: 13px; font-weight: 800; margin-bottom: 8px; }
.rc-green .rc-title { color: var(--success); }
.rc-blue .rc-title { color: var(--blue); }
.rc-warn .rc-title { color: var(--warn); }
.rc-body { font-size: 12px; line-height: 1.6; color: #3a4a6b; }
.rc-body strong { font-weight: 700; color: var(--navy); }

/* RELANCE */
.relance-row { display: grid; grid-template-columns: 60px 1fr; gap: 0; background: white; border: 1.5px solid var(--border); border-radius: 12px; overflow: hidden; margin-bottom: 8px; }
.rel-day { display: flex; align-items: center; justify-content: center; padding: 14px 8px; background: var(--navy); color: white; font-family: 'Plus Jakarta Sans', sans-serif; font-size: 12px; font-weight: 800; text-align: center; }
.rel-body { padding: 14px 18px; }
.rel-ctx { font-size: 11px; color: var(--mid); margin-bottom: 8px; }
</style>
</head>
<body>

<header>
  <div class="h-left">
    <h1>💬 Script DM — Flux B · Réparateur du Peuple</h1>
    <p>Instagram · TikTok · WhatsApp · Tentative de close en DM → VSL en backup</p>
  </div>
  <div class="h-pills">
    <span class="hpill hp-b">Close en DM</span>
    <span class="hpill hp-g">VSL backup</span>
    <span class="hpill hp-p">Objections</span>
    <span class="hpill hp-w">Relances</span>
  </div>
</header>

<div class="wrap">

  <!-- INTRO -->
  <div class="intro-grid" style="margin-top:8px">
    <div class="ig-card">
      <div class="ig-label">Objectif principal</div>
      <div class="ig-val">Closer directement en DM</div>
    </div>
    <div class="ig-card">
      <div class="ig-label">Objectif secondaire</div>
      <div class="ig-val">Envoyer vers la VSL</div>
    </div>
    <div class="ig-card">
      <div class="ig-label">Offre cible</div>
      <div class="ig-val">Pro 397€ → Starter 97€</div>
    </div>
  </div>

  <!-- FLOW -->
  <div class="flow">
    <h3>🗺️ Parcours DM — Vue d'ensemble</h3>
    <div class="flow-steps">
      <div class="flow-step fs-blue"><span class="icon">💬</span>Message entrant</div>
      <div class="flow-arrow">→</div>
      <div class="flow-step fs-blue"><span class="icon">🪝</span>Accroche</div>
      <div class="flow-arrow">→</div>
      <div class="flow-step fs-blue"><span class="icon">🔍</span>Qualification</div>
      <div class="flow-arrow">→</div>
      <div class="flow-step fs-green"><span class="icon">💰</span>Close DM</div>
      <div class="flow-arrow">→</div>
      <div class="flow-step fs-green"><span class="icon">✅</span>Vente Pro</div>
    </div>
    <div class="flow-steps" style="margin-top:8px; padding-top:8px; border-top:1px dashed var(--border)">
      <div class="flow-step fs-navy" style="opacity:0.4; min-width:90px"></div>
      <div class="flow-arrow" style="opacity:0">→</div>
      <div class="flow-step fs-navy" style="opacity:0.4; min-width:90px"></div>
      <div class="flow-arrow" style="opacity:0">→</div>
      <div class="flow-step fs-navy" style="opacity:0.4; min-width:90px"></div>
      <div class="flow-arrow">↓ si hésitation</div>
      <div class="flow-step fs-purple"><span class="icon">🎬</span>Envoyer VSL</div>
      <div class="flow-arrow">→</div>
      <div class="flow-step fs-warn"><span class="icon">📞</span>Appel / Starter</div>
    </div>
  </div>

  <!-- TYPES D'ENTRÉE -->
  <div class="sdiv">Types de messages entrants</div>

  <div class="entry-grid">
    <div class="entry-card">
      <div class="entry-icon">🤩</div>
      <div>
        <div class="entry-tag et-1">Type A</div>
        <div class="entry-title">Curiosité directe</div>
        <div class="entry-examples">"Comment tu fais ça ?"<br>"C'est vrai que tu gagnes autant ?"<br>"T'as une formation ?"</div>
      </div>
    </div>
    <div class="entry-card">
      <div class="entry-icon">🙋</div>
      <div>
        <div class="entry-tag et-2">Type B</div>
        <div class="entry-title">Intérêt explicite</div>
        <div class="entry-examples">"Je suis intéressé par ta formation"<br>"Je veux me lancer"<br>"C'est quoi les tarifs ?"</div>
      </div>
    </div>
    <div class="entry-card">
      <div class="entry-icon">😤</div>
      <div>
        <div class="entry-tag et-3">Type C</div>
        <div class="entry-title">Douleur exprimée</div>
        <div class="entry-examples">"J'ai besoin de gagner de l'argent"<br>"J'ai pas de job"<br>"J'arrive pas à finir le mois"</div>
      </div>
    </div>
    <div class="entry-card">
      <div class="entry-icon">🤔</div>
      <div>
        <div class="entry-tag et-4">Type D</div>
        <div class="entry-title">Scepticisme</div>
        <div class="entry-examples">"C'est pas une arnaque ?"<br>"Tout le monde dit ça"<br>"C'est réaliste vraiment ?"</div>
      </div>
    </div>
  </div>

  <!-- ══════════════════════════
       ÉTAPE 1 — ACCROCHE
  ══════════════════════════ -->
  <div class="sdiv">Étape 1 — Réponse d'accroche selon le type de message</div>

  <!-- TYPE A -->
  <div class="conv-block">
    <div class="conv-header">
      <div class="conv-step-num csn-blue">A</div>
      <div>
        <div class="conv-title">Type A — Curiosité directe</div>
        <div class="conv-sub">Il pose une question sur ce que tu fais</div>
      </div>
      <div class="conv-tag ct-obj">Objectif : ouvrir</div>
    </div>
    <div class="conv-body">
      <div class="msg-row">
        <div class="msg-label ml-prospect">👤 Prospect</div>
        <div class="bubble bubble-prospect">"Comment tu fais pour gagner de l'argent comme ça ?"</div>
      </div>
      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Haha bonne question 😄 En gros je répare des téléphones en déplacement — je vais chez les clients directement. Zéro local, zéro patron.<br><br>T'es dans quelle situation toi ? T'as un job, t'es étudiant ?"</div>
      </div>
      <div class="warn-note"><strong>⚠️ Règle n°1 :</strong> Ne jamais envoyer le lien ou le prix en premier message. D'abord ouvrir la conversation. Toujours finir par une question.</div>
    </div>
  </div>

  <!-- TYPE B -->
  <div class="conv-block">
    <div class="conv-header">
      <div class="conv-step-num csn-green">B</div>
      <div>
        <div class="conv-title">Type B — Intérêt explicite</div>
        <div class="conv-sub">Il dit qu'il est intéressé ou demande les tarifs</div>
      </div>
      <div class="conv-tag ct-obj">Objectif : qualifier vite</div>
    </div>
    <div class="conv-body">
      <div class="msg-row">
        <div class="msg-label ml-prospect">👤 Prospect</div>
        <div class="bubble bubble-prospect">"Je suis intéressé par ta formation, c'est quoi les tarifs ?"</div>
      </div>
      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Cool que tu te manifestes 🙌<br><br>Avant de te donner les infos, j'ai besoin de comprendre ta situation pour voir si c'est vraiment fait pour toi.<br><br>T'es dans quelle situation là — t'as un job, t'es étudiant ?"</div>
      </div>
      <div class="note"><strong>💡 Ne pas donner le prix direct.</strong> Même si il le demande. Qualifier d'abord — ça augmente la valeur perçue et évite les "c'est trop cher" à froid.</div>
    </div>
  </div>

  <!-- TYPE C -->
  <div class="conv-block">
    <div class="conv-header">
      <div class="conv-step-num csn-warn">C</div>
      <div>
        <div class="conv-title">Type C — Douleur exprimée</div>
        <div class="conv-sub">Il exprime un problème financier ou une frustration</div>
      </div>
      <div class="conv-tag ct-obj">Objectif : créer l'espoir</div>
    </div>
    <div class="conv-body">
      <div class="msg-row">
        <div class="msg-label ml-prospect">👤 Prospect</div>
        <div class="bubble bubble-prospect">"Franchement j'ai besoin de trouver quelque chose, j'arrive plus à finir le mois"</div>
      </div>
      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Je comprends, j'ai été dans cette situation aussi.<br><br>Ce que je fais m'a changé la vie — je répare des téléphones en déplacement et je gagne bien ma vie sans patron et sans horaires fixes.<br><br>Tu veux qu'on en parle ? T'as quel âge et t'es dans quelle situation ?"</div>
      </div>
      <div class="success-note"><strong>✅ Empathie d'abord</strong>, proposition ensuite. Ne pas sauter directement sur la formation. Il doit sentir que tu le comprends avant de lui proposer quoi que ce soit.</div>
    </div>
  </div>

  <!-- TYPE D -->
  <div class="conv-block">
    <div class="conv-header">
      <div class="conv-step-num csn-red">D</div>
      <div>
        <div class="conv-title">Type D — Scepticisme</div>
        <div class="conv-sub">Il remet en question ou pense que c'est une arnaque</div>
      </div>
      <div class="conv-tag ct-obj">Objectif : désarmer</div>
    </div>
    <div class="conv-body">
      <div class="msg-row">
        <div class="msg-label ml-prospect">👤 Prospect</div>
        <div class="bubble bubble-prospect">"C'est pas une arnaque ça ? Tout le monde dit qu'il gagne de l'argent sur internet"</div>
      </div>
      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Haha je comprends la méfiance, c'est sain 😄<br><br>Moi je vends pas du rêve — je répare des téléphones physiquement, chez les clients, en Île-de-France. C'est un vrai métier qui existe depuis des années.<br><br>La différence c'est que j'ai trouvé comment le faire sans local et sans formation de 2 ans.<br><br>T'as déjà réparé des téléphones ou t'es partis de zéro ?"</div>
      </div>
      <div class="note"><strong>💡 Ne pas défendre.</strong> Valider la méfiance, puis ancrer dans le concret (physique, réel, IDF). Finir par une question qui l'amène à parler de lui.</div>
    </div>
  </div>

  <!-- ══════════════════════════
       ÉTAPE 2 — QUALIFICATION
  ══════════════════════════ -->
  <div class="sdiv">Étape 2 — Qualification · 3 questions max</div>

  <div class="conv-block">
    <div class="conv-header">
      <div class="conv-step-num csn-blue">2</div>
      <div>
        <div class="conv-title">Séquence de qualification</div>
        <div class="conv-sub">Toujours dans cet ordre — 1 question à la fois, jamais les 3 d'un coup</div>
      </div>
      <div class="conv-tag ct-obj">Qualifier</div>
    </div>
    <div class="conv-body">

      <div class="msg-row">
        <div class="msg-label ml-us">💬 Question 1 — Situation</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"T'es dans quelle situation là ? T'as un job, t'es étudiant, ou t'as pas d'activité en ce moment ?"</div>
      </div>
      <div class="note"><strong>→ Écoute la réponse.</strong> Cette réponse te dit son niveau d'urgence et son disponibilité.</div>

      <div class="msg-row">
        <div class="msg-label ml-us">💬 Question 2 — Motivation</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Et c'est quoi ton objectif avec ça — juste un complément ou tu veux vraiment en faire quelque chose de sérieux ?"</div>
      </div>
      <div class="note"><strong>→ Écoute.</strong> Si il dit "complément" → Starter possible. Si il dit "sérieux" → viser la Pro directement.</div>

      <div class="msg-row">
        <div class="msg-label ml-us">💬 Question 3 — Budget</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Dernière question — si c'est vraiment fait pour toi, t'as un budget pour te former ? Genre t'es dans la capacité d'investir quelques centaines d'euros pour apprendre un truc qui peut te rapporter beaucoup plus ?"</div>
      </div>
      <div class="warn-note"><strong>⚠️ La question budget</strong> — la poser de cette façon (investissement → retour) et non pas "t'as de l'argent". Ça cadre le prix comme un investissement avant même qu'on l'annonce.</div>

    </div>
  </div>

  <!-- LECTURE DES RÉPONSES -->
  <div class="routes">
    <div class="route-card rc-green">
      <div class="rc-title">✅ Prospect qualifié</div>
      <div class="rc-body">
        Répond oui au budget · Objectif sérieux · Disponible<br><br>
        → <strong>Passer directement au close</strong>
      </div>
    </div>
    <div class="route-card rc-blue">
      <div class="rc-title">🤔 Hésitant / Curieux</div>
      <div class="rc-body">
        Intéressé mais pas sûr · Besoin de voir plus<br><br>
        → <strong>Envoyer la VSL + suivre</strong>
      </div>
    </div>
    <div class="route-card rc-warn">
      <div class="rc-title">⚡ Pas de budget Pro</div>
      <div class="rc-body">
        Budget limité · Objectif complément · Étudiant<br><br>
        → <strong>Proposer Starter 97€</strong>
      </div>
    </div>
  </div>

  <!-- ══════════════════════════
       ÉTAPE 3 — CLOSE EN DM
  ══════════════════════════ -->
  <div class="sdiv">Étape 3 — Tentative de close directe en DM</div>

  <div class="conv-block">
    <div class="conv-header">
      <div class="conv-step-num csn-green">3</div>
      <div>
        <div class="conv-title">Le pitch + annonce du prix en DM</div>
        <div class="conv-sub">Pour les prospects qualifiés uniquement — budget confirmé</div>
      </div>
      <div class="conv-tag ct-close">Close</div>
    </div>
    <div class="conv-body">

      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi — Pitch condensé</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Ok parfait, t'as exactement le profil pour que ça marche.<br><br>Voilà ce que j'ai créé : une <strong>formation complète</strong> pour apprendre à réparer des téléphones en déplacement et trouver tes premiers clients dès la semaine 1.<br><br>Dedans t'as :<br>→ Les vidéos terrain filmées en POV<br>→ Mes fournisseurs directs aux prix pros<br>→ Comment trouver tes clients (Leboncoin, Facebook, quartier)<br>→ Des lives hebdo avec moi en direct<br>→ Un groupe privé<br>→ Et accès à mon réseau de clients en sous-traitance<br><br>Et je te garantis <strong>500€ en 90 jours</strong> — sinon je te rembourse entièrement."</div>
      </div>

      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi — Annonce du prix</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"C'est <strong>397€</strong> en une fois, ou <strong>3 × 133€</strong> si tu préfères étaler.<br><br>En 8 réparations t'as tout rentabilisé.<br><br>T'en penses quoi ?"</div>
      </div>

      <div class="warn-note"><strong>⚠️ Après "T'en penses quoi ?" — NE RIEN AJOUTER.</strong> Attendre la réponse. La tentation de meubler le silence est forte. Résiste. Celui qui parle en premier après le prix perd.</div>

    </div>
  </div>

  <!-- ══════════════════════════
       ÉTAPE 4 — OBJECTIONS
  ══════════════════════════ -->
  <div class="sdiv">Étape 4 — Traitement des objections</div>

  <div class="obj-grid">

    <!-- OBJECTION 1 -->
    <div class="obj-item">
      <div class="obj-item-head">
        <div class="obj-icon">💸</div>
        <div class="obj-title">"C'est trop cher" / "J'ai pas les moyens"</div>
      </div>
      <div class="obj-body">
        <div class="obj-col">
          <div class="obj-col-label">❌ À ne pas dire</div>
          <div class="bubble bubble-prospect" style="font-size:12px">"Je peux faire un geste sur le prix"<br><br>"C'est pas si cher quand même"</div>
        </div>
        <div class="obj-col">
          <div class="obj-col-label">✅ Script</div>
          <div class="bubble bubble-us" style="font-size:12.5px; align-self:flex-start; border-radius:10px">"Par rapport à quoi ?<br><br>Un iPhone cassé ça vaut 100-200€ de réparation en boutique. Toi t'en prends 50 de bénéf. En 8 réparations t'as tout rentabilisé.<br><br>La vraie question c'est : est-ce que t'as envie de continuer sans revenus ou t'as envie d'investir dans quelque chose qui marche ?"</div>
        </div>
      </div>
    </div>

    <!-- OBJECTION 2 -->
    <div class="obj-item">
      <div class="obj-item-head">
        <div class="obj-icon">🤔</div>
        <div class="obj-title">"J'ai besoin de réfléchir"</div>
      </div>
      <div class="obj-body">
        <div class="obj-col">
          <div class="obj-col-label">❌ À ne pas dire</div>
          <div class="bubble bubble-prospect" style="font-size:12px">"Prends ton temps, pas de pression !"<br><br>"Reviens quand tu veux"</div>
        </div>
        <div class="obj-col">
          <div class="obj-col-label">✅ Script</div>
          <div class="bubble bubble-us" style="font-size:12.5px; align-self:flex-start; border-radius:10px">"Je comprends. Mais dis-moi — c'est quoi le truc qui te bloque vraiment ?<br><br>Parce que 'réfléchir' c'est souvent une question précise qu'on a pas encore posée. C'est le prix ? Le fait que ça marche vraiment ? Autre chose ?"</div>
        </div>
      </div>
    </div>

    <!-- OBJECTION 3 -->
    <div class="obj-item">
      <div class="obj-item-head">
        <div class="obj-icon">😰</div>
        <div class="obj-title">"J'ai peur de pas y arriver / c'est compliqué"</div>
      </div>
      <div class="obj-body">
        <div class="obj-col">
          <div class="obj-col-label">❌ À ne pas dire</div>
          <div class="bubble bubble-prospect" style="font-size:12px">"T'inquiète c'est facile !"<br><br>"N'importe qui peut le faire"</div>
        </div>
        <div class="obj-col">
          <div class="obj-col-label">✅ Script</div>
          <div class="bubble bubble-us" style="font-size:12.5px; align-self:flex-start; border-radius:10px">"C'est normal d'avoir cette peur. Mes élèves l'avaient tous au départ.<br><br>C'est pour ça que la formation existe — tu fais pas ça seul. Les vidéos montrent exactement les gestes. Et les lives hebdo sont là pour tes questions.<br><br>Et si t'as tout fait et que ça marche pas — je te rembourse. Y'a aucun risque."</div>
        </div>
      </div>
    </div>

    <!-- OBJECTION 4 -->
    <div class="obj-item">
      <div class="obj-item-head">
        <div class="obj-icon">⏰</div>
        <div class="obj-title">"J'ai pas le temps"</div>
      </div>
      <div class="obj-body">
        <div class="obj-col">
          <div class="obj-col-label">❌ À ne pas dire</div>
          <div class="bubble bubble-prospect" style="font-size:12px">"C'est pas long !"<br><br>"Tu gères ça facilement"</div>
        </div>
        <div class="obj-col">
          <div class="obj-col-label">✅ Script</div>
          <div class="bubble bubble-us" style="font-size:12.5px; align-self:flex-start; border-radius:10px">"Combien d'heures par semaine t'as de libre ?<br><br>Parce que mes élèves qui démarrent font ça le week-end. 2-3 réparations le samedi c'est déjà 100-150€.<br><br>Si t'as 4-5 heures par semaine, ça marche."</div>
        </div>
      </div>
    </div>

    <!-- OBJECTION 5 -->
    <div class="obj-item">
      <div class="obj-item-head">
        <div class="obj-icon">🛠️</div>
        <div class="obj-title">"J'ai jamais touché à un téléphone"</div>
      </div>
      <div class="obj-body">
        <div class="obj-col">
          <div class="obj-col-label">❌ À ne pas dire</div>
          <div class="bubble bubble-prospect" style="font-size:12px">"C'est pas grave"<br><br>"C'est simple tu vas voir"</div>
        </div>
        <div class="obj-col">
          <div class="obj-col-label">✅ Script</div>
          <div class="bubble bubble-us" style="font-size:12.5px; align-self:flex-start; border-radius:10px">"Tous mes élèves étaient partis de zéro. C'est même mieux parce que t'as pas de mauvaises habitudes à corriger.<br><br>Les vidéos sont filmées en POV — tu vois exactement ce que je fais, comme si t'étais avec moi. Et t'as les lives pour poser tes questions en direct."</div>
        </div>
      </div>
    </div>

    <!-- OBJECTION 6 -->
    <div class="obj-item">
      <div class="obj-item-head">
        <div class="obj-icon">🤷</div>
        <div class="obj-title">"Comment je trouve des clients ?"</div>
      </div>
      <div class="obj-body">
        <div class="obj-col">
          <div class="obj-col-label">❌ À ne pas dire</div>
          <div class="bubble bubble-prospect" style="font-size:12px">Donner toute la méthode gratuitement en DM</div>
        </div>
        <div class="obj-col">
          <div class="obj-col-label">✅ Script</div>
          <div class="bubble bubble-us" style="font-size:12.5px; align-self:flex-start; border-radius:10px">"C'est une des choses les plus importantes que j'enseigne dans la formation — Leboncoin, Facebook Marketplace, ton quartier, et surtout mon réseau de clients en sous-traitance.<br><br>Je t'explique tout ça en détail à l'intérieur. C'est pour ça que ça marche rapidement pour mes élèves."</div>
        </div>
      </div>
    </div>

  </div>

  <!-- ══════════════════════════
       ÉTAPE 5 — BACKUP VSL
  ══════════════════════════ -->
  <div class="sdiv">Étape 5 — Backup VSL · Si il a besoin de plus</div>

  <div class="conv-block">
    <div class="conv-header">
      <div class="conv-step-num csn-purple">5</div>
      <div>
        <div class="conv-title">Envoyer vers la VSL</div>
        <div class="conv-sub">Si après les objections il reste hésitant — besoin de voir pour croire</div>
      </div>
      <div class="conv-tag ct-fall">VSL Backup</div>
    </div>
    <div class="conv-body">

      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi — Transition vers la VSL</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Écoute, j'ai fait une vidéo qui explique tout en détail — le concept, comment ça marche, les résultats de mes élèves, et ce qui est inclus dans la formation.<br><br>Regarde ça — ça prend 10-12 minutes — et dis-moi ce que t'en penses après : <strong>[LIEN VSL]</strong> 👊"</div>
      </div>

      <div class="note"><strong>💡 Après avoir envoyé la VSL</strong> — ne pas demander "t'as regardé ?" immédiatement. Attendre au moins 2-3 heures avant de relancer.</div>

      <div class="msg-row" style="margin-top:4px">
        <div class="msg-label ml-us">💬 Toi — Relance après VSL (2-3h)</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"T'as eu le temps de regarder ? T'en as pensé quoi ?"</div>
      </div>

      <div class="msg-row">
        <div class="msg-label ml-prospect">👤 Il a regardé — intéressé</div>
        <div class="bubble bubble-prospect">"Ouais j'ai vu c'est pas mal"</div>
      </div>

      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Super ! Qu'est-ce qui t'a le plus parlé ?<br><br>Et là t'es prêt à te lancer ou il te reste des questions ?"</div>
      </div>

      <div class="warn-note"><strong>⚠️ S'il dit "c'est pas mal" sans s'emballer</strong> — ne pas relancer le pitch. Poser une question ouverte sur ce qui lui a plu. Laisser lui exprimer son intérêt avant de revenir sur le prix.</div>

    </div>
  </div>

  <!-- ══════════════════════════
       ÉTAPE 6 — DOWNSELL STARTER
  ══════════════════════════ -->
  <div class="sdiv">Étape 6 — Downsell Starter · Si budget insuffisant pour la Pro</div>

  <div class="conv-block">
    <div class="conv-header">
      <div class="conv-step-num csn-warn">6</div>
      <div>
        <div class="conv-title">Proposer la Starter 97€</div>
        <div class="conv-sub">Uniquement si il dit clairement qu'il ne peut pas se permettre la Pro</div>
      </div>
      <div class="conv-tag ct-obj2">Downsell</div>
    </div>
    <div class="conv-body">

      <div class="msg-row">
        <div class="msg-label ml-prospect">👤 Prospect</div>
        <div class="bubble bubble-prospect">"397€ c'est trop pour moi là, j'ai pas ça"</div>
      </div>

      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Je comprends. Écoute, j'ai aussi une option d'entrée à <strong>97€</strong> — c'est la formation vidéo complète pour apprendre les bases et faire tes premières réparations.<br><br>C'est moins complet que la Pro — pas de lives, pas de groupe privé, pas de sous-traitance — mais c'est suffisant pour démarrer et faire tes premiers euros.<br><br>Ça te permettrait de te lancer et d'avoir les fonds pour rejoindre la Pro après si tu veux aller plus loin.<br><br>Ça t'intéresse ?"</div>
      </div>

      <div class="warn-note"><strong>⚠️ Ne proposer la Starter qu'après un vrai refus sur le prix</strong> — pas en première intention. Sinon tu dévalues la Pro et tu perds des ventes à 397€.</div>

    </div>
  </div>

  <!-- ══════════════════════════
       CLOSE FINAL
  ══════════════════════════ -->
  <div class="sdiv">Close final — Envoyer le lien de paiement</div>

  <div class="conv-block">
    <div class="conv-header">
      <div class="conv-step-num csn-green">✅</div>
      <div>
        <div class="conv-title">Il dit oui — Envoyer le lien immédiatement</div>
        <div class="conv-sub">Ne jamais laisser refroidir un "oui" — envoyer le lien dans la foulée</div>
      </div>
      <div class="conv-tag ct-close">Vente</div>
    </div>
    <div class="conv-body">

      <div class="msg-row">
        <div class="msg-label ml-prospect">👤 Prospect</div>
        <div class="bubble bubble-prospect">"Ok je suis partant, je fais comment ?"</div>
      </div>

      <div class="msg-row">
        <div class="msg-label ml-us">💬 Toi</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Parfait ! Voilà le lien de paiement sécurisé : <strong>[LIEN STRIPE / SYSTEME.IO]</strong><br><br>Dès que c'est validé tu reçois un email avec l'accès à la formation. Si t'as la moindre question pendant ou après n'hésite pas 🙌"</div>
      </div>

      <div class="msg-row" style="margin-top:4px">
        <div class="msg-label ml-us">💬 Toi — Suivi 30 min après (si pas payé)</div>
        <div class="bubble bubble-us" style="align-self:flex-end">"Hé, t'as pu accéder au lien sans problème ?"</div>
      </div>

      <div class="note"><strong>💡 Si pas de réponse après 30 min</strong> — envoyer ce message simple. Pas de pression, juste vérifier si il y a eu un problème technique. Souvent ça suffit à relancer.</div>

    </div>
  </div>

  <!-- ══════════════════════════
       SÉQUENCE DE RELANCES
  ══════════════════════════ -->
  <div class="sdiv">Séquence de relances — Si il disparaît</div>

  <div class="relance-row">
    <div class="rel-day">J+1</div>
    <div class="rel-body">
      <div class="rel-ctx">Il a répondu mais s'est arrêté sans dire oui ou non</div>
      <div class="bubble bubble-us" style="align-self:flex-start; font-size:12.5px; border-radius:10px">"Hé, je voulais juste savoir où t'en es — t'as eu le temps de réfléchir ?"</div>
    </div>
  </div>

  <div class="relance-row">
    <div class="rel-day">J+3</div>
    <div class="rel-body">
      <div class="rel-ctx">Toujours pas de réponse — relance avec une preuve sociale</div>
      <div class="bubble bubble-us" style="align-self:flex-start; font-size:12.5px; border-radius:10px">"Je pensais à toi — un de mes élèves vient de me partager ses résultats du mois. [Insérer screenshot] C'est ce genre de résultats qui attend ceux qui se lancent 🔥<br><br>T'es toujours chaud ?"</div>
    </div>
  </div>

  <div class="relance-row">
    <div class="rel-day">J+7</div>
    <div class="rel-body">
      <div class="rel-ctx">Dernière relance — créer une urgence légère</div>
      <div class="bubble bubble-us" style="align-self:flex-start; font-size:12.5px; border-radius:10px">"Dernière fois que je te contacte là-dessus — j'ai des places limitées dans le groupe cette semaine.<br><br>Si t'es partant dis-moi, sinon pas de souci on reste en contact 👊"</div>
    </div>
  </div>

  <div class="relance-row">
    <div class="rel-day">J+14</div>
    <div class="rel-body">
      <div class="rel-ctx">Il a dit non ou rien — garder la relation pour plus tard</div>
      <div class="bubble bubble-us" style="align-self:flex-start; font-size:12.5px; border-radius:10px">"Pas de souci si c'est pas le bon moment. Je continue à poster mes réparations et mes résultats ici — si un jour tu veux te lancer, n'hésite pas à revenir vers moi 🙌"</div>
    </div>
  </div>

  <!-- RÈGLES D'OR -->
  <div class="sdiv">Les règles d'or du script DM</div>

  <div style="display:grid; grid-template-columns:1fr 1fr; gap:10px; margin-bottom:8px">

    <div class="note" style="border-color:rgba(52,199,123,0.3); background:rgba(52,199,123,0.04)">
      <strong style="color:var(--success)">✅ Toujours faire</strong><br><br>
      → Finir chaque message par une question<br>
      → Attendre la réponse avant d'envoyer le message suivant<br>
      → Qualifier avant d'annoncer le prix<br>
      → Envoyer le lien immédiatement après un oui<br>
      → Rester naturel — parler comme à un pote
    </div>

    <div class="note" style="border-color:rgba(239,68,68,0.3); background:rgba(239,68,68,0.04)">
      <strong style="color:var(--red)">❌ Ne jamais faire</strong><br><br>
      → Envoyer le prix en premier message<br>
      → Envoyer le lien VSL sans avoir qualifié<br>
      → Meubler le silence après le prix<br>
      → Relancer plus de 3 fois<br>
      → Donner toute la méthode gratos en DM
    </div>

  </div>

  <div class="warn-note" style="border-radius:10px; border:1.5px solid rgba(245,158,11,0.25)">
    <strong>⚠️ Règle finale :</strong> Un prospect qui ne répond pas n'est pas un prospect perdu. Il reçoit les posts, les stories, les résultats. La relation continue. Ne pas insister au-delà de 3 relances — revenir naturellement via le contenu organique.
  </div>

</div>
</body>
</html>
