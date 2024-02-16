# Design of a Git Repository

- The git repository is divided into two parts:

    1. ```index```

    2. ```object database``` also known as *Git's memory bank*

## Index

- When we run an ```add``` command, git makes a copy of the file in the index

- We can think of this area as the ```staging area``` where files to be committed
are *tracked*

- If you add a file *again*, it'll get *overwritten* in the ```index```

- However, files are not deleted from the index after a commit

- Therefore, the index keeps growing as more files are added to it

## Object Database

- When we run a ```commit``` command, git:

    1. Copies the contents of the ```index```

    2. Stores them into its memory banks

    3. Represents that version with a commit object

- This means that git now has a third copy of your file(s)
