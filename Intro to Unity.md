# Table of Content

- [Getting Started](#getting-started)
- [Editor User Interface](#editor-user-interface)
  - [Project View](#project-view)
  - [Scene View](#scene-view)
  - [Game View](#game-view)
  - [Hierarchy View](#hierarchy-view)
  - [Console View](#console-view)
  - [Inspector View](#inspector-view)
- [GameObject and Components](#gameobject-and-components)
- [Class Practice](#class-practice)

---

## Getting started

- Install [Unity Hub](https://unity3d.com/get-unity/download)
- Install [Unity 2020.3.6f1](unityhub://2020.3.6f1/338bb68529b2) using Unity Hub
  - It can be found in `"Unity Hub => Installs => Add => Download Archive => Unity 2020.x => Unity 2020.3.6 => Unity Hub"`
- Install [Visual Studio Community 2019](https://visualstudio.microsoft.com/vs/)
- Once everything is installed, you can create a new empty project via `"Unity Hub => Projects => New => Choose Universal Render Pipeline Template => give your project a name and place => Create"`

## Editor User Interface

There are few main windows that will be used thought out your development.

- Project View (Window > General > Project)
- Scene View (Window > General > Project)
- Game View (Window > General > Project)
- Hierarchy View (Window > General > Project)
- Console View (Window > General > Console)
- Inspector View (Window > General > Project)

![Unity Editor Window](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Editor%20Window.png?alt=media&token=38d6497e-74ab-465a-bedb-e859a0ec14ed)

### Project View

Project window is where all your assets located during development, just like windows explorer. These assets can be your audio files, scripts, prefab, models, material, texture. You get the idea...

![Unity Project View](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Project%20Window.png?alt=media&token=81d00362-edb6-4649-a5d8-7d906b3767e1)

Lets go also through what folders you may commonly found in project view, and what can be found in these folders.

- `_External` - Imported packages from outside of your project.
- `_Scene` - Your scene file and generated light maps.
- `Scripts` - Your C# scripts, Assembly definition, Assembly References.
- `Prefabs` - Prefabricated game objects
- `Materials` - All sorts of materials
- `Textures` - All sorts of textures
- `Audios` - All sorts of audio files

You can also search for files, select filters on the top right corner of the project views, there are ways for you to combine your query to search for a specific category of files. But we don't need to worry about that at this stage.

---

### Scene View

This is your go to spot for everything about creating your project, it's a god view of the world you created. In this space, you can visually inspect the GameObjects placed down in the world.

![Unity Scene View](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Scene%20Window.png?alt=media&token=0708a61e-4037-45ab-be24-6a486f01ad14)

If you look closely, you will notice there are few other options you can play with the scene view. Starting from the top left, you can toggle different `Draw Mode` on how the scene to be rendered, `2D Switch` to toggle the perspective of the camera, then `Light Switch`, `Audio Switch`, `Visual Effects Switch`, `Hidden Objects`, `Grid`. Normally, you won't need them, but they can be handy in varies circumstances.

![Unity Scene View Draw Mode](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Scene%20View%20Mode.png?alt=media&token=d7ff701d-eed1-46e4-aed2-4725002a126e)

Going to the top right, you will see `Component Editor Tools Panel`, `Scene View Camera Setting`, `Gizmos Toggle` and a search bar to highlight queried GameObjects.

Look right below it, you will find the tool to show/control the orientation of your scene view camera, it will also help you oriented yourself with Unity's Coordinate System.

Okay, still with me? There are more!

Look just a bit above the scene view, you will find the toolbar used to interacts with the GameObjects in the scene view.

![Unity Scene View Tool Bar](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Scene%20View%20Toolbar.png?alt=media&token=60a878b3-4523-449a-a840-2460cd7b41c3)

Again, starting from the left, you have

- Hand Tool - to move around your scene view camera.
- Move Tool - to move around your GameObjects
- Rotate Tool - to rotate around your GameObjects
- Scale Tool - to scale up and down your GameObjects
- Rect Tool - to transform the dimension of your UI GameObjects or anything having a Rect Transform.
- Move, Rotate, Scale tool - one tool that move, rotate scale GameObjects.
- Editor Tools - to use your custom editor tools (Don't need to worry about this one yet)
- Position Handle Mode - toggle betweens local || global pivots.
- Rotation Handle Mode - toggles between local || global rotation.
- Toggle grid snapping - hardly ever used with the new ProGrid packages.

---

### Game View

Game View is where you see your masterpiece in action, in this view, you can enter play mode to test and interact with your project the way you intended/ or to surprise yourself.

![Unity Game View](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Game%20Window.png?alt=media&token=94ecf75d-3413-498d-af25-025d5cb45288)

To enter Play mode, let's first take our eye to the top of the editor window. You will notice three buttons on the top that looks like these.

![Unity Game View Mode](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Play%20Pause%20Step.png?alt=media&token=fe009555-10c6-4316-9fbc-504f7c69f182)

Same deal going from the left, you have

- Play button - to enter play mode.
- Pause button - to pause the execution of your project.
- Step button - to go to the next step in execution of your project.

But before we go in there, coz we are no where near there yet. Let's also talk about the utility tools on the Game view windows. Again, starting from the left, you have

- `List of Display` - toggle which view of the cameras to display onto the game view.
- `Game View Dimension Setting` - to change how the aspect ratio or the resolution of the display.
- `Scale tool` - to digitally shrink or grow the display. Onto the right, you have
- `Maximize on Play` - that maximize your game view when you enters the play mode
- `Mute Audio` - da.
- `Stats` - display all kinds of data about your running project.
- `Gizmos` - same as the one in Scene view window.

---

### Console View

Console view is just like any other debug console in other application, it display a list of messages used to help you identify the issues/messages in your project.

![Unity Console View](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Console%20View.png?alt=media&token=ad4b3306-1ee6-4686-9016-5cde02c2dc15)

The options available in this view starting on the left are

- `Clear Console` - Clear the console and options to clear on entering the play mode or when building the project.
- `Collapse` - Stack the logs that are identical to one another.
- `Error Pause` - Pause the project execution on error.
- `Editor Menu` - Toggle what log will be print onto the console view.

On the right, you have

- Typical `search bar`
- `Log Level Filters` - to filter out the logs based on your choice (Message, Warning, Error).

### Hierarchy View

Hierarchy view is equally important as the previously mentioned views but significantly less complex. This is simply the place where you manages the hierarchy of your project.

In this view, you can check all the GameObjects you have placed down in the world, how they are parented and whether those GameObject are prefab instances or not.

You can also create new GameObjects from this view by `right-clicking` on the empty area, you will see a list of categories that you can use to quickly navigate to the GameObjects you want to create. The categories are pretty self-explanatory, so we won't be going through each and everyone of them.

Another thing you can do with Hierarchy View is that you can load multiple Scene at the same time. "Why load multiple scenes?" you may ask,by loading multiple scenes, you can segregate the features of your project. One example is that, if I have a object pool that may be used multiple times through out different scenes. It may be costly to unload/reload them every time when we switch to a new scene. By keeping a pool scene open, the pool can be accessible any time via your scripted behaviors. And this is one application of the multi-scene hierarchy.

![Unity Hierarchy View](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Hierachy%20Window.png?alt=media&token=0ec985f6-3812-40f0-88a9-698a9a406d20)

### Inspector View

Inspector view as the name suggests is an inspector that inspect every object in your project, this can be anything such as text file, C# scripts, audio control group.

![Unity Inspector View](https://firebasestorage.googleapis.com/v0/b/react-portfolio-c495c.appspot.com/o/sp-demo-assets%2Fscreenshots%2FUnity%20Inspector%20Window.png?alt=media&token=4f110b2b-ead4-43ba-9ab2-21e8a38ae680)

## GameObjects and Components

Everything created in your project is a GameObject, GameObjects is a containers created to house different components to assemble features/behavior of an Object.

Let's talk what we have learned so far and try to apply those knowledge

## Class Practice

- Create a Simple Box
- Create a bouncing ball
- Store the two objects as prefab
- Try out a different object and store it as prefab
