# Flutter Masterclass
## Introduction
This project serves as a demo to showcase some key features to make flutter development an incredible experience

## Table of Contents
- Arquitecture
- Testing
- Native
- Configuration
- Libraries

## Arquitecture
We follow a clean arquitecture approach that enforces seperation of concerns. This allows our code to be more readable, testable and less error-prone. Our own custom approach to the arquitecture is to have three main layers.

### Presentation
This layer holds all the logic related to the UI. It has little to no business logic and primarily serves to display views and widgets to the user and receive user interaction. By keeping this layer free from all business logic, we can safely work on UI design and not have to worry about breaking functionality. Additionaly, this also has the benefit of making the views and widgets relatively lean, thus further enhancing readability.

This layer also holds our state controllers. These controllers focus on reducing state and making calls to either a usecase or a repository.

### Domain
This layer is where the main business logic of the application resides, it is the "meat" of the app. The layer is primary split into models, repositories and use cases.
- Models: Holds the bussiness entities of the application
- Repositories: Holds the abstract class that specify what a repository implementation must fullfill. By keeping the abstraction in this layer, we can improve testability.
- Usecases: Usecases are where application specific business logic is performed. These usecases are single responsibility classes that allow our business logic to be seperated from the flutter framework.

### Data
This layer holds the repository implementations and primarily focuses on making database and API requests. By seperating this layer from the business logic, we can achieve tremendous independency from specific database and API providers, making transitions to different providers relatively easy.


## Testing
### Unit Tests

### Integration Tests

### E2E Testing

## Native 
### Method Channels

### Event Channels

## Libraries
### GENERAL

### SUGGESTED

## Configuration
