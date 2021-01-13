# Project2 - Sprites
  
In this project we are going to explore class hierarchy and abstraction.  
  
## Sprite
The Sprite Class represents any Object which can be drawn on the screen.  It is an abstraction of the Blob class from before.  It provides the basic functionality that is common to **all** such objects.

### Properties
All Sprites must have a Position and Velocity vectors.  (Sprites that do not move simply have a Zero velocity vector~)  
These properties should be **protected** in occordance with *encapsulation* standards.
  
### Constructors
You should provide Three Constructors for the Sprite class.  
**Default Constructor**  
`public Sprite()` : Default Values (Zero Vector) for both Position and Velocity.  
  
**Position Only**  
`public Sprite(Vector2 s)` : Provide an initial position, but default Zero velocity.

**Fully Define**
`public Sprite(Vector2 s, Vector2 v)` : Provide both initial position and velocity.

### Bonus Constructors
Sometimes it is useful to provide multiple easy ways to do the same thing~  Providing additional Constructors for other use cases can make your coding cleaner and easier.  For example, in this class, you may find it useful to have Constructors which take primitive values and then use those to create Vector2 objects internally.  
  
**Position Only (floats)**
`public Sprite(float x, float y)` : this will allow you to create a Sprite like this:  `new Sprite(300, 588);` rather than `new Sprite(new Vector2(300, 588));`
  
**Fully Define (floats)**
`public Sprite(float x, float y, float dx, float dy)`

**Copy Constructor**
`public Sprite(Sprite toCopy)` : Sometimes it is useful to replicate an Object rather than manually set all of its values every time.
