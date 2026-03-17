# Linux Basic Commands Assignment

**Course:** Networking
**Name:** Umutoniwase Benefice
**ID:** 27368

---

## Environment Details

* **Operating System:** Ubuntu Linux (running on Oracle VirtualBox)
* **Username:** vboxuser
* **Shell:** Bash
* **Host OS:** Windows

This assignment was completed using the Ubuntu terminal. All commands were executed manually to demonstrate understanding of Linux directory management, navigation, and file copying using both relative and absolute paths.

---

## Objective of the Assignment

The objective of this assignment is to:

* Understand Linux directory structures
* Practice creating nested directories
* Navigate directories using terminal commands
* Copy directories and files using relative and absolute paths
* Understand the difference between copying a directory and copying files inside a directory
* Interpret terminal colors and warning messages

---

## Directory Structure Creation

A main directory called `Practice` was created in the home directory. Inside `Practice`, the following directories were created:

* Command
* Else
* P1
* P2

Inside `P1`, a nested directory structure was created:

```
P1 → Hi → Hello → P3 → Here
```

### Commands Used

```bash
mkdir -p Practice/P1/Hi/Hello/P3/Here
mkdir -p Practice/Command
mkdir -p Practice/Else
mkdir -p Practice/P2
```

---

## Verifying Directory Structure

To verify that all directories were created correctly, the recursive list command was used:

```bash
ls -R Practice
```

This command displays all directories and subdirectories starting from the `Practice` folder.

---

## Navigation Commands Used

The following commands were used throughout the assignment:

* `cd` – change directories
* `pwd` – print current directory
* `ls` – list directory contents

### Example

```bash
cd ~/Practice/P2
pwd
```

---

## Question 3 – Copying a Directory

### Concept

The goal was to copy the entire directory `P3`, including all its contents, into the `Command` directory.

When copying directories in Linux, the `-r` (recursive) option must be used.

### Command (Relative Path)

```bash
cp -r ../P1/Hi/Hello/P3 ../Command
```

This copies the directory `P3` itself along with all its contents.

### Verification

```bash
ls ../Command
```

---

## Question 4 – Copying Files Only

### Concept

Only the files inside the `P3` directory were copied, not the directory itself.

This was done using the wildcard `*`, which matches all files in a directory.

### Commands

**Relative Path:**

```bash
cp ../P1/Hi/Hello/P3/* ../Command
```

**Absolute Path:**

```bash
cp /home/vboxuser/Practice/P1/Hi/Hello/P3/* /home/vboxuser/Practice/Command
```

### Important Note

Warnings such as:

```
Is a directory
```

are expected because `*` does not include directories unless `-r` is used.

---

## Difference Between Question 3 and Question 4

* **Question 3:** Copies the entire `P3` directory (including subdirectories and files)
* **Question 4:** Copies only the files inside `P3`, not the directory itself

---

## File and Directory Colors in Linux

Linux uses colors in the terminal to distinguish file types:

* **Blue:** Directories
* **White (default):** Regular files

The directory `Here` appears in blue because it is a directory.

---

## What I Learned

* Creating nested directories using `mkdir -p`
* Navigating directories using `cd` and `pwd`
* Understanding relative vs absolute paths
* Copying directories vs copying files
* Interpreting Linux terminal warnings and colors

---

## Conclusion

This assignment provided hands-on experience with Linux file system management and improved my confidence in using terminal commands. These skills are essential for working effectively in a Linux environment.
