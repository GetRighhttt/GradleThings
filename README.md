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
- `tasks` defines a unit of work
  - invoked form the command line
  - `./gradlew build` is considered a build task
  - see a full list of available tasks by running `./gradlew tasks`
  - can also create own custom tasks
  - task can have dependencies on other tasks
  - creates a task graph of dependencies
- `wrapper` is the script used to invoke Gradle and run tasks
  - always committed into version control
  - no local Gradle installation required for anyone building your project
  - contains a specific version of gradle for the project
  - ALWAYS use the Gradle wrapper script for safety (unless initializing new gradle project)
