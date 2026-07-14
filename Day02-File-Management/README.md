# Day 02 - File and Directory Management

## Commands Learned

### mkdir
Used to create a new directory (folder).

Example:
mkdir project

### touch
Used to create an empty file.

Example:
touch notes.txt

### cp
Used to copy files or directories.

Example:
cp file1.txt file2.txt

### mv
Used to move or rename files/directories.

Example:
mv old.txt new.txt

### rm
Used to delete files.

Example:
rm file.txt

### rmdir
Used to delete an empty directory.

Example:
rmdir testfolder

---

# Interview Questions

### 1. What does mkdir do?

Answer:
Used to create a new directory (folder).

Example:
mkdir logs

---

### 2. Difference between cp and mv?

Answer:

cp:
Copies a file or directory and keeps the original.

Example:
cp file1.txt file2.txt

mv:
Moves or renames a file or directory.

Example:
mv file1.txt file2.txt

---

### 3. How do you rename a file?

Answer:

Using mv command.

Example:
mv oldname.txt newname.txt

---

### 4. What does rm -rf do?

Answer:

rm = remove

-r = recursive

-f = force

It forcefully deletes a directory and all its contents without asking for confirmation.

Example:
rm -rf project

Note: Use carefully because deleted files cannot be recovered easily.

---

### 5. Difference between rm -r and rmdir?

Answer:

rmdir:
Deletes only empty directories.

Example:
rmdir testfolder

rm -r:
Deletes directories along with all files and subdirectories.

Example:
rm -r project
