giDay 3 - Linux File Management & Permissions
Objective

Learn how Linux handles files, directories, permissions, ownership, and file searching.
Topics Covered

    Linux File Hierarchy

    Creating Files and Directories

    Copying Files

    Moving and Renaming Files

    Deleting Files

    Viewing File Contents

    Searching Files

    Finding Files

    File Permissions

    Ownership

    Wildcards

Important Commands
Check Current Directory

pwd

List Files

ls
ls -l

Create Directories

mkdir project
mkdir -p DevOps/Linux/Day3

Create Files

touch file1.txt
touch file2.txt
touch app.log db.log server.log

Copy Files and Directories

cp file1.txt backup.txt
cp -r DevOps BackupDevOps

Move and Rename Files

mv file1.txt file1_old.txt
mv file2.txt Archive/

Delete Files and Directories

rm backup.txt
rm -r BackupDevOps

View File Content

cat notes.txt
head notes.txt
tail notes.txt
less notes.txt

Search Content

grep Docker notes.txt
grep -i docker notes.txt

Find Files

find . -name notes.txt
find . -name "*.txt"

File Permissions

ls -l
chmod +x notes.txt
chmod 755 notes.txt
chmod 600 notes.txt

Ownership

sudo chown ubuntu notes.txt
sudo chgrp ubuntu notes.txt

Folder Structure

tree

Mini Project

Created a Linux file management project structure:

Day-03-File-Management
├── backup
│   └── notes.txt
├── docs
│   ├── linux_commands.txt
│   └── notes.txt
└── logs
    ├── app.log
    └── db.log

Learning Outcome

    Learned file and directory management.

    Practiced copying, moving, and deleting files.

    Learned to search files and content.

    Understood Linux permissions and ownership.

    Built a mini project using Linux commands.

Conclusion

Day 3 provided practical experience with Linux file operations and permissions, which are essential skills for DevOps, Cloud, Docker, Kubernetes, Jenkins, and System Administration.
