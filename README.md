## README

# Directory Index Generator

A simple bash script that automatically generates an `index.html` file in your repository's root directory, listing all subdirectories and linking to their respective `index.html` files.

## Purpose

This tool is designed for repositories that consist of multiple named folders, each containing an `index.html` file. Instead of manually updating the main `index.html` file each time you add a new directory, this script does it for you automatically.

## Installation

1. Download the `generate-index.sh` script to your repository's root directory
2. Make the script executable:
   ```bash
   chmod +x generate-index.sh
   ```

## Usage

After adding a new directory with an `index.html` file, simply run:

```bash
./generate-index.sh
```

The script will:
- Create or overwrite the top-level `index.html` file
- Find all subdirectories containing an `index.html` file
- Generate links to each directory in a clean, styled list
- Add a timestamp showing when the index was last updated

## Features

- Ignores hidden directories (those starting with a dot)
- Only includes directories that actually contain an `index.html` file
- Creates a responsive, mobile-friendly layout
- Includes basic styling for a clean presentation

## Customization

You can modify the HTML and CSS in the script to change the appearance of your index page. Look for the section between the `cat > "$OUTPUT_FILE" << EOF` and the first `EOF` to make styling changes.

## License

This script is released under the MIT License. Feel free to modify and use it as needed for your projects.

