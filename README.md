## Installation

Ensure you have Node.js installed. Clone the repository and navigate to the project directory.

```git clone https://github.com/vladyslavfolkuian/size.git```

Install dependencies:

```npm install```

## Usage
Run the program using Node.js with the following command:

```node index.js [folder-name]```

Replace ```[folder-name]``` with the directory you want to analyze.

## Example

Running ```node index.js [folder-name]``` will generate a JSON file ```[folder-name]-size.json``` with content similar to:

```json
{
  "files": [
    {
      "filePath": "myFolder/file1.json",
      "size": 1024,
      "formattedSize": "1 KiB"
    },
    {
      "filePath": "myFolder/file2.webp",
      "size": 500,
      "formattedSize": "500 Bytes"
    },
    {
      "filePath": "myFolder/subfolder/file3.webp",
      "size": 2048,
      "formattedSize": "2 KiB"
    }
  ],
  "totalSize": "3.50 KiB",
  "totalSizeInBytes": 3572
}
```
## Description:

- **Title**: `getDirectorySize()`
- **Summary**: This Node.js program calculates the total size of `.webp` and `.json` and `.mp3` files within a specified directory. It outputs detailed information in a JSON file, including individual file sizes, formatted sizes, and the total size.
- **Author**: vladyslavfolkuian
