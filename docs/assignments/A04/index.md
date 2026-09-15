# A4 – [Topic]

## Objective

![A4_motor](A4_motor.png)

The goal of this assignment was to design a motor mount that could attach to a rigid wall and hold up the motor above.  All of the motor specs were provided on the website where the image was taken A few other values were given or selected, such as the 300 N load, my choice of material, and initial lengths for the features.  I decided to go with ABS as my material and 34 mm for the width of both features.  I chose 34 mm because it felt close to the dimensions of the motor but with a reasonable amount of space in case more room was needed.

## Feature 1

![Feature 1 Knowables](Feature_1_knowables.png)

Getting ready to work on the first feature, I wrote down everything I knew the value of and needed to find that was relevant to the first feature.  I would reference this again when it was time to insert values after solving for what I needed symbolically.  This step is always helpful for keeping myself focused on what I am supposed to be working on.  This early on into the assignment I wasn't clear on the dimensions I needed to find, and misidentified my variables.  I would change the height measurement to the proper thickness variable once the math started.

![Feature 1 FBD](Feature_fbd.png)

After putting down my knowable values, I put drew a FBD of the first feature.  By this point in the process, the final technical appearance wasn't completely clear, but it was certain that it would behave as a cantilever beam so it came out resembling a typical beam image as opposed to the final product.

![Feature 1 reactions](Feature_1_reactions.png)

The first unknown that I needed to calculate was the moment for the first feature.  This needed to be found in order to calculate the thickness of the first feature, so using the FBD to find reactions and solved for the moment symbolically, then I found the value of the first moment for this assignment.

![Feature 1 work](Feature_1_work.png)

With the moment acquired, I applied the same process to the thickness.  I combined the formula for inertia of a box beam with the formula for deflection that was discussed in class to isolate the thickness.  This would be one of two competing values for thickness, with the other being the thickness derived from the yield stress of the selected material.  Also combining with the inertia, the thickness could be isolated.  Once the numbers were inserted, I could determine the governing thickness for the feature.

![Feature_1_results](Feature_1_results.png)

With both of the thicknesses solved for symbolically, calculating the values themselves was quick.  Once both values were accounted for, I found the governing thickness to be from the yield stress since it was the largest and could fit both requirements.  This would be used again when putting together the CAD model.  Now it was time to move onto feature 2.

## Feature 2

![Feature 2 Knowables](Feature_2_knowables.png)

Same as the first feature, I started with putting my known values down with the target values I planned to solve for.  Barring a few dimensions related to piecing the features together, the values are mostly the same as the first feature and would reflect a similar technical analysis.  

![Feature 2 FBD](Feature_2_fbd.png)

The FBD for this feature represents the piece that is fixed to wall A.  It wasn't as useful for the following calculations as the first FBD because the dimensions that I would be using involved all the pieces together.  A more accurate representation would've included more detail related to the first feature and the combined length that would be necessary for the moment of the second feature.

![Feature 2 work](Feature_2_work.png)

All values that were solved for were found symbolically first, then found numerically by plugging values from the knowns list.  Just like the first feature, two required thicknesses were acquired via the deflection and yield stress, then compared to find the governing thickness for the model.  Again, the thickness required for the yield stress proved to be the larger value and was selected as the governing thickness of feature 2.

## Sketch

![Sketch](A4_sketch.png)

Using the values collected from the first two features and a rough idea of the bolts garnered from the details on the motor webpage, I put together a sketch that would be a rough draft for the CAD model.  I was not certain where the hole dimensions would go, I decided I would figure it out once I had pieced together the two features.  For the sketch, I drew it as an isometric sketch, but I ended up portraying it at the wrong angle.  However it was still close enough for me to be confident moving into the final stages.

## CAD Model (Parametric)

![A4 Equations](A4_equations.png)

The first thing I did in CAD was put all of the given and chosen values into the parametric equations so that they could be referenced for the dimensions of the features.  Not all of these would be needed, but were placed in here regardless so CAD had all information available should it be needed.  The biggest issue I ran into here was the "Evaluates to" column using English units rather than the millimeters I wanted, so I had to take a break from SolidWorks to search for how to swap the base units.

![Feature 1](Feature_1.png)

![Feature 2](Feature_2.png)

Starting with the first feature, I sketched out the model and extruded it using the dimensions from the parametric equations.  This was the quickest part of the assignment but I found a way to extend the process through an incomplete understanding of SolidWorks and how to manipulate features compared to Creo Parametric.

![A4 Bolts 1](A4_bolts1.png)

![A4 Bolts 2](A4_bolts2.png)

![A4 Ribs](A4_ribs.png)

![CAD Model](A4_CAD.png)

[A4.SLDPRT](A4.SLDPRT)

## Communicate

This assignment took 7-8 hours to accomplish.
