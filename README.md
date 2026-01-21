# Operation Rescue
User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$ mkdir ~/Desktop/three-axes-rescue
mkdir: cannot create directory ‘/c/Users/User/Desktop/three-axes-rescue’: File exists

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$ cd ~/Desktop/three-axes-rescue

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$ pwd
/c/Users/User/Desktop/three-axes-rescue

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$ git init
Reinitialized existing Git repository in C:/Users/User/Desktop/three-axes-rescue/.git/

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$ git add README.md

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$ git commit -m "Initial commit: rescue operation"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$ git remote add origin https://githab.com/zaharharkov62-byte/three-axes-rescue.git
error: remote origin already exists.

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$ git push -u origin main
branch 'main' set up to track 'origin/main'.
Everything up-to-date


User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/three-axes-rescue (main)
$ cd ~/Desktop

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop
$ mkdir backup-computer
cd backup-computer
mkdir: cannot create directory ‘backup-computer’: File exists

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ git clone https://github.com/zaharharkov62-byte/three-axes-rescue.git
Cloning into 'three-axes-rescue'...
remote: Repository not found.
fatal: repository 'https://github.com/zaharharkov62-byte/three-axes-rescue.git/' not found

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ cd three-axes-rescue
bash: cd: three-axes-rescue: No such file or directory

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ ls
''$'\026''ssh -T git@github.com'  ''$'\026''ssh -T git@github.com.pub'

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ git remote -v
fatal: not a git repository (or any of the parent directories): .git

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ git log --oneline
fatal: not a git repository (or any of the parent directories): .git

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ ls -la
total 22
-rw-r--r-- 1 User 197121 419 Jan 22 02:02 ''$'\026''ssh -T git@github.com'
-rw-r--r-- 1 User 197121 105 Jan 22 02:02 ''$'\026''ssh -T git@github.com.pub'
drwxr-xr-x 1 User 197121   0 Jan 22 02:16  ./
drwxr-xr-x 1 User 197121   0 Jan 22 02:00  ../

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ git pull origin main --allow-unrelated-histories
git push -u origin main
fatal: not a git repository (or any of the parent directories): .git
fatal: not a git repository (or any of the parent directories): .git

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ ls -la ~/.ssh/
total 14
drwxr-xr-x 1 User 197121   0 Jan 22 01:50 ./
drwxr-xr-x 1 User 197121   0 Jan 22 01:50 ../
-rw-r--r-- 1 User 197121 419 Jan 22 01:50 id_ed25519
-rw-r--r-- 1 User 197121 104 Jan 22 01:50 id_ed25519.pub

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ ssh-keygen -t rsa -b 4096 -C "zaharharkov62@gmail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/User/.ssh/id_rsa):
Enter passphrase for "/c/Users/User/.ssh/id_rsa" (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/User/.ssh/id_rsa
Your public key has been saved in /c/Users/User/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:QMHCTio9xQs7f1KIyHpziB2M4hCLvXGT46Cl+8cYkMQ zaharharkov62@gmail.com
The key's randomart image is:
+---[RSA 4096]----+
|.  o .o.         |
|.E. *..          |
|+X O =.          |
|@.# O ..         |
|=O % +  S        |
|=.B = .          |
| o * o           |
|. . o            |
| ...             |
+----[SHA256]-----+

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ git remote -v
fatal: not a git repository (or any of the parent directories): .git

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ git log --oneline
fatal: not a git repository (or any of the parent directories): .git

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ ls -la
total 22
-rw-r--r-- 1 User 197121 419 Jan 22 02:02 ''$'\026''ssh -T git@github.com'
-rw-r--r-- 1 User 197121 105 Jan 22 02:02 ''$'\026''ssh -T git@github.com.pub'
drwxr-xr-x 1 User 197121   0 Jan 22 02:16  ./
drwxr-xr-x 1 User 197121   0 Jan 22 02:00  ../

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/backup-computer
$ echo "=== ОТЧЕТ ДЛЯ ВАСИЛИСЫ ПРЕМУДРОЙ ==="
echo ""
echo "1. Ссылка на GitHub репозиторий:"
echo "https://githab.com/zaharharkov62-byte/three-axes-rescue"echo ""
echo "2. Проверка SSH:"
ssh -T git@github.com
=== ОТЧЕТ ДЛЯ ВАСИЛИСЫ ПРЕМУДРОЙ ===

1. Ссылка на GitHub репозиторий:
https://githab.com/zaharharkov62-byte/three-axes-rescueecho
2. Проверка SSH:
The authenticity of host 'github.com (140.82.121.4)' can't be established.
ED25519 key fingerprint is: SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
