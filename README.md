# FieldOfView
A simple Field of View system for the Unity Engine with target detection and obstacle blocking

# How To Use
- Import both scripts into your project

- Ensure FieldOfViewEditor is inside of the Editor folder inside of Unity or else your build will fail to compile!

- Set up two new Layers, one for your Target objects and one for your Obstacle objects

![New Layers](https://i.imgur.com/4H19Eg4.png)

- Set your player (target) to be on the Target layer

- Set any obstacles that block the enemies field of view to be on the Obstacle layer

![Field Of View Inspector](https://i.imgur.com/PW20aYg.png)

- Attach the FieldOfView script to your Enemy

- Configure the view radius and angle properties to your liking

![Field Of View Inspector](https://i.imgur.com/q0Ovpzw.png)

- Set the target layer mask to be your Target layer

- Set the obscruction layer mask to be your Obstacle layer


## FAQ

**Why isnt my raycast detecting the player / obstacles?**  
Check your objects have colliders, Raycasts need to hit colliders to work  
Check your objects are assigned to the correct layers  
Check your FieldOfView script is looking at the right layers in the inspector

**Why is my build failing with these scripts?**  
FieldOfViewEditor needs to be inside a folder called Editor
