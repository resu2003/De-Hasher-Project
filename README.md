# Advanced Hash Cracker
An advanced hash cracking CLI tool with support for multiple hashing algorithms, multithreading, and integration with online hash cracking APIs.

## Features

- Supports MD5, SHA-1, SHA-256, SHA-384, and SHA-512 hashing algorithms.
- Multithreading for improved performance when cracking multiple hashes simultaneously.
- Integration with multiple online hash cracking APIs to leverage their databases.
- Options for brute-force attacks using a wordlist, though currently not implemented in the provided code snippets.

## Installation

### Prerequisites

- Python 3.x installed
- pip package manager installed

### Steps

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/advanced-hash-cracker.git
   cd advanced-hash-cracker

2.  **Install dependencies:**
     ```sh
    pip install -r requirements.txt

# Usage
-----

### Command-line Interface

To use the hash cracker tool, execute `hash_cracker.py` with appropriate options:

 - `python hash_cracker.py [-s HASH] [-f FILE] [-d DIRECTORY] [-t THREADS]`

### Options

-   `-s HASH`: Crack a single hash value.
-   `-f FILE`: Crack hashes from a file.
-   `-d DIRECTORY`: Search for hashes in files within a directory.
-   `-t THREADS`: Number of threads for multithreading (default is 4).

### Examples

1.  **Crack a single hash:**
    ```sh
    python hash_cracker.py -s 098f6bcd4621d373cade4e832627b4f6

3.  **Crack hashes from a file:**

    ```sh
    python hash_cracker.py -f hashes.txt

5.  **Search for hashes in a directory:**

    ```sh
    python hash_cracker.py -d /path/to/directory

7.  **Adjust the number of threads for cracking:**

    ```sh
    python hash_cracker.py -f hashes.txt -t 8

# Implementation Details
----------------------

The tool utilizes a combination of predefined hashing APIs and supports multithreading for concurrent hash cracking. It categorizes hash types (MD5, SHA-1, SHA-256, SHA-384, SHA-512) and uses corresponding APIs for cracking. Results are saved to files when cracking hashes from files or directories.

### APIs Used

-   `beta`: Hashtoolkit API
-   `gamma`: Nitrxgen API
-   `theta`: MD5Decrypt API
-   `crackstation`: Crackstation API
-   `hashes_org`: Hashes.org API

### Notes

-   Ensure proper internet connectivity and handle network errors gracefully.
-   Some APIs may have rate limits or restrictions that could affect performance.
-   Consider customizing or extending the tool based on specific requirements or additional APIs.

# Acknowledgments
---------------

-   Inspired by the need for a versatile cybersecurity and penetration testing hash cracking tool.
-   Special thanks to the contributors of the hash-cracking APIs used in this tool.

# Summary

This markdown document provides a structured and informative overview of the Advanced Hash Cracker tool, covering its features, installation process, usage examples, implementation details, licensing information, and acknowledgements. You can adjust the URLs, project structure, and licensing details as you've done before publishing it on GitHub.
