# Flutter Architecture Showcase [WIP]

The goal of this project is to demonstrate different approaches to Flutter apps architecture and state management (BLoC,
Redux, Mobx, Getx – you name it). There is already a great repository
[brianegan/flutter_architecture_samples][1] solving a similar task, but this project has a slightly different goal.

Instead of being the centralized repository with all the source code controlled by one maintainer, it will contain
references to other repositories. This project will define "specifications", so all referenced repositories should
implement the same task.

## Benefits

- Each pattern can be implemented in multiple ways by different authors.
- The popularity of each approach can be measured by the number of stars of each separate repository.
- Authors of each solution control and update it independently.

## Requirements

In order to add the reference to your solution into this repository, the solution should follow these rules:

- It should implement the specifications defined in this repository.
- It should have proper license (e.g. BSD3).

## Notes

The specifications are currently WIP. The main goal is to define something simple enough from one side (we don't want to
create a sample project with 10.000 LOC), and demonstrate some corner cases from another side (because the devil is
always in the details, while the "default" ToDo app looks good with almost any approach).

[1]: https://github.com/brianegan/flutter_architecture_samples
