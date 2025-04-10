## Why should you consider Modularization in Android Development?

Organizing the codebase into multiple self-contained and loosely coupled modules, structuring them into independent features and/or layers that serve a clear purpose, is beneficial because it allows for better organization and maintenance, increases encapsulation, facilitates code reuse, optimizes build times, improves team collaboration by reducing potential conflicts, and supports more isolated and efficient testing.

## The difference between `implementation` and `api` in Gradle

Use `implementation` to declare an internal dependency that is only accessible within the module; consumers of this module cannot access it. This improves encapsulation and compilation performance because changes in dependencies do not trigger recompilation of the consuming modules.
Use `api` to declared a shared dependency that is exposed to other modules. Consumers of this module can also use the dependency, and any change to it will trigger recompilation of all of them.