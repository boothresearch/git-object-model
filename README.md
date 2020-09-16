# git-object-model

 - Don't believe me that, behind its scary exterior, Git is just a bunch of plain ol' files?
 - Let's give it a whirl. [Create a workspace by clicking here](https://gitpod.io/#https://github.com/boothresearch/git-object-model).
 - For your experimentation, commands that you will need:
    - To list the contents of the `.git/objects` folder,

        ```shell
        ls .git/objects -I "info" -I "pack" -R
        ```
        
    (Notice that the files are actually stored in subfolders that start with the first two characters of the digest, for performance reasons.)
    - To pretty-print the contents of an object with a SHA starting with e.g. `3b18e512` (the first 6 or 7 characters will do),

        ```shell
        git cat-file -p 3b18e512
        ```
 - Create a new file called "first.md", commit it, and try listing the content of .git/objects.
 - Use `git cat-file` to read each object. Add another file, commit it, and repeat.
 - Check out the contents of `.git/refs`.
 - Explore and ask questions!
 
