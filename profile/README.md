Project Sparkle (SPJF)
==========

SparkleJ Framework *(SPJF, code name Sparkle)* is a Java-based framework for creating graphical applications with an API 
inspired by MIT Scratch. It provides a modern, object-oriented approach to building interactive applications and 
many customization options, while maintaining the simplicity and accessibility that Scratch is known for.

## Project Goals

These goals are what this project aims at achieving, in chronological order. Below each goal is a brief description of why
it matters, and when it was created (approximately).
1. *Provide a Scratch-like Java API, but offer more flexibility without making things harder overall.*
   - Some, like me, find code blocks and many restrictions very inconvenient for project creation. Sparkle fixes those issues
   by not featuring these two altogether. APIs are more flexible, and Java code is used instead of code blocks.
   - This goal was the primary fuel for working on Sparkle ever since the very beginning (May 2025).
2. *Create a bridge between Scratch and Java worlds, allowing to advance step-by-step and allowing Scratchers to learn Java
and get a taste of real-world programming.*
   - Schools often teach students only procedural programming paradigm (which first appeared in good old **C**) 
   and basics of programming, focusing mostly on working with existing software, which is usually *not even remotely* related to programming. 
   - As a result, students that want to learn programming in school don't get any idea about real-world programming. Especially the OOP paradigm,
   the one that skyrocketed in popularity and is very practical today.
   - Sparkle solves that by providing a well-structured OOP-based interface and layers of simplification for newbies. Maybe it's even
   school-friendly? We'll find out some day...
   - This goal was placed in March 2026, and was already fulfilled upon its placement :]
3. *Prove that Java is not "old and slow", but rather a good choice for graphical apps.*
   - Many people think Java is a very slow platform for an unexplainable reason... Maybe because it was like that in its early days.
   Nowadays, it's completely different. JIT compilers can optimize JVM bytecode at runtime so good, it can compete against GCC-compiled
   C/C++ binaries, and sometimes even exceed their performance!
   - Moreover, performance isn't everything. Take a look at *Minecraft*, a game we all know and love. Original Minecraft is written
   in Java (with LWJGL for C++ bindings, and Sparkle uses LWJGL!). You might say it's not optimal, but that's because of the game's code itself,
   not the platform. Many optimization mods exist (like OptiFine, Sodium, etc.) and with them, the game runs *much* faster.
   - Sparkle has a potential to prove the world Java is evolving like any other platform, including C++ and Python. Maybe it will even
   revive Java gaming? Or it's just me `(._.);`
   - This goal was placed in April 2026.

## Overview

While Sparkle shares conceptual similarities with Scratch, it's a completely different framework, with some aspects of its own design. 
The framework allows developers to write Java code instead of using code blocks, providing greater flexibility and access to Java's extensive ecosystem.

### This project is for you if:
- You want more power and flexibility than what can be achieved through block scripts;
- You know about Scratch and want something closer to its syntax;
- You know basic OOP and Java and want to advance your Java skills without being constrained or limited.

### This project is *not* for you if:
- You do not like writing code, or if Java structures scare you;
- You prefer simplicity to flexibility;
- You want an exact copy of Scratch's model in Java.

*Don't take it too personally if any of these statements are true for you! You still can try out Sparkle; this paragraph acts
as a warning that you **might** not enjoy coding with it, **not** as a restriction layer. `(^u^)`*

---

## Core Features

- **Sprite-based programming**: Create and manipulate sprites with properties like position, rotation, costumes, and sounds
- **Stage management**: Control the application stage with backdrops, custom drawing, and layer management
- **Event-driven architecture**: Comprehensive event system for handling user input, stage state changes, and custom events
- **Rendering engine** (SparkleGraphics): 2D rendering capabilities with support for transformations, effects, and custom drawing
- **Audio engine** (SparkleAudio): Play and manipulate sounds with various effects
- **Physics**: 2D hitbox system for collision detection

## Key Components

The framework is structured into several key components:

1. **Core Elements**: Sprites, stages, and event dispatcher provide the basic Scratch-like functionality
2. **Data Management**: Variables and lists (via `.variable` subpackage) with custom "blocks" implemented as Java methods
3. **System Architecture**: Application context, vanilla components (audio manager, graphics manager, etc.), and support for custom user-made components

## Getting Started

To get started with Sparkle:

1. Add the dependency to your Maven project:
   ```xml
   <dependency>
       <groupId>net.fokinatorr.sparkle</groupId>
       <artifactId>sparkle-core</artifactId>
       <version>(your desired version)</version>
       <classifier>(your desired native library classifier)</classifier>
   </dependency>
   ```
2. Create a class extending `SparkleApp` (to be implemented)
3. Implement your application logic using the Sparkle API

An IDE plugin for Sparkle is planned for future releases.

Enjoy! :D

---

## Development Status

The framework is currently under active development with most core features implemented.

_Note: The project is **still in beta**_; feel free to contribute via pull requests, suggest features and improvements, and report bugs/issues. Please, make sure to be constructive in your posts, _nobody_ likes whiners/spammers ;)

## License

MIT License - see [the license](../LICENSE) file for details.
