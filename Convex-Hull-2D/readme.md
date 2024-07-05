# Convex Hull

## I. Definition
> A subset $S$ of the plane is called *convex* if and only if for any pair of points $p, q \in S$ the line segment $\overline{pq}$ is completely contained in $S$. The *convex hull* $\mathcal{CH}(S)$ of a set $S$ is the smallest convex set that contains $S$. To be more precise, it is the intersection of all convex sets that contain $S$.

<div style="text-align: center;">
    <img src="img/img1.png" alt="Example of convex/non-convex polygon" />
</div>

## II. Algorithms
The first definition of convex hulls is of little help when we want to design an algorithm to compute the convex hull. It talks about the intersection of all convex sets containing $P$. Now, we  can define the edge of $\mathcal{CH}(P)$:
> Both end point $p, q$  of such an edge are point of $P$, and if we direct the line through $p, q$ such that \mathcal{CH}(P)$ lies to the right, then all the point of $P$ must lie to the right of this line. The reverse is also true: if all points of  $P \setminus \{p, q\}$ lie to right of the directed line through $p, q$, then $\overline{pq}$ is and edge of $\mathcal{CH}(P)$

**Example:**

<div style="text-align: center;">
    <img src="img/img2.png" alt="Example of an edge in CH(P)" />
</div>