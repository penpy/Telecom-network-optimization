# Telecom-network-optimization
Algorithms to optimize the total cost of links in a telecommunication network under some constraints.

An example of a network.

![](Network_example.png)

Constraints :

- Select a set of at least three digital hubs. Connect them together to form a single ring.
- Connect end offices to digital hubs. Each end office must be connected to one of the slected digital hubs. Each hub can be connected to a limited number of end offices.
- Connect customers to end offices. A large enough proportion of the customers must be connected. Each end office can be connected to a limited number of customers.

The connections and selected hubs have attributed cost. The goal is to minimize the total cost.

## Optimization algorithms

-[MILP_Small_data](MILP_Small_data): an algorithm using mixed-integer linear programming to compute the minimum cost. However it works only for small enough networks. Dependency: PuLP.

-[ILS_Large_data.ipynb](ILS_Large_data.ipynb): an iterated local search that computes an approximation of the minimum cost in polynomial time complexity.
