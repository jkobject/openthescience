# OpenTheScience Repository Instructions

**ALWAYS follow these instructions first and only fallback to additional search and context gathering if the information here is incomplete or found to be in error.**

## Repository Overview
OpenTheScience is a minimal repository focused on "opening science" with the goal of making scientific knowledge and processes more accessible. Currently, it contains only foundational files but is structured to grow into a larger project.

## Working Effectively

### Repository Bootstrap and Exploration
- Clone the repository: `git clone <repository-url>`
- Navigate to repository: `cd openthescience`
- Check repository status: `git status --porcelain`
- Explore repository structure: `ls -la` (shows README.md, LICENSE, .github/)
- View commit history: `git log --oneline -10`

### Current Repository State (Validated Commands)
**All commands below have been validated to work:**

- `ls -la` - Lists all files including hidden directories
- `cat README.md` - Shows: "just open the f*** science"
- `cat LICENSE` - Shows full Unlicense (public domain) license text
- `git status` - Always shows clean working tree (validated)
- `git log --oneline` - Shows minimal commit history
- `find . -type f -name "*.md"` - Finds documentation files
- `find . -name ".*" -type d` - Finds hidden directories (.git, .github)

### Build and Test Instructions
**IMPORTANT: This repository currently has NO build system, dependencies, or tests.**

- **DO NOT attempt to run:** `npm install`, `pip install`, `make`, `cargo build`, or similar build commands
- **NO package.json, requirements.txt, Cargo.toml, or other dependency files exist**
- **NO test directories or test files exist**
- **NO CI/CD workflows exist in .github/workflows/**

### Development Workflow
Since this is a minimal repository:

1. **Before making changes:**
   - `git status` - Verify clean working tree
   - `git branch` - Check current branch
   - `ls -la` - Verify repository contents

2. **After making changes:**
   - `git add .` - Stage changes
   - `git status` - Review staged changes
   - `git commit -m "descriptive message"` - Commit changes
   - `git push` - Push to remote

3. **Repository exploration:**
   - `find . -type f` - List all files
   - `git ls-files` - List tracked files (currently: LICENSE, README.md)

## Validation Requirements
**Manual validation steps for any changes:**

1. **Always verify these commands work after changes:**
   - `cd /path/to/repo && ls -la` - Should show README.md, LICENSE, .github/
   - `git status` - Should show current status without errors
   - `cat README.md` - Should display content without errors

2. **File structure validation:**
   - Repository root should contain: README.md, LICENSE, .github/, .gitignore
   - .github/ should contain: copilot-instructions.md (this file)
   - **NO build artifacts, dependencies, or temporary files should be committed**

## Repository Structure Reference
```
openthescience/
├── .git/                    # Git repository metadata
├── .github/                 # GitHub configuration
│   └── copilot-instructions.md
├── .gitignore              # Files to exclude from git
├── LICENSE                  # Unlicense (public domain)
└── README.md               # Project description
```

## Common Tasks and Expected Outcomes

### Repository Information Commands
- `git remote -v` - Shows origin remote URL
- `git branch -a` - Shows all branches including remote tracking
- `wc -l README.md LICENSE` - Shows line counts (README: 2 lines, LICENSE: 24 lines)

### File Content Verification
- README.md contains exactly: "# openthescience\njust open the f*** science\n"
- LICENSE contains full Unlicense public domain dedication
- No other source files, configuration files, or build scripts exist

## Future Development Guidelines
When this repository grows beyond its current minimal state:

1. **Before adding build systems:**
   - Update these instructions with exact build commands
   - Include timeout requirements for builds (use 60+ minute timeouts)
   - Add "NEVER CANCEL" warnings for long-running processes

2. **Before adding tests:**
   - Document exact test commands and expected runtime
   - Include validation scenarios that must pass
   - Add linting and formatting requirements

3. **Before adding dependencies:**
   - Document exact installation commands
   - Include any environment setup requirements
   - Validate all dependency installation steps

## Critical Reminders
- This repository is PUBLIC DOMAIN (Unlicense) - no copyright restrictions
- Repository purpose: "opening science" - making scientific knowledge accessible
- Current state: Minimal/starter repository with room for growth
- **NO build system exists** - do not attempt build operations
- **NO tests exist** - do not attempt test execution
- Always check `git status` before and after making changes