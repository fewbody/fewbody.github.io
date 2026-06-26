---
title: "QFBD Research Group - Publications"
layout: gridlay
excerpt: "QFBD Research Group -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

<!-- ## Group highlights -->

## Full List of publications

* <em>Jin Lei</em><br /> 
Exterior complex scaling enables physics-informed neural networks for nuclear reactions <br /> 
<a href="https://doi.org/10.1103/sjz4-pq6p">Phys. Rev. C 113, 064618 (2026)</a>

* <em>Hao Liu, Jin Lei, and Zhongzhou Ren</em><br /> 
Channel couplings redirect absorbed flux from peripheral loss to fusion in weakly bound nuclear reactions <br /> 
<a href="https://doi.org/10.1016/j.physletb.2026.140479">Phys. Lett. B 877, 140479 (2026)</a>

* <em>Hao Liu, Jin Lei, and Zhongzhou Ren</em><br /> 
Coherent absorption dynamics: The dual role of off-diagonal couplings in weakly bound nuclei <br /> 
<a href="https://doi.org/10.1103/bgwc-x5wj">Phys. Rev. C 113, 054601 (2026)</a>

* <em>Jin Lei</em><br /> 
Reduced basis emulator for elastic scattering in continuum-discretized coupled-channels calculations <br /> 
<a href="https://doi.org/10.1103/n24x-d9gm">Phys. Rev. C 113, 044610 (2026)</a>

* <em>Jin Lei</em><br /> 
Direct boundary matching: A bound-state technique for nuclear scattering with Lagrange-Legendre functions <br /> 
<a href="https://doi.org/10.1103/ddcx-cslb">Phys. Rev. C 113, 024614 (2026)</a>

* <em>Jin Lei</em><br /> 
Numerical assessment of convergence in the post-form ichimura-austern-vincent model <br /> 
<a href="https://journals.aps.org/prc/abstract/10.1103/PhysRevC.112.014609">Phys. Rev. C 112, 014609 (2025)</a>

* <em>Jin Lei</em><br /> 
Continuum effects and the Trojan horse mechanism in halo nuclei-induced reactions: Implications for heavy isotope synthesis <br /> 
<a href="https://doi.org/10.1103/PhysRevC.111.034610">Phys. Rev. C 111, 034610 (2025)</a>

* <em>Junzhe Liu, Jin Lei, Zhongzhou Ren</em><br /> 
COLOSS: Complex-scaled Optical and couLOmb Scattering Solver <br /> 
<a href="https://doi.org/10.1016/j.cpc.2025.109568">Computer Physics Communications 311 (2025) 109568</a>

* <em>Hao Liu, Jin Lei, and Zhongzhou Ren</em><br /> 
Kolmogorov-Arnold networks in nuclear binding energy prediction <br /> 
<a href="https://doi.org/10.1103/PhysRevC.111.024316">Phys. Rev. C 111, 024316 (2025)</a>

* <em>Junzhe Liu, Jin Lei, Zhongzhou Ren</em><br /> 
A complex scaling method for efficient and accurate scattering emulation in nuclear reactions <br /> 
<a href="https://doi.org/10.1016/j.physletb.2024.139070">Phys. Lett. B 858 (2024) 139070</a>

* <em>G. Villanueva, A.M. Moro, J. Casal, Jin Lei</em><br /> 
Neutron-transfer induced breakup of the Borromean nucleus 9Be <br /> 
<a href="https://doi.org/10.1016/j.physletb.2024.138766">Phys. Lett. B 855 (2024) 138766</a>

* <em>K. Wang, Y. Y. Yang, Jin Lei, A. M. Moro, V. Guimarães, J. G. Li, F. F. Duan, Z. Y. Sun, G. Yang, D. Y. Pang, S. W. Xu, J. B. Ma, P. Ma, Z. Bai, Q. Liu, J. L. Lou, H. J. Ong, B. F. Lv, S. Guo, M. Kumar Raju, X. H. Wang, R. H. Li, X. X. Xu, Z. Z. Ren, Y. H. Zhang, X. H. Zhou, Z. G. Hu and H. S. Xu</em><br /> 
Elastic scattering and breakup reactions of the mirror nuclei 12B and 12N on 208Pb using ab initio structure input <br /> 
<a href="https://doi.org/10.1103/PhysRevC.109.014624">Phys. Rev. C 109, 014624 (2024)</a>

* <em>Jin Lei and Antonio M. Moro</em><br /> 
Advancing the Ichimura-Austern-Vincent model with continuum-discretized coupled-channels wave functions for realistic descriptions of two-body projectile breakup <br /> 
<a href="https://doi.org/10.1103/PhysRevC.108.034612">Phys. Rev. C 108, 034612</a>

* <em>Yazhou Lu, Jin Lei, and Zhongzhou Ren</em><br /> 
Systematic single-folding optical potential for 6Li and 7Li based on KD02 potentials <br /> 
<a href="https://doi.org/10.1103/PhysRevC.108.024612">Phys. Rev. C 108, 024612 (2023)</a>

* <em>Junzhe Liu, Jin Lei, and Zhongzhou Ren</em><br /> 
Testing the validity of the surface approximation for reactions induced by weakly bound nuclei with a fully quantum-mechanical model <br /> 
<a href="https://doi.org/10.1103/PhysRevC.108.024606">Phys. Rev. C 108, 024606 (2023)</a>

* <em>Hao Liu, Shinsuke Nakayama, Jin Lei, and Zhongzhou Ren</em><br /> 
Comparison of Ichimura-Austern-Vincent and Glauber models for the deuteron-induced inclusive breakup reaction in light and medium-mass nuclei <br /> 
<a href="https://doi.org/10.1103/PhysRevC.108.014617">Phys. Rev. C 108, 014617 (2023)</a>

{% for publi in site.data.publist %}
  <p>
    <strong>{{ publi.title }}</strong><br />
    <em>{{ publi.authors }}</em><br />
    <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  </p>
{% endfor %}