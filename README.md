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
