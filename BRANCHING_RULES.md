# IRC Rover Git Workflow

## Branches

- main: stable, competition-ready code only
- integration: subsystem merge and testing branch
- p10-p21: role-specific development branches

## Rules

1. Do not push directly to main.
2. Each role works only in their assigned branch.
3. Completed work is merged into integration first.
4. integration is tested before merging into main.
5. Version-specific ROS files must be clearly labeled.

## ROS Version Rule

- Common code should remain compatible with ROS 2 Humble and ROS 2 Jazzy where possible.
- Humble-only files should be placed in folders ending with `_humble`.
- Jazzy-only files should be placed in folders ending with `_jazzy`.

## Do Not Commit

- build/
- install/
- log/
- .venv/
