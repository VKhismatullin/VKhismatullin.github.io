---
layout: page
title: Chaos and decision-making
description: Why beauty is in simplicity
img: assets/img/publication_preview/ex_1.jpg
importance: 1
category: in proceedings
related_publications: true
---


These days all professional poker players know that Texas Hold'em is solved ([Reference](https://webdocs.cs.ualberta.ca/~bowling/papers/15science.pdf)). However, poker in itslef is far from being solved. Out of all the open problems, I find two key problems of interest. 

1. Firstly, what is the optimal strategy in tournaments where pure GTO is never optimal, as one has to exploit weak players earlier on to get an advantage other GTO players once the weak ones are eliminated.

2. Secondly, what are some predictive characteristics of players that reflect their chances to win games. Gaining information about it may allow us to come up with a betting algorithm on the players themselves.


I started this paper with the idea to solve the first problem, however, pivoted to the second one very soon. This is a first step in what hoperfully turns out to be a realistic solution to both problems. Please note that while the model in this paper deviates slightly from Heads-On Poker by allowing infinite bets, it does provide insides into how balanced the game is. 

I derive a series of equation that solves the game analytically. Graphs confirm that adequate levels of risk-aversion and player predictability (average hand range size) lead to balanced games, although the second player has an advantage. At the same time, we observe very beautiful fractal-like graphs for very low risk aversion/ high hand range.


You can find the code deriving optimal strategy in [this GitHub repository](https://github.com/VKhismatullin/SolvingNaivePoker) and read the paper below.

<div style="width:100%; height:600px;">
  <iframe 
    src="/assets/pdf/Naive_Poker.pdf" 
    width="100%" 
    height="100%" 
    style="border:none;">
      This browser does not support PDFs. Please download the PDF to view it: 
      <a href="/assets/pdf/Naive_Poker.pdf">Download PDF</a>.
  </iframe>
</div>



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/ex_1.gif" title="Game theory beauty" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/ex_2.gif" title="Game theory beauty" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    My favorite fractal-like graphs - observed for very high inverse risk-aversion.
</div>