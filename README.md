# Introduction-to-Scene-Hierarchy-in-unity

**The Hierarchy window**
![Alt text](/1.png)
The default Hierarchy window view when you open a new Unity project
The Hierarchy window displays every GameObject
in a Scene, such as models, Cameras, or Prefabs
You can use the Hierarchy window to sort and group the GameObjects you use in a Scene. When you add or remove GameObjects in the Scene view, you also add or remove them from the Hierarchy window.
The Hierarchy window can also contain other Scenes, with each Scene
 containing their own GameObjects.

 **Parenting**
Unity uses the concept of parent-child hierarchies, or parenting, to group GameObjects. An object can contain other GameObjects that inherit its properties.You can link GameObjects together to help move, scale, or transform a collection of GameObjects. When you move the top-level object, or parent GameObject, you also move all child GameObjects.
You can also create nested parent-child GameObjects. All nested objects are still descendants of the original parent GameObject, or root GameObject.
Child GameObjects inherit the movement and rotation of the parent GameObject. To learn more about this, see documentation on the Transform component
![Alt text](/2.png)
