# OpenArm 2.0 Take-Home Submission

## Tasks Completed
- Task 1: Industrial design concept 
- Task 2: Exterior CAD model
- Task 3: Camera & cable integration 
- Task 4: Mobile base + manipulator integration
- Task 5: Manufacturability & materials

---

## Task 1: Industrial Design Concept

**Concept A — Modern, Sleek, and Commercial (Chosen Direction)**  
 
![Concept A](images/concepta.png)

**Concept B — Industrial and Functional**  

![Concept B](images/conceptb.jpg)

*Note: The ZED stereo head is supposed to be at the top and center of the robot, not at the left shoulder of the robot. These details were generated incorrectly in the image.*

**Rationale for Concept A:**  
I chose Concept A as the direction to carry forward. Because the arm is used for teleoperation research, a friendly, approachable look makes it less intimidating for users. I believe this is critical considering the frequency of human-robot interaction. While Concept B would be better given time or resource constraints, Concept A brings the robot closer to being a credible product. The smooth surfaces also align well with 3D printing and sheet metal manufacturing in a small-shop context.

---

## Task 2: Exterior CAD Model

**CAD Model:**  

![Cad Model](images/cadss.png)

**Explanation:**  
I built my exterior shell in Onshape by working on top of the provided OpenArm 2.0 STEP file sourced from docs.openarm.dev. I imported the robot's internal structure as a reference, then created a separate Part Studio for my shell so I wouldn't accidentally modify the mechanics.

Instead of modeling the whole arm, I focused on the main body and head housing. I used the Loft tool to create the main pillar section from the front plane that wrapped the base bracket to the smaller rounded shape near the shoulder. I made sure the shell had clearance around the internal parts. As a rough guide, I added about 20mm of space around larger components and 5-10mm around smaller sections. These were my main assumptions, since I don't have exact internal dimensions.

For the head housing, I extruded a block forward from the top of the pillar, matching the depth of the ZED camera bracket. I rounded the edges with a fillet and cut out a window for the camera lenses so they wouldn't be blocked.

To make the design more polished and serviceable, I planned ventilation slots on the arm using a linear pattern to help with heat dissipation. I also planned for a panel split line, though I simplified both in this version. While I didn't model the hollow interior for cable routing, I kept it in mind as a functional requirement. I colored the exterior shell white to match my Concept A design direction, giving the arm a cleaner, more approachable look.

Although this is a simplified version where I didn't model every surface, I focused on showing the key ideas: wrapping the internal structure, leaving room for components, and creating a design that could be manufactured in a small shop. With more time and experience, I'd refine the surfaces and add more detailed panel splits.

**File:** 
https://cad.onshape.com/documents/2bc80f60b1c6dd7224b3004b/w/d4c8081ecb45f7441266ba00/e/a1c2a0642ac821b66e6316ae?renderMode=0&uiState=6a3236a4654e2233d116c505

*Note: My STEP file was too big for GITHUB, therefore, I was unable to upload it. I shared a link through OnShape instead.*

---

## Task 3: Camera & Cable Integration

**Explanation:**  
The OpenArm 2.0 has four cameras: two wrist Arducams (left/right), one ceiling Arducam (top of robot), and one ZED stereo head (front of the robot at the top). All cables are routed internally through the hollow shell. A service loop is included at the elbow joint to allow rotation without pinching. Heat dissipation is managed through passive vents.

---

## Task 4: Mobile Base + Manipulator Integration

**Sketches:**  
![Task 4](images/task4img.png)

*Note: The batteries are supposed to lie in the mobile base of the robot, not in the central support beam. The wiring runs through the central support beam instead. These details were generated incorrectly in the image.*
 
**Explanation:**  
For the mobile base, I thought about a simple, low-profile cart that could support the arm while keeping it stable. I took some inspiration from a Roomba for the base to give it a clean, polished look. The arm would mount to a flat, rigid plate on top of the base. The plate would have holes drilled to match the arm's existing mounting bolt pattern so that the arm could be securely screwed to it. The plate itself would then be bolted to the base frame underneath to keep the arm rigid and stable during movement. The base itself would have four wheels, with two powered wheels positioned to align with the center of gravity to ensure good control. The wheels are placed near the outer corners to maximize stability. In order to ensure stability and avoid the robot tipping over, the batteries and compute hardware are placed as low as possible in the base. This is done to lower the overall center of gravity. The arm is mounted slightly toward the rear of the base so that when the arm extends forward, the combined center of gravity remains well within the base, preventing the robot from tipping over.

---

## Task 5: Manufacturability & Materials

**Explanation:**  
Given the small-shop, light-assembly context, I would use 3D-printed parts and off-the-shelf sheet metal. The outer shell could be 3D-printed using PETG or ABS since these are common materials known for being strong and affordable. For structural parts like the mounting plate, I would use aluminum sheet metal since it's lightweight and rigid. I would use screws rather than snap-fits to hold everything together, since screws make service and replacement easier. For metal parts, I would outsource laser cutting while doing all the 3D-printing in the shop.

---

## What I Would Do Next
With more time or hardware access, I would:
1. Practice/build on my CAD skills so that I can make a more detailed CAD.
2. Refine the CAD surfaces to better match Concept A.
3. 3D print a prototype section to test.
4. Conduct a tip-over test with the mobile base prototype.

---

## Notes
- AI-generated images are labeled as such and used only for concept visualization.
- All written explanations and the CAD model are my own work.
- I made simplifying assumptions about internal dimensions and focused on demonstrating the design thinking process.
- I focused on completing all non-CAD tasks fully and modeling a representative arm housing section in Onshape. I would love to learn more and build on my skills at the internship.
