# Quiz 1 Review (Rewritten)

## Question 1

This question concerns the hospital-resident problem (RHP). Assume there are n hospitals and n residents, and every hospital has exactly one position. In a natural variant, called RHPI, preference lists may be incomplete: a hospital does not have to rank every resident, and a resident does not have to rank every hospital. A hospital cannot be matched with a resident who is missing from its list, and a resident cannot be matched with a hospital that is missing from theirs.

Before stating what a good RHPI solution is, it helps to list the instabilities that can occur in a valid RHPI solution and that stop it from being good.

**(a)** Complete the definition below by selecting every phrase that belongs in it.

> One possible instability is a pair (h, r′) in which resident r′ is unmatched and …

1. hospital h appears on r′'s preference list;
2. hospital h prefers its current resident r to r′;
3. hospital h prefers r′ to the resident it is currently assigned;
4. hospital h is also unmatched.

**(b)** Describe how to build an instance with n hospitals and n residents, for any sufficiently large even n, in which every hospital's and every resident's preference list has length 2, and every valid solution matches exactly n/2 residents.

## Question 2

Imagine that each scenario below arises when the Gale–Shapley algorithm is run on n employers and n applicants, with the employers proposing. For each one, give a good asymptotic lower bound Ω(·) on the number of iterations of the while-loop. Leave out low-order terms and irrelevant constant factors. If the answer involves a logarithm of any base, just write log n.

| Scenario | Lower bound on iterations |
|---|---|
| All applicants except log n of them end up with their least-preferred employer. | Ω(?) |
| Every employer has the same preference list. | Ω(?) |
| A group of n^(4/3) applicants is ranked below all other applicants by every employer, although the employers order the members of this group differently. | Ω(?) |
| 30% of the employers and 30% of the applicants agree in advance that each of them will rank the members of the other group ahead of everyone else. | Ω(?) |

## Question 3: Reductions — True or False

A computer scientist, X, wants to solve problem A. They design an algorithm that reduces A to a problem B for which an algorithm already exists. For an instance I of A, let r(I) denote the instance of B that X's algorithm produces. Select all the true statements about X's solution.

1. If B can itself be solved by a reduction to a problem C, then A can be solved by reducing it directly to C, without passing through B.
2. For every instance I of A, the solution to the B-instance r(I) produced by the reduction is identical to the solution to I.
3. Suppose the reduction turns an instance of A of size n into an instance of B of size f(n), and the algorithm for B runs in Θ(g) time. Then X's solution to A runs in Ω(g(f(n))) time.
4. Every instance I of A can be reduced to some instance J of B; that is, for every I there exists an instance J of B such that J = r(I).
