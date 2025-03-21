#!/bin/bash

# generate-index.sh
# Script to generate a top-level index.html file that lists all subdirectories
# and links to the index.html file inside each of them

# Define the output file
OUTPUT_FILE="index.html"

# Generate the HTML header
cat > "$OUTPUT_FILE" << EOF
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Directory Index</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        h1 {
            color: #333;
            border-bottom: 1px solid #eee;
            padding-bottom: 10px;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        li {
            margin: 10px 0;
            padding: 10px;
            background-color: #f5f5f5;
            border-radius: 5px;
        }
        a {
            text-decoration: none;
            color: #0366d6;
            font-weight: bold;
        }
        a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <h1>Directory Index</h1>
    <ul>
EOF

# Find all directories (excluding hidden ones) in the current directory
for dir in */; do
    # Skip hidden directories
    if [[ "$dir" == .* ]]; then
        continue
    fi
    
    # Remove trailing slash from directory name
    dirname=${dir%/}
    
    # Check if the directory contains an index.html file
    if [ -f "$dir/index.html" ]; then
        # Add directory to the list with a link to its index.html
        echo "        <li><a href=\"$dir\">$dirname</a></li>" >> "$OUTPUT_FILE"
    fi
done

# Generate the HTML footer
cat >> "$OUTPUT_FILE" << EOF
    </ul>
    <p><small>Last updated: $(date)</small></p>
</body>
</html>
EOF

echo "Generated $OUTPUT_FILE successfully!"
