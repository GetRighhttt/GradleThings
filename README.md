# GradleThings
Repository to demonstrate how to work with Gradle.

### What is Gradle?
- Build automation tool
  - Takes your code and packages it into deployable unit
  - applies to small or large projects
  - written in the Kotlin language
  - can also be written in Groovy
  - highly configurable to meet project needs

#### Why use Gradle
- Makes building and running applications very easy
- no need for people using your projects to install Gradle
  - Gradle wrapper comes bundled in with project
  - Just run `./graldew build` and you should be ok
- Very concise; no XML configuration needed
- lightning fast

#### Key Gradle Concepts
- `build.gradle.kts` is the Gradle build script file 
  - defines how project is build
  - written in Kotlin DSL
  - lives in top-level of the project
  - has `plugins`, `repositories`, and `dependencies`; also houses some metadata
- 
