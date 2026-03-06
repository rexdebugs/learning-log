# Terminal Cheat Sheet (Day 8)

## Viewing files

-'cat file' = print entire file (small files)
-'less file' = scrollable viewer; search with '/word'; quit with 'q'
-'head file' = first 10 lines

- 'head -n 5 file' = first 5 lines
  -'tail file' = last 10 lines
  -'tail -n 5 file' = last 5 lines
  -'tail -f file' = follow file updates (quit with Ctrl+C)

## Searching inside files (skill check)

-'grep "text" file' = lines containing text
-'grep -i "text" file' = case-insensitive
-'grep -n "text" file' = show line numbers
-'grep -R "text" .' = search recursively in this folder

## Finding files by name

-'find . -name "name.txt"' = find exact filename under current folder
-'find . -name "\*.md"' = find all Markdown files

## Pipes + redirection

-'|' pipe = send output of left command into right command
-'ls | grep ".md"'
-'grep -R "WSL" . | less'
-'>' = write output to file (overwrite)
-'ls > files.txt'
-'>>' = append output to file
-'echo "note" >> notes.txt'

## Panic button

-'Ctrl + C' = stop a running command

SSH setup complete on Day 9.
