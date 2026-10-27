# A7 – [Topic]

## Objective

![Objectives](objectives_A7.png)

![Workflow](workflow_A7.png)

## Preparation

![Bracket Material](Bracket_Material_A7.png)

The first step before beginning this assignment was to assign the material I chose from the previous assignments to my bracket, which in this case was ASTM A36 Steel.  

![Bracket Fixtures](Bracket_Fixtures_A7.png)

Next, I applied the proper fixtures and load to the bracket.  I chose the underside of the upper-bracket as my fixed boundary because it would be the main point of contact when it was positioned correctly with the T-beam.  Then, I applied a downward load of 600 lbf on the bar holding the strap, which was also taken from the previous assignments.  The last step for preparing the bracket for analysis was to apply a mesh.  I chose to create the meshes ahead of time, for coarse and mid, and rerun the studies when I returned to make changes to the original model.  This was just a simple way to speed up the process, however my misunderstanding of the assignment instructions made this step a lot more complicated when I would return to it.

## Test 1

<table>
  <tr>
    <th></th>
    <th>Coarse</th>
    <th>Mid</th>
    <th>Fine</th>
  </tr>

  <!-- MAX STRESS -->
  <tr>
    <td><b>Max Stress and location</b></td>
    <td>
      <img src="Test1_vonmises_coarse_A7.png" width="250"><br>
      1.537 x 10^5 psi<br>
    </td>
    <td>
      <img src="Test2_vonmises_mid.png" width="250"><br>
      1.747 x 10^5 psi<br>
    </td>
    <td>
      <img src="Test1_vonmises_fine.png" width="250"><br>
      4.749 x 10^4 psi<br>
    </td>
  </tr>

  <!-- MAX DEFLECTION -->
  <tr>
    <td><b>Max deflection and location</b></td>
    <td>
      <img src="Test1_deflection_coarse.png" width="250"><br>
      9.244 x 10^-2 in<br>
    </td>
    <td>
      <img src="Test2_deflection_mid.png" width="250"><br>
      9.688 x 10^-2 in<br>
    </td>
    <td>
      <img src="Test1_deflection_fine.png" width="250"><br>
      2.249 x 10^-2 in<br>
    </td>
  </tr>

  <!-- MASS -->
  <tr>
    <td><b>Mass</b></td>
    <td>0.85 lbs</td>
    <td>0.85 lbs</td>
    <td>0.85 lbs</td>
  </tr>

  <!-- SAFETY FACTOR -->
  <tr>
    <td><b>Safety Factor</b></td>
    <td>2.36 x 10^-1</td>
    <td>2.075 x 10^-1</td>
    <td>7.635 x 10^-1</td>
  </tr>

  <!-- NUMBER OF ELEMENTS -->
  <tr>
    <td><b>Number of elements</b></td>
    <td>1746</td>
    <td>9944</td>
    <td>65166</td>
  </tr>
</table>

Applying the formula for convergence to stress, deflection, and FOS, only deflection sat below the limit of 7%.  This meant that I needed to create a third study for the fine mesh, which I would accomplish at a later point.  Returning to check for convergence a second time, my numbers for the fine mesh are a lot farther away, indicating an issue occurred somewhere along the way.  For now, after the three tests there remains to be any convergence.

## Test 2

Following the first study, I returned to the original model to make a design change that might improve the chance of convergence happening.  I decided to triple the already delicate thickness of the side walls of the bracket, increasing them to about 0.12 inches.  Afterwards, I reopened each of the studies and ran them a second time so that the changes were now incorporated into the FEA.  I then collected the numbers again and filled out the table below.

<table>
  <tr>
    <th></th>
    <th>Coarse</th>
    <th>Mid</th>
    <th>Fine</th>
  </tr>

  <!-- MAX STRESS -->
  <tr>
    <td><b>Max Stress and location</b></td>
    <td>
      <img src="Test3_vonmises_coarse.png" width="250"><br>
      1.533 x 10^5 psi<br>
    </td>
    <td>
      <img src="Test4_vonmises_mid.png" width="250"><br>
      1.705 x 10^5 psi<br>
    </td>
    <td>
      <img src="2_vonmises_fine.png" width="250"><br>
      4.817 x 10^4 psi<br>
    </td>
  </tr>

  <!-- MAX DEFLECTION -->
  <tr>
    <td><b>Max deflection and location</b></td>
    <td>
      <img src="Test3_deflection_coarse.png" width="250"><br>
      9.215 x 10^-2 in<br>
    </td>
    <td>
      <img src="Test4_deflection_mid.png" width="250"><br>
      9.691 x 10^-2 in<br>
    </td>
    <td>
      <img src="2_deflection_fine.png" width="250"><br>
      2.247 x 10^-2 in<br>
    </td>
  </tr>

  <!-- MASS -->
  <tr>
    <td><b>Mass</b></td>
    <td>0.98 lbs</td>
    <td>0.98 lbs</td>
    <td>0.98 lbs</td>
  </tr>

  <!-- SAFETY FACTOR -->
  <tr>
    <td><b>Safety Factor</b></td>
    <td>2.365 x 10^-1</td>
    <td>2.127 x 10^-1</td>
    <td>7.528 x 10^-1</td>
  </tr>

  <!-- NUMBER OF ELEMENTS -->
  <tr>
    <td><b>Number of elements</b></td>
    <td>1716</td>
    <td>10178</td>
    <td>72109</td>
  </tr>
</table>

## Test 3

![Addition](Bracket_addition_A7.png)



<table>
  <tr>
    <th></th>
    <th>Coarse</th>
    <th>Mid</th>
    <th>Fine</th>
  </tr>

  <!-- MAX STRESS -->
  <tr>
    <td><b>Max Stress and location</b></td>
    <td>
      <img src="Test5_vonmises_coarse.png" width="250"><br>
      1.405 x 10^4 psi<br>
    </td>
    <td>
      <img src="Test6_vonmises_mid.png" width="250"><br>
      1.854 x 10^4 psi<br>
    </td>
    <td>
      <img src="3_vonmises_fine.png" width="250"><br>
      5.988 x 10^3 psi<br>
    </td>
  </tr>

  <!-- MAX DEFLECTION -->
  <tr>
    <td><b>Max deflection and location</b></td>
    <td>
      <img src="Test5_deflection_coarse.png" width="250"><br>
      1.169 x 10^-3 in<br>
    </td>
    <td>
      <img src="Test6_deflection_mid.png" width="250"><br>
      1.23 x 10^-3 in<br>
    </td>
    <td>
      <img src="3_deflection_fine.png" width="250"><br>
      2.837 x 10^-4 in<br>
    </td>
  </tr>

  <!-- MASS -->
  <tr>
    <td><b>Mass</b></td>
    <td>1.00 lbs</td>
    <td>1.00 lbs</td>
    <td>1.00 lbs</td>
  </tr>

  <!-- SAFETY FACTOR -->
  <tr>
    <td><b>Safety Factor</b></td>
    <td>2.58</td>
    <td>1.955</td>
    <td>6.056</td>
  </tr>

  <!-- NUMBER OF ELEMENTS -->
  <tr>
    <td><b>Number of elements</b></td>
    <td>1798</td>
    <td>10323</td>
    <td>74765</td>
  </tr>
</table>

## Reflection




