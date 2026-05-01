# Aero Engine

### What is Aero?
Aero is project that stemmed from one of my college courses where learned how propritary game enginges function and built our own base-level system in C++. My final project was to integrate Lua into the project. I've decided that I wanted to continue development, and fully develop my own game engine on side.

This project mainly stems for my interest in the backend works of similar engines. I've been developing within the Roblox engine for more than 7-8 years at this point, hence why I chose Lua as my scripting language. I don't plan to make it exactly the same as roblox, but I want to mix behaviors between all of the engines I have worked with

### Goals
At the end of this project, I hope to have a game engine that will achieve the following:

- No C++ scripting from end-user
- Lots of different utilities for development
- Luau language Integration [^1]
- Built out editor
- Outside library integrations
  - Jolt Physics Engine [^2]
  - Either Vulkan Or DX12 Rendering Engine
  - FMOD Sound Engine


### Current Implementations
- Currently written with mostly in C++ using Raylib as our base
- ECS GameObject system
- Custom scene file format
- Scripting capabilities using Lua
- A simple 2D Platformer game built on it

## Current Architecture Drawbacks
- My implementation of custom scripts is not the best, it can use some work to use less memory and overall be more performant and scaleable
- You currently can only attach one lua script to each GameObject.
- The code organization is messy and the native C++ to Lua functions for each class need to be written better
- No use of private environment tables for each script (The switch to Luau should help with sandboxing better)

Feel free to shoot me suggestions on features that would be nice to have in an engine, as well as suggestions for bettering my code! I always am striving to be a better developer so anything helps.

---
[^1]: [Luau Repository](https://github.com/luau-lang/luau?tab=readme-ov-file)
[^2]: [Jolt Repository](https://github.com/jrouwe/JoltPhysics)
