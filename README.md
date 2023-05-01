# Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks

This project was realized by 

**Juan C Higuera C**

**Diego A Heredia F**

And was presented for the course **Introduction To Sociophysics** of the National University of Colombia.

In this work we review the formalism of **statistical mechanics** of **multiplex networks**.

## Abstract
In this work we give an introduction to the modeling of multiplex networks, first with a multilinear approach and second with a multilink formalism developed by Ginestra Bianconi for multiplex networks with the presence of correlation between types of relationships. Then the formalism for canonical and microcanonical sets of these networks  and the calculus of the Gibbs Entropy are presented. Finally, an introduction to diffusion in multiplex networks is presented, for this supralaplacian operators are built and an example of the importance of spectral analysis for the study of diffusion dynamics in multiplex networks is given.

## ¿Why this is important? 
Multiplex networks are models of network that considered multiple types of relations, this models are important because almost all complex networks are multiplex networks.

When we characterize the topology of a network, a point of comparison is necessary, because how much clustering coefficient is necessary to characterize a network as a clustered network? the solution of this point comparison problem is given by the Maximum Entropy Principle (MaxEnt), this principle allows us to build a set of random networks with some preselected topological properties, in this way we can build null hypothesis networks and compare their properties with the topological properties of our network of interest. In this work we review some aspects of the application of Maximum Entropy Principle in multiplex networks.

## Formalism of multiplex networks 

### Multilinear approach

The first aproximation of multiplex networks is given for a multilineal treatment, in this treatment we describe mathematicaly the network using a vector of adyacency matrix, one for each type of relationship

$$\vec{A} = \left( A^1,.......,A^M  \right)$$

and we can define a vector of degrees, one for each type of relationship

$$ \vec{k_i} = \left ( k^1_i,. . .k^{\alpha} . . , k^M_i \right)  i = 1,...,N. $$

this treatment assume independence of the different types of relationship, for this reason is unrealistic. 

To measure the correlation between different types of relationship its possible define a overlapping coefficient, this its given by the total number of pairs of nodes that are connected with two type of relations 	&alpha; and &beta;.

$$ O^{\alpha ,\beta} = \sum_{i< j} a^{\alpha}_{ij} a^{\beta}_{ij}$$

The pressence of this overlapping make necessary the construction of a more apropiate formalism. The formalism presented here was developed by Ginestra Bianconi in [1].

### Multilink approach
First we can define a multilink, multilink its a vector that caracterized the relation between two nodes in all of the relationships of the network,that is:

$$\vec{m} = (m_1,m_2,...,m_\alpha,...,m_M)$$
where M are the number of types of relationships, and the components of the vector take the values 0 or 1 if the two nodes are connected with the specific type of relationship.

This definition allow us to define a multiadyacency matrix

$$   A^{\vec{M}}_{ij} = \prod_{\alpha = 1}^M  \left( a^{\alpha}_{ij}m_{\alpha} + (1-a^{\alpha}_{ij})(1 - m_{\alpha}) \right)$$

and a multidegree

$$k^{\vec{m}}_i = \sum_{j = 1}^N A^{\vec{m}}_{ij}$$

This formalism based on multilink permit us applied the statistical mechanics machinery on multiplex networks with correlated types of relationship.

## Maximum Entropy Principle (MaxEnt)
The Maximum Entropy Principle are a principle of statistical inference, in this we build probability distributions that has some restrictions extracted from our real data and maximizes the Shannon Entropy. The maximization of Shannon Entropy ensure us that the probability distribution are the most random distribution that fulfills the restrictions. In this way the maximum entropy principle allow us to build null-hypothesis distributions.

The application of this principle in multiplex networks are in the pdf of this repository.

## Maximum Entropy Principle in multiplex networks
In the study of multiplex networks, the maximum entropy principle is used to predict the probability distribution of a network ensemble, given a set of constraints. The entropy of the ensemble is defined and maximized with respect to the constraints and normalization conditions. By using Lagrange multipliers and imposing specific structural features, the probability distribution of the networks in the ensemble can be derived. This distribution is useful for analyzing and predicting the behavior of multiplex networks under certain conditions.


### Multilinear approach to uncorrelated multiplex networks

In the case of uncorrelated multiplex networks, where there is no correlation between different types of relationships, the probability of having a multiplex network can be expressed as:

$$ P(\vec{G}) = \prod_{\alpha = 1}^M P_{\alpha}(G^{\alpha})$$

By replacing this equation in the entropy equation, we arrive at:

$$
S = \sum_{\alpha = 1}^M S^{\alpha} = - \sum_{\alpha = 1}^M \sum_{G^{\alpha}} P_{\alpha}(G^{\alpha})ln\left(P_{\alpha}(G^{\alpha})\right)
$$

This equation expresses that the entropy of a multiplex network ensemble is equal to the sum of the entropies of the ensembles for each of the relationships.

For uncorrelated networks, the multilinear approach is sufficient. We will assume that $F_{\mu}(\vec{G})$ is a linear combination of constraints $f_{\mu , \alpha}({G^{\alpha}})$ on the networks $G^{\alpha}$ for each type of relationship, i.e.,

$$
F_{\mu}(\vec{G}) = \sum_{\alpha = 1}^M f_{\mu , \alpha}(G^{\alpha})
$$
### Multilink approach to correlated multiplex networks

## Diffusion in multiplex networks

### Supralaplacian matrix

### Example of application of the spectral analysis of supralaplacian matrix

## References

[1] BIANCONI, Ginestra. Statistical mechanics of multiplex net-
works: Entropy and overlap. Physical Review E, 2013, vol. 87,
no 6, p. 062806.

[2] LEE, Kyu-Min; MIN, Byungjoon; GOH, Kwang-Il. Towards
real-world complexity: an introduction to multiplex networks.
The European Physical Journal B, 2015, vol. 88, no 2, p. 48.

[3] BOCCALETTI, Stefano, et al. The structure and dynamics
of multilayer networks. Physics Reports, 2014, vol. 544, no 1,
p. 1-122.

[4] G omez, S, et al. Diffusion Dynamics on Multiplex Networks.
Physical Review Letters, 2013, vol 110.

