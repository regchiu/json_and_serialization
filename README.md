# json_and_serialization

Automated serialization using code generation.

## One-time code generation

By running flutter `pub run build_runner build` in the project root, you generate JSON serialization code for your models whenever they are needed. This triggers a one-time build that goes through the source files, picks the relevant ones, and generates the necessary serialization code for them.

While this is convenient, it would be nice if you did not have to run the build manually every time you make changes in your model classes.

## Generating code continuously

A watcher makes our source code generation process more convenient. It watches changes in our project files and automatically builds the necessary files when needed. Start the watcher by running flutter `pub run build_runner watch` in the project root.

It is safe to start the watcher once and leave it running in the background.



