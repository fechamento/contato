# contato
PS C:\Users\SAMSUNG\Desktop\Landing Page> ^C
PS C:\Users\SAMSUNG\Desktop\Landing Page> Set-Location -Path 'C:\Users\SAMSUNG\Desktop\Landing Page'; Write-Host "`n=== Status do Git ==="; 
git status; Write-Host "`n=== Configuração do Remote ==="; git remote 
-v

=== Status do Git ===
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)      
        .vscode/

=== Configuração do Remote ===
origin  https://github.com/operacaofechamento/contato.git (fetch)     
origin  https://github.com/operacaofechamento/contato.git (push)      
PS C:\Users\SAMSUNG\Desktop\Landing Page> git config --get user.name; 
git config --get user.email
PS C:\Users\SAMSUNG\Desktop\Landing Page> git config --global user.name "operacaofechamento"; git config --global user.email "leosiqueira2006@gmail.com"; Write-Host "`n=== Configurações do usuário ==="; git config --get user.name; git config --get user.email; Write-Host "`n=== Criando commit inicial ==="; git add .; git commit -m "Initial commit"; 
git branch -M main; Write-Host "`n=== Fazendo push ==="; git push -u origin main

=== Configurações do usuário ===
operacaofechamento
leosiqueira2006@gmail.com

=== Criando commit inicial ===
[main (root-commit) 56de814] Initial commit
 4 files changed, 129 insertions(+)
 create mode 100644 .vscode/fechamento
 create mode 100644 .vscode/launch.json
 create mode 100644 README.md
 create mode 100644 index.html

=== Fazendo push ===
info: please complete authentication in your browser...
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (7/7), 4.73 KiB | 372.00 KiB/s, done.
Total 7 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/operacaofechamento/contato.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\SAMSUNG\Desktop\Landing Page> ^C
PS C:\Users\SAMSUNG\Desktop\Landing Page> git status; Write-Host "`n=== Último commit ==="; git log --oneline -n 1; Write-Host "`n=== Tentando push novamente ==="; git push -u origin main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

=== Último commit ===
56de814 (HEAD -> main, origin/main) Initial commit

=== Tentando push novamente ===
branch 'main' set up to track 'origin/main'.
Everything up-to-date
PS C:\Users\SAMSUNG\Desktop\Landing Page> git remote set-url origin https://github.com/fechamento/contato.git; git push -u origin main      
remote: Permission to fechamento/contato.git denied to operacaofechamento.
fatal: unable to access 'https://github.com/fechamento/contato.git/': 
The requested URL returned error: 403
PS C:\Users\SAMSUNG\Desktop\Landing Page> 
