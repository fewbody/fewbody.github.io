---
title: "Codes - QFBD Research Group"
layout: textlay
excerpt: "Open-source nuclear reaction solvers and emulators developed in the group, plus teaching examples."
permalink: /codes/
---

<div markdown="0">

<h1><span class="l-en">Codes</span><span class="l-zh">代码</span></h1>

<p class="lede l-en">Almost every result on this site came out of a solver written in the group. Most are on GitHub together with the paper that documents them. If a code you need is not public yet, write to us.</p>
<p class="lede l-zh">网站上几乎每个结果都来自组里自己写的程序，大部分随论文放在 GitHub。某套代码如果还没公开，可以写信询问。</p>

<h2><span class="l-en">Reaction solvers</span><span class="l-zh">反应求解器</span></h2>

<div class="code-grid">

  <div class="code-card">
    <h4>smoothie</h4>
    <p class="l-en">Fortran 95. Inclusive nonelastic breakup in the Ichimura-Austern-Vincent model, with distorted-wave or continuum-discretized coupled-channel wave functions for the projectile. The production code behind most of the incomplete-fusion work.</p>
    <p class="l-zh">Fortran 95。用 Ichimura-Austern-Vincent 模型计算非弹性破裂，也就是只探测一个碎片、另一个碎片被吸收或转移的过程。入射核波函数可用畸变波近似，也可用连续离散化耦合道，把束缚态和离散后的破裂态联立求解。组里大部分不完全熔合工作由它完成。</p>
    <p class="links"><a href="https://github.com/jinleiphys/smoothie">GitHub</a></p>
  </div>

  <div class="code-card">
    <h4>transfer</h4>
    <p class="l-en">Fortran 95. Distorted-wave transfer and nonelastic breakup engine, including the unitary transformation of the exit-channel potential used to probe off-shell sensitivity.</p>
    <p class="l-zh">Fortran 95。计算畸变波转移和非弹性破裂。程序可对出射道势做幺正变换，在保持弹性散射结果不变的同时改变无法直接测量的离壳部分，用来检查反应预测对这部分有多敏感。</p>
    <p class="links"><a href="https://github.com/jinleiphys/transfer">GitHub</a></p>
  </div>

  <div class="code-card">
    <h4>inhomoR</h4>
    <p class="l-en">Lagrange-mesh R-matrix solver for inhomogeneous equations, the numerical core of source-term problems such as nonelastic breakup. Extended with the Vincent-Fortune contour method for the post-form integrals.</p>
    <p class="l-zh">用 Lagrange 网格和 R 矩阵求解右端带驱动源的薛定谔方程，是非弹性破裂计算的数值核心。Vincent-Fortune 围道方法把难收敛的 post 形式积分移到复平面上处理。</p>
    <p class="links"><a href="https://github.com/jinleiphys/inhomoR">GitHub</a> <a href="https://doi.org/10.1103/PhysRevC.102.014608">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>COLOSS</h4>
    <p class="l-en">Complex-scaled optical and Coulomb scattering solver. Handles local and Perey-Buck nonlocal optical potentials by rotating the contour so that scattering states become square integrable.</p>
    <p class="l-zh">用复标度求解光学势和库仑散射。把坐标或积分围道转入复平面后，原本持续振荡的散射态会衰减并变得平方可积。局域势只作用在同一点，Perey-Buck 非局域势还会联系不同位置的波函数，两者都可用同一套基展开处理。</p>
    <p class="links"><a href="https://github.com/jinleiphys/COLOSS">GitHub</a> <a href="https://doi.org/10.1016/j.cpc.2025.109568">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>SLAM.jl</h4>
    <p class="l-en">Julia. General scattering solver on a Lagrange-Legendre basis using direct boundary matching, which imposes scattering boundary conditions with bound-state machinery and no Bloch operator. Written to be emulated.</p>
    <p class="l-zh">Julia。基于 Lagrange-Legendre 基的通用散射求解器。在有限半径处直接匹配已知的外区散射波，这样就能沿用束缚态的矩阵求解方式，不需要 Bloch 算符；程序接口也便于建立代理模型。</p>
    <p class="links"><a href="https://github.com/jinleiphys/SLAM.jl">GitHub</a> <a href="https://doi.org/10.1103/ddcx-cslb">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>swift.jl</h4>
    <p class="l-en">Julia. Three-body Faddeev solver with realistic nucleon-nucleon forces and a three-nucleon interaction; triton bound state and neutron-deuteron scattering with Coulomb and complex scaling.</p>
    <p class="l-zh">Julia。三体 Faddeev 求解器，把三体薛定谔方程拆成相互耦合的分量，使用真实核子核子力和三体力。程序可算氚核束缚态与中子氘散射，并包含库仑作用和复标度处理。</p>
    <p class="links"><a href="https://github.com/jinleiphys/swift.jl">GitHub</a></p>
  </div>

</div>

<h2><span class="l-en">Numerics and machine learning</span><span class="l-zh">数值与机器学习</span></h2>

<div class="code-grid">

  <div class="code-card">
    <h4>HPRMAT</h4>
    <p class="l-en">Fortran 90/95 and CUDA. High-performance R-matrix linear algebra: direct LU, mixed precision, and a cuSOLVER drop-in replacement for the dense solves that dominate large coupled-channel calculations, including a multi-GPU path.</p>
    <p class="l-zh">Fortran 90/95 加 CUDA。大规模 R 矩阵和耦合道计算会产生很大的稠密线性方程，HPRMAT 专门加速这一步。它支持直接 LU、用较低精度分解再以高精度修正的混合精度算法、cuSOLVER 替换接口和多 GPU 计算。</p>
    <p class="links"><a href="https://github.com/jinleiphys/HPRMAT">GitHub</a> <a href="https://arxiv.org/abs/2512.11590">arXiv</a></p>
  </div>

  <div class="code-card">
    <h4>PINN-ECS</h4>
    <p class="l-en">Python and JAX. Physics-informed neural network solver for nuclear scattering, using an exterior complex scaling boundary so the oscillating asymptotic region becomes trainable while the optical potential stays on the real axis.</p>
    <p class="l-zh">Python 加 JAX。把核散射方程直接写进神经网络的训练目标。外部复标度只在远处把振荡波转成衰减函数，使网络能够学习，同时光学势仍在实轴上计算。</p>
    <p class="links"><a href="https://github.com/jinleiphys/PINN-ECS">GitHub</a> <a href="https://doi.org/10.1103/sjz4-pq6p">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>BiLNN</h4>
    <p class="l-en">PyTorch. Bidirectional recurrent surrogate mapping a global optical potential to nucleon-nucleus scattering wave functions over 1 to 200 MeV, twelve target nuclei and partial waves up to l = 30, differentiable end to end. Available from the author on request.</p>
    <p class="l-zh">PyTorch。双向循环网络代理模型，训练后可直接从全局光学势给出核子核散射波函数，无需每次重解微分方程。覆盖 1 到 200 MeV、十二个靶核、l 到 30，并可直接计算波函数对输入参数的导数。代码可向作者索取。</p>
    <p class="links"><a href="https://doi.org/10.1103/qw54-df4l">Paper</a></p>
  </div>

  <div class="code-card">
    <h4>STARS</h4>
    <p class="l-en">Fortran 90/95 and CUDA. Coupled-channel and continuum-discretized coupled-channel production code with a reduced-basis emulator on the Fortran side. Internal to the group at present.</p>
    <p class="l-zh">Fortran 90/95 加 CUDA。用于耦合道和连续离散化耦合道的主力代码，可把多个内部状态及其相互转化联立求解。Fortran 端还带降基代理，从少量完整解中提取主要形状来快速近似新结果。目前只在组内使用。</p>
    <p class="links"><a href="https://doi.org/10.1103/n24x-d9gm">Emulator paper</a></p>
  </div>

</div>

<h2><span class="l-en">Teaching examples</span><span class="l-zh">教学示例</span></h2>

<p class="l-en">Short, self-contained programs that solve the deuteron bound state four different ways. This is the usual first week for a new student in the group: the same physical answer reached through four numerical routes, so that the method and the physics can be told apart.</p>
<p class="l-zh">四个独立小程序，用四种数值方法求同一个氘核束缚态。这通常是新生进组第一周的练习：把结果对到相同精度，再分清差异来自物理输入还是数值方法。</p>

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
