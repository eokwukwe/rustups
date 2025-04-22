# minigrep

A simple `rust` command line tool that interacts with file and command line input/output. This is a simplified version of the classic command line search tool grep (globally search a regular expression and print). In the simplest use case, grep searches a specified file for a specified string. To do so, grep takes as its arguments a file path and a string. Then it reads the file, finds lines in that file that contain the string argument, and prints those lines.

The sample file is `poem.txt`. 

To run the program:
```bash
cargo run -- <search word> <file to search> > <output file>

E.g.
cargo run -- to poem.txt > output.txt
```

The default search is **case-sensitive**. To make the search **case-insensitive**, set the env variable `IGNORE_CARE` to `true`.
```bash
//case-insensitive search

IGNORE_CASE=1 cargo run -- TO poem.txt > output.txt

```
