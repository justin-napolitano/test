# Sync Submodules Script

A shell script to initialize and update all Git submodules in a repository to their latest remote commits. It supports nested submodules and ensures synchronization across the entire project.

## Features

- Initializes submodules if they are not already initialized.
- Updates all submodules recursively to their latest commits from remote repositories.
- Validates that the script is run from the root of the repository by checking for the `.gitmodules` file.
- Provides clear success and error messages.

## Tech Stack

- Shell script (Bash)
- Git commands for submodule management

## Getting Started

### Prerequisites

- Git installed on your system
- A cloned repository containing submodules

### Installation and Usage

1. Save the script `gh_submodule_sync.sh` to your local repository root.
2. Make the script executable:
   ```sh
   chmod +x gh_submodule_sync.sh
   ```
3. Run the script:
   ```sh
   ./gh_submodule_sync.sh
   ```

## Project Structure

```
├── gh_submodule_sync.sh  # Script to sync submodules
├── index.md              # Documentation file
└── README.md             # This README file
```

- `gh_submodule_sync.sh`: The main shell script to initialize and update submodules.
- `index.md`: Additional documentation with usage and explanation.
- `README.md`: Project overview and instructions.

## Future Work / Roadmap

- Add argument support to specify branches or tags for submodules.
- Enhance error handling with detailed logs.
- Add support for dry-run mode to preview changes.
- Integrate with CI pipelines to automate submodule syncing.
- Provide support for other version control systems or submodule alternatives.
