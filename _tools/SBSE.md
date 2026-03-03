---
title: "GA— Genetic Algorithm-Based Co-Change Recommendation for Infrastructure-as-Code"
collection: tools
type: "Research project"
permalink: /tools/SSBSE
venue: "Journal of Systems and Software (JSS)"
year: "2025"
location: "ETS, University of Quebec, Canada"
---

<article style="max-width:980px; margin:0 auto; font-family:Arial, Helvetica, sans-serif; color:#222; line-height:1.65;">

  <!-- Header -->
  <header style="margin:26px 0 18px 0;">
    <div style="font-size:13px; color:#555; letter-spacing:.3px; text-transform:uppercase;">
      Tool · Research Tool
    </div>

    <div style="display:flex; flex-wrap:wrap; gap:10px; font-size:14px; color:#444;">
      <span><strong>Focus:</strong> Infrastructure-as-Code (IaC) file co-change recommendation</span>
      <span>•</span>
      <span><strong>Method:</strong> Mono-objective Genetic Algorithm with hybrid heuristics</span>
    </div>
  </header>

  <!-- Hero image -->
  <figure style="margin:18px 0 22px 0; padding:12px; border:1px solid #ddd; border-radius:14px;">
    <img src="/images/sbse25.jpg" alt="GA IaC Tool" style="width:100%; height:auto; display:block; border-radius:10px;">
    <figcaption style="font-size:13px; color:#555; margin-top:8px;">
      GA-IaCRec — Optimization-based recommendation of files likely to co-change with a given IaC file.
    </figcaption>
  </figure>

  <!-- Synopsis -->
  <section style="margin-bottom:26px; padding:16px; border:1px solid #ddd; border-radius:14px;">
    <h2 style="font-size:18px; margin:0 0 10px 0; border-bottom:1px solid #eee; padding-bottom:8px;">
      Synopsis
    </h2>

    <p style="font-size:14px; margin:0;">
      Infrastructure-as-Code (IaC) files evolve together with configuration scripts, templates, and dependent
      artifacts. As repositories grow in size and coupling, developers face difficulty identifying which files
      should be modified together.
    </p>

    <p style="font-size:14px; margin-top:10px;">
      <strong>GA-IaCRec</strong> is an automated recommendation tool that predicts files likely to co-change
      with a given IaC file. The tool formulates the recommendation problem as an
      <strong>optimization task</strong> and uses a <strong>mono-objective Genetic Algorithm (GA)</strong>
      to generate a ranked list of candidate files.
    </p>
  </section>

  <!-- Methodology -->
  <section style="margin:0 0 26px 0;">
    <h2 style="font-size:20px; margin:0 0 14px 0; border-bottom:2px solid #000; padding-bottom:6px;">
      Methodology
    </h2>

    <div style="display:grid; gap:14px;">

      <div style="border:1px solid #ddd; border-radius:14px; padding:14px;">
        <div style="font-weight:700; margin-bottom:6px;">1 — Hybrid Heuristic Modeling</div>
        <div style="font-size:14px;">
          The recommendation model combines two complementary heuristics:
          <ul>
            <li><strong>File Similarity:</strong> Structural and contextual similarity between files.</li>
            <li><strong>Change History:</strong> Historical co-change frequency extracted from version control data.</li>
          </ul>
          These heuristics form the fitness basis for the optimization process.
        </div>
      </div>

      <div style="border:1px solid #ddd; border-radius:14px; padding:14px;">
        <div style="font-weight:700; margin-bottom:6px;">2 — Genetic Algorithm Optimization</div>
        <div style="font-size:14px;">
          The tool encodes candidate file sets as chromosomes and evolves them using:
          <ul>
            <li>Selection</li>
            <li>Crossover</li>
            <li>Mutation</li>
          </ul>
          The GA searches for the optimal combination of files maximizing the recommendation fitness score.
          The output is a <strong>ranked list</strong> from most to least likely co-changing files.
        </div>
      </div>

      <div style="border:1px solid #ddd; border-radius:14px; padding:14px;">
        <div style="font-weight:700; margin-bottom:6px;">3 — Empirical Evaluation</div>
        <div style="font-size:14px;">
          The approach was evaluated on <strong>20 open-source Ansible and Puppet projects</strong>.
          Results show that the approach correctly recommended co-changing files in
          <strong>86% of commits within the Top-10 recommendations</strong>.
          Instance Space Analysis (ISA) revealed stronger performance for IaC files
          relying heavily on external modules and maintained by dedicated developers.
        </div>
      </div>

    </div>
  </section>

  <!-- Characteristics -->
  <section style="margin-bottom:26px;">
    <h2 style="font-size:18px; margin:0 0 10px 0; border-bottom:1px solid #eee; padding-bottom:8px;">
      Key Characteristics
    </h2>

    <div style="font-size:14px; line-height:1.7;">
      <ul>
        <li>Optimization-based recommendation model</li>
        <li>Designed specifically for Infrastructure-as-Code ecosystems</li>
        <li>Supports Puppet (.pp) and Ansible (YAML-based) projects</li>
        <li>Balances structural similarity and evolutionary history</li>
        <li>Produces ranked Top-N recommendations</li>
        <li>Validated on large-scale real-world repositories</li>
      </ul>
    </div>
  </section>

  <!-- Research Reference -->
  <section style="margin-bottom:26px; padding:16px; border:1px solid #ddd; border-radius:14px;">
    <h2 style="font-size:18px; margin:0 0 10px 0;">Research Reference</h2>
    <div style="font-size:14px;">
      Bessghaier, N., Ouni, A., Sayagh, M., Chouchen, M., & Mkaouer, M. W.
      <em>Towards understanding code review practices for infrastructure-as-code: An empirical study on OpenStack projects.</em>
      Empirical Software Engineering, 2025.
      <br><br>
      DOI: https://doi.org/10.1007/s10664-025-10654-w
    </div>
  </section>

  <!-- Download -->
  <section style="padding:16px; border:1px solid #ddd; border-radius:14px;">
    <h2 style="font-size:18px; margin:0 0 10px 0;">Download</h2>

    <div style="font-size:14px;">
      <strong>Source code:</strong>
      <a href="https://github.com/stilab-ets/iacreview" target="_blank" rel="noopener noreferrer"
         style="color:#0b57d0; text-decoration:none;">
        https://github.com/stilab-ets/iacreview
      </a>
      <div style="margin-top:6px; color:#444;">
        Repository includes datasets, experimental scripts, and implementation details.
      </div>
    </div>
  </section>

</article>
