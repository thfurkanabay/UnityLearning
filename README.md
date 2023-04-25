# Unity Learning Pathway
This project is where I write what I learned for unity and develop on it <br/>
[Syntax Rules](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

**Project naming**
- use lowercase
- use dashes
- be specific. you may find you have to differentiate between similar ideas later - ie use purchase-rest-service instead of service or rest-service.
- be consistent. consider usage from the various GIT vendors - how do you want your repositories to be sorted/grouped?
[Source](https://stackoverflow.com/questions/11947587/is-there-a-naming-convention-for-git-repositories)
## Pipeline

## Methods

**Private and Public Medhods**
- Private method,  dışarıdan erişilir
- Public method dışarıdan erişimez
- [HideInInspector] public yapsan da arayüzde gözükmez
- [SerializeField] private olsa da arayüzde gözükür
Ayni zamanda; 
- public ==> read and write
- [SerializeField] private ==> read only


- Update Method : checking constantly, called every single frame
- transform.translate: move via x,y,z coordinate
- Vector3: represent 3d point
- transform.translate(Vector3.forward * Time.deltaTime * Speed)
- Late update
Rigidbody
Colliders
GameObject
horizantalInput= Input.GetAxis("Horizantal"); /horizantal ayzıyoruz çünkü ıNput managerin içindeki ismi bu aynı zmanada aslındaa Input manager fornksiyounu çağırmış ve çalıştırmı oluyoruz.
* Input
- KeyCode: 


- Instantiate() : Create a copy its already exist ..... 

- verticalInput

https://miro.medium.com/v2/resize:fit:572/format:webp/1*7IR7CcCFXWUo1n192Pby4A.png![image](https://user-images.githubusercontent.com/26336737/218953365-7faeacd2-e35f-4c6d-9253-0373831444d8.png)

**Unit-1**
- New Functionality
- Vehicle moves down the road at a constant speed
- When the vehicle collides with obstacles, they fly into the air
- New Concepts & Skills
- C# Scripts
- Start vs Update
- Comments
- Methods
- Pass parameters
- Time.deltaTime
- Multiply (*) operator
- When the player presses the up/down arrows, the vehicle will move forward and backward
- When the player presses the left/right arrows, the vehicle turns 
- New Concepts & Skills
- Empty objects 
- Get user input
- Translate vs Rotate
- The player can move left and right based on the user’s left and right key presses
- The player will not be able to leave the play area on either side
- New Concepts & Skills
- Adjust object scale
- If-statements
- Greater/Less than operators

Components
Collider and RigidBody

![image](https://user-images.githubusercontent.com/26336737/218960067-d2a8694b-0572-4bc8-8e85-752804c566a6.png) </br>

## Name Convension

[Naming Convension Source](https://github.com/justinwasilenko/Unity-Style-Guide#scene-structure)

All Public Functions Should Have A Summary

/// <summary>
/// Fire a gun
/// </summary>
public void Fire()
{
// Fire the gun.
}
## My Setups
**Scene Layout Setup**
- Layout olarak sol üstte scene sol altta game view sağ tarafta hierarcy altında project onun sağğında inspector


## PlayerControl
- Kullanıcıdan bazı **Inputlar** alınacak ve **Action** lara dönüştürülecek
 

## Tips and Tricks
Kamerayi playera sabitle, offset ver oyun nereden takip edilcekse onu gameobjet olsrak ata.

## Sources
- [private and public methods](https://stackoverflow.com/questions/52906797/when-should-i-use-public-private-or-serializefield-unity-c-sharp)
- https://www.researchgate.net/publication/323179176_Game_Engine_Solutions
- 

## To be learn 
- Gamemanager e ne konur? 
- [Extern nedir?](https://gelecegiyazanlar.turkcell.com.tr/konu/egitim/objective-c-ile-ios-201/extern-bellek-sinifi)
- https://learn.unity.com/tutorial/the-real-time-production-cycle#
-  Invoke() [ Link ](https://www.youtube.com/watch?v=_cmlXcCd6WI),Invoke(nameof(CompleteLevel), 5f); << use with nameof
-  name of ?
-  InvokeRepeating() ?
## Extra works
- [ ] https://learn.unity.com/tutorial/bonus-features-1-share-your-work# Checklist 

## Unity Graphics
### Render
- [Render Pipeline from unity manual](https://docs.unity3d.com/Manual/BestPracticeLightingPipelines.html)
### Shaders
- A program that runs on the GPU.
- [Sources Unity Manual](https://docs.unity3d.com/Manual/Shaders.html)

## PlayerPrefs
- **Description:** PlayerPrefs is a class that stores Player preferences between game sessions. It can store string, float and integer values into the user’s platform registry.

## 1 March 2023 Notes

- Destroy(): 
- Destroy(gameObject):
- New Functionality
- The player can press the Spacebar to launch a projectile prefab,
- Projectile and Animals are removed from the scene if they leave the screen
- New Concepts & Skills
- Create Prefabs
- Override Prefabs
- Test for Key presses
- Instantiate objects
- Destroy objects 
- Else-if statements
- Random.Range():
- SpawnManager
- New Functionality
- The player can press the S to spawn an animal
- Animal selection and spawn location are randomized
- Camera projection (perspective/orthographic) selected
- New Concepts & Skills
- Spawn Manager
- Arrays
- Keycodes
- Random generation
- Local vs Global variables
- Perspective vs Isometric projections
- New Functionality
- Animals spawn on a timed interval and walk down the screen 
- When animals get past the player, it triggers a “Game Over” message
- If a projectile collides with an animal, both objects are removed
- New Concepts & Skills
- Create custom methods/functions
- InvokeRepeating() to repeat code
- Colliders and Triggers 
- Override functions
- Log Debug messages to console

- New progress
- New project for your Personal Project
- Camera positioned and rotated based on project type
- All key objects in scene with unique materials
- New concepts & skills: 
- Primitives
- Create new materials
- Export Unity packages
- 3.1
- New Functionality
- Player jumps on spacebar press
- Player cannot double-jump
- Obstacles and Background move left
- Obstacles spawn on intervals
- Key Concepts and Skills
- GetComponent
- ForceMode.Impulse
- Physics.Gravity
- Rigidbody constraints
- Rigidbody variables
- Booleans
- Multiply/Assign (“*) Operator
- And (&&) Operator
- OnCollisionEnter()

**Çıkardıkalrım**
- objede ulaşmak istediğimize getcomponentle ulaşıcaz
- rigidbody add force ile force verip force mod ile force tipini seçebilriiz.
- rigidbody contraint ile ozisyon ve roation dondurabiliriz.
- oyuncu ilerletmektense diğerlerine moveleft giib bir fonksiyon yazılabilri.
- Physics.Gravity ile yerçekimine etki edebiliriz
- oncolliedipom enter iele örneğin yere değdi mi değmedi mi bunu kontrol edebiriz.
- 

- 3.2
- Background repeats seamlessly
- Background stops when player collides with obstacle
- Obstacle spawning stops when player collides with obstacle
- Obstacles are destroyed off-screen
- New Concepts and Skills:
- Repeat background
- Get Collider width
- Script communication
- Equal to (==) operator
- Tags
- CompareTag(
**Çıkardıkalrım**
- Eğer sonsux yapcaksak box collider uzunluğunun yarısından itibaren detect edip positionunun startpos yapararız.
- oyun bitimini collide olunca yapabiliriz.
- oyun bitince obstacle spawnlamayı durdurmalıyız.
- campoare tag ile istediğimiz obje türünü yokedebiriiz.
- script comm. için scripti bir obje oluştrup hierarcydeki ilgili objeden getcomponen tile scripti çekip işlem yapabiliriz bunun için kullancamız değerler public olmalı.


- 3.3
- The player starts the scene with a fast-paced running animation
- When the player jumps, there is a jumping animation
- When the player crashes, the player falls over
- New Concepts and Skills:
- Animation Controllers
- Animation States, Layers, and Transitions
- Animation parameters
- Animation programming
- SetTrigger(), SetBool()
- Not (!) operator

**Çıkardıkalrım**
- animasyonar arı geçiş yapmak trigger vs layer ve parameterlarla kontrol ediklir.
- aimatorü tantııoryz ardından özelliklerile oynuyoruzç
- not operator ==false gbi çalışır.

- 3.4
- Music plays during the game
- Particle effects at the player’s feet when they run
- Sound effects and explosion when the player hits an obstacle
- New Concepts and Skills:
- Particle systems 
- Child object positioning
- Audio clips and Audio sources 
- Play and stop sound effects

**Çıkardıkalrım**
- script çağırımları start ta yapılır.
- Ears-> listerner, speakers -> audiosource davranışı yapar
- audio soruce çağıırrp playoneshot gibi fonksiyonkar kullanılabilir.
- ana müzik direkt main kameraya eklenebilir.


- 4.1
- Camera rotates around the island based on horizontal input
- Player rolls in direction of camera based on vertical input
- New Concepts and Skills:
- Texture Wraps
- Camera as child object
- Global vs Local coordinates
- Get direction of other object

- 4.2 
- Enemy spawns at random location on the island
- Enemy follows the player around 
- Spheres bounce off of each other 
- New Concepts and Skills:
- Physics Materials
- Defining vectors in 3D space
- Normalizing values !!
- Methods with return values
**Çıkardıkalrım**
- eğer bir değer dömdürceksek void değil döndürülen tipte metod yaz retuen yaz. ve fnsiyonu çağır.

- 4.3 

- When the player collects a powerup, a visual indicator appears
- When the player collides with an enemy while they have the powerup, the enemy goes flying
- After a certain amount of time, the powerup ability and indicator disappear
- New Concepts and Skills:
- Debug concatenation
- Local component variables 
- IEnumerators and WaitForSeconds()
- Coroutines
- SetActive(true/false) 
**Çıkardıkalrım**
- eğer power up yapcaksan ıenumaratorla power up çöelliğinin gitmesini kopntrol edebilrisin.

- 4.4
-  Enemies spawn in waves
- The number of enemies spawned increases after every wave is defeated
- A new power up spawns with every wave
- New Concepts and Skills:
- For-loops
- Increment (++) operator
- Custom methods with parameters
- FindObjectsOfType
 **Çıkardıkalrım**
- wave oluştrmak için for loop kullanabilrisin
- parametreli metohdlar


- 5.1
- Random objects are tossed into the air on intervals
- Objects are given random speed, position, and torque
- If you click on an object, it is destroyed
- New Concepts and Skills: 
- 2D View
- AddTorque 
- Game Manager
- Lists
- While Loops
- Mouse Events

- 5.2 
- There is a UI element for score on the screen
- The player’s score is tracked and displayed by the score text when hit a target
- There are particle explosions when the player gets an object
- New Concepts and Skills:
- TextMeshPro 
- Canvas
- Anchor Points
- Import Libraries
- Custom methods with parameters
- Calling methods from other scripts

 **Çıkardıkalrım**
- bir koda tek bir değer verip prefablerde farklılaştırlabilir.
- Custom methods with parameters- işimize score güncellerken falan diğer yerlerde kullanabilirz değeri döndüen fonsiyon olarrak kullanarka.

- 5.3 
- 
 **Çıkardıkalrım**
- start corputine bilgi gerekiyorsa bu bilgiyi fonsksiyondan önce bilmeliyiz.
- A functional Game Over screen with a Restart button
- When the Restart button is clicked, the game resets
- New Concepts and Skills: 
- Game states 
- Buttons
- On Click events
- Scene management Library
- UI Library
- Booleans to control game states

- 5.4
- Title screen that lets the user start the game
- Difficulty selection that affects spawn rate
- New Concepts and Skills:
- AddListener() 
- Passing parameters between scripts
- Divide/Assign (/=) operator
- Grouping child objects

**The user testing process typically follows this high level structure:**
- Define the objectives.
- Plan the session. 
- Facilitate the session.
- Evaluate the results


- Optimization
- Serialized Fields
- readonly / const / static / protected 
- Event Functions
- FixedUpdate() vs. Update() vs. LateUpdate()
- Awake() vs. Start()
- Object Pooling

- Searching on Unity Answers, Forum, Scripting API
- Troubleshooting to resolve bugs
- AddRelativeForce, Center of Mass, RoundToInt
- Modulus/Remainder (%) operator
- Looping through lists
- Custom methods with bool retu


- Data persistence
- DontDestroyOnLoad()
- public static MainManager Instance;
- This is the static class member declaration. Note the keyword static after the keyword public. This keyword means that the values stored in this class member will be shared by all the instances of that class. 
For example, if there were ten instances of MainManager in your scene, they would all share the same value stored in Instance. If any of those 10 MainManagers changed the value in it, it would also be changed for the other nine.
- Singleton
- This pattern is called a singleton. You use it to ensure that only a single instance of the MainManager can ever exist, so it acts as a central point of access.
- How can data persist between sessions?
https://connect-prd-cdn.unity.com/20210602/learn/images/197dfde6-d842-4bce-bffa-a0fab3140687_0.jpg.1600x0x1.jpg![image](https://user-images.githubusercontent.com/26336737/224675095-11363c96-4355-42ed-9e1d-3340118ba4f9.png)
- 2.What is Abstraction?
- The first pillar of OOP is all about keeping your code clean and simple for the programmer using it, whether that is you or someone else. Abstraction is the process of removing complex code from the scripts where other programmers will see it, and only exposing the functionality other programmers really need. When you “abstract out” the details, you reduce duplicate code and provide easy access to the most useful functions. You’re actually already quite familiar with this pillar, because you’ve benefited from it frequently throughout this pathway. Whenever you call on a method to perform a task rather than writing out all of the code by hand, you’re benefiting from abstraction! 
```
private void Start()
{
    for (int i = 0; i < 3; i++)
    {
        Instantiate(enemyPrefab, GenerateSpawnPosition(),   
        enemyPrefab.transform.rotation);
    }
}
```
yerine
```
void SpawnEnemyWave() // create new higher-level method 
{
    for (int i = 0; i < 3; i++)
    {
        Instantiate(enemyPrefab, GenerateSpawnPosition(), 
        enemyPrefab.transform.rotation);
    }
}

private void Start()
{
    SpawnEnemyWave(); // call higher-level method in Start()
}
```

- Inheritance is the process of creating a primary class (also known as a parent class) from which other classes (called child classes) can be created. A child class takes on, or inherits, all of the features of the parent class automatically. It’s common to have different classes share similar features in an application. For example, a video game may feature many different types of enemy classes, but they are likely to share the same core features, such as managing their own health and the ability to deal damage to the player. With inheritance, the need to write that health and damage functionality for each individual enemy class is eliminated, so that you can focus on writing functionality that’s unique to each class. 
Flow chart showing the relationship between parent classes and child classes. Enemy class is at the top of the diagram with arrows pointing downward to three child classes: Thief class, Scoundrel class, and Self-identifying ‘bad guy’ class. Both parent and child classes have the shared behaviors of “deal damage” and “reduce health”, but each child class also has a unique behavior not shared by the parent or the other child classes
https://connect-prd-cdn.unity.com/20210530/learn/images/2d1b6807-43a2-4fa6-9d6b-99ee50c8ff9f_93.png.2000x0x1.png![image](https://user-images.githubusercontent.com/26336737/224711260-be49cd3f-ccdc-48e5-ba57-7149c9a30e33.png)

You’ve already been making use of inheritance with every script you’ve written in Unity so far. By default, whenever you create a new class, it inherits from MonoBehaviour: 
public class SomeClass : MonoBehaviour { }
MonoBehaviour is the base class from which all core Unity scripting functionality inherits. Without MonoBehaviour, you wouldn’t be able to call OnTriggerEnter, GetComponent, or even use Start or Update! 
In the diagram above, it might appear that all of the child enemy classes would lose their ability to access Unity functionality, because they exchanged their inheriting class from MonoBehaviour to Enemy. Fortunately, since the Enemy class inherits from Monobehaviour, the children of the Enemy class are also considered children of MonoBehaviour!

## 3.What is polymorphism?

- Image of four pillars in a row, labeled from left to right with Abstraction, Encapsulation, Inheritance, and Polymorphism. The third pillar labeled Polymorphism is highlighted.
Select image to expand

- Although inheriting core functionality from a parent class can be helpful, there are many situations where you don’t want the child class to perform exactly the same action as the parent class. Polymorphism allows you to change the functionality of what an object inherits from its parent class. 
```
public class Enemy : MonoBehaviour 
{ 
    public void DealDamage () 
    {
        Player.Health -= 10;
    }
}
```
- In the above example, the Enemy class has a DealDamage method that removes 10 points from the Player’s health whenever it’s called. The Thief class, a child of Enemy, can call this method without declaring it in the class. 
```
public class Thief : Enemy
{
    private void Update()
    {
        if (Player.isSeen)
        {
            DealDamage(); // method from parent class can be called
        }
    }
}
```
- This is fine if you want the Thief to deal exactly the same amount of damage as the Enemy class, but what if you wanted it to be a different value? These changes are accomplished through the process known as method overriding. 
The method that you want to override in the parent class must first be marked for overriding. This is done by making it a virtual method: 
```
public class Enemy : MonoBehaviour { 

    public virtual void DealDamage () { // virtual keyword allows overriding

        Player.Health -= 10;
    }
}
```
- Identifying a method as virtual indicates that it can, but doesn’t have to, be overridden. This is ideal for the current example, because while the Thief child class may need to modify the DealDamage method, another child class, such as the Scoundrel class, may not.
Once DealDamage is set to virtual, the Thief class can override it by creating its own  method for DealDamage. Here, instead of virtual, we’ll use the override notation. You can now add new functionality into the method specifically for the Thief class: 
```
public class Thief : Enemy
{
    public override void DealDamage() // can override virtual methods from parent class
    {
        Player.Health -= 2;
        CommitPettyTheft();
    }
    private void Update()
    {
        if (Player.isSeen)
        {
            DealDamage();
        }
    }
}
```
- The Thief class now deals a smaller amount of damage than the parent Enemy class, and also calls one of the Thief-specific methods. Now, when DealDamage is called in Update by a Thief object, the customized DealDamage method will be called instead of the parent method. 

- .What is encapsulation?
 Image of four pillars in a row, labeled from left to right with Abstraction, Encapsulation, Inheritance, and Polymorphism. The fourth pillar labeled Encapsulation is highlighted.

A major theme of encapsulation is safety in code — in other words, the process of ensuring that code is only used as it is intended to be used, and the values and data you are manipulating can’t be corrupted. In encapsulated code, other programmers can’t easily change the values of variables or the properties of objects. It’s impossible to account for all of the different ways that other scripts might access your code, so it's far better to encapsulate what you’ve created so it can only perform as intended. 
## 2.Overview
- In the previous tutorials, you learned about the four pillars of object-oriented programming and how they are applied: 
Abstraction: reducing duplicate code by “abstracting out” repeated details or information.
Encapsulation: “encapsulating” data and the methods that manipulate that data together in a class, protecting it from misuse by other classes.
Inheritance: child classes deriving (or “inheriting”) behavior from parent classes.
Polymorphism: changing (“morphing”) methods into many (“poly”) forms (i.e., method overloading and method overriding).
In this submission challenge, you will create a new project from scratch, demonstrating each of these pillars in the code. 
Carefully plan your program’s architecture at a high level before you begin coding. Along the way, you’ll have an opportunity to practice branching and merging code using version control software.
This challenge is not going to be easy, but you’ll be a more thoughtful, strategic programmer by the time you complete it!
A successful submission will include:
A link to your project’s GitHub repo, showing multiple commits with commit messages and at least two branches
Demonstration of abstraction (higher-level methods that abstract unnecessary details)
Demonstration of inheritance (parent/child classes)
Demonstration of polymorphism (method overriding or overloading)
Demonstration of encapsulation (getters and setters),

## Shaders and Materials
- daha öncekiler silindi göz gezdirip önemlileri not alabşlirsin
- Textures are regular image files in formats you might be familiar with, such as BMP, TIF, PNG, and JPG. 
- The data in image files is organized into channels. Black and white images, also known as grayscale images, have just one channel to indicate the shade of gray in each pixel. Color images require three channels, red, green, and blue (RGB), which combine to create the colors you see on your computer display.  
- Some image file formats have four channels: red, green, blue, and alpha (RGBA). The alpha channel typically contains transparency data.

https://user-images.githubusercontent.com/26336737/233952865-3b092039-8e37-4804-9be5-150c033a43f7.mp4

- Meshes made by modeling applications, such as Autodesk® 3ds Max® and Maya®, or Blender®, generate their own sets of 2D coordinates called UV coordinates. UV coordinates are like the XY coordinates in regular 2D spaces, but they are called UV to differentiate them from the coordinate system of the environment (XYZ). UV coordinates are relative to the mesh, not the 3D space in your scene.
- UV mapping is the process of unwrapping the surface of a 3D model to create a flat surface, then applying a 2D texture map to it. In the process, the modeling application generates the UV coordinates that allow the texture to be wrapped back onto the model.
- Since Ellen’s body material uses the Metallic workflow, this map is grayscale. Although the metallic data is in the R, G, and B channels of the texture file, the shader only reads the R channel. 
- Transparency is controlled with the alpha channel of the base map (The A in RGBA). Low values make the base map color less visible and high values make it more visible. You can make a mesh entirely invisible by setting the alpha channel values to zero, or you can create translucent effects by setting the alpha values in the mid-range. 
- In the real world, translucent substances refract light, which means they change its direction. Refraction is an advanced shader effect that we won’t attempt here; however, we can create a translucent glass object that looks pretty convincing.  
- 5.  In the Inspector, on the Glass Jar material, locate Surface Options (at the top of the Material section) and the Surface Type property. Change this value from Opaque to Transparent. 
- The front half of the jar disappears! It looks like a cutout. This is happening because of the Render Face setting. Render Face is usually set to Front because the shader only needs to render the surface of the mesh facing the viewer. However, with transparent objects, the shader needs to render both the front and back. 
- 6.  Set Render Face to Both.
- The jar still looks strange because we are giving it conflicting instructions: Surface Type is Transparent but the alpha channel still has the default values, which indicate no transparency. 
- Instead of modeling meshes of items like these, artists use alpha clipping in their textures to make part of a simple mesh invisible. Alpha clipping is a much more efficient way to create detailed objects — it’s easier to create and easier for the computer to process at runtime.
- 4.  Examine the plant from all angles. The leaves are visible from the top, but not from the bottom! This happens because these meshes are single-sided: there is no separate mesh on the back of the object (as there is with a cube, for example). 
- Now the leaves look like printouts of leaves on paper! You can fix that with alpha clipping.
- You have used transparent effects in two ways: by making the entire jar object transparent with the Transparent surface type, and by making the leaves on the plant partially transparent using alpha clipping. Well done!
- https://docs.unity3d.com/Manual/StandardShaderMaterialParameterNormalMap.html
- http://www.opengl-tutorial.org/intermediate-tutorials/tutorial-13-normal-mapping/
- Normal Maps and Height Maps are both types of Bump Map. They both contain data for representing apparent detail on the surface of simpler polygonal meshes, but they each store that data in a different way.
- As you will recall, normals are values in the mesh data that define the direction each vertex is facing. A normal map sets these values over an entire surface, which directs the shader to create the illusion that fragments (pixels) on the surface are facing different directions.
- Height maps indicate the relative height of each pixel from the mesh. These are single-channel (grayscale) maps in which each pixel value indicates a relative distance from the mesh surface. When you use an RGB image as a height map, the shader only reads the green channel.
- Select image to expand
Height maps are not used as commonly as normal maps. They are useful for creating a dramatic effect, but they also stretch the base map, which is not usually desirable if the base map is not a solid color. 
- cclusion, in 3D graphics, is the blockage of light by an object. A crack in a sidewalk and the thin dark shadow line between the fingers of a closed fist are examples of occlusion.
- Even in PBR, ambient light can reflect in odd ways where it should be occluded. An occlusion map adds shadows to these occluded areas.
- Look very closely at a real-world object that has a smooth surface, such as the glass on your smartphone, covered with fingerprints, or your favorite coffee cup that has become scratched and worn. If you wanted to model these items and include details like the fingerprints or scratches, you can use ** microsurface mapping ** to add a level of detail that isn’t otherwise captured in your base map or normal map.
- Emissive materials appear to give off their own light. You can use an emission map to specify areas where your surface will glow. 
- Observe the emission map for Ellen, on display in the Textures Exhibit of our gallery.It is mostly black, but look closely and you will see three green dots. The dots in this map line up with the lights on the back of Ellen’s neck and the top of her robot arm.
- The color on the map affects the color of the light. In addition, The HDR color picker gives the non-black areas of the emissive map glowing colored light. 
- HDR stands for high dynamic range. HDR colors have an additional luminosity outside the regular range of display colors. These are useful for glowing objects and intense specular reflections. The HDR color picker has an intensity slider to control how much additional luminosity is added to the color.
- https://learn.unity.com/project/make-a-flag-move-with-shadergraph --> Shader Graph

## Shader Graph

![e490d65c-a67a-4aa9-a155-9f534e5bf047_CC_Shad_SG_2_2 jpg 1200x0x1](https://user-images.githubusercontent.com/26336737/234270639-316a5911-5638-42eb-9547-5436aea13862.jpg)

- he Shader Graph toolbar (1) is where you will save your shader asset.
- The Blackboard (2) contains the properties that will be available to artists who use this shader to create materials. Here you can define property types as well as their names, attributes, and default values.
- Your workspace (3) is where you will create the node graph of your shader. 
- The Main Preview window (4) will give you a real-time update of what your shader looks like and how it behaves.
- The Graph Inspector window (5) will show you the current settings, properties, and values of any node you have selected.
- The Master Stack (6) is the end point of a Shader Graph that defines the final surface appearance of a shader. It lists the major shader properties of a Vertex and a - Fragment shader and provides you with the end nodes where you will plug in the necessary values.
- https://docs.unity3d.com/Packages/com.unity.shadergraph@10.7/manual/Shader-Graph-Window.html
- The basic shimmer is made with a procedural noise map. Procedural means that the texture is created by some formula or algorithm, not from an image or other physical source. Shader Graph provides a few procedural noise maps to choose from. Each one generates a cloud-like map with lighter and darker areas in a seemingly random pattern.
- 












