---
title: "A tool for the detection of structural aesthetic defects of android mobile user interfaces"
collection: tools
type: "Research project"
permalink: /tools/ADDET
venue: "National School of Computer Science " 
location: "Tunis, Tunisia"
---
<article style="max-width:980px; margin:0 auto; font-family:Arial, Helvetica, sans-serif; color:#222; line-height:1.65;">

  <!-- Header -->
  <header style="margin:26px 0 18px 0;">
    <div style="font-size:13px; color:#555; letter-spacing:.3px; text-transform:uppercase;">
      Tool · Research Tool
    </div>

    <h1 style="font-size:32px; margin:6px 0 10px 0; line-height:1.2;">
      ADDET — Android UI Structural Aesthetic Defects Detection
    </h1>

    <div style="display:flex; flex-wrap:wrap; gap:10px; font-size:14px; color:#444;">
      <span><strong>Focus:</strong> Structural aesthetic quality of mobile user interfaces (MUIs)</span>
      <span>•</span>
      <span><strong>Method:</strong> Static analysis + optimization-based defect identification</span>
    </div>
  </header>

  <!-- Hero image -->
  <figure style="margin:18px 0 22px 0; padding:12px; border:1px solid #ddd; border-radius:14px;">
    <img src="../images/addet.png" alt="ADDET UI" style="width:100%; height:auto; display:block; border-radius:10px;">
    <figcaption style="font-size:13px; color:#555; margin-top:8px;">
      ADDET — tool support for assessing structural aesthetic properties and detecting UI defects in Android MUIs.
    </figcaption>
  </figure>

  <!-- Synopsis + Key points -->
  <section style="display:flex; flex-wrap:wrap; gap:18px; align-items:flex-start; margin-bottom:26px;">

    <!-- Synopsis -->
    <div style="flex:1 1 560px; padding:16px; border:1px solid #ddd; border-radius:14px;">
      <h2 style="font-size:18px; margin:0 0 10px 0; border-bottom:1px solid #eee; padding-bottom:8px;">
        Synopsis
      </h2>

      <p style="margin:10px 0 0 0; font-size:14px;">
        Android app user interfaces should be free from structural aesthetic defects. These defects often reflect
        poor design decisions that undermine consistency and reduce usability. To address this, we propose
        <strong>ADDET</strong>, a tool that determines the <strong>structural aesthetic dimension</strong> of mobile user interfaces (MUIs).
        Automating this evaluation supports designers by providing objective signals about design quality.
      </p>

      <p style="margin:10px 0 0 0; font-size:14px;">
        Our approach is organized into <strong>two modules</strong>, described below.
      </p>
    </div>

    <!-- Highlights -->
    <aside style="flex:1 1 280px; padding:16px; border:1px solid #ddd; border-radius:14px;">
      <h2 style="font-size:18px; margin:0 0 10px 0; border-bottom:1px solid #eee; padding-bottom:8px;">
        Highlights
      </h2>

      <div style="font-size:14px; padding:8px 0; border-bottom:1px solid #eee;">
        <strong>Analysis type:</strong> Static analysis of a tree-structured layout
      </div>
      <div style="font-size:14px; padding:8px 0; border-bottom:1px solid #eee;">
        <strong>Metrics used:</strong> 15 geometric (structural/aesthetic) metrics
      </div>
      <div style="font-size:14px; padding:8px 0;">
        <strong>Defect rules:</strong> Formulated as an optimization problem
      </div>
    </aside>

  </section>

  <!-- Modules -->
  <section style="margin:0 0 26px 0;">
    <h2 style="font-size:20px; margin:0 0 14px 0; border-bottom:2px solid #000; padding-bottom:6px;">
      Approach overview
    </h2>

    <div style="display:grid; grid-template-columns:1fr; gap:14px;">

      <!-- Module 1 -->
      <div style="border:1px solid #ddd; border-radius:14px; padding:14px;">
        <div style="font-weight:700; margin-bottom:6px;">Module 1 — Metrics assessment</div>
        <div style="font-size:14px; color:#222;">
          Based on static analysis of a tree-structured layout of the MUI. We compute
          <strong>15 geometric metrics</strong> (structural/aesthetic metrics) to assess structural properties
          and identify conditions under which a defect should be triggered.
        </div>
      </div>

      <!-- Module 2 -->
      <div style="border:1px solid #ddd; border-radius:14px; padding:14px;">
        <div style="font-weight:700; margin-bottom:6px;">Module 2 — Defects detection</div>
        <div style="font-size:14px; color:#222;">
          Manually combining metrics and defects is time-consuming and user-dependent when defining detection rules.
          We therefore model defect identification as an <strong>optimization problem</strong>, enabling systematic discovery
          of effective detection rules.
        </div>
      </div>

    </div>
  </section>

  <!-- Call to action -->
  <section style="margin:0 0 30px 0; padding:16px; border:1px solid #ddd; border-radius:14px;">
    <h2 style="font-size:18px; margin:0 0 10px 0;">Download</h2>

    <div style="font-size:14px;">
      <strong>ADDET parser:</strong>
      <a href="https://github.com/NarjessBessghaier/Defects_Detection_Tool" target="_blank" rel="noopener noreferrer"
         style="color:#0b57d0; text-decoration:none;">
        Defects_Detection_Tool (GitHub)
      </a>
      <div style="margin-top:6px; color:#444;">
        Download the parser and start evaluating your Android apps’ user interfaces.
      </div>
    </div>
  </section>

</article>
