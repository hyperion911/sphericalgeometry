# sphericalgeometry
A Python module of various spherical computational geometry related functions.

This module is a work-in-progress including various spherical geometry functions that I needed and could not find in the well-known libraries.
The functions work on sets of points on the unit sphere.

The list of existing functions (some do not exist yet):

-`sphere_convhull` - Computes the spherical convex hull of a set of points on the unit sphere (unfinished)

-`pspolydist` - Computes the minimum distance from a point to a polyline on a sphere (unfinished). This is an adaptation to Python of the original MATLAB function [`p_spoly_dist`](https://www.mathworks.com/matlabcentral/fileexchange/52734-p_spoly_dist) by Michael Yoshpe (in-work).

-`insphericalpolygon` - Returns points inside of spherical polygon (in-work)

## Some basic notions of spherical geometry
### Great circles and geodesics

In "regular" Euclidean 2D geometry, the shortest path between two points on the plane is simply the segment between them. But when the points are on a sphere, the shortest path on the sphere is not a straight 3D segment - since this segment crosses the sphere but is not part of it. Instead, this would be a "line on the sphere" - more formally called a geodesic.

Given two "close" points on the sphere, they define a unique circle on the sphere which passes through them. We call this circle a "great circle". The great circle is separated in two paths, both of them connecting the two points. The geodesic (again - the shortest path between them) is the smallest part of the great circle.

TODO: add figure

Now consider the two poles of the sphere (the North pole and the South Pole, by analogy to the Earth, which is not a sphere). What is the shortest path between them? In fact, since the sphere is centrally symmetric around its center, there are an infinity of geodesics. Any 


### Convexity on the plane and on the sphere

TODO

Convexity of antipodal points

Quasi-convexity

### Gnomonic projection

TODO

Finding the spherical convex hull of hemispherical points using the central=gnomonic projection.

Which plane should the points be projected unto?



### Is Convex Hull always the solution?

TODO

See [this question](https://mathoverflow.net/questions/76875/convex-hull-on-a-riemannian-manifold) on Math Overflow.

### Minimum-perimeter bounding spherical polygon

## References:

See specific functions docs for references.
