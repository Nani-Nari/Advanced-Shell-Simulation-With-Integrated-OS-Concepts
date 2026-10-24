# Advanced Shell Simulation — Deliverable 1

A Python-based Unix-like shell demonstrating basic command execution, built-in utilities, foreground and background processes, and job control.

## Requirements
- Python 3.9 or later
- Linux, macOS, or Windows Subsystem for Linux (WSL)

> This project relies on POSIX signals and is not compatible with native Windows Command Prompt or PowerShell.

## Run
```bash
python3 myshell.py
```

## Built-in commands
`cd`, `pwd`, `exit`, `echo`, `clear`, `ls`, `cat`, `mkdir`, `rmdir`, `rm`, `touch`, `kill`, `jobs`, `fg`, `bg`, `stop`, `help`.

## Examples
```text
pwd
echo Hello from myshell
mkdir demo
cd demo
touch notes.txt
ls -l
cd ..
rmdir demo
sleep 30 &
jobs
stop 1
bg 1
fg 1
fakecommand
exit
```

Job numbers and process IDs depend on the current session. To stop a foreground job, press Ctrl+Z; Ctrl+C interrupts it.

## Report
See `docs/` for the APA 7 report in Word formats, including terminal execution figures.

## Limitations
This is an educational shell, not a full Bash replacement. It does not support pipes, redirection, or full terminal foreground-process-group control.
