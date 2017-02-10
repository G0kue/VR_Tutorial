New Unity project

Delete the Camera in the scene

Make new plane

Asset Store search (SteamVR) may aswell download and import (Ball Pack) at this stage too

Install and say accept all

SteamVR folder > Prefabs > Camera Rig

Drag and drop camera Rig into scene (Can position how ever you like), Blue border is essentially the room scale roughlt 2m * 1.5m

On Hierachy expand [CameraRig], this is the individual parts of the Vive.

Click on either hand and create either a 3D object or drag in a model making sure its a child of the Controller and not Model. (You can disable the Model at this point)

Add a Rigid Body to the Object making sure to set anguluar drag to 0, No gravity and is Kinematic

Make prefabs of balls from ball pack - Making sure they have Rigid bodys and Colliders attached - set collision detection to continuous.

Make new empty game object rename it something like (Spawner)- Place it somewhere where the player will be able to hit the spawned objects

Make a new script and copy mine onto it making sure to name it (Spawner)

Drag script onto the Spawner gameobject

Set the Objects size to how many prefabs you want to spawn

Drag and drop prefabs into the script 

Create a new physics Material set it to (0,0,1) with bounce combine set to maximum

Can dupilcate the Spawner and place it all around the player if you want.

if you want the balls to destory themselves you can make a script and attach it to the prefabs name it something like detroy create and set a new public float named life to 5 (This will be the seconds)
and in the make a new method called destory objects Destroy (gameObject, life); - this will detroy the balls after 5 seconds of being spawned.





 
