# File Packer and Unpacker Tool

## Overview
This Java-based tool allows you to pack multiple files into a single packed file and later unpack them. It is a command-line utility designed to handle regular files such as `.txt`, `.c`, `.cpp`, `.java`, and `.py`.

## Features
- **Packing**: Combines multiple files into a single packed file.
- **Unpacking**: Extracts files from the packed file to their original form.
- **Supports Regular File Types**: Works with `.txt`, `.c`, `.cpp`, `.java`, and `.py` files.
- **User-Friendly**: Simple command-line interface for ease of use.

---

## How to Use

### Prerequisites
- Java Development Kit (JDK) installed on your system.
- Basic knowledge of running Java programs from the command line.

---

### Steps to Run the Program

1. **Download the Code**:
   - Download the `Packer.java` and `Unpacker.java` files from the repository.

2. **Compile the Code**:
   - Open a terminal or command prompt.
   - Navigate to the directory where the files are located.
   - Compile the Java files using the following commands:
     ```
     javac Packer.java
     javac Unpacker.java
     ```

3. **Packing Files**:
   - Run the `Packer` class to pack files:
     ```
     java Packer
     ```
   - Follow the on-screen instructions:
     - Enter the name of the directory containing the files you want to pack.
     - Enter the name of the packed file you want to create.
   - The program will display the names of the files being packed and the total number of files packed.

4. **Unpacking Files**:
   - Run the `Unpacker` class to unpack files:
     ```
     java Unpacker
     ```
   - Follow the on-screen instructions:
     - Enter the name of the packed file you want to unpack.
   - The program will extract the files to the current directory and display the names of the unpacked files.

---

## Example

### Packing Files
1. Create a directory named `FilesToPack` and add some `.txt`, `.java`, or other regular files.
2. Run the `Packer` program:
3. Enter `FilesToPack` as the directory name and `PackedFile.pack` as the packed file name.
4. The program will pack the files and display a summary.

### Unpacking Files
1. Run the `Unpacker` program:
2. Enter `PackedFile.pack` as the packed file name.
3. The program will extract the files and display a summary.

---

## Code Structure

### Packer.java
- **Purpose**: Combines multiple files into a single packed file.
- **Key Features**:
- Reads files from a specified directory.
- Writes file headers and content into the packed file.
- Supports specific file extensions.

### Unpacker.java
- **Purpose**: Extracts files from a packed file.
- **Key Features**:
- Reads the packed file and extracts individual files.
- Recreates the original files with their names and content.

---

## Limitations
- Only supports regular files (`.txt`, `.c`, `.cpp`, `.java`, `.py`).
- The packed file format is specific to this tool and may not be compatible with other utilities.
- Does not handle nested directories during packing.

---

## Future Enhancements
- Add support for more file types.
- Implement nested directory handling during packing and unpacking.
- Add error handling for invalid file paths or corrupted packed files.

---

## License
This project is open-source and available under the MIT License. Feel free to modify and distribute it as needed.


