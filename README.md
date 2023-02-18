# UnityLearning
This project is where I write what I learned for unity and develop on it <br/>
[Syntax Rules](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
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

verticalInput

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

![image](https://user-images.githubusercontent.com/26336737/218960067-d2a8694b-0572-4bc8-8e85-752804c566a6.png)

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

## To be learn 
- Gamemanager e ne konur? 
- [Extern nedir?](https://gelecegiyazanlar.turkcell.com.tr/konu/egitim/objective-c-ile-ios-201/extern-bellek-sinifi)
- https://learn.unity.com/tutorial/the-real-time-production-cycle#
-  Invoke() [ Link ](https://www.youtube.com/watch?v=_cmlXcCd6WI)
## Extra works
- [ ] https://learn.unity.com/tutorial/bonus-features-1-share-your-work# Checklist 
