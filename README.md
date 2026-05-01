# Aula de git e github

## Novos comandos para o git

### Comandos

# 📋 Listar todas as branches existentes
$ git branch
* main # o asterisco mostra a branch atual

# 🌿 Criar uma nova branch chamada "feature/login"
$ git branch feature/login

# 🔀 Mudar para a branch feature/login
$ git checkout feature/login
Switched to branch 'feature/login'

# 💡 Atalho moderno: criar + mudar de uma vez (use sempre este!)
$ git checkout -b feature/cadastro
Switched to a new branch 'feature/cadastro'

# 💼 Trabalho na nova feature... edita arquivos, faz commits...
$ echo "função de cadastro" > cadastro.py
$ git add . && git commit -m "feat: adiciona tela de cadastro"

# 🔙 Voltar para a main quando terminar
$ git checkout main

# 🤝 Juntar (merge) a feature na main
$ git merge feature/cadastro
Updating a3f5b9c..7e2c1d4
Fast-forward
cadastro.py | 1 +

# 🗑️ Deletar a branch (já foi mesclada, não precisa mais)
$ git branch -d feature/cadastro
