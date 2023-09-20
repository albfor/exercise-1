# Exercise 1

## Walkthrough
1. Create a directory called exercise-1 and move into it.
```bash
mkdir exercise-1
cd exercise-1
```
2. Create a repository and run **git status** and **git log**.
```bash
git init
```
```bash
git status
```
```bash
git log
```
3. Create **README.md** and write **# Exercise 1** to it.
```bash
echo "# Exercise 1" > README.md
```
4. Run **git status**. You should have an **untracked** file. 
```bash
git status
```
5. **Try** to remove **README.md** using **git rm**. Remove the file using the bash command **rm**.
```bash
git rm README.md
```
```bash
rm README.md
```
6. Do **step 3** and add **README.md** to the **staging** area of the repo.

See step 3.
```bash
git add README.md
```
7. Run **git status** and **unstage** the change using **git rm**.
```bash
git status
```
```bash
git rm --cached README.md
```
