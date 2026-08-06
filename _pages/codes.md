---
title: "Codes - QFBD Research Group"
layout: textlay
excerpt: "Open-source nuclear reaction solvers and emulators developed in the group, plus teaching examples."
permalink: /codes/
---

<div markdown="0">

<h1><span class="l-en">Codes</span><span class="l-zh">代码</span></h1>

<p class="lede l-en">Almost every result on this site came out of a solver written in the group. Most are on GitHub together with the paper that documents them. If a code you need is not public yet, write to us.</p>
<p class="lede l-zh">这个网站上几乎每一个结果，都出自组里自己写的求解器。它们大多和记录它们的论文一起挂在 GitHub 上。如果你需要的代码还没有公开，写信给我们。</p>

<h2><span class="l-en">Reaction solvers</span><span class="l-zh">反应求解器</span></h2>

<div class="code-grid">

  <div class="code-card">
    <h4>smoothie</h4>
    <p class="l-en">Fortran 95. Inclusive nonelastic breakup in the Ichimura-Austern-Vincent model, with distorted-wave or continuum-discretized coupled-channel wave functions for the projectile. The production code behind most of the incomplete-fusion work.</p>
    <p class="l-zh">Fortran 95。在 Ichimura-Austern-Vincent 模型下计算非弹性破裂，入射核波函数可选畸变波或连续离散化耦合道。大部分不完全熔合工作背后的生产代码。</p>
    <p class="links"><a href="https://github.com/jinleiphys/smoothie">GitHub</a></p>
  </div>

  <div class="code-card">
    <h4>transfer</h4>
    <p class="l-en">Fortran 95. Distorted-wave transfer and nonelastic breakup engine, including the unitary transformation of the exit-channel potential used to probe off-shell sensitivity.</p>
    <p class="l-zh">Fortran 95。畸变波转移与非弹性破裂计算引擎，包含用于探测离壳敏感性的出射道势幺正变换。</p>
    <p class="links"><a href="https://github.com/jinleiphys/transfer">GitHub</a></p>
  </div>

  <div class="code-card">
    <h4>inhomoR</h4>
    <p class="l-en">Lagrange-mesh R-matrix solver for inhomogeneous equations, the numerical core of source-term problems such as nonelastic breakup. Extended with the Vincent-Fortune contour method for the post-form integrals.</p>
    <p class="l-zh">求解非齐次方程的 Lagrange 网格 R 矩阵程序，是非弹性破裂这类带源项问题的数值核心。后来加入了 Vincent-Fortune 围道方法处理 post 形式的积分。</p>
    <p class="links"><a href="https://github.com/jinleiphys/inhomoR">GitHub</a> <a href="https://doi.org/10.1103/PhysRevC.102.014608">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>COLOSS</h4>
    <p class="l-en">Complex-scaled optical and Coulomb scattering solver. Handles local and Perey-Buck nonlocal optical potentials by rotating the contour so that scattering states become square integrable.</p>
    <p class="l-zh">复标度光学势与库仑散射求解器。通过旋转积分围道让散射态变得平方可积，从而同时处理局域势和 Perey-Buck 非局域势。</p>
    <p class="links"><a href="https://github.com/jinleiphys/COLOSS">GitHub</a> <a href="https://doi.org/10.1016/j.cpc.2025.109568">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>SLAM.jl</h4>
    <p class="l-en">Julia. General scattering solver on a Lagrange-Legendre basis using direct boundary matching, which imposes scattering boundary conditions with bound-state machinery and no Bloch operator. Written to be emulated.</p>
    <p class="l-zh">Julia。基于 Lagrange-Legendre 基的通用散射求解器，用直接边界匹配施加散射边界条件，只需束缚态机制，不需要 Bloch 算符。从设计上就是为代理模型准备的。</p>
    <p class="links"><a href="https://github.com/jinleiphys/SLAM.jl">GitHub</a> <a href="https://doi.org/10.1103/ddcx-cslb">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>swift.jl</h4>
    <p class="l-en">Julia. Three-body Faddeev solver with realistic nucleon-nucleon forces and a three-nucleon interaction; triton bound state and neutron-deuteron scattering with Coulomb and complex scaling.</p>
    <p class="l-zh">Julia。采用真实核子核子力和三体力的三体 Faddeev 求解器；可算氚核束缚态以及带库仑和复标度的中子氘散射。</p>
    <p class="links"><a href="https://github.com/jinleiphys/swift.jl">GitHub</a></p>
  </div>

</div>

<h2><span class="l-en">Numerics and machine learning</span><span class="l-zh">数值与机器学习</span></h2>

<div class="code-grid">

  <div class="code-card">
    <h4>HPRMAT</h4>
    <p class="l-en">Fortran 90/95 and CUDA. High-performance R-matrix linear algebra: direct LU, mixed precision, and a cuSOLVER drop-in replacement for the dense solves that dominate large coupled-channel calculations, including a multi-GPU path.</p>
    <p class="l-zh">Fortran 90/95 与 CUDA。高性能 R 矩阵线性代数：直接 LU、混合精度，以及针对大规模耦合道计算中占主导的稠密求解的 cuSOLVER 替换实现，并包含多 GPU 路径。</p>
    <p class="links"><a href="https://github.com/jinleiphys/HPRMAT">GitHub</a> <a href="https://arxiv.org/abs/2512.11590">arXiv</a></p>
  </div>

  <div class="code-card">
    <h4>PINN-ECS</h4>
    <p class="l-en">Python and JAX. Physics-informed neural network solver for nuclear scattering, using an exterior complex scaling boundary so the oscillating asymptotic region becomes trainable while the optical potential stays on the real axis.</p>
    <p class="l-zh">Python 与 JAX。求解核散射的物理信息神经网络，用外部复标度边界让振荡的渐近区变得可训练，同时把光学势保留在实轴上。</p>
    <p class="links"><a href="https://github.com/jinleiphys/PINN-ECS">GitHub</a> <a href="https://doi.org/10.1103/sjz4-pq6p">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>BiLNN</h4>
    <p class="l-en">PyTorch. Bidirectional recurrent surrogate mapping a global optical potential to nucleon-nucleus scattering wave functions over 1 to 200 MeV, twelve target nuclei and partial waves up to l = 30, differentiable end to end. Available from the author on request.</p>
    <p class="l-zh">PyTorch。双向循环代理模型，把全局光学势映射到核子核散射波函数，覆盖 1 至 200 MeV、十二个靶核以及 l 直到 30 的分波，端到端可微。可向作者索取。</p>
    <p class="links"><a href="https://doi.org/10.1103/qw54-df4l">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>STARS</h4>
    <p class="l-en">Fortran 90/95 and CUDA. Coupled-channel and continuum-discretized coupled-channel production code with a reduced-basis emulator on the Fortran side. Internal to the group at present.</p>
    <p class="l-zh">Fortran 90/95 与 CUDA。耦合道及连续离散化耦合道的生产代码，Fortran 侧自带降基代理。目前仅组内使用。</p>
    <p class="links"><a href="https://doi.org/10.1103/n24x-d9gm">Emulator paper</a></p>
  </div>

</div>

<h2><span class="l-en">Teaching examples</span><span class="l-zh">教学示例</span></h2>

<p class="l-en">Short, self-contained programs that solve the deuteron bound state four different ways. This is the usual first week for a new student in the group: the same physical answer reached through four numerical routes, so that the method and the physics can be told apart.</p>
<p class="l-zh">四个短小自洽的程序，用四种不同方法求解氘核束缚态。这通常是新生进组的第一周内容：同一个物理答案，用四条数值路径各走一遍，从而把方法和物理分开来看。</p>

<ul>
  <li><span class="l-en">Coordinate space with a Gaussian potential, Numerov integration.</span><span class="l-zh">坐标空间，高斯势，Numerov 积分。</span>
    <a href="https://raw.githubusercontent.com/fewbody/fewbody.github.io/downloads-storage/np_bound_numerov.pdf">slides</a>,
    <a href="https://raw.githubusercontent.com/fewbody/fewbody.github.io/downloads-storage/numerov_np_bound.zip">code</a></li>
  <li><span class="l-en">Momentum space with a Gaussian potential.</span><span class="l-zh">动量空间，高斯势。</span>
    <a href="https://raw.githubusercontent.com/fewbody/fewbody.github.io/downloads-storage/np_bound_momentum.pdf">slides</a>,
    <a href="https://raw.githubusercontent.com/fewbody/fewbody.github.io/downloads-storage/momentumspace_np_bound.zip">code</a></li>
  <li><span class="l-en">Momentum space with a realistic nucleon-nucleon force.</span><span class="l-zh">动量空间，真实核子核子力。</span>
    <a href="https://raw.githubusercontent.com/fewbody/fewbody.github.io/downloads-storage/np_bound_with_realistic_force.pdf">slides</a>,
    <a href="https://raw.githubusercontent.com/fewbody/fewbody.github.io/downloads-storage/momentumspace_deuteron_bound.zip">code</a></li>
  <li><span class="l-en">R-matrix method with a Gaussian potential.</span><span class="l-zh">R 矩阵方法，高斯势。</span>
    <a href="https://raw.githubusercontent.com/fewbody/fewbody.github.io/downloads-storage/np_bound_with_R-matrix.pdf">slides</a>,
    <a href="https://raw.githubusercontent.com/fewbody/fewbody.github.io/downloads-storage/Rmatrix_np_bound.zip">code</a></li>
</ul>

</div>
