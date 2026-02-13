# GitHub Actions Lab

## Workflow 1 – Dependent Jobs
- **Purpose:** Demonstrates job dependencies using `needs`.
- **Jobs:** build → test → deploy
- **Key Concepts:** 
  - `needs:` creates sequential execution.
  - `runs-on:` specifies the OS.
  - Multiple steps per job simulate real tasks.

## Workflow 2 – Multi-Platform Testing
- **Purpose:** Demonstrates independent jobs running in parallel on different OS.
- **Jobs:** ubuntu-job, windows-job, macos-job
- **Key Concepts:**
  - Jobs without `needs:` run simultaneously.
  - OS-specific commands (`uname -a`, `systeminfo`) show platform behavior.
  - Creating and viewing files in each OS demonstrates basic CI steps.

## Challenges
- YAML syntax errors are common → always validate before push.
- YAML file has to change main to master
- Windows commands differ from Linux/macOS → used `type` instead of `cat`.

## Screenshots
- Include workflow file content and Actions tab views.
