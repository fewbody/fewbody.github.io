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
<p class="lede l-zh">我们做核反应理论。两个原子核碰撞后，原本进入碰撞区的概率会分到弹性散射、破裂、转移和熔合等过程。我们要算清这些份额，也要判断现有数据究竟能把答案定准到什么程度。</p>

<p class="l-en">The systems we care about most are weakly bound: <sup>6</sup>Li, <sup>7</sup>Li, <sup>9</sup>Be, and halo nuclei such as <sup>11</sup>Be, <sup>8</sup>B and <sup>6</sup>He. They are interesting for a structural reason that becomes a reaction problem. Their separation energies are so small that the projectile can come apart during the collision, so the continuum is not a correction to the reaction, it is part of the reaction. Every clean two-body notion, the optical potential, the fusion cross section, the spectroscopic factor, has to be re-derived once breakup channels are open, and the re-derivation usually changes the answer.</p>
<p class="l-zh">我们最关心弱束缚核：<sup>6</sup>Li、<sup>7</sup>Li、<sup>9</sup>Be，以及 <sup>11</sup>Be、<sup>8</sup>B、<sup>6</sup>He 这类晕核。拆开它们往往只需一两个 MeV，最松的分离能比普通稳定核小一个量级。它们还没接近靶核中心就可能散开，入射核不再是一个始终完整的粒子。散开后允许碎片逃逸的状态统称连续态，必须和原来的束缚态一起计算。光学势、熔合截面和谱因子也要在这些破裂通道打开后重新检查。</p>

<h2><span class="l-en">Lines of work</span><span class="l-zh">主要方向</span></h2>

<ul class="line-list">

  <li>
    <span class="line-tag">01 &middot; Inclusive breakup and incomplete fusion</span>
    <h3 class="l-en">Separating elastic breakup from everything else</h3>
    <h3 class="l-zh">把弹性破裂和其余部分分开</h3>
    <p class="l-en">When only one fragment of a broken-up projectile is detected, the measured cross section mixes elastic breakup, in which both fragments survive, with nonelastic breakup, in which the undetected fragment is absorbed, excites the target, or is transferred. The Ichimura-Austern-Vincent model separates the two exactly within a three-body picture. Our work established the numerical equivalence of the post and prior forms of that model, extended it to use continuum-discretized coupled-channel wave functions instead of distorted waves, and applied it to the long-standing question of why complete fusion is suppressed for weakly bound projectiles. The answer that came out of it is that incomplete fusion is a one-step direct capture process, and that the suppression is a Trojan Horse effect rather than a loss of flux. More recently we removed the spectator approximation on the detected fragment, which generalizes the sum rules of the model and shows that the standard structureless treatment is really a total cross section summed over the internal states of that fragment.</p>
    <p class="l-zh">破裂后只探测到一个碎片，测得的截面会混入两类过程。两个碎片都飞走叫弹性破裂；没被探测的碎片被靶吸收、激发靶核或转移进去，叫非弹性破裂。Ichimura-Austern-Vincent 模型在三体近似下分开这两部分。我们证明了 post 和 prior 这两种数学写法在数值上等价，又把原先的畸变波换成连续离散化耦合道波函数，也就是把入射核的束缚态和离散后的连续态联立求解。计算表明，不完全熔合可理解为一步直接俘获，完全熔合的压低来自入射流量被重新分配到这条路径。最近的工作去掉了旁观者近似，不再假定被探测碎片完全不参与反应；通常把它视为无内部结构的结果，其实对应于对该碎片所有内部状态求和后的总截面。</p>
  </li>

  <li>
    <span class="line-tag">02 &middot; Absorption mechanisms in coupled-channel theory</span>
    <h3 class="l-en">Where the absorbed flux actually goes</h3>
    <h3 class="l-zh">被吸收的粒子究竟去了哪里</h3>
    <p class="l-en">A coupled-channel calculation with imaginary potentials tells you how much flux disappears, but not what it disappeared into. We derive exact decompositions of that loss. A generalized optical theorem splits the absorption of a composite projectile into direct, breakup and interference pieces, and shows that the common simplification of dropping certain off-diagonal imaginary couplings biases the split by tens of percent. An incoming-wave boundary condition combined with a complex potential separates true fusion from peripheral loss and locates the crossover at the Coulomb barrier. The same machinery produces the Feshbach dynamic polarization potential with the full continuum coupling retained, which turns out to be genuinely nonlocal rather than of Perey-Buck form, and it rests on an exact and unique construction of the coupled-channel Green's function that we proved separately.</p>
    <p class="l-zh">耦合道方法把弹性、激发和破裂等状态写成一组相互连接的方程。方程里的虚势记录有多少概率离开这些显式通道，却不说明它去了哪里。我们用广义光学定理把复合入射核的吸收分成直接、破裂和两者的干涉项；若删掉不同通道之间由虚势产生的耦合，分解结果会偏差几十个百分点。入射波边界条件只允许进入核内区的波，配合复势后可以区分真正的熔合与靶核外围的损失，二者的交叉点落在库仑位垒上。Feshbach 动力学极化势则把所有破裂通道的影响压缩成弹性道看到的等效势。保留完整连续态耦合后，这个势依赖两个空间位置，是非局域的，不属于常用的 Perey-Buck 形式。这里还需要耦合道格林函数来描述振幅如何在各通道传播，我们另外给出了它的严格构造和唯一性证明。</p>
  </li>

  <li>
    <span class="line-tag">03 &middot; Solvers and emulators</span>
    <h3 class="l-en">Making a coupled-channel calculation cheap enough to repeat</h3>
    <h3 class="l-zh">让同一个计算能反复跑</h3>
    <p class="l-en">Most of the questions above only become answerable if the underlying solve is cheap. We work on the numerical side directly: bound-state techniques that impose scattering boundary conditions without Bloch operators, complex scaling and exterior complex scaling, Lagrange-mesh and R-matrix methods, GPU linear algebra for the dense systems that coupled channels produce, and reduced-basis emulators built by proper orthogonal decomposition and Galerkin projection that reproduce a full continuum-discretized calculation to below 0.1 percent while running two orders of magnitude faster. A calculation you can only afford to run once is a calculation you cannot do statistics on, which is why this line feeds directly into the next one.</p>
    <p class="l-zh">散射波在远处持续振荡，计算区域却不能真的延伸到无穷远。我们用直接边界匹配和 R 矩阵连接有限内区与已知的外区解；复标度及外部复标度把振荡波转成容易数值处理的衰减函数；Lagrange 网格减少积分工作。大规模耦合道还会产生稠密线性方程，我们把这部分搬到 GPU。降基代理先对一批完整解做本征正交分解，找出少数主要形状，再通过 Galerkin 投影近似新参数下的解。它比完整的连续离散化计算快两个数量级，误差仍在 0.1% 以内。只有单次求解足够便宜，才能反复改变参数并做统计推断。</p>
  </li>

  <li>
    <span class="line-tag">04 &middot; Uncertainty quantification</span>
    <h3 class="l-en">What the data actually determine</h3>
    <h3 class="l-zh">数据究竟定住了什么</h3>
    <p class="l-en">Optical potentials are fitted objects with a dozen or more parameters, and the fits are famously ambiguous. Rather than accept that as folklore, we measure it. Two tools do the work. Bayesian calibration with exact likelihood gradients gives a full posterior for a coupled-channel model rather than a single best fit. Fisher-information geometry counts how many independent parameter directions a data set can constrain at all, and the count is typically far smaller than the number of parameters being varied, which is worth knowing before an error bar is quoted. An earlier result on the same line showed that the apparent threshold anomaly in elastic scattering of weakly bound nuclei does not survive a proper bootstrap treatment of the fit uncertainty.</p>
    <p class="l-zh">光学势通常有十几个拟合参数。不同参数组合可能给出几乎一样的角分布，所以一条最优拟合曲线并不能说明参数已经确定。带精确似然梯度的贝叶斯标定保留所有与数据相容的参数区域及其概率。Fisher 信息几何检查观测量对各参数组合的敏感度，把能够独立辨认的组合数出来；这个数通常远小于实际调整的参数个数。误差棒要在这种多解性算清之后才可信。我们更早还发现，弱束缚核弹性散射中看似存在的阈异常，在用自举法反复重采样数据并重新拟合后不再显著。</p>
  </li>

  <li>
    <span class="line-tag">05 &middot; Machine learning, where it earns its place</span>
    <h3 class="l-en">Differentiability is the argument, not novelty</h3>
    <h3 class="l-zh">什么时候才用神经网络</h3>
    <p class="l-en">Neural networks enter this work for one of two concrete reasons: they are differentiable, or they are fast. Physics-informed networks can solve the scattering problem once an exterior complex scaling boundary makes the oscillating asymptotic behaviour tractable. A bidirectional recurrent architecture, with the radial coordinate playing the role usually given to time, maps a global optical potential onto nucleon-nucleus scattering wave functions across a wide range of energies, masses and partial waves, and it is differentiable end to end. Symbolic regression applied to a Kolmogorov-Arnold network for nuclear masses returns terms recognisable from the mass formula. What we avoid is using a network where a conventional solver already gives the answer and the interpretation.</p>
    <p class="l-zh">神经网络在这里要解决明确的计算问题。物理信息神经网络把散射方程的残差直接写进训练误差，外部复标度再把远处持续振荡的波变成容易训练的衰减函数。双向循环网络则把径向坐标当作序列，学习全局光学势到核子核散射波函数的映射，覆盖较宽的能量、质量和分波范围。它端到端可微，可以直接求出波函数对势参数的导数。我们也把 Kolmogorov-Arnold 网络用于核质量，再用符号回归把网络学到的关系写成公式，检查其中是否出现熟悉的质量公式项。若传统求解器已经又快又容易解释，就没有必要换成网络。</p>
  </li>

</ul>

<h2><span class="l-en">Open problems we are working toward</span><span class="l-zh">还没解决的问题</span></h2>

<ul>
  <li><span class="l-en">Merging a microscopic description of the projectile's internal structure with the reaction calculation, so that a cluster model potential is no longer the weakest link in a breakup prediction.</span><span class="l-zh">把从核子相互作用出发算出的入射核内部结构接进反应计算，减少对经验团簇模型势的依赖。</span></li>
  <li><span class="l-en">Four-body breakup with more than two charged fragments, which the Faddeev route handles badly and which a distorted-wave treatment of a three-body projectile may reach.</span><span class="l-zh">计算带两个以上带电碎片的四体破裂。常用的严格少体方法 Faddeev 在多个带电粒子下很难处理，三体入射核的畸变波方案可能更可行。</span></li>
  <li><span class="l-en">Decay as the time-reversed problem: two-body alpha decay first, then two-proton emission, in the same continuum framework used for breakup.</span><span class="l-zh">把衰变看成时间反演的散射问题：先算两体的 alpha 衰变，再处理双质子发射，沿用破裂计算中允许粒子逃逸的连续态框架。</span></li>
  <li><span class="l-en">Surrogate reactions, where an inclusive breakup measurement stands in for a neutron-induced cross section that cannot be measured directly. The nonelastic breakup formalism is the natural language for this and the remaining gap is quantitative.</span><span class="l-zh">有些中子诱发反应截面无法直接测量，只能改测一个容易实现的破裂反应，再反推出目标截面，这叫替代反应。非弹性破裂理论提供了两者之间的联系，难点在于把关系算准。</span></li>
  <li><span class="l-en">Chiral effective field theory optical potentials inside a Bayesian reaction calibration, so that the uncertainty budget runs from the nuclear force to the observable without a phenomenological break in the middle.</span><span class="l-zh">把由手征有效场论核力推导的光学势接进贝叶斯反应标定，让核力近似带来的不确定度一路传到最终观测量，不在中间换成纯经验势。</span></li>
</ul>

<h2><span class="l-en">How we work</span><span class="l-zh">工作方式</span></h2>

<p class="l-en">Three habits, stated plainly because they shape what a student here does day to day. Physics first: a good chi-squared with the wrong mechanism is worthless, so the physical argument is made before the fit is quoted. Numerics get checked against something independent, a published number, an analytic limit or a second code, and the agreement is reported to a stated number of digits. And the codes are written by us and released, because a result that nobody else can reproduce is not yet a result.</p>
<p class="l-zh">机制错了，卡方再漂亮也没用。我们先说明物理过程，再讨论拟合。数值结果必须找独立参照，可以是已发表的数字、解析极限或第二套代码，并明确报告吻合到几位有效数字。组里的代码由我们自己维护，适合公开的版本随论文发布，方便别人复现和检查。</p>

<p><a href="{{ site.url }}{{ site.baseurl }}/codes"><span class="l-en">The codes</span><span class="l-zh">代码</span></a> &nbsp;&middot;&nbsp; <a href="{{ site.url }}{{ site.baseurl }}/publications"><span class="l-en">Publications</span><span class="l-zh">论文</span></a> &nbsp;&middot;&nbsp; <a href="{{ site.url }}{{ site.baseurl }}/opening"><span class="l-en">Join the group</span><span class="l-zh">加入我们</span></a></p>

</div>
