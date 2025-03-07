# Homework 4: Structural Patterns – Singleton & Adapter 🎯

## Overview 📚
In this assignment, I applied two important structural design patterns: **Singleton** and **Adapter**. The task is divided into two main parts:

---

## 🔧 Part 1: Configuration Manager (Singleton Pattern)

**Singleton Pattern** ensures that only one instance of the configuration manager exists in the application.

### What has been done:
- Created a `ConfigurationManager` class that loads a set of key-value configuration settings (e.g., `maxPlayers`, `defaultLanguage`, `gameDifficulty`).
- Added a method to retrieve configuration values by key.
- Implemented **lazy initialization** to create the instance only when needed.
- Created a method to print all settings for testing.

### What should work ✅:
- Calling `getConfig("maxPlayers")` should return `"100"`.
- Calling the print method should display all the configuration settings.

---

## 🧩 Part 2: Chat Service Adapter (Adapter Pattern)

**Adapter Pattern** is used to integrate the legacy chat system with the new application.

### What has been done:
- Created a `LegacyChatService` class to simulate the old system.
- Defined a `ChatService` interface with the method `sendMessage`.
- Implemented the `ChatServiceAdapter` class that maps calls from the new interface to the legacy chat service.

### What should work ✅:
- When calling `sendMessage("Hello world!")` through the adapter, the output should be:  
  **`Legacy Chat: Hello world!`**

### Next steps ➡️:
- To proceed further, click on the **adapter**.

---

## General Requirements ✅

- **Documentation**: The code is well-commented, explaining the logic behind the implementation.
- **Testing**: 
  - The `ConfigurationManager` returns and prints the correct configuration values.
  - The `ChatServiceAdapter` correctly translates the messages.
- **Code Quality**: 
  - The principles of **Single Responsibility** and **Dependency Inversion** are followed.
  - Naming conventions and organization are clear and follow best practices.

---

## Compilation & Execution Instructions ⚙️

1. **Compile the Java files.**
2. **Run the demo classes**:
   - `ConfigManagerDemo` for Part 1
   - `ChatAdapterDemo` for Part 2  
   to observe the expected output.

---

-Satim Askhat! 😄
