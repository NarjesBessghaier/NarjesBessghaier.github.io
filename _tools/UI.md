---
title: "Mobile apps UI defects detection and restructuring Framework"
collection: tools
type: "Research project"
permalink: /tools/UI
venue: "National School of Computer Science " 
location: "Tunis, Tunisia"
---

<!-- Page content (keep your YAML front-matter in the file above this section) -->

<article style="max-width:980px; margin:0 auto; font-family:Arial, Helvetica, sans-serif; color:#222; line-height:1.65;">

  <!-- Header -->
  <header style="margin:26px 0 18px 0;">
    <div style="font-size:13px; color:#555; letter-spacing:.3px; text-transform:uppercase;">
      Tool · Research Project
    </div>

    <h1 style="font-size:32px; margin:6px 0 10px 0; line-height:1.2;">
      Mobile Apps UI Defects Detection and Restructuring Framework
    </h1>

    <div style="display:flex; flex-wrap:wrap; gap:10px; font-size:14px; color:#444;">
      <span><strong>Venue:</strong> National School of Computer Science</span>
      <span>•</span>
      <span><strong>Location:</strong> Tunis, Tunisia</span>
    </div>
  </header>

  <!-- Hero image -->
  <figure style="margin:18px 0 22px 0; padding:12px; border:1px solid #ddd; border-radius:14px;">
    <img src="../images/framework.png" alt="UI framework overview" style="width:100%; height:auto; display:block; border-radius:10px;">
    <figcaption style="font-size:13px; color:#555; margin-top:8px;">
      Framework overview — detection of UI structural defects and automated restructuring recommendations.
    </figcaption>
  </figure>

  <!-- Synopsis + Highlights -->
  <section style="display:flex; flex-wrap:wrap; gap:18px; align-items:flex-start; margin-bottom:26px;">

    <!-- Synopsis -->
    <div style="flex:1 1 520px; padding:16px; border:1px solid #ddd; border-radius:14px;">
      <h2 style="font-size:18px; margin:0 0 10px 0; border-bottom:1px solid #eee; padding-bottom:8px;">
        Synopsis
      </h2>

      <p style="margin:10px 0 0 0; font-size:14px; color:#222;">
        We present an automated approach for restructuring a user interface (UI) structural design based on its data model.
        The framework checks violations of 13 generic structural design standards inspired by Google Material Design and
        then generates recommendations for each violated guideline based on the evaluated UI specifications.
      </p>

      <p style="margin:10px 0 0 0; font-size:14px; color:#222;">
        As a proof of concept, we used ADDET to evaluate the quality of the original and restructured versions of
        511 user interfaces, considering both the number of aesthetic defects and aesthetic properties. Results show a
        significant positive difference (mean improvement: <strong>0.59</strong>) in favor of restructured interfaces, with improvements across
        <strong>7 quality metrics</strong>. We also observed potential accessibility gains through larger element sizes in some designs.
      </p>
    </div>

    <!-- Key facts -->
    <aside style="flex:1 1 260px; padding:16px; border:1px solid #ddd; border-radius:14px;">
      <h2 style="font-size:18px; margin:0 0 10px 0; border-bottom:1px solid #eee; padding-bottom:8px;">
        Key facts
      </h2>

      <div style="font-size:14px; padding:8px 0; border-bottom:1px solid #eee;">
        <strong>Standards checked:</strong> 13 structural guidelines
      </div>
      <div style="font-size:14px; padding:8px 0; border-bottom:1px solid #eee;">
        <strong>Dataset:</strong> 511 user interfaces
      </div>
      <div style="font-size:14px; padding:8px 0; border-bottom:1px solid #eee;">
        <strong>Mean improvement:</strong> 0.59 (restructured vs. original)
      </div>
      <div style="font-size:14px; padding:8px 0;">
        <strong>Improved metrics:</strong> 7 quality metrics
      </div>
    </aside>

  </section>

  <!-- Secondary figure -->
  <figure style="margin:0 0 26px 0; padding:12px; border:1px solid #ddd; border-radius:14px;">
    <img src="../images/frame1.png" alt="Framework pipeline illustration" style="width:100%; height:auto; display:block; border-radius:10px;">
    <figcaption style="font-size:13px; color:#555; margin-top:8px;">
      Framework pipeline — from guideline violation detection to restructuring recommendations.
    </figcaption>
  </figure>

  <!-- Media & Links -->
  <section style="margin:0 0 30px 0; padding:16px; border:1px solid #ddd; border-radius:14px;">
    <h2 style="font-size:18px; margin:0 0 10px 0;">Media &amp; resources</h2>

    <div style="font-size:14px; margin-bottom:10px;">
      <strong>Video snippet:</strong>
      <a href="https://www.youtube.com/watch?v=Se3ZCDsPXEU" target="_blank" rel="noopener noreferrer"
         style="color:#0b57d0; text-decoration:none;">
        Framework (YouTube)
      </a>
    </div>

    <div style="font-size:14px;">
      <strong>Source code / download:</strong>
      <a href="https://github.com/NarjessBessghaier/UI-Restructuring" target="_blank" rel="noopener noreferrer"
         style="color:#0b57d0; text-decoration:none;">
        UI-Restructuring (GitHub)
      </a>
      <div style="margin-top:6px; color:#444;">
        Download the framework and start restructuring your Android apps’ user interfaces.
      </div>
    </div>
  </section>

</article>
