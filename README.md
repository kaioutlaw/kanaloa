# kanaloa

# Background:
Previously, the front thrusters were mounted on an aluminum bar that overhung inwards off of the side of the pontoons . This worked as a mounting solution until we discovered that the torque created by the weight of the thruster were causing torsion on the pontoons. To prevent further damage, a new mounting solution had to be created. The solution is to mount the thrusters in front of the pontoon by having aluminum bars extending out from each side of the pontoon past the end so that two cross bars can be attached and the thruster can be mounted there.

# Analysis 
Having aluminum bars extend out far in front and having a load applied causes significant amount of moment. To be sure that the bolts used , 1/4 - 20 in this case, can withstand the load, we must calculate the Maximum shear stress at the bolts and compare that to the max clamping load of the bolt. If the max clamping load is greater than the max shear force, the bolts are sufficient. 

# Max moment created by forward thrust

1) Assuming that the thruster shaft is 2ft below the mount, and the thruster is providing 110[lb] thrust, we can calculate the moment to
   be M = F*D = 110[lb]*2[ft] = 220 [lb*ft]. 

2) Now if we assume that the moment is to be distributed throughout all of the bolts equally, and there are 12 bolts total on the   
   aluminum    mounts, we see that the moment at each bolt to be M(bolt) = M(total)/(Number of bolts) = 220[lb]/12 = 18.33[lb*f].

3) Now to find the shear force at each bolt, we need to find the moment arm. The moment arm is located at the midpoint between the 
   first and the last bolt. The bolts are equally spaced by 6in and there are 6 on each aluminum rod, hence the bolts span a length of
   30in and the midpoint is at 15in from either end bolt.
  
4) To find the shear force at each bolt, V = M/d can be used. Where V is the shear force, M is the M(bolt) and d is the distance of the
   bolt from the moment arm. We can see that the shear force will be greatest at the bolt closest to the moment arm. The distance of the
   bolt closest to the moment arm is 3in, or 0.25ft. The maximum shear force is then, V(max) = M/d = 18.33[lb*ft]/0.25ft = 73.33 [lb]

5) Now we are able to see whether the bolts will fail under these conditions. Now a common misconception is that by calculating shear
   stress and comparing the solution to then the rated maximum shear strength of the bolt, we can see if it fails or now. The problem
   with this is that bolts are not rated for shear strength but for tensile strength. Also, in actuality, the shear stress is not what
   determines if a bolt will fail or not.

6) What keeps two plates together is not the bolts shear strength, but the bolts ability to clamp the two materials together,
   compressing it, and thus a causing large frictional force between those two plates. This is rated and can be looked up as Maximum
   Clamping Load for a specific bolt. 

7) In our cause, for the 1/4-20 bolt, the maximum clamping load is 2020[lb]. The frictional coefficient (mu) for Aluminum on Aluminum is
   1.05. Thus the frictional force can be calculated as Ff = (mu)*N where Ff is the frictional force, mu is the frictional coefficient 
   anf the N is the normal force. Ff = 2020*1.05 = 2121 [lb]

8) We see that the frictional force is approximately 29x larger than the Max shear force, so we can conclude that the mounts will not
   break off of the pontoons under these conditions. 

# Max moment created by Reverse thrust and Weight of the thruster

Follow the same concept as previous calculation. 

1) In the previous calculations, we neglected the weight of the thruster because the moment caused by the weight of the thruster will 
   actually counteract the moment caused by forward thrust, and we wanted to calculate the worst cause senario. 

2) In contrast, when the thrusters are going in reverse, the moment caused by the weight of the thrusters will supplement the moment  
   created by the reverse thrust, so we want to take the weight into consideration in this calculation.

3) The weight of the thruster is 55lb. The distance from the mount to the first bolt is 5.4ft. The moment created by the weight can be
   calculated by M(weight) = w*d = 55[lb]*5.4[ft] =297[lb*ft].

4) The reverse power of the thruster is rated at 70%. We assume that the thruster shaft is 2ft below the mounts. So the moment created
   by full reverse can be calculated by M(thrust) = f*d = 110[lb]*0.70*2[ft] = 154[lb*ft]

5) The total moment is then M(total) = M(weight) + M(thrust) = 297 + 154 = 451 [lb*ft]

6) Now the moment distributed to each bolt is M(bolt) = M(total)/(number of bolts) = 451/12 = 37.6[lb*ft]

7) The maximum shear force is then V(max) = M(bolt)/d, where d is the distance from the moment arm to the closest bolt.
   V(max) = 37.6/0.25 = 150[lb]

8) The maximum clamping load is 14x greater than the maximum shear force, so it is safe to say that under these conditions, the mounts 
   will not break off. 

# additional info

Two crossbars were also added to ensure safety. We attached this directly to the ski of the pontoon. The bolts on the crossbars will bear a load, but instead of shear force, these bolts will have tensile force acting on them. This is a good design choice because bolts are alot stronger in tensile than in shear.


