# delolder

A Bash script that deletes files older than a specified number of days.

## Usage

```bash
./delolder [-v|-d] N [--] dirs
```

### Options

- `-v` : Verbose mode. Prints each deleted file.
- `-d` : Dry-run mode. Prints files that would be deleted without deleting them.
- `--` : Ends option parsing, allowing directory names beginning with `-`.

## Examples

Dry run:

```bash
./delolder -d 10 test_dir
```

Verbose delete:

```bash
./delolder -v 10 test_dir
```

Delete silently:

```bash
./delolder 10 test_dir
```
