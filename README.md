# MVVM Framework

A Flutter library for implementing the Model-View-ViewModel (MVVM) architectural pattern. <br/>
This framework simplifies state management and promotes a clean separation of concerns in Flutter applications.

## Advantages of Transitioning to MVVM

- **Enforced Separation**<br/> 
The MVVM architecture enforces a strict separation between business logic (ViewModel) and the UI (View).<br/>
This ensures a clean architecture by preventing the mixing of concerns, which can lead to a more organized and scalable codebase.

- **Improved Readability**<br/>
By isolating business logic within the ViewModel, the code becomes more structured, readable, and easier to maintain, simplifying collaboration and future development.

- **Enhanced Testability**<br/>
ViewModels are inherently unit-testable, enabling comprehensive testing of business logic.<br/> Views are simplified, making widget testing more efficient by allowing the mocking and manipulation of model data returned to the View.

- **Centralized State Management**<br/>
A base MVVM class provides a unified approach to handling common states such as loading and error handling, significantly reducing boilerplate code and improving consistency across the application.

Adopting the MVVM architecture results in a more robust, maintainable, and testable codebase, ultimately enhancing the overall development experience and product quality.

## Features

- **MVVM Architecture**<br/>
Provides base classes for Model, View, ViewModel, and the MVVM component.

- **Flutter Bloc**<br/>
Built on top of `flutter_bloc` for state management.<br/>
This framework extends `flutter_bloc`, allowing you to leverage all its features while providing additional capabilities through the MVVM component. This ensures flexibility for scenarios where the MVVM component may not fully address specific requirements.

- **Cross-Platform**<br/>
Compatible with iOS, Android, macOS, Windows, Linux, and Web.

- **Loading Handling**<br/>
Manage loading states globally for the entire application or customize them for specific components.

- **Error Handling**<br/>
Manage error states globally for the entire application or customize them for specific components.

## Usage

Refer to the [Basic Example](example/lib/basic_example.dart) for a quick start guide on how to use this framework.

## Examples

Check the `example` folder for a complete Flutter application demonstrating the usage of this framework. For more information, refer to the [Example README](example/README.md).

## Code Snippets

This library comes with useful VS Code snippets to help you quickly scaffold MVVM components.

### Installation

Copy the [mvvm.code-snippets](https://github.com/Draxent/mvvm_framework/blob/main/.vscode/mvvm.code-snippets) file in the `.vscode` folder of your project.

### Available Snippets

| Trigger       | Snippet Content            |
|---------------|----------------------------|
| `mvvm`        | Create a complete MVVM component |
| `mvvm view`   | Create a MVVM view widget  |
| `mvvm view-model` | Create a MVVM view model |
| `mvvm model`  | Create a MVVM model        |
| `mvvm test`   | Create a MVVM test setup   |

These snippets assume that your application uses the following libraries:

- `freezed` for immutable data classes.
- `injectable` for dependency injection.
- `mockito` for mocking in tests.

Make sure these libraries are included in your project to fully utilize the provided snippets.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.
