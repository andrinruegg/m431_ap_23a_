While Testing I found many different and simple problems:

- ## X Ragdoll Issue:
In the game, I expected to have normal controls, but after playing a few times, I cycled through all the keyboard keys and discovered that pressing 'X' activated a ragdoll effect and caused the player's camera to glitch out of the map for no apparent reason. There was no purpose for the ragdoll feature, so I went to the player control blueprint and removed the keybind for 'X' to prevent this from happening.

<img width="1059" alt="Screenshot 2023-10-30 091910" src="https://github.com/andrinruegg/m431_ap_23a_/assets/143380551/7ef185e0-0126-4aca-a89b-4c4d3effb351">

After ragdolling you fell out of the map, as you can see here.

- ## Alt + Alt = Roll: 
During testing the keys, I found an animation that I had forgotten to delete while still experimenting. It was an animation for a roll. When pressing 'Alt' back to back, the character would perform an awkward roll. I removed this feature similarly to how I removed the ragdoll effect: by deleting the keybind in the player control blueprint.
[Here is a short Video how it looked like](https://youtu.be/iaETo6M9Dt4)


- ## Missing Collisions: 
I noticed some trees and small rocks scattered across the map, and then realized that I forgot to create a collision for a specific tree type. To fix this, I deleted the trees, adjusted collision settings as closely as possible using the foliage editor, and enabled collisions for the brushes, ultimately resolving the issue.

- ## Entity Animations:
In the realization phase, I discussed the peculiar entity animation issue when it followed the player. To solve this, instead of creating a new animation (which would take a lot of effort), I opted to turn the entity into a ghost. Since the entity was already transparent, this seemed like a complete win. I adjusted the entity's height to make it appear as if it were flying, removed the existing animations, and now it quietly floats toward the player, creating an eerie effect.

- ## First-Person Mode:
Initially, I changed from third-person to first-person mode by placing a camera in the character's head. However, at the beginning, I faced the problem of limited movement in the up-down direction. I wasn't sure how to resolve this initially, but later I discovered sockets that allow attachment of things. I connected the camera to the head socket, enabling the camera to follow the mouse's direction in all orientations, effectively solving the issue.




