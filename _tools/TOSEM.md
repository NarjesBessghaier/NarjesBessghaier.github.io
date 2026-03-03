---
title: "ConfigRF — ML-Based Identification and Classification of Configuration Files"
collection: tools
type: "Research project"
permalink: /tools/TOSEM
venue: "ACM Transactions on Software Engineering and Methodology (TOSEM)"
year: "2023"
location: "ÉTS, University of Quebec, Canada"
---
<article style="max-width:980px; margin:0 auto; font-family:Arial, Helvetica, sans-serif; color:#222; line-height:1.65;">

  <!-- Header -->
  <header style="margin:26px 0 18px 0;">
    <div style="font-size:13px; color:#555; letter-spacing:.3px; text-transform:uppercase;">
      Tool · Research Tool
    </div>

    <div style="display:flex; flex-wrap:wrap; gap:10px; font-size:14px; color:#444;">
      <span><strong>Focus:</strong> Identification and classification of deployment & runtime configuration files</span>
      <span>•</span>
      <span><strong>Method:</strong> TF-IDF + Random Forest (Binary & Multi-class classification)</span>
    </div>
  </header>

  <!-- Hero image -->
  <figure style="margin:18px 0 22px 0; padding:12px; border:1px solid #ddd; border-radius:14px;">
    <img src="/images/tosem23.jpg" alt="Configuration RF Model" style="width:100%; height:auto; display:block; border-radius:10px;">
    <figcaption style="font-size:13px; color:#555; margin-top:8px;">
      ConfigRF — Automatic identification and classification of configuration files composing a configuration system.
    </figcaption>
  </figure>

  <!-- Synopsis -->
  <section style="margin-bottom:26px; padding:16px; border:1px solid #ddd; border-radius:14px;">
    <h2 style="font-size:18px; margin:0 0 10px 0; border-bottom:1px solid #eee; padding-bottom:8px;">
      Synopsis
    </h2>

    <p style="font-size:14px; margin:0;">
      Modern software systems rely on complex <strong>configuration systems</strong> composed of
      multiple interconnected configuration files used during deployment and runtime.
      However, configuration files do not follow a strict standard and often share
      formats and extensions with regular source code files.
    </p>

    <p style=" margin-top:10px;">
    <div style="font-size:14px;">
      To address this challenge, we propose <strong>ConfigRF</strong>, a machine learning–based
      approach that:
      <ul>
        <li>Automatically distinguishes configuration files from non-configuration files</li>
        <li>Classifies configuration files into nine empirically derived configuration types</li>
      </ul>
      The model was validated on 635 OpenStack projects.
      </div>
    </p>
  </section>

  <!-- Methodology -->
  <section style="margin:0 0 26px 0;">
    <h2 style="font-size:20px; margin:0 0 14px 0; border-bottom:2px solid #000; padding-bottom:6px;">
      Methodology
    </h2>

    <div style="display:grid; gap:14px;">

      <!-- Step 1 -->
      <div style="border:1px solid #ddd; border-radius:14px; padding:14px;">
        <div style="font-weight:700; margin-bottom:6px;">1 — Empirical Ground Truth Construction</div>
        <div style="font-size:14px;">
          A corpus of <strong>1,756 manually analyzed configuration files</strong> was built using
          a mixed card sorting technique, identifying nine configuration categories.
          An additional 1,756 non-configuration files were curated to form a balanced dataset.
        </div>
      </div>

      <!-- Step 2 -->
      <div style="border:1px solid #ddd; border-radius:14px; padding:14px;">
        <div style="font-weight:700; margin-bottom:6px;">2 — Text Representation (TF-IDF)</div>
        <div style="font-size:14px;">
          Each file is transformed into a numerical vector using
          <strong>Term Frequency–Inverse Document Frequency (TF-IDF)</strong>.
          TF-IDF assigns weights to terms based on their discriminative power across files,
          enabling the model to automatically learn configuration-related patterns.
        </div>
      </div>

      <!-- Step 3 -->
      <div style="border:1px solid #ddd; border-radius:14px; padding:14px;">
        <div style="font-weight:700; margin-bottom:6px;">3 — Feature Selection & Reduction</div>
        <div style="font-size:14px;">
          To improve robustness and avoid overfitting:
          <ul>
            <li>Pearson’s Chi-square test is used for feature relevance selection</li>
            <li>Correlation analysis removes highly collinear features</li>
            <li>Redundancy analysis further reduces feature overlap</li>
          </ul>
        </div>
      </div>

      <!-- Step 4 -->
      <div style="border:1px solid #ddd; border-radius:14px; padding:14px;">
        <div style="font-weight:700; margin-bottom:6px;">4 — Random Forest Classification</div>
        <div style="font-size:14px;">
          A <strong>Random Forest (RF)</strong> classifier is trained using stratified
          bootstrapping (100 bootstrap runs) to ensure statistical robustness.
          Two tasks are performed:
          <ul>
            <li><strong>Binary classification:</strong> Configuration vs. Non-configuration</li>
            <li><strong>Multi-class classification:</strong> Classification into nine configuration types</li>
          </ul>
        </div>
      </div>

    </div>
  </section>

  <!-- Performance -->
  <section style="margin-bottom:26px;">
    <h2 style="font-size:18px; margin:0 0 10px 0; border-bottom:1px solid #eee; padding-bottom:8px;">
      Empirical Performance
    </h2>

    <div style="font-size:14px; line-height:1.7;">
      <strong>Binary Classification (Configuration vs Non-Configuration)</strong><br>
      • Median AUC: <strong>0.91</strong><br>
      • Median Brier Score: 0.12<br>
      • Median Precision: 0.86<br>
      • Median Recall: 0.83<br><br>

      <strong>Multi-Class Classification (Nine Configuration Types)</strong><br>
      • Median Weighted AUC: <strong>0.92</strong><br>
      • Median Brier Score: 0.04<br>
      • Median Weighted Precision: 0.84<br>
      • Median Weighted Recall: 0.82<br><br>

      Remarkably, labeling as few as <strong>100 files</strong> is sufficient to train a model
      achieving strong predictive performance.
    </div>
  </section>

  <!-- Characteristics -->
  <section style="margin-bottom:26px;">
    <h2 style="font-size:18px; margin:0 0 10px 0; border-bottom:1px solid #eee; padding-bottom:8px;">
      Key Characteristics
    </h2>

    <div style="font-size:14px; line-height:1.7;">
      <ul>
        <li>Handles heterogeneous file formats (.py, .yaml, .sh, .ini, .conf, etc.)</li>
        <li>Extension-agnostic (does not rely solely on file extensions)</li>
        <li>Robust to mixed configuration/source-code repositories</li>
        <li>Statistically validated via bootstrapping</li>
        <li>Supports research on full configuration systems rather than isolated files</li>
      </ul>
    </div>
  </section>

  <!-- Research Reference -->
  <section style="margin-bottom:26px; padding:16px; border:1px solid #ddd; border-radius:14px;">
    <h2 style="font-size:18px; margin:0 0 10px 0;">Research Reference</h2>
    <div style="font-size:14px;">
      Bessghaier, N., Sayagh, M., Ouni, A., & Mkaouer, M. W. (2023).<br>
      <em>What Constitutes the Deployment and Runtime Configuration System? An Empirical Study on OpenStack Projects.</em><br>
      ACM Transactions on Software Engineering and Methodology (TOSEM).<br><br>
      DOI: https://doi.org/10.1145/3607186
    </div>
  </section>

  <!-- Download -->
   
  <section style="padding:16px; border:1px solid #ddd; border-radius:14px;">
    <h2 style="font-size:18px; margin:0 0 10px 0;">Download</h2>

    <div style="font-size:14px;">
      <strong>Source code:</strong>
      <a href="https://github.com/stilab-ets/CongIdentification" target="_blank" rel="noopener noreferrer"
         style="color:#0b57d0; text-decoration:none;">
        https://github.com/stilab-ets/CongIdentification
      </a>
      <div style="margin-top:6px; color:#444;">
        Repository includes Labeled datasets, experimental scripts, and Trained models.
      </div>
    </div>
  </section>
    
     

</article>



