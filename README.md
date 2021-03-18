# CanDrA Scripts

Scripts for downloading, compiling and running
[CanDrA v+](https://bioinformatics.mdanderson.org/public-software/candra/).

## Requirements

`Bash`, `Perl`, `make`, `wget`, `tar`, `jq`.

## Usage

```bash
# Display help
./task

# Download CanDrA
./task download-candra

# List available databases
./task list-db
# Download database
./task download-db <key>

# Prepare installation
./task prepare
# Run CanDrA
./task run <db-key> <file>
```
