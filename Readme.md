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
6. commit branch baru `git commit -m "adding readme file"`
7 lihat log: `git log -n2` `-n`: untuk mendefinikasi banyaknya log commit yang mau dilihat
8. menyimpan perubahan ke stash area karna masih Work in progress `git stash`
9. pindah branch dari add/file ke main:
    - `git checkout -b main` (branch main baru)
    - `git checkout main` (jika branch sudah ada)
10. kembalikan ke stash WIP `git stash pop`
11. Tambahkan beberapa line di test.txt
12. `git add test.txt`
13. Commit perubahan di test.txt: `git commit -m "menambahkan beberapa line"`
14. Melihat perubahan line di file Readme.md: `git diff Readme.md`
15. Add Readme.md ke staging area: `git add Readme.md`
16. Commit perubahan di Readme.md: `git commit -m "menambahkan step git"`
17. Melihat log lebih simple: `git log --oneline`
18. Checkout main: `git checkout main`
19. Bikin branch baru dari main: `git checkout add/features`
20. Add some lines ke Readme.md
21. Git add Readme.md: `git add Readme.md`
22. Commit Readme.md: `git add Readme.md` lalu `git commit -m "add failed line"`
23. Merge add/features branch ke add/file:
    - `git checkout add/file`
    - `git merge add/features`

24. push branch baru ke remote
25. Create Repository di Github
26. Copy url repository di Github
27. Check remote list: `git remote -v`
28. git push ke remote: `git remote add origin https://github.com/gmkhai/belajar_github.git`



# How to make conflicted file:
1. `git checkout add/file`
2. Adding new line di text.txt
3. `git add test.txt`
4. `git commit -m "adding new line"`
5. `git checkout fix/readme`
6. Adding new line to text.txt in the same line as add/file
7. `git stash`
8. `git merge add/file`
9. `git stash pop`


# Resolve conflict:
1. Kalau terjadi conflict seperti gambar di bawah ini:

![Screenshot 2024-09-08 125054.png](<Screenshot 2024-09-08 125054.png>)

2. Yang perlu kita lakukan:
    - Diskusikan dengan team mates mana yang bener
    - Apakah accept both changes, incoming changes, current changes
    - Klik salah satu antara ketiga pilihan itu
    - save file
    - `git status`: untuk melihat status git repository

    ![alt text](<Screenshot 2024-09-08 125246.png>)
    - `git add Readme.md`
    - `git commit -m "message"`
    - `git push origin nama-branch`
