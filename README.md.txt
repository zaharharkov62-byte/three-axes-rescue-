User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4)
$ git init
Initialized empty Git repository in C:/Users/User/Desktop/Новая папка (4)/.git/

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md.txt

nothing added to commit but untracked files present (use "git add" to track)

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git add ^C

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ ^[[200~ ^C
bash: $'\E[200~': command not found

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git add README.md
fatal: pathspec 'README.md' did not match any files

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md.txt

nothing added to commit but untracked files present (use "git add" to track)

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ cat > app-config.json << 'EOF'
{
  "appName": "IT Kingdom Production",
  "version": "1.0.0",
  "database": {
    "host": "localhost",
    "port": "5432",
    "username": "admin",
    "password": "password123",
    "name": "production_db"
  },
  "server": {
    "port": 3000,
    "host": "0.0.0.0",
    "debug": true
  },
  "features": {
    "enableMagic": true,
    "enableCurses": true,
    "batteryDrain": "5min",
    "cloudDirection": "down",
    "dataFlow": "reverse"
  },
  "cache": {
EOF "ttl": 0y": "evaporate",

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git add app-config.json
warning: in the working copy of 'app-config.json', LF will be replaced by CRLF the next time Git touches it

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git commit -m "Initial: damaged config from Koschey"
[master (root-commit) 12d8c89] Initial: damaged config from Koschey
 1 file changed, 28 insertions(+)
 create mode 100644 app-config.json

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ cat > app-config.json << 'EOF'
{
  "appName": "IT Kingdom Production",
  ... (содержимое файла)
}
EOF

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git add app-config.json
warning: in the working copy of 'app-config.json', LF will be replaced by CRLF the next time Git touches it

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git commit -m "Initial: damaged config from Koschey"
[master 45a94b2] Initial: damaged config from Koschey
 1 file changed, 1 insertion(+), 25 deletions(-)

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git rm app-config.json
rm 'app-config.json'

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ cat > backup-config.json << 'EOF'
{
  "appName": "IT Kingdom Production",
  "version": "1.0.0",
  "database": {
    "host": "db.it-kingdom.ru",
    "port": 5432,
    "username": "app_user",
    "password": "secure_password_here",
    "name": "production_db"
  },
  "server": {
    "port": 3000,
    "host": "0.0.0.0",
    "debug": false
  },
  "features": {
    "enableMagic": true,
    "enableCurses": false,
    "batteryOptimization": true,
    "cloudDirection": "up",
    "dataFlow": "normal"
  },
  "cache": {
EOF "endpoint": "https://monitor.it-kingdom.ru"

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git mv backup-config.json app-config.json
fatal: not under version control, source=backup-config.json, destination=app-config.json

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git commit -m "Recovery: restored working config from backup"
[master a78a818] Recovery: restored working config from backup
 1 file changed, 4 deletions(-)
 delete mode 100644 app-config.json

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git add .gitignore
git commit -m "Security: added .gitignore rules to protect from future attacks"
fatal: pathspec '.gitignore' did not match any files
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md.txt
        backup-config.json

nothing added to commit but untracked files present (use "git add" to track)

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ echo "=== ИСТОРИЯ КОММИТОВ ==="
git log --oneline

echo -e "\n=== ВОССТАНОВЛЕННЫЙ КОНФИГ ==="
cat app-config.json

echo -e "\n=== ФАЙЛ .gitignore ==="
cat .gitignore
=== ИСТОРИЯ КОММИТОВ ===
a78a818 (HEAD -> master) Recovery: restored working config from backup
45a94b2 Initial: damaged config from Koschey
12d8c89 Initial: damaged config from Koschey

=== ВОССТАНОВЛЕННЫЙ КОНФИГ ===
cat: app-config.json: No such file or directory

=== ФАЙЛ .gitignore ===
cat: .gitignore: No such file or directory

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md.txt
        backup-config.json

nothing added to commit but untracked files present (use "git add" to track)

User@DESKTOP-I6DQE1D MINGW64 ~/Desktop/Новая папка (4) (master)
$
