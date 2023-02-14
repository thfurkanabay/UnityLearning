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
## Name Convension
All Public Functions Should Have A Summary

/// <summary>
/// Fire a gun
/// </summary>
public void Fire()
{
// Fire the gun.
}



## Sources
- [private and public methods](https://stackoverflow.com/questions/52906797/when-should-i-use-public-private-or-serializefield-unity-c-sharp)
