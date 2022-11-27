# GAMES103-HW1

## Introduction
That is my first small task about simulation based on physics.

## Rigid Body Dynamics
First, we update the linear velocities V and angular velocities ω by multiplying damping coefficients.

After that, we deal with the collision between the bunny and the boundry like wall or floor.

Finally, we update the linear status X by explicit integral and rotation by quaternion

## Collision Handle
we can use signed distance function to detect every vertices if their function values are negative, which means the bunny has collided with the boundry. 

To deal with the collision, we can impose impulse to the linear velocity of the entire bunny and update the angular velocity. 

## Interaction
Users can press 'r' to initialize the bunny and press 'l' to launch it. 
