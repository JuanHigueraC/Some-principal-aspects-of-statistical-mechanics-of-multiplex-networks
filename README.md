# Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks

This project was realized by 

**Juan C Higuera C**

**Diego A Heredia F**

And was presented for the course **Introduction To Sociophysics** of the National University of Colombia.

In this work we review the formalism of **statistical mechanics** of **multiplex networks**.

## Abstract
In this work we give an introduction to the modeling of multiplex networks, first with a multilinear approach and second with a multilink formalism developed by Ginestra Bianconi for multiplex networks with the presence of correlation between types of relationships. Then the formalism for canonical and microcanonical sets of these networks and we calculate the Gibbs Entropy. Finally, an introduction to diffusion in multiplex networks is presented, for this supralaplacian operators are built and an example of the importance of spectral analysis for the study of diffusion dynamics in multiplex networks is given.

## ¿Why this is important? 
Multiplex networks are models of network that considered multiple types of relations, this models are important because almost all complex networks are multiplex networks.

When we characterize the topology of a network, a point of comparison is necessary, because how much clustering coefficient is necessary to characterize a network as a clustered network? the solution of this point comparison problem is given by the Maximum Entropy Principle (MaxEnt), this principle allows us to build a set of random networks with some preselected topological properties, in this way we can build null hypothesis networks and compare their properties with the topological properties of our network of interest. In this work we review some aspects of the application of Maximum Entropy Principle in multiplex networks.

## Formalism of multiplex networks 

### Multilinear approach

The first aproximation of multiplex networks is given for a multilineal treatment, in this treatment we describe mathematicaly the network using a vector of adyacency matrix, one for each type of relationship

![image](https://github.com/JuanHigueraC/Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks/blob/657ba3a3eec1eb8752ca714aaf9cccce428689b2/Images/adyacencia.PNG)

and we can define a vector of degrees, one for each type of relationship

![image](https://github.com/JuanHigueraC/Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks/blob/0b6681326849f93a8b0105454703b4532ee8c12c/Images/grado.PNG)

this treatment assume independence of the different types of relationship, for this reason is unrealistic. 

To measure the correlation between different types of relationship its possible define a overlapping coefficient, this its given by the total number of pairs of nodes that are connected with two type of relations 	&alpha; and &beta;.

![image](https://github.com/JuanHigueraC/Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks/blob/0b6681326849f93a8b0105454703b4532ee8c12c/Images/sobrelapamiento.PNG)

The pressence of this overlapping make necessary the construction of a more apropiate formalism. The formalism presented here was developed by Ginestra Bianconi in [1].

### Multilink approach
First we can define a multilink, multilink its a vector that caracterized the relation between two nodes in all of the relationships of the network,that is:

![image](https://github.com/JuanHigueraC/Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks/blob/a3a7e2d11260476c6480e7d01854844e144b4916/Images/multilink.PNG)
where M are the number of types of relationships, and the components of the vector take the values 0 or 1 if the two nodes are connected with the specific type of relationship.

This definition allow us to define a multiadyacency matrix

![image](https://github.com/JuanHigueraC/Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks/blob/a3a7e2d11260476c6480e7d01854844e144b4916/Images/multiadyacencia.PNG)

and a multidegree

![image](https://github.com/JuanHigueraC/Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks/blob/a3a7e2d11260476c6480e7d01854844e144b4916/Images/multigrado.PNG)

This formalism based on multilink permit us applied the statistical mechanics machinery on multiplex networks with correlated types of relationship.

## Maximum Entropy Principle (MaxEnt)
The Maximum Entropy Principle are a principle of statistical inference, in this we build probability distributions that has some restrictions extracted from our real data and maximizes the Shannon Entropy. The maximization of Shannon Entropy ensure us that the probability distribution are the most random distribution that fulfills the restrictions. In this way the maximum entropy principle allow us to build null-hypothesis distributions.

The application of this principle in multiplex networks are in the pdf of this repository.

