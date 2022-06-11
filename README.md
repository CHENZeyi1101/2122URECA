<img width="880" height = "80" alt = "Serial Title"
    src="doc/images/readme.jpg">

#  Markov-Chain-Approaches-to-Payoff-Optimization-in-the-Self-Organizing-Network-Coloring-Game

This is a research project under the Undergraduate Research Experience on Campus (URECA) Programme, NTU.

## Contents

- [Abstract](#Abstract)
- [Keywords](#Keywords)
- [Descriptions](#Descriptions)
- [Instructions](#Instructions)
- [License](#License)
- [Author](#Author)



## Abstract

The model of Network Coloring Game (NCG) is
used to simulate conflict resolving and consensus reaching
procedures in social science. In this work, we adopted some
Markov Chain Techniques into the investigation of NCG. Firstly,
with no less than ∆ + 2 colors provided, we proposed and
proved that the conflict resolving time has its expectation to
be O(log n) and the variance O((log n)^2), thus is Op (log n), where
n is the number of vertices and ∆ is the maximum degree
of the network. This was done by introducing an absorbing
Markov Chain into NCG.Secondly, we developed an algorithms
to reduce the network in post-conflict-resolution adjustments
when a Borda rule is applied among players. Markov Chain
Monte Carlo methods were employed to estimate both local and
global optimal payoffs. Supporting experimental results were
given to illustrate the corresponding procedures.

## Keywords
Network Coloring Game, Social Choices, Absorbing Markov Chain, Monte Carlo Simulation, Color Sampling

## Descriptions
"Local" contains the codes for local optimal value detection, which simulates the detailed procedure for players to reach the optimal payoff from the initial proper coloring. "Glocal contains the codes for reaching global optimal value, using Simulated Annealing methods.

The pre-defined functions include:

* IsProper.py: function to identify whether the given color assignment is proper.
* Preference_Generator.py: function to generate the preference matrix of the players in network.
* CreateNetwork.py: Create a random network with certain number of vertices, where an edge has 0.3 probability to exist between each pair of vertices.
* ProperColoring_Generator.py: Generate the initial proper coloring after conflict resolving.
* RemoveVertex.py: Remove the leaving vertex from the network.

Functions in "local" file include:

* NetworkReduction.py: Reduce the network in each iteration based on assumptions made in Part IV.
* Metropolis Hasting in NCG.py: Sampling uniformly from proper colorings using Metroplis-Hasting Algorithm.
* WelfareGenerator.py: Record the local optimal welfares as a list.

Functions in "global" file include:

* Simulated Annealing Algorithm.py: Apply simulated annealing on proper colorings to find global maximum.
* WelfareFunction: Output the system payoff given a particular coloring assignment. 

## Instructions
The complete code of expriments is given in the main file, and the procedures generating local and global optimal payoffs are also given in the "local" and "global" files respectively.

## License
The MIT License

## Author
Chen Zeyi <chenzeyi111@gmail.com>

