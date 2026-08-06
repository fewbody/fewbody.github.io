---
title: "Research - QFBD Research Group"
layout: textlay
excerpt: "Nuclear reaction theory for weakly bound nuclei: inclusive breakup, coupled channels, scattering solvers, emulators and uncertainty quantification."
sitemap: false
permalink: /research/
---

<div markdown="0">

<h1><span class="l-en">Research</span><span class="l-zh">研究方向</span></h1>

<p class="lede l-en">We are a theory group. The question underneath everything we do is simple to state and hard to answer: when two nuclei collide, where does the flux go, and how much of that answer is actually determined by the data we have?</p>
<p class="lede l-zh">我们是一个理论组。所有工作底下的问题都很好说，但很难回答：两个原子核相撞时，流去了哪里；而这个答案中，有多少是真正被我们手上的数据定住的？</p>

<p class="l-en">The systems we care about most are weakly bound: <sup>6</sup>Li, <sup>7</sup>Li, <sup>9</sup>Be, and halo nuclei such as <sup>11</sup>Be, <sup>8</sup>B and <sup>6</sup>He. They are interesting for a structural reason that becomes a reaction problem. Their separation energies are so small that the projectile can come apart during the collision, so the continuum is not a correction to the reaction, it is part of the reaction. Every clean two-body notion, the optical potential, the fusion cross section, the spectroscopic factor, has to be re-derived once breakup channels are open, and the re-derivation usually changes the answer.</p>
<p class="l-zh">我们最关心的体系是弱束缚核：<sup>6</sup>Li、<sup>7</sup>Li、<sup>9</sup>Be，以及 <sup>11</sup>Be、<sup>8</sup>B、<sup>6</sup>He 这类晕核。它们之所以有意思，起因是结构，落点却是反应：分离能太小，入射核在碰撞过程中就会散开，于是连续态不是反应的修正项，它本身就是反应的一部分。一旦破裂道打开，光学势、熔合截面、谱因子这些干净的两体概念都必须重新推导，而重新推导之后答案通常会变。</p>

<h2><span class="l-en">Lines of work</span><span class="l-zh">工作线索</span></h2>

<ul class="line-list">

  <li>
    <span class="line-tag">01 &middot; Inclusive breakup and incomplete fusion</span>
    <h3 class="l-en">Separating elastic breakup from everything else</h3>
    <h3 class="l-zh">把弹性破裂和其余部分分开</h3>
    <p class="l-en">When only one fragment of a broken-up projectile is detected, the measured cross section mixes elastic breakup, in which both fragments survive, with nonelastic breakup, in which the undetected fragment is absorbed, excites the target, or is transferred. The Ichimura-Austern-Vincent model separates the two exactly within a three-body picture. Our work established the numerical equivalence of the post and prior forms of that model, extended it to use continuum-discretized coupled-channel wave functions instead of distorted waves, and applied it to the long-standing question of why complete fusion is suppressed for weakly bound projectiles. The answer that came out of it is that incomplete fusion is a one-step direct capture process, and that the suppression is a Trojan Horse effect rather than a loss of flux. More recently we removed the spectator approximation on the detected fragment, which generalizes the sum rules of the model and shows that the standard structureless treatment is really a total cross section summed over the internal states of that fragment.</p>
    <p class="l-zh">当破裂后只探测到入射核的一个碎片时，测到的截面把两类过程混在一起：弹性破裂，即两个碎片都存活；以及非弹性破裂，即未被探测的碎片被吸收、激发靶核或发生转移。Ichimura-Austern-Vincent 模型在三体图像内把两者严格分开。我们的工作确立了该模型 post 形式与 prior 形式在数值上的等价，把它从畸变波推广到使用连续离散化耦合道波函数，并用它回答了一个长期问题：弱束缚入射核的完全熔合为什么被压低。得到的答案是，不完全熔合是一个单步直接俘获过程，而这种压低是特洛伊木马效应，不是流的损失。最近我们去掉了对被探测碎片的旁观者近似，把模型的求和规则推广，并说明标准的无结构处理实际上是对该碎片内部态求和后的总截面。</p>
  </li>

  <li>
    <span class="line-tag">02 &middot; Absorption mechanisms in coupled-channel theory</span>
    <h3 class="l-en">Where the absorbed flux actually goes</h3>
    <h3 class="l-zh">被吸收的流究竟去了哪里</h3>
    <p class="l-en">A coupled-channel calculation with imaginary potentials tells you how much flux disappears, but not what it disappeared into. We derive exact decompositions of that loss. A generalized optical theorem splits the absorption of a composite projectile into direct, breakup and interference pieces, and shows that the common simplification of dropping certain off-diagonal imaginary couplings biases the split by tens of percent. An incoming-wave boundary condition combined with a complex potential separates true fusion from peripheral loss and locates the crossover at the Coulomb barrier. The same machinery produces the Feshbach dynamic polarization potential with the full continuum coupling retained, which turns out to be genuinely nonlocal rather than of Perey-Buck form, and it rests on an exact and unique construction of the coupled-channel Green's function that we proved separately.</p>
    <p class="l-zh">带虚部势的耦合道计算告诉你有多少流消失了，却不告诉你它变成了什么。我们推导这种损失的严格分解。广义光学定理把复合入射核的吸收分成直接、破裂和干涉三部分，并说明常见的"丢掉某些非对角虚耦合"的简化会让这个分解偏差几十个百分点。入射波边界条件配合复势，可以把真正的熔合和外围损失分开，并把两者的交叉点定位在库仑位垒处。同一套机制还给出保留全部连续态耦合的 Feshbach 动力学极化势，结果表明它是真正非局域的，并不具有 Perey-Buck 形式；这套推导建立在我们另行证明的耦合道格林函数的严格且唯一的构造之上。</p>
  </li>

  <li>
    <span class="line-tag">03 &middot; Solvers and emulators</span>
    <h3 class="l-en">Making a coupled-channel calculation cheap enough to repeat</h3>
    <h3 class="l-zh">把耦合道计算做到便宜到可以反复做</h3>
    <p class="l-en">Most of the questions above only become answerable if the underlying solve is cheap. We work on the numerical side directly: bound-state techniques that impose scattering boundary conditions without Bloch operators, complex scaling and exterior complex scaling, Lagrange-mesh and R-matrix methods, GPU linear algebra for the dense systems that coupled channels produce, and reduced-basis emulators built by proper orthogonal decomposition and Galerkin projection that reproduce a full continuum-discretized calculation to below 0.1 percent while running two orders of magnitude faster. A calculation you can only afford to run once is a calculation you cannot do statistics on, which is why this line feeds directly into the next one.</p>
    <p class="l-zh">上面这些问题，大多只有在底层求解足够便宜时才谈得上回答。我们直接做数值这一侧：不借助 Bloch 算符就施加散射边界条件的束缚态技术，复标度与外部复标度，Lagrange 网格与 R 矩阵方法，针对耦合道产生的稠密矩阵的 GPU 线性代数，以及用本征正交分解加 Galerkin 投影构造的降基代理，它能在快两个数量级的同时把完整的连续离散化计算复现到 0.1% 以内。一个只跑得起一次的计算，是没法在上面做统计的，这也是这条线直接接到下一条的原因。</p>
  </li>

  <li>
    <span class="line-tag">04 &middot; Uncertainty quantification</span>
    <h3 class="l-en">What the data actually determine</h3>
    <h3 class="l-zh">数据究竟定住了什么</h3>
    <p class="l-en">Optical potentials are fitted objects with a dozen or more parameters, and the fits are famously ambiguous. Rather than accept that as folklore, we measure it. Two tools do the work. Bayesian calibration with exact likelihood gradients gives a full posterior for a coupled-channel model rather than a single best fit. Fisher-information geometry counts how many independent parameter directions a data set can constrain at all, and the count is typically far smaller than the number of parameters being varied, which is worth knowing before an error bar is quoted. An earlier result on the same line showed that the apparent threshold anomaly in elastic scattering of weakly bound nuclei does not survive a proper bootstrap treatment of the fit uncertainty.</p>
    <p class="l-zh">光学势是拟合出来的对象，往往有十几个参数，而这种拟合的多解性是出了名的。与其把它当作口口相传的经验，我们直接去度量它。两件工具承担了主要工作：带精确似然梯度的贝叶斯标定，给出耦合道模型的完整后验，而不是一个最优拟合点；Fisher 信息几何，用来数一组数据究竟能约束多少个独立的参数方向，而这个数目通常远小于被变动的参数个数，这件事应该在给出误差棒之前就知道。同一条线上更早的一个结果表明，弱束缚核弹性散射中看起来存在的阈异常，在对拟合不确定度做了合适的自举处理之后并不成立。</p>
  </li>

  <li>
    <span class="line-tag">05 &middot; Machine learning, where it earns its place</span>
    <h3 class="l-en">Differentiability is the argument, not novelty</h3>
    <h3 class="l-zh">理由是可微性，不是新颖</h3>
    <p class="l-en">Neural networks enter this work for one of two concrete reasons: they are differentiable, or they are fast. Physics-informed networks can solve the scattering problem once an exterior complex scaling boundary makes the oscillating asymptotic behaviour tractable. A bidirectional recurrent architecture, with the radial coordinate playing the role usually given to time, maps a global optical potential onto nucleon-nucleus scattering wave functions across a wide range of energies, masses and partial waves, and it is differentiable end to end. Symbolic regression applied to a Kolmogorov-Arnold network for nuclear masses returns terms recognisable from the mass formula. What we avoid is using a network where a conventional solver already gives the answer and the interpretation.</p>
    <p class="l-zh">神经网络进入这项工作，只出于两个具体理由之一：它可微，或者它快。物理信息神经网络可以求解散射问题，前提是用外部复标度把振荡的渐近行为变得可处理。一种双向循环结构，把通常留给时间的角色交给径向坐标，能把全局光学势映射到核子核散射波函数，覆盖很宽的能量、质量和分波范围，并且端到端可微。对核质量的 Kolmogorov-Arnold 网络做符号回归，能读回质量公式中可辨认的项。我们避免的是：在传统求解器已经能给出答案和解释的地方去用网络。</p>
  </li>

</ul>

<h2><span class="l-en">Open problems we are working toward</span><span class="l-zh">正在推进的开放问题</span></h2>

<ul>
  <li><span class="l-en">Merging a microscopic description of the projectile's internal structure with the reaction calculation, so that a cluster model potential is no longer the weakest link in a breakup prediction.</span><span class="l-zh">把入射核内部结构的微观描述与反应计算合并，使团簇模型势不再是破裂计算中最薄弱的一环。</span></li>
  <li><span class="l-en">Four-body breakup with more than two charged fragments, which the Faddeev route handles badly and which a distorted-wave treatment of a three-body projectile may reach.</span><span class="l-zh">含两个以上带电碎片的四体破裂，Faddeev 路线处理得不好，而对三体入射核做畸变波处理可能走得通。</span></li>
  <li><span class="l-en">Decay as the time-reversed problem: two-body alpha decay first, then two-proton emission, in the same continuum framework used for breakup.</span><span class="l-zh">把衰变作为时间反演的问题：先做两体的 alpha 衰变，再做双质子发射，使用与破裂相同的连续态框架。</span></li>
  <li><span class="l-en">Surrogate reactions, where an inclusive breakup measurement stands in for a neutron-induced cross section that cannot be measured directly. The nonelastic breakup formalism is the natural language for this and the remaining gap is quantitative.</span><span class="l-zh">替代反应：用非弹性破裂的测量去替代无法直接测量的中子诱发截面。非弹性破裂形式体系正是描述它的自然语言，剩下的差距是定量层面的。</span></li>
  <li><span class="l-en">Chiral effective field theory optical potentials inside a Bayesian reaction calibration, so that the uncertainty budget runs from the nuclear force to the observable without a phenomenological break in the middle.</span><span class="l-zh">把手征有效场论的光学势放进贝叶斯反应标定，使不确定度预算能从核力一路贯通到观测量，中间不出现唯象的断点。</span></li>
</ul>

<h2><span class="l-en">How we work</span><span class="l-zh">工作方式</span></h2>

<p class="l-en">Three habits, stated plainly because they shape what a student here does day to day. Physics first: a good chi-squared with the wrong mechanism is worthless, so the physical argument is made before the fit is quoted. Numerics get checked against something independent, a published number, an analytic limit or a second code, and the agreement is reported to a stated number of digits. And the codes are written by us and released, because a result that nobody else can reproduce is not yet a result.</p>
<p class="l-zh">三个习惯，直说出来，因为它们决定了学生在这里每天做什么。物理优先：机制错了的漂亮卡方毫无价值，所以先把物理论证讲清楚，再报拟合结果。数值必须和独立的东西对照，可以是已发表的数字、解析极限或第二套代码，而且要说明吻合到几位有效数字。代码由我们自己写并公开，因为别人复现不了的结果还算不上结果。</p>

<p><a href="{{ site.url }}{{ site.baseurl }}/codes"><span class="l-en">The codes</span><span class="l-zh">代码</span></a> &nbsp;&middot;&nbsp; <a href="{{ site.url }}{{ site.baseurl }}/publications"><span class="l-en">Publications</span><span class="l-zh">论文</span></a> &nbsp;&middot;&nbsp; <a href="{{ site.url }}{{ site.baseurl }}/opening"><span class="l-en">Join the group</span><span class="l-zh">加入我们</span></a></p>

</div>
