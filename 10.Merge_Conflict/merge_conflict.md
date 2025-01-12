# Merge Conflict

A **merge conflict** occurs in Git when changes from two branches cannot be automatically merged because they modify the same part of a file in conflicting ways. Git cannot decide which changes to keep, so it stops the merge process and marks the conflicting sections in the affected files.

## Example

### Scenario
- Branch `main` modifies line 10 of `file.txt`.
- Branch `feature` also modifies line 10 of `file.txt` differently.

### Conflict Resolution
- Git marks the conflict with `<<<<<<<`, `=======`, and `>>>>>>>` in the file.
- You need to manually edit the file to choose or combine the changes.

## Steps to Resolve
1. Open the conflicting file and resolve the conflict.
2. Stage the resolved file using:
   ```bash
   git add <file>

