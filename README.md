# Rigid Body Simulation System

## Introduction
That is my first small task about simulation based on physics.

In this case, we can see a Stanford bunny hitting the wall or floor angrily and being bounced off.

The task is based on Unity.

## Rigid Body Dynamics
First, we update the linear velocities V and angular velocities ω by multiplying damping coefficients.

After that, we deal with the collision between the bunny and the boundry like wall or floor.

Finally, we update the linear state X by explicit integral and rotation state by quaternion

## Collision Handle
we can use signed distance function to detect every vertices if their function values are negative, which means the bunny has collided with the boundary. 

To deal with the collision, we can impose impulse to the linear velocity of the entire bunny and update the angular velocity. 

## Interaction
Users can press 'r' to initialize the bunny and press 'l' to launch it. 

## Shape Marching
In this section, we use shape marching to finish the dynamics. 

First，all vertices move freely.

After that, we adjust the position of all vertices by rigid body constraints.

## Effects
<img width="404" alt="image" src="https://user-images.githubusercontent.com/53171201/209612932-81ec94da-e0c5-40d0-9da5-a9d022222be0.png">
<img width="274" alt="image" src="https://user-images.githubusercontent.com/53171201/209613043-a22dcbd7-fa78-4f32-973f-74ab7b12cf05.png">
