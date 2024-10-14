# Exports-Tree

Run `npx exports-tree` to display the export structure of JavaScript or TypeScript files, starting from a specified directory and up to a defined depth.

### Options:
- `--version`  
  Show the version number. `[boolean]`
  
- `-p, --path`  
  Path to start scanning from. `[string]` (default: `"."`)
  
- `-d, --depth`  
  Maximum depth to traverse. `[number]`
  
- `-i, --ignore`  
  Patterns to ignore (e.g., directories or file types). `[array]`  
  (default: `["node_modules", ".git", ".husky", "coverage", ".next"]`)
  
- `--help`  
  Show help information. `[boolean]`

### Notes:
- When specifying options like `-d` (depth) or `-i` (ignore), you **must explicitly provide a path**. You can use `.` to represent the current directory.
  
### Examples:
1. To display the export structure with a depth of 2 levels, run:
   npx exports-tree . -d 2

2. To display the export structure of a specific project with a depth of 2 levels and ignoring .png files, run:
    npx exports-tree /path/to/project -d 2 -i .png
