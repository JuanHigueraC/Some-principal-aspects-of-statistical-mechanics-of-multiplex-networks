# Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks

This project was realized by 

**Juan C Higuera C**

**Diego A Heredia F**

And was presented for the course **Introduction To Sociophysics** of the National University of Colombia.

In this work we review the formalism of **statistical mechanics** of **multiplex networks**.

## ¿Why this is important? 
Multiplex networks are models of network that considered multiple types of relations, this models are important because almost all complex networks are multiplex networks.

When we characterize the topology of a network, a point of comparison is necessary, because how much clustering coefficient is necessary to characterize a network as a clustered network? the solution of this point comparison problem is given by the Maximum Entropy Principle (MaxEnt), this principle allows us to build a set of random networks with some preselected topological properties, in this way we can build null hypothesis networks and compare their properties with the topological properties of our network of interest. In this work we review some aspects of the application of Maximum Entropy Principle in multiplex networks.

## Formalism of multiplex networks 

The first aproximation of multiplex networks is given for a multilineal treatment, in this treatment we describe mathematicaly the network using a vector of adyacency matrix, one for each type of relationship

![image](https://github.com/JuanHigueraC/Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks/blob/657ba3a3eec1eb8752ca714aaf9cccce428689b2/Images/adyacencia.PNG)

and we can define a vector of degrees, one for each type of relationship

![image](https://github.com/JuanHigueraC/Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks/blob/0b6681326849f93a8b0105454703b4532ee8c12c/Images/grado.PNG)

this treatment assume independence of the different types of relationship, for this reason is unrealistic. To measure the correlation between different types of relationship its possible define a overlapping coefficient, this its given by the total number of pairs of nodes that are connected with two type of relations 	&Alpha; and &Beta;.

![image](https://github.com/JuanHigueraC/Some-principal-aspects-of-statistical-mechanics-of-multiplex-networks/blob/0b6681326849f93a8b0105454703b4532ee8c12c/Images/sobrelapamiento.PNG)



