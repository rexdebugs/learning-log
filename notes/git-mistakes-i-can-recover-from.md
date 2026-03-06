# Git mistakes I can recover from

## 1) I edited a file and staged it, but I'm not ready to commit

- I can unstage it with: 'git restore --staged <file>'
- This keeps my edits, it only removes it from the staging area.

## 2) I edited a file and want to undo my changes

- I can restore the last committed version with: 'git restore <file>'
- This dicards uncommitted edits in my working folder.

## 3) I deleted a file by mistake

- If the file was committed before, I can bring it back with: 'git restore <file>'

## My calm checklist when I mess up

1. Run 'git status' to see what state I'm in.
2. If I staged something accidentally: 'git restore --staged <file>'
3. If I want to undo edits: 'git restore <file>'
4. If I deleted a committed file: 'git restore <file>'
