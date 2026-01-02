# Claudio Test Harness

Integration test harness for [claudio](https://github.com/jamie--stewart/claudio) containers.

## Purpose

This repo is used by automated integration tests to verify that claudio containers can:
- Clone repositories via SSH
- Create branches and commits
- Push to remote
- Create and merge pull requests

## Structure

```
runs/
├── claude-yolo.txt        # Counter for claude-yolo container tests
└── claude-yolo-swift.txt  # Counter for claude-yolo-swift container tests
```

Each file contains a run counter that gets incremented by integration tests.

## Usage

This repo is automatically updated by `make validate` in the claudio project.
