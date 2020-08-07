# Draw-your-Domain
Draw Domain! We do the node generation, triangulation, and provide an approximation to the Poisson equation!

## Introduction
- Our goal is to generate the nodes and do the triangulations for the users.
Just tell us your computational domain.
We make nodes, triangulations, and even for the approximation to the Possion equation.

## Frame Work
#### Step1. Draw the computational domain(closed curve)
![1](https://user-images.githubusercontent.com/38487909/89611992-aa8ae480-d8b9-11ea-98a2-132790899c6d.JPG)
#### Step2. Fill the inside and find the boundary
![2](https://user-images.githubusercontent.com/38487909/89612152-14a38980-d8ba-11ea-9f7c-9d94b0792682.JPG)
#### Step3. Node generation
![3](https://user-images.githubusercontent.com/38487909/89612156-166d4d00-d8ba-11ea-8b8f-aa6103ac669f.JPG)
#### Step4. Triangulation
![4](https://user-images.githubusercontent.com/38487909/89612158-1705e380-d8ba-11ea-967a-f107576851f1.JPG)
#### Step5. Poisson solver (g!=0)
![5](https://user-images.githubusercontent.com/38487909/89612160-1705e380-d8ba-11ea-9f4b-4529e5a50888.JPG)

## Conclusion
- I had difficulties in triangulation when the image is concave because 'delaunay' generates triangles located outside of the interested domain.
To overcome these difficulties, I have found a major characteristics of these triangles and have succeeded to exclude those.
It is meaningful that it can be implementes in any shape of domain.
