# VocabulistApp
The best personal vocabulary iOS app

## Project Overview
I was the lead contract developer for an iOS app designed to enhance English word/vocabulary skills. The app enables users to discover new words through a daily Word of the Day feature, add words to their favorites collection, and learn through daily and practice word games that uses spaced repetition systems. Users can also access and replay historical daily challenges and word collections through an archives system.

* [Check out the app!](www.vocabulistapp.com) _(Currently in beta testing)._
* **NDA**: Due to my NDA with the client, only limited information about this project can be shared. But reference check (email, audio and video calls) with client is available upon request.

## Design and Architecture
* Dependency injection (custom DI container) to enhance modularity and testing capabilities across services, repositories, and app state management.
* Scalable and maintainable architecture with repository and service layers, utilizing protocol abstractions. Implemented concrete implementations separated through extensions for better code organization.
* Comprehensive offline data persistence using CoreData with seven interrelated entities managing complex relationships and attributes.
* Custom caching and synchronization logic improving speed and efficiency.
* Audio playback capabilities via HTTP using AVFoundation framework.
* Modern Swift concurrency with async/await for all network and database operations.
* StoreKit's SubscriptionStoreView for modern native swift paywall and subscription management.

## Notable Technical Features
* Real-time data synchronization.
* External API integration: Integrated four external API endpoints with custom handling and error management, enhancing data reliability and application resilience.
* Custom animations and transitions. Haptic feedback integration.
* Localized notifications system.
* Subscription management with StoreKit API.
* SharePlay integration for content sharing.
* Advanced logging system using OSLog framework, with capability to retrieve, filter, and format logs into text files for bug reporting.
* Comprehensive preview system using stub data and preview containers, allowing rapid UI iteration and testing across all views.
* Sophisticated paywall implementation using custom feature presentation.
* Integration with system pasteboard for enhanced user experience.
* Implemented comprehensive error handling with custom error types and user-friendly error presentation.

## Tech Stack
* SwiftUI
* CoreData
* Swift Concurrency
* StoreKit
* AVFoundation
* UserNotifications framework
* OSLog for advanced logging
* XCTest for unit testing and UI testing
* MessageUI framework for bug reporting
* Custom date formatting utilities
* Comprehensive use of Swift's latest property wrappers and property observers

## Notable User Feautres
* TabView: to navigate to different tabs.
* HomeView: Word of the Day details, play games, view settings.
* Favorites Management: allows users to favorite words from the daily word list and track their progress.
* Search View: Implemented robust search functionality with history tracking, clear history option, and paste detection for seamless word lookup.
* Word Details: Detailed word information including pronunciation audio playback, definitions, examples, and part of speech categorization
* Settings Management: comprehensive settings interface for notification preferences, subscription management, and data management including Webkit and Bug reporting.
* Games: multiple game modes for daily vocabulary challenges, supporting both single-session and archival play modes.
* Game Mode: tracking and visualization of user progress across different game modes.
* Archive & Retrieval: an archival system for previous challenges and daily words, giving users access to historical data.
* Paywall: To subscribe to premium features.
