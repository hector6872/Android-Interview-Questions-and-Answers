## Why should you consider Modularization in Android Development?

Modularization speeds build time, allows reusability, enables parallel development, isolates features to reduce coupling, and facilitates the implementation of Dynamic Feature modules.

## The difference between `implementation` and `api` in Gradle

Use `implementation` to declare an internal dependency that is only accessible within the module; consumers of this module cannot access it. This improves encapsulation and compilation performance because changes in dependencies do not trigger recompilation of the consuming modules.
Use `api` to declared a shared dependency that is exposed to other modules. Consumers of this module can also use the dependency, and any change to it will trigger recompilation of all of them.