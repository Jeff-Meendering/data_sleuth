# DataSleuth

A lightweight, multi-threaded cybersecurity tool for quickly searching through large volumes of database dumps and text files. Built with Rust and a modern egui interface, it’s perfect for analyzing sensitive data without compromising performance.

## Features

- **Fast & Parallel:** Leverages Rayon for multi-threaded searching.
- **Flexible Keywords:** Supports multiple keywords with both case-sensitive and insensitive options.
- **Intuitive Interface:** Drag-and-drop support along with file and folder browsing.
- **Real-Time Feedback:** Live counters for matching lines and files processed.
- **Custom Output:** Saves search results to a user-specified output file.
- **Secure Processing:** All operations are performed locally without altering original files.

## Quick Start

### Prerequisites

- [Rust](https://www.rust-lang.org/tools/install) (v1.70.0 or later)
- Cargo (included with Rust)

### Installation & Build

1. **Clone the Repository:**
    ```bash
    git clone [repository-url]
    cd DataSleuth
    ```

2. Build the Application:
    ```bash
    cargo build --release
    ```

### Running the Application

- Via Cargo:

    ```bash
    cargo run --release
    ```

- Directly:

    ```bast
    ./target/release/DataSleuth.exe
    ```

## How to Use

    1. Launch the Application: Open the tool.
    2. Select Files/Folders: Drag-and-drop your text files or use the "Browse Files/Folders" buttons.
    3. Input Keywords: Enter one or more keywords (separated by semicolons, e.g., error;warning;critical).
    4. Choose Options: Toggle case sensitivity if needed.
    5. Select Output: Pick an output directory where the results will be saved (default file name is output.txt).
    6. Start Search: Click the "Search" button and watch the real-time progress indicators update.

## Security Considerations

    - Local Processing: The tool processes files on your machine; no data is sent over the network.
    - Data Integrity: Original files remain unmodified, and results are written to a new output file.
    - Best Practices: Always follow proper security protocols when handling sensitive data.