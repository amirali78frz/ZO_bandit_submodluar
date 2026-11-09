This folder contains the code files used in the paper titled "Bandit Online Submodular Minimisation Using Zeroth-Order Oracles".

Link to the paper: "".

We consider online submodular minimisation under bandit feedback, where at
each round a decision maker plays a subset and observes only its cost,
while the cost functions, and hence their minimiser, change over time.
Existing bandit methods only guarantee static regret, which compares
against a single fixed subset and is a weak benchmark when the minimiser
moves. This paper provides, to the best of our knowledge, the first method
with guarantees for tracking a moving minimiser in this setting. We
propose a zeroth-order method built on a two-point oracle for the
Lov\'asz extension whose two evaluations are both subsets that can be
played. The perturbed and base points are rounded by a common random
threshold, and drawing the smoothing direction from the unit sphere makes
the base evaluation a zero-mean control variate, so the oracle is an
unbiased estimator of the smoothed gradient. We establish dynamic regret
bounds of order $O((1+\sqrt{P^\ast_N})N^{3/4})$ in general and
$O((1+\sqrt{P^\ast_N})N^{2/3})$ under a sufficiently small drift,
where $P^*_N$ is the path length of the minimiser sequence, together with
the corresponding $O(N^{3/4})$ and $O(N^{2/3})$ static regret bounds.
Numerically, the method attains lower regret than the baseline algorithm of
Hazan and Kale (2012), with the advantage growing with the path length.
