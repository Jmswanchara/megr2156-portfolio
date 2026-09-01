# A2 – Truss Stress Analysis

## Objective

![Mission Parameters](parameters_ss.png)

Above are the parameters given for designing my own truss.  My approach to my design began with picking out the most straight-forward design that I could think of, I didn't want to work with a truss that had more components and internal forces than necessary.  I ended up falling on a basic design that I was familiar with from Statics.

# Design

![Truss FBD](Truss_FBD2.jpg)

This design is reliable for this assignment because it keeps the number of elements to a minimum. With the full truss laid out, I could examine the external forces and find the relationship between the vertical components of the supports at A and B.  A had an x component, but since there wasn't a matching external force I knew that this force would be equal to zero.

![Initial Truss Forces](Initial_Truss_Forces.png)

After marking down the forces on the truss FBD, I calculated Ay and By through the moment about A and the net force in the y direction where the P forces canceled out.  With two equations and two unknowns, I was able to solve for the magnitude of the forces in N.  The result was that I found the vertical components for A and B were opposite of each other.  

![Joint B Forces](Joint_B_Forces.png)

The pin at A has an additional force compared to the roller at B, so I chose to start at joint B for calculating my way through all the internal forces of the truss.  I first drew out the free body diagram and then wrote the net force equations in the x and y before isolating the force I wanted, which was Fbc and Fbe respectively in this case.  Then I inserted my known values and got the numerical forces of both.  I would occasionally need to add some extra calculations for necessary trigonometry when splitting force components.  This process was duplicated for every joint on the way to pin A.

[Truss Final Part](trussfinal.prt.1)
