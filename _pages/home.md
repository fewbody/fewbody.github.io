---
title: "QFBD Research Group"
layout: homelay
excerpt: "QFBD Research Group"
sitemap: false
permalink: /
---


<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 400">
  <!-- White Background -->
  <rect width="800" height="400" fill="white"/>
  
  <!-- Abstract Quantum Representation - Simplified and Modified -->
  <g transform="translate(120, 180)">
    <!-- Main Orbital Paths with Different Colors -->
    <path d="M0,0 C30,-50 80,-30 100,0 C120,30 80,80 30,70 C-20,60 -30,30 0,0" fill="none" stroke="#3A86FF" stroke-width="4" opacity="0.9">
      <animate attributeName="stroke-width" values="4;5;4;3;4" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.9;1;0.9;0.8;0.9" dur="5s" repeatCount="indefinite"/>
    </path>
    <path d="M0,0 C-30,-40 -80,-10 -90,30 C-100,70 -60,90 -10,70 C40,50 30,30 0,0" fill="none" stroke="#FF006E" stroke-width="4" opacity="0.9">
      <animate attributeName="stroke-width" values="4;3;4;5;4" dur="4.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.9;0.8;0.9;1;0.9" dur="5.5s" repeatCount="indefinite"/>
    </path>
    <path d="M0,0 C-10,40 20,80 60,70 C100,60 110,20 80,-10 C50,-40 10,-30 0,0" fill="none" stroke="#8338EC" stroke-width="4" opacity="0.9">
      <animate attributeName="stroke-width" values="4;5;4;5;4" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.9;1;0.9;1;0.9" dur="6s" repeatCount="indefinite"/>
    </path>
    
    <!-- Central Nucleus Particle -->
    <circle cx="0" cy="0" r="10" fill="#FB5607">
      <animate attributeName="r" values="10;11;10;9;10" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.9;1;0.9;1" dur="3s" repeatCount="indefinite"/>
    </circle>
    
    <!-- Electron Particles Moving Along Paths -->
    <circle r="6" fill="#3A86FF">
      <animateMotion path="M0,0 C30,-50 80,-30 100,0 C120,30 80,80 30,70 C-20,60 -30,30 0,0" dur="8s" repeatCount="indefinite"/>
      <animate attributeName="r" values="6;5;6;7;6" dur="4s" repeatCount="indefinite"/>
    </circle>
    
    <circle r="6" fill="#FF006E">
      <animateMotion path="M0,0 C-30,-40 -80,-10 -90,30 C-100,70 -60,90 -10,70 C40,50 30,30 0,0" dur="10s" repeatCount="indefinite"/>
      <animate attributeName="r" values="6;7;6;5;6" dur="5s" repeatCount="indefinite"/>
    </circle>
    
    <circle r="6" fill="#8338EC">
      <animateMotion path="M0,0 C-10,40 20,80 60,70 C100,60 110,20 80,-10 C50,-40 10,-30 0,0" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="r" values="6;5;6;5;6" dur="3.5s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Updated Main Title with Modern Gradient -->
  <g transform="translate(420, 220)">
    <text x="0" y="0" font-family="'Helvetica Neue', Arial, sans-serif" font-size="44" font-weight="800" text-anchor="middle" fill="url(#modern-gradient)" letter-spacing="1">
      QUANTUM FEW-BODY
      <animate attributeName="fill-opacity" values="1;0.9;1;0.95;1" dur="7s" repeatCount="indefinite"/>
    </text>
    <text x="0" y="50" font-family="'Helvetica Neue', Arial, sans-serif" font-size="28" font-weight="300" text-anchor="middle" fill="#333333" letter-spacing="2">DYNAMICS RESEARCH GROUP</text>
  </g>

  <!-- Updated Energy Levels - More Bold -->
  <g transform="translate(650, 180)">
    <line x1="0" y1="0" x2="65" y2="0" stroke="#FF006E" stroke-width="4">
      <animate attributeName="stroke-width" values="4;5;4;3;4" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="65;70;65;60;65" dur="7s" repeatCount="indefinite"/>
    </line>
    <line x1="0" y1="-20" x2="65" y2="-20" stroke="#FB5607" stroke-width="4">
      <animate attributeName="stroke-width" values="4;3;4;5;4" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="65;60;65;70;65" dur="6s" repeatCount="indefinite"/>
    </line>
    <line x1="0" y1="-40" x2="65" y2="-40" stroke="#8338EC" stroke-width="4">
      <animate attributeName="stroke-width" values="4;5;4;5;4" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="65;70;65;70;65" dur="8s" repeatCount="indefinite"/>
    </line>
    <line x1="0" y1="20" x2="65" y2="20" stroke="#3A86FF" stroke-width="4">
      <animate attributeName="stroke-width" values="4;3;4;3;4" dur="5.5s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="65;60;65;60;65" dur="7.5s" repeatCount="indefinite"/>
    </line>
    
    <!-- Animated Connection Lines - Updated -->
    <path d="M30,-40 C40,-40 40,-20 30,-20" fill="none" stroke="#FFBE0B" stroke-width="2" stroke-dasharray="4,2">
      <animate attributeName="stroke-dasharray" values="4,2;5,2;4,3;4,2" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.8;1;0.8;1" dur="4s" repeatCount="indefinite"/>
    </path>
    <path d="M30,-20 C40,-20 40,0 30,0" fill="none" stroke="#FFBE0B" stroke-width="2" stroke-dasharray="4,2">
      <animate attributeName="stroke-dasharray" values="4,2;4,3;5,2;4,2" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.8;1;0.8;1" dur="5s" repeatCount="indefinite"/>
    </path>
    <path d="M30,0 C40,0 40,20 30,20" fill="none" stroke="#FFBE0B" stroke-width="2" stroke-dasharray="4,2">
      <animate attributeName="stroke-dasharray" values="4,2;5,2;4,3;4,2" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.8;1;0.8;1" dur="6s" repeatCount="indefinite"/>
    </path>
  </g>
  
  <!-- Updated Probability Cloud -->
  <g transform="translate(400, 120)">
    <ellipse cx="0" cy="0" rx="330" ry="65" fill="url(#modern-cloud)" opacity="0.15">
      <animate attributeName="rx" values="330;340;330;320;330" dur="15s" repeatCount="indefinite"/>
      <animate attributeName="ry" values="65;70;65;60;65" dur="12s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.15;0.2;0.15;0.1;0.15" dur="10s" repeatCount="indefinite"/>
      <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="120s" repeatCount="indefinite"/>
    </ellipse>
  </g>
  
  <!-- Updated Animated Quantum Dots - Brighter -->
  <g>
    <circle cx="200" cy="300" r="4" fill="#FF006E">
      <animate attributeName="r" values="4;6;4;2;4" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.6;1;0.6;1" dur="4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="550" cy="280" r="4" fill="#8338EC">
      <animate attributeName="r" values="4;2;4;6;4" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.6;1;0.6;1" dur="5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="650" cy="120" r="4" fill="#FFBE0B">
      <animate attributeName="r" values="4;6;4;2;4" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.6;1;0.6;1" dur="6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="300" cy="70" r="4" fill="#3A86FF">
      <animate attributeName="r" values="4;2;4;6;4" dur="4.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.6;1;0.6;1" dur="4.5s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Gradients - Updated with Modern Palette -->
  <defs>
    <linearGradient id="modern-gradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#3A86FF"/>
      <stop offset="25%" stop-color="#8338EC"/>
      <stop offset="50%" stop-color="#FF006E"/>
      <stop offset="75%" stop-color="#FB5607"/>
      <stop offset="100%" stop-color="#FFBE0B"/>
      <animate attributeName="x1" values="0%;10%;0%" dur="10s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="100%;90%;100%" dur="10s" repeatCount="indefinite"/>
    </linearGradient>
    
    <radialGradient id="modern-cloud" cx="50%" cy="50%" r="50%" fx="50%" fy="50%">
      <stop offset="0%" stop-color="#FFBE0B" stop-opacity="0.7"/>
      <stop offset="40%" stop-color="#8338EC" stop-opacity="0.5"/>
      <stop offset="70%" stop-color="#FF006E" stop-opacity="0.4"/>
      <stop offset="100%" stop-color="#3A86FF" stop-opacity="0.2"/>
      <animate attributeName="fx" values="50%;45%;50%;55%;50%" dur="10s" repeatCount="indefinite"/>
      <animate attributeName="fy" values="50%;45%;50%;55%;50%" dur="12s" repeatCount="indefinite"/>
    </radialGradient>
  </defs>
</svg>

**About QFBD Research Group:**


The Quantum Few-Body Dynamics Research Group was established in 2020 and 
is affiliated with School of Physics Science and Engineering at Tongji University, 
led by Professor Jin Lei. The group's research focuses on utilizing quantum 
few-body models to study nuclear reaction processes, especially weakly bound nuclei induced reactions. 
The group's theoretical work involves quantum scattering theory, 
quantum few-body models, Faddeev equations, Continuum-Discretized Coupled-Channels (CDCC), DWBA, 
and the Ichimura-Austern-Vincent model.

<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="4000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li>
        <li data-target="#carousel" data-slide-to="3"></li>
        <li data-target="#carousel" data-slide-to="4"></li>
        <li data-target="#carousel" data-slide-to="5"></li>
        <li data-target="#carousel" data-slide-to="6"></li>
    </ol>

    <!-- Items -->
    <div class="carousel-inner" markdown="0">
        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/sigmaR.jpeg" alt="Slide 1" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/PhysRevLett.123.jpeg" alt="Slide 2" />
        </div>
    </div>
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>


In previous work, the group used the quantum three-body IAV model to study 
the breakup and fusion reactions of weakly bound nuclei. 
Some of the group's representative works include

1. Jin Lei and Antonio M. Moro, ‘Unraveling the Reaction Mechanisms Leading to Partial Fusion of Weakly Bound Nuclei’, Phys. Rev. Lett. 123, 232501 (2019).
2. Jin Lei and Antonio M. Moro, ‘Puzzle of Complete Fusion Suppression in Weakly Bound Nuclei: A Trojan Horse Effect?’, Phys. Rev. Lett. 122, 042503 (2019).
3. Jin Lei and Antonio M. Moro, ‘Numerical assessment of post-prior equivalence for inclusive breakup reactions’, Phys. Rev. C 92, 061602(R) (2015). Editors’ Suggestion
4. Rodrigo Navarro Pérez and Jin Lei, ‘Is the unusual near-threshold potential behavior in elastic scattering of weakly-bound nuclei a precision error?’, Physics Letters B 795, 200–205 (2019).
5. A. Di Pietro, A.M. Moro, Jin Lei and R. de Diego, ‘Insights into the dynamics of breakup of the halo nucleus 11Be on a 64Zn target’, Physics Letters B 798, 134954 (2019).
6. Jin Lei, L. Hlophe, Ch. Elster, A. Nogga, F. M. Nunes and D. R. Phillips, ‘Few-body universality in the deuteron- alpha system’, Phys. Rev. C 98, 051001(R) (2018).
7. Jin Lei and Antonio M. Moro, ‘Post-prior equivalence for transfer reactions with complex potentials’, Phys. Rev. C 97, 011601(R) (2018).



The group plans to recruit one doctoral student, one master's student, and postdoctoral researchers every year. You can contact the group at jinl@tongji.edu.cn.

We are grateful for funding from [Tongji University](https://en.tongji.edu.cn/index.htm) and [NSFC](http://www.nsfc.gov.cn).

<figure class="third">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/tongji.jpeg" style="width: 110px">
</figure>
