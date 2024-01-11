# MergeArchive - A Basic Tar-Like File Format in C#

MergeArchive is a simple C# program that implements a basic tar-like file format with a command-line interface (CLI) for packing and unpacking files. This project is intended for educational purposes and serves as a minimal example.

## Usage

### Pack Files

To pack files into a MergeArchive:

```bash
dotnet run pack myarchive.mar file1.txt file2.png
```

### Unpack Files

To unpack files from a MergeArchive:

```
dotnet run unpack myarchive.mar output_folder
```

### Code Explanation

The code consists of a simple C# console application with two main functionalities:

1. Packing Files:

    - The `Pack` method takes a list of file paths and creates a tar-like archive.
    - It uses GZip compression and stores file names along with their content sizes.

2. Unpacking Files:

    - The `Unpack` method extracts files from the tar-like archive to a specified output folder.
    - It reads the archive, recreates the files, and stores them in the output folder.

### Requirements

- .NET Core SDK

### How to Run

1. Clone this repository
```bash
git clone https://github.com/TheDomCraft/MergeArchive.git
cd MergeArchive
```
2. Run the program
```bash
dotnet run pack output.mar file1.txt file2.png
```
or 
```bash
dotnet run unpack input.mar output_folder
```