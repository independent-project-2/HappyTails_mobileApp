# HappyTail

A Flutter mobile application built with MVVM (Model-View-ViewModel) architecture.

## Folder Structure

This project follows the MVVM architecture pattern for better code organization, maintainability, and testability.

```
lib/
├── main.dart                          # Application entry point
├── app/
│   ├── app.dart                       # Main app configuration
│   └── routes/
│       ├── app_routes.dart            # Route definitions
│       └── route_config.dart          # Route configuration
├── core/
│   ├── constants/
│   │   ├── api_constants.dart         # API endpoints and keys
│   │   ├── app_constants.dart         # App-wide constants
│   │   └── asset_constants.dart       # Asset paths
│   ├── theme/
│   │   ├── app_theme.dart             # App theme configuration
│   │   ├── colors.dart                # Color palette
│   │   └── text_styles.dart           # Text styles
│   ├── utils/
│   │   ├── validators.dart            # Input validators
│   │   ├── helpers.dart               # Helper functions
│   │   └── date_formatter.dart        # Date/time utilities
│   └── errors/
│       ├── exceptions.dart            # Custom exceptions
│       └── failures.dart              # Failure classes
├── data/
│   ├── models/
│   │   ├── user_model.dart            # User data model
│   │   └── pet_model.dart             # Pet data model
│   ├── repositories/
│   │   ├── user_repository.dart       # User data operations
│   │   └── pet_repository.dart        # Pet data operations
│   └── services/
│       ├── api_service.dart           # API client
│       ├── local_storage_service.dart # Local storage
│       └── auth_service.dart          # Authentication service
├── viewmodels/
│   ├── auth/
│   │   ├── login_viewmodel.dart       # Login business logic
│   │   └── register_viewmodel.dart    # Registration logic
│   ├── home/
│   │   └── home_viewmodel.dart        # Home screen logic
│   └── profile/
│       └── profile_viewmodel.dart     # Profile screen logic
└── views/
    ├── auth/
    │   ├── login_screen.dart          # Login UI
    │   └── register_screen.dart       # Registration UI
    ├── home/
    │   ├── home_screen.dart           # Home UI
    │   └── widgets/
    │       ├── pet_card.dart          # Reusable pet card
    │       └── home_header.dart       # Home header widget
    ├── profile/
    │   └── profile_screen.dart        # Profile UI
    └── widgets/
        ├── custom_button.dart         # Custom button widget
        ├── custom_text_field.dart     # Custom input field
        └── loading_indicator.dart     # Loading widget
```

## Architecture Overview

### MVVM Pattern
- **Model**: Data layer (`data/models`, `data/repositories`, `data/services`)
- **View**: UI layer (`views/`) - Only responsible for displaying data
- **ViewModel**: Business logic layer (`viewmodels/`) - Handles user interactions and state management

### Key Principles
- Separation of concerns
- Dependency injection for better testability
- Reactive programming with state management
- Repository pattern for data abstraction

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
