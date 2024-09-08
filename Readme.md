1. Make directory
2. masuk ke dir baru
3. git init
4. git config user.name isiin username GitHub
5. git config user.email email GitHub
6. git checkout -b main


alur hands-on
1. create repository bari
2. bukin file baru
3. modify existing file
4. create branch baru `git checkout -b add/file`
5. add new file ke staging: `git add .` atau `git add namafile`
5. commit branch baru `git commit -m "adding readme file"`
6 lihat log: `git log -n2` `-n`: untuk mendefinikasi banyaknya log commit yang mau dilihat
7. menyimpan perubahan ke stash area karna masih Work in progress `git stash`
8. pindah branch dari add/file ke main:
    - `git checkout -b main` (branch main baru)
    - `git checkout main` (jika branch sudah ada)
9. kembalikan ke stash WIP `git stash pop`
10. Tambahkan beberapa line di test.txt
11. `git add test.txt`
12. Commit perubahan di test.txt: `git commit -m "menambahkan beberapa line"`
13. Melihat perubahan line di file Readme.md: `git diff Readme.md`
14. Add Readme.md ke staging area: `git add Readme.md`
15. Commit perubahan di Readme.md: `git commit -m "menambahkan step git"`
16. Melihat log lebih simple: `git log --oneline`
17. Checkout main: `git checkout main`
18. Bikin branch baru dari main: git checkout add/features
19. Add some lines ke Readme.md
20. Git add Readme.md: git add Readme.md
21. Commit Readme.md: git add Readme.md lalu git commit -m "add failed line"
22. Merge add/features branch ke add/file:
    - git checkout add/file
    - git merge add/features

6. push branch baru ke remote
