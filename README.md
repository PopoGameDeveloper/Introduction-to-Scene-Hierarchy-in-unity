# Introduction-to-Scene-Hierarchy-in-unity

<h1>The Hierarchy window</h1>

![Alt text](/1.png)
The default **Hierarchy** window view when you open a new Unity project
The Hierarchy window displays every GameObject
in a Scene, such as models, Cameras, or Prefabs
You can use the Hierarchy window to sort and group the GameObjects you use in a Scene. When you add or remove GameObjects in the Scene view, you also add or remove them from the Hierarchy window.
The Hierarchy window can also contain other Scenes, with each **Scene**
 containing their own GameObjects.

<h1>Parenting</h1>
 
Unity uses the concept of parent-child hierarchies, or parenting, to group GameObjects. An object can contain other GameObjects that inherit its properties.You can link GameObjects together to help move, scale, or transform a collection of GameObjects. When you move the top-level object, or parent GameObject, you also move all child GameObjects.
You can also create nested parent-child GameObjects. All nested objects are still descendants of the original parent GameObject, or root GameObject.
Child GameObjects inherit the movement and rotation of the parent GameObject. To learn more about this, see documentation on the Transform component
![Alt text](/2.png)
**Child 1** and **Child 2** are the child GameObjects of **Parent**. **Child 3** is a child GameObject of **Child 2**, and a descendant GameObject of **Parent**.

<h1>Organize GameObjects</h1>

<h1>Create new GameObjects</h1>

To create a new GameObject in the Hierarchy window:
1. Right-click on empty space in the selected Scene.
2. Select the GameObject you want to create.
You can also press **Ctrl+Shift+N** (Windows) or **Command+Shift+N** (macOS) to create a new empty GameObject.
**Note**: New GameObjects are created in “rename” mode automatically. To disable this behavior, select the More (⋮) menu in the Hierarchy window and deselect **Rename New Objects.**

<h1>Toggle child GameObject visibility</h1>

To toggle the visibility of child GameObjects:
1. Select the drop-down arrow (►) to the left of the parent GameObject.
2. Press **Alt** while clicking the drop-down arrow (►) to toggle visibility of all descendant GameObjects of the root GameObject.
3. Select the drop-down arrow again (▼) to collapse all descendant GameObjects.

<h1>Create child GameObjects</h1>

To create a child GameObject:
- Drag the GameObject onto the parent GameObject in the Hierarchy.

![Alt text](/3.png)
Object 4 is selected and is being dragged onto Object 1, so Object 4 can become a child of Object 1.

<h1>Create parent GameObjects</h1>

You can add a new GameObject into the Hierarchy view as the parent of existing GameObjects.
To create a parent GameObject:
1. Right-click a GameObject, or select multiple GameObjects on the same level and right-click.
2. Select **Create Empty Parent.**
You can also press **Ctrl+Shift+G** (Windows) or **Command+Shift+G** (macOS) to create a parent GameObject.
**Note**: If you have set a default parent GameObject, Create Empty Parent creates the new GameObject as a child of the default parent, not as the parent of the selected GameObjects.

<h1>Create sibling GameObjects</h1>

A sibling GameObject is a GameObject with the same hierarchy as another child GameObject. To create a sibling GameObject:
1. Drag the GameObject above or below an existing GameObject.
2. Use the horizontal blue line to determine the order of the GameObject.
![Alt text](/4.jpg)
Drag **Object 4** (selected) between **Object 2** and **Object 3** (indicated by the blue horizontal line), to create a sibling GameObject under the parent GameObject **Object 1** (highlighted in a blue).

<h1>Duplicate GameObjects</h1>

To duplicate GameObjects, right-click the target GameObject and select **Duplicate.** 
You can also press **Ctrl+D**  (Windows) or **Command+D** (macOS) to duplicate the selected GameObject.

<h1>Paste GameObjects as child</h1>

You can cut or copy a selected GameObject and then paste it as a child of another GameObject. Pasted child GameObjects keep their world position.
To paste a GameObject as child:
1. Right-click the selected GameObject, and then select **Cut** or **Copy.**
2. Right-click the intended parent GameObject, and then select **Paste as Child.**
You can also press **Ctrl+Shift+V** (Windows) or **Command+Shift+V** (macOS) to paste a GameObject as a child.

<h1>Organize GameObjects with default parent</h1>

You can make any GameObject in the Hierarchy window a “default parent”. When you drag a GameObject into the Scene view, Unity automatically makes this GameObject the child of the GameObject you set as the default parent.
To make a GameObject a default parent:
1. In the Hierarchy window, right-click on the GameObject.
2. Select **Set as Default Parent.**
When you drag a GameObject into the Scene view, in the Hierarchy window, the child GameObject is indented below the default parent GameObject. The name of the default parent GameObject is bold.
![Alt text](/5.jpg)
In this image, the **Cube** GameObject is the default parent. When the user drags the **Car** GameObject into the Scene view, Unity automatically makes it the child of the **Cube** GameObject.
To remove default parent status from a GameObject:
1. In the Hierarchy window, right-click on the GameObject.
2. Select **Clear Default Parent.**
The name of the GameObject that was previously the default parent is no longer bold. When you drag a GameObject into the Scene view, it appears at the top level in the Hierarchy window. In other words, Unity does not make this GameObject the child of the GameObject that was previously the default parent.

![Alt text](/6.png)

In this image, no GameObjects in the Hierarchy window are set as the default parent. When the user drags the **Car** GameObject into the Scene view, Unity adds it at the top level of the hierarchy.
You can only set one default parent per Scene. In the Hierarchy window, if you set a GameObject as the default parent, and then you make a different GameObject in the same Scene the default parent, only the second GameObject is the default parent.
If you have multiple Scenes in the Hierarchy window, and you set default parents in each Scene, when you drag a GameObject into the Scene view, Unity makes the default parent GameObject in the active Scene the parent of the new GameObject.

![Alt text](/7.png)
In this image, the **Cube** GameObjects in both **Scene1** and **Scene2** are set as default parents. Unity sets the **Cube** in Scene1 as the parent of the **Car** GameObject, because **Scene1** is the active Scene.
You can set a keyboard shortcut for the default parent setting in the Shortcuts manager. On the Shortcuts window, assign a keyboard shortcut to **Hierarchy View > Set as Default Parent**. If there is no default parent set, and in the Hierarchy window you select a GameObject, use the shortcut to make this GameObject the default parent. When a default parent is set, use the shortcut to remove default parent status from any GameObject that has it.

<h1>Set Scene visibility and pickability</h1>

Click the Scene visibility icon to hide and show GameObjects in the Scene view
 without changing their in-application visibility.
Select the Scene picking icon to toggle the ability to select GameObjects in the Scene view while you are editing.
These controls are useful for working with large or complex Scenes where it’s difficult to view and select specific GameObjects.
![Alt text](/8.png)
Scene visibility icons/toggles
For more information, see the documentation on Scene visibility and Scene picking.

<h1>Sort GameObjects</h1>

By default, the Hierarchy window lists GameObjects in the order they’re created. You can drag the selected GameObject up or down in the Scene to change the order of the GameObjects.

<h1>Alphanumeric sorting</h1>

To sort GameObjects in alphanumeric order:
1. Select **Edit > Preferences** (macOS: **Unity > Settings).**
2. Select **Enable Alphanumeric Sorting.**
When selected, an icon appears in the Hierarchy window that allows you to toggle between **Transform** sorting (the default value) or **Alphabetical** sorting.
![Alt text](/9.png)

<h1>Multi-Scene editing</h1>
You can have more than one Scene open in the Hierarchy window at the same time. For more information, see the Multi Scene Editing page.

<h1>Override indicator</h1>

When you edit a Prefab instance in a Scene, Unity displays a indicator next to the parent GameObject in the hierarchy. This indicator highlights any Prefab that has non-default override values in any of its child GameObjects. To open the Overrides dropdown directly from the Hierarchy window click on the override indicator. The override indicator appears as a blue line in the left side of the margin and is identical to the instance override in the **Inspector**
window. For more information, see Instance overrides.
 ![Alt text](/10.png)
 This image shows the override indicator displayed next to Prefab A when its child, GameObject C, has a value in a non-default state.
