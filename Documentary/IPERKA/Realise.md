# Realise 
Before hopping in, please check out this small gameplay: [Gameplay](https://youtu.be/QzJG0K9xBcc) <br>
Here are a few Pictures of my project where I want to show off the realistic graphic: 
<img  alt="Screenshot 2023-10-26 113529" src="https://github.com/andrinruegg/m431_ap_23a_/assets/143380551/67d7a757-a372-4db3-acb3-cc164d4e4776">
<img  alt="Screenshot 2023-10-26 114119" src="https://github.com/andrinruegg/m431_ap_23a_/assets/143380551/c681990c-03ad-4692-b337-2582de9f4aa2">

<br>

_______________
# How I approached the tasks:
When you look at the planning: [Plan.md]: https://github.com/andrinruegg/m431_ap_23a_/blob/main/Documentary/IPERKA/Plan.md <br>
You can see the multiple tasks I set myself. Before starting out, I always informed myself about the things I do. An example is how I should create a map. I looked up for tutorials and then I just did my tasks. If i was happy with the completed task, I went to the next one. After every task I also checked if the task was done right.

# Setup Tasks:
At the beginning, I had to download multiple apps: Epic Games and Blender. Then, on Epic Games, I had to download various versions of Unreal Engine. Initially, I tried downloading the newest version (5.3). 
Unfortunately, when I attempted to open the app, it consistently crashed. The reason for this was an old driver.  <br>
I went to the official Intel website, downloaded the app, and obtained the latest version for my CPU (Intel Core i7, 11th gen).  <br>
Before arriving at that solution, I acquired Unreal Engine 4. <br>
However, I lacked experience with it, and it also had outdated tools, so I tried finding another way to handle that problem. With the necessary apps installed, I began educating myself. I watched simple tutorials for UE5 and Blender and started experimenting on my own.  <br>
Before commencing map-making (one of my first tasks), I tested features like landscaping and various cool add-ons such as the easy building system. <br>
I created a small island for experimentation. <br>
The map-making process took longer than expected because I thoroughly enjoyed it. <br>
I acquired numerous textures and 3D models from the internet and aimed to create a realistic forest. Additionally, I implemented sounds.

## By the way, I also made a small tutorial Video how to make an Horror Enviroment 😄: https://youtu.be/7xzplbQVI2Y <br> 
This is a shortened video down to 7 minutes. It took a few hours to edit and create so please watch it! (Also dont forget to subscribe to my channel for more!)
___

**The next task was creating an entity:** I tried many things. I went into Blender and attempted to create some scary characters for my game, but I just wasn't able to do it. The problem arose because I created characters and implemented them in the game, but they didn't have a skeleton, so animations didn't work on them. I tried everything. Eventually, I gave up on that idea. Then I came up with something new. UE5 has a simple character for everyone who starts out, and I used that playable character in the game. As it already had a skeleton, it was easy. I created new textures and made the entity red and not easily visible in the dark. 

Then, I encountered problems with the animations again. I attempted to create a simple AI system where the entity can follow the player. I made it so that the entity follows the player when he sees him, but that affected the animations somehow. Sadly, this was a problem I couldn't fix. When he sees you, he runs to you, but it looks a bit weird. I didn't spend much time on that problem because I knew I couldn't fix it. So I moved forward.

I changed the game mode. Initially, it was a simple third-person mode, but I altered it to the first person. Here is how I did it: I began with creating a follow camera. I set it into the player's head, but it looked weird as I couldn't move my head in the game, so I could only look forward. To fix that, I attached the camera to the head socket so that it mimics first-person view—seeing everywhere where my head moves—allowing a 360° turn. I removed the sky, making it dark to enhance the eerie atmosphere. I added fog into the game and adjusted the location to the player's height. I increased the fog density and made the fog dark grey. Consequently, while playing, one couldn't see much in the game as there was no light, just a dark fog.

My next idea was to add a light to the camera. I attached it to the socket and adjusted the strength of the light and the field where it could look. I also changed the camera's field of view to 110° to make the first-person mode look scarier.

___
## Blueprints

**In my project I worked with blueprints instead off with codes. But what are blueprints?**

<r> <br> <br>
**What Are Blueprints?**

Blueprints are visual tools in UE5. They're used to build and define how things work in a game and bascially remove the whole programming part.

**How Do They Work?**

Instead of typing lines of code, you connect colorful shapes and boxes to make things happen in the game(Like you see in the pictures below). It's a bit like drawing lines between different actions or ideas.

**What Can You Do with Blueprints?**

You can create new objects (like characters or items), give them behaviors, and make them do things in the game world.
They help in setting up events and making decisions, like "When this happens, do that."

**Why Are They Useful?**

They're helpful because you don't need to be a coding expert to make cool stuff happen in your game. They're like a simpler way to tell the game what to do.
Level Blueprint:

What it is: It's like a big control center for everything happening in a specific level of the game. It manages events that affect the entire level or specific objects in it.
What it does: It helps control events across the whole level, like actions for different objects, level streaming, and setting up event triggers.


**Blueprint Class:**

What it is: Think of it as a template that adds new functions or behavior to game objects. These are created visually, not through coding, and act like new types of objects.
What it does: Allows easy addition of new behavior or functionality to objects in the game without having to write code for each new thing.

**Data-Only Blueprint:**

What it is: It's a type of Blueprint that only allows tweaking existing properties and components without adding new ones.
What it does: It's useful for making variations of existing objects without changing their core structure.

**Blueprint Interface:**

What it is: A collection of function names that can be shared among different Blueprints.
What it does: Ensures that different Blueprints have certain functions they must have, enabling them to communicate and share data.

**Blueprint Macro Library:**

What it is: It's like a box containing pre-made sequences of actions that can be easily reused in different Blueprints.
What it does: Saves time by storing and reusing common sequences of actions or nodes for execution and data transfer.

**Animation Blueprint:**

What it is: An Animation Blueprint controls how a character or object moves and animates within the game.
What it does: It defines how different animations blend and play out, governing the movement and appearance of characters or objects in the game.
In essence, Blueprints in Unreal Engine are tools that simplify game development by allowing designers to create functionality and behaviors without extensive coding. The Animation Blueprint, specifically, focuses on creating and managing animations for characters or objects within the game.

<img width="483" alt="Screenshot 2023-10-30 070920" src="https://github.com/andrinruegg/m431_ap_23a_/assets/143380551/dc879ee3-306e-41a0-9674-1e6583bae7c2">
<img width="483" alt="Screenshot 2023-10-30 070947" src="https://github.com/andrinruegg/m431_ap_23a_/assets/143380551/4ecf5b0e-0a20-4da6-af4c-75518d8a2f80">


## Testworld
Throughout the project, I also had a testing world. The funny thing is that the testing world looks better and has more functions than my own project, as I spent more time experimenting around. Here is a short clip of it: [My Testworld](https://youtu.be/P7YN6_LdMsM)
In this test world, I gained experience with AI, tools, building, and more. If you're wondering about the quality, it's because I ran this test world on my computer at home, where it works much better.

## Repository 
Creating the Git repository was the hardest task for me, not only because I am bad at documenting but also because I had no experience with Git and only a few weeks left when I started.

The first thing I did was creating a markdown file and putting in the simple IPERKA, then I created a markdown file for every IPERKA itself and linked them to the start page. I saw how some people designed the initial site and thought it looked cool, so I used the UE5 icon for my project's logo and wrote a few small things about myself. Then, I started following the plan; I began with the "inform" part. I easily knew what to write, but after getting into a flow, I always suddenly forgot what else I could write for the IPERKA parts, which is why the files aren't that big. "Inform" was the easiest part. After that, I moved on to "plan." I made an example table, but the thing is that in these weeks, I did the most things for my project, and yes, I know it was way too late.

Then, I moved on to the "realize" part. I thought about writing down everything I did and explained a few important things like Blueprints.
