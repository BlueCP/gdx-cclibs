# Cypher Cove libraries for [LibGDX](https://github.com/libgdx/libgdx)
This repository contains libraries for use with the LibGDX framework.

## Libraries

### [FlexBatch](flexbatch)

A library for for batching many small custom objects optimally. It can be used as a flexible version of SpriteBatch, but where the sprites can have custom parameters, multi-texturing, bump-mapped lighting, etc.

### [CoveTools](covetools)

A library containing utility classes, including AssignmentAssetManager, which allows assets to be specified, loaded, and referenced with very little code.

### [GdxToKryo](gdxtokryo)

A library containing serializers for using Kryo with LibGDX's classes, as well as utilities for making it easy to implement backward compatibility (reading old data in newer versions of your game/app even if you've updated LibGDX to a newer version).

## Working with the sources
There is a top level project with a module for each of the artifacts within the repository, and one additional separate project in the **examples** directory.

Deployment uses some defined local properties. The included `gradle.properties` has blank versions of these that can be uncommented to keep Gradle `build` from complaining.

If making a pull request, please format your code similar to LibGDX. Namely:

- Opening brackets on same line
- Spaces around all operators and after commas
- Spaces before opening parentheses in method declarations
- No Hungarian notation

The **examples** project should be imported as a separate project using `examples/build.gradle`.
