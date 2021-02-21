# Flutter Architecture Showcase [WIP]

The goal of this project is to demonstrate different approaches to Flutter apps architecture and state management (BLoC,
Redux, Mobx, Getx – you name it). There is already a great repository
[brianegan/flutter_architecture_samples][1] solving a similar task, but this project has a slightly different goal.

Instead of being the centralized repository with all the source code controlled by one maintainer, it will contain
references to other repositories. This project defines specifications, so all referenced repositories should implement
the same task.

## Benefits

- Each pattern can be implemented in multiple ways by different authors.
- The popularity of each approach can be measured by the number of stars of each separate repository.
- Authors of each solution control and update it independently.

## Requirements

In order to add the reference to your solution into this repository, the solution should follow these rules:

- It should implement the specifications defined in this repository.
- It should have proper license (e.g. BSD3).

## Specifications

Create a Firebase connected app that allows registered users to add new posts with images. Take a look at
the [following mock-ups][2].

### Screens

1. Sign in/sign up page. For the sake of simplicity let's agree that only registered users can view and add new posts.
   One social login would be enough, e.g. Google Auth.
2. Simple feed with all the posts ordered by date: image, title, first line of content. Click on the list item opens
   post details screen.
3. Post details with a slider of images at the top, and the post content.
4. New post form. User should enter title, content and add from 1 to 5 images. No post editing/deleting is allowed.

### Push notifications

User should receive push notifications about the latest post added:

1. If the app is in a background, push notification appears. Clicking on it opens post details screen.
2. If the app is in a foreground, an in-app notification appears with post icon and title.
3. If the user is on the main screen and receives push notification, a new post appears in the main feed on the top.

### Architecture

The app should follow [clean architecture][3] principles and chosen state management pattern (BLoC, Mobx, Getx, or
whatever).

[1]: https://github.com/brianegan/flutter_architecture_samples

[2]: https://www.figma.com/file/aQEkg4oDDgOyTt98ykUhhD/flutter-architecture-showcase

[3]: https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html
