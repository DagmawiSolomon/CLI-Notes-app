### Project: CLI Note-Taking App

#### Overview
The CLI Note-Taking App is a powerful, keyboard-driven tool designed for users who prefer a command-line interface for managing notes. With a focus on simplicity, efficiency, and productivity, the app is ideal for developers, students, or anyone who wants to streamline the process of taking notes, organizing information, and creating study material. It combines essential note-taking functionality with advanced features like hotkeys, notebooks, and flashcards, offering a versatile experience for a variety of use cases.

#### Key Features

1. **Hotkeys to Add Selected Text to Notes**  
   Users can quickly capture snippets of text by simply selecting them and using predefined hotkeys. This feature makes it effortless to add important content to your notes while reading, coding, or browsing other documents in the terminal.

2. **Notebooks for Organization**  
   Notes can be categorized into notebooks, allowing users to keep their information organized. Whether you're separating notes for different projects, subjects, or personal thoughts, the notebook system makes it easy to manage and retrieve your notes.

3. **Flashcards for Study**  
   Users can transform their notes into flashcards directly from the CLI, enabling easy revision of key concepts. Flashcards can be auto-generated from notebook content or created manually, with options for spaced repetition to aid in memory retention.

4. **Conditional Build Features via CLI**  
   The app can be customized at build time using **Rust’s Cargo features**, allowing users to include or exclude specific functionality (e.g., notebooks, flashcards, hotkeys). This enables lightweight, modular builds depending on the user’s needs. From the command line, users can choose to build the app with or without certain features, streamlining the app’s functionality for minimal environments.

   - **Example Commands:**
     - To build the app with the `notebooks` and `hotkeys` features:
       ```bash
       cargo build --features "notebooks hotkeys"
       ```
     - To build the app without the default features and only include `flashcards`:
       ```bash
       cargo build --no-default-features --features "flashcards"
       ```

#### Additional Features

- **Tagging System**: Tag notes with custom labels for better categorization and searchability.
- **Search Functionality**: Quickly search through notes and notebooks using keywords, filters, or tags.
- **Export Options**: Export notes or notebooks in various formats such as Markdown, plain text, or JSON for external use.
- **Customizable Shortcuts**: Customize hotkeys and commands to fit your workflow.
- **Version Control for Notes**: Track changes in your notes and revert to previous versions if needed.

#### Technical Specifications

- **Language**: Rust
- **Storage**: SQLite for persistent storage or flat-file storage for simplicity
- **User Interface**: Command-line interface with minimalist design and keyboard shortcuts
- **Dependencies**: Minimal, focusing on portability and performance
- **Conditional Compilation**: Utilize Cargo features to include/exclude functionality based on build configuration.

#### Use Cases

- Developers can quickly document code snippets or ideas while working.
- Students can organize lecture notes into notebooks and use flashcards for efficient studying.
- Researchers can easily tag and categorize their findings into different notebooks, adding notes directly from the terminal.

The CLI note-taking app is designed to enhance productivity, providing an easy and intuitive way to capture and manage information through the command line while staying organized and focused. The ability to customize builds makes the app highly adaptable to different user environments and needs.

DISCONTINUED
