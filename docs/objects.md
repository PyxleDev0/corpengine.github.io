# Objects Documentation

| Table of Contents | 
| ----------- |
| [1.1 - Object Types](#object-types) |

* Objects are what creates the whole service & parent-children system. Every Service & Object type is an Object.

All Objects have this attributes:
1. name (the string used to access objects by the user)
2. type (engine use only, don't change this!)
3. parent (the parent object)
4. children & childrenQueue

All Objects have this methods:
1. getGameService() (Returns the GameService)
2. getEngine() (Returns the Engine)
3. getChild(name: str) (Returns the child with the name)
4. getChildren() (Returns the children list)

> Objects like Camera, SoundService, UserInputService, EngineEventService, EngineRenderService, Assets, Object do not have children. Thus they don't have any children-related methods or attributes.

***

<span id="object-types"></span>
## 1.1 - Object Types
- There is some object types you can use during your development.

| Object Types |
| ----------- |
| [1.1.1 - Entity](#entity) |

<span id="entity"></span>
### 1.1.1 - Entity
* Entity Object type is mainly used for visually shown alive Objects. They have their position, image, rotation and more.

Attributes:
1. image (A Pygame Surface, get an image from Assets Service)
2. position (A list containing x and y positions of the Entity)
3. render (A boolean deciding if the Entity should be rendered or not)
4. collisionGroup (An integer deciding which collision group the Entity is in)
5. size (The scaling values list containing x and y scale)
6. rotation (A number deciding which side Entity is facing)

Methods:
1. isColliding(objName, parent='Workspace')
   - Returns if the given Entity with the name is currently colliding with the Entity.
   - Giving the parent parameter is optional. On default, It checks for every child in Workspace. If you give another Object, it checks for every child of the Object.
> Currently (v1.2), checking for collision at Entities inside Entities is not possible.

---
Written January 29, 2022 by PyxleDev0
