# Desert of the Real Notes
*[Syllabus](https://github.com/igaln/DesertOfTheReal)*

## Class 1
* Second Life
* by midterm will pitch a VR project

* Experience Design
* UX Design
* On~/Off~ Boarding
* Visit new Microsoft Volumetric lab
* VR as a production tool

* Social VR: to put 2-3 people in VR
* origami crane as a symbol of peace in the hiroshima vr experience
* [Virtually Dating](https://www.facebook.com/VirtuallyDating/videos/1323818351059949/)
* Mirror is a key point where the user recognizes itself
* Edge computing
* [Social VR Examples](https://www.youtube.com/user/EVENTLabBarcelona/videos)


* Recommended Unity V: 2018.3.14

* [Sachka Unseld](http://www.saschkaunseld.com/)
* [Jaron Lanier](http://www.jaronlanier.com/)
* [Sara Ludy](https://www.artsy.net/artist/sara-ludy)
* [Char Davies](http://www.immersence.com/)

## Class 2
* If I declare a variable or a method in a parent class and then create a new class that inherits that one, vars and functions don't have to be re-declared
* mesh renderer takes a mesh filter that takes a mesh

**Mesh Filter (Mesh) -> Mesh Renderer (Material) -> Shader -> Camera**

* Rigid body es la cumbia
* Rigidbody adds physics to the gameobject. it adds gravity unless kinematics is desabled
* Collider adds spatial presence to the element

## Class 3: Transform
* 30 hrs VRChat
* `Vector3` for 3D and `Vector2` for 2D
* You can decalre a vector3 to start with certain direction
```
public Vector3 direction;

Start(){
    direction = Vector3.forward();    //(z = 1)
    direction = Vector3.back();       //(z = -1)
}
```
* Everything in Unity is a GameObject
* GameObject have Transform -> (Position, Rotation, Scale)
* Asset Stoer: cmd + 9
* Collision and triggers
* When making a collision 1 of the bodys has to have physics and one of them has to be the trigger
* `Collider.OnTriggerEnter()` to detect collision
* [VR Template Assignment](https://docs.google.com/document/d/1vV7A1Zz-pEoObyHuzCjF37o9z5xA-rVIphS__lY2IMk/edit?ts=5d815252#)

## Class 4
* `FindObjectOfType` returns the first active object of typet
* A Class name is a Type
* Collections of specific types can be build with `FindObjectOfType`:
 `Bullet[] bullets = FindObjectsOfType<Bullet>();`
* Feedback on VR project:
    * How to create an environment that creates the desire of transmuting in other
    * Empathy process
    * Virtual embodyment
    * Gradual transition
    * Metpamorphosis - Kafka
* Feedback Sarah
    * Think on the conversation (?)
    * same persons can have different experiences
    * design whole UX narrative
    * Both experience from human to non-human but mapping the other's movement
    * Figure out there is another person
    * Add time variable to create the narrative arch
    * Human rigging with final (something)
    * Process
        1. prototype with white box to check how the narrative's flow works
        2. include assets
    * Look for VR narrative social experiences
    * Talk to Carrie and Ellen
    * [Be another Lab](http://beanotherlab.org/home/work/tmtba/body-swap/)
    * [Half + half](https://uploadvr.com/half-half-multiplayer-vr/)
    * [Animate](youtube.com/watch?v=MuUUgxsZ9tk) on [Quill](https://quill.fb.com/)

## Class 5
* Use of Unity Events `UnityEngine.Events`
* UnityEvents.Invoke() sends a message
* When using `Serialized` data can be sent as serial messages (events) through the inspector bay attaching classes that receive it
* When sending, the event is sent using Invoke
* When receiving, there has to be a method in the class that receives the parameter sent
* `FindObjectOfType<Type>()`

## Class 6: UX / Performance
* [Practical VR - A design cheat sheet](https://virtualrealitypop.com/practical-vr-ce80427e8e9d)
* [UX VR Design, Jessica Brillhart](https://www.youtube.com/watch?v=fgzgC7UOOSo)
* 60 fps or more
* Sarah's Feedback
    * things to interact with before the main interaction, like touching other objects durint the wallway during onboarding
    * sometimes is better to just tell people what to do
    * not mess up with the cameras
    * interaction by zones
    * hand tracking integrated in quest?
    * feedback when connecting is very importatn in order to tell players they are doing correct
    * value all cases: i'm looking at the glass and the axoltl, no. what ahppens?
    * prove concept with white boxes in the headset
    * would be interest to know what happen if characters switch and then stay like that. what motivates the user to switch?
    * build alternative interactions to keep the player in the experience.
    * build game flow chart.

## Class 8 
### Inverse kinematics
* To predict how the body elements move
* asset store -> Final IK
* create bridges between IK and the character
### Networking
Cliente <-> Server
* spawning means the server tells all clients to instantiate an object
* new netwotking structure happens in the low level
* `[SyncVar]` variable type is used to sync different vars within the network
* `[Command]` then `Cmd<functionname>` syncs a function
* Local Authority sets that in every machine the Local Player is the only who can move/control the scene in their machine
