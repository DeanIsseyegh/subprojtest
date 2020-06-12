# subprojtest
Simple project with a submodule where it cannot be configured properly on Ubuntu but can on MacOs

Step 1: Run `./gradlew parent1:taskFromRoot` and `./gradlew parent-with-sub-modules:taskFromRoot`. Notice you see the message `Hi, I'm from root!`

Step 2: Run `./gradlew parent-with-sub-modules:submodule1:taskFromSubmodule`. Notice on Ubuntu 18.04 you see the message `Task 'taskFromSubmodule' not found in project ':parent-with-sub-modules:submodule1' but on MacOS you see `Hi, I'm from a submodule parent!`
