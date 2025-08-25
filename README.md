# herding
A work-in-progress cattle herding mod for Red Dead Redemption II.

This mod brings a new layer of realism to the world of Red Dead Redemption 2 by allowing you to dynamically herd cattle. It uses advanced logic to control animal behavior, creating a responsive and immersive herding experience.

The mod automatically detects nearby cows and bulls, forming a herd that you can guide and direct. Animals will follow your movements, adjusting their speed and path to stay together. When you're not actively herding, the animals will settle into natural idle behaviors like grazing or resting, making the world feel more alive.

Features
Intelligent Herding: Animals respond to your movements, forming a cohesive herd that follows you.

Responsive AI: Cows and bulls will change their speed based on their distance from the herd's center, ensuring a tight, believable formation.

Dynamic Behavior: When idle, the animals will graze, wander, or rest, adding to the game's ambient wildlife.

Automatic Herd Management: The mod automatically adds new nearby cattle to your herd and removes any that are too far away or have died.

One-Key Spawn (Debug Feature): Pressing the F1 key will instantly spawn a test herd of 20 cows and bulls around your current location for easy testing.

Optimized Performance: The code is designed for efficiency, with optimized update intervals and a caching system to ensure smooth gameplay without performance drops.

Installation
Prerequisites: You must have Script Hook RDR2 installed. You can download it from the official developer's website.

Download: Download the latest release of the mod from the Releases page on this repository.

Usage
The mod is designed to be plug-and-play. Once installed, it will automatically begin herding any nearby cattle. You can also press F1 at any time to spawn a new test herd.

Building from Source
If you are a developer and wish to compile the mod yourself, follow these steps:

Prerequisites:

Visual Studio: You will need a version of Visual Studio (e.g., Visual Studio 2022) with the "Desktop development with C++" workload installed.

Script Hook RDR2 SDK: Download the Script Hook RDR2 SDK from Alexander Blade's website. This contains the necessary header files and libraries to compile the mod.

External Libraries: Place the inc folder from the Script Hook RDR2 SDK into your project's root directory.

Project Setup:

Create a new C++ project in Visual Studio.

Add all the source files (.cpp, .h) from this repository to your project.

In the project properties, go to C/C++ > General > Additional Include Directories and add the path to the inc folder from the Script Hook RDR2 SDK.

In the project properties, go to Linker > General > Additional Library Directories and add the path to the lib folder from the Script Hook RDR2 SDK.

In Linker > Input, add ScriptHookRDR2.lib to the Additional Dependencies.

Compilation:

Set the solution configuration to Release and the platform to x64.

Compile the project. This will generate a .asi file in your project's Release folder.

The generated .asi file is your mod and should be placed in the game's root directory.
