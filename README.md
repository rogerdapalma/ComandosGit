
```markdown
# Comandos Básicos do Git e GitHub

## 1. Configurar Git
Configura o Git com seu nome e e-mail. Essas informações serão usadas para identificar as suas contribuições.

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@example.com"
```

## 2. Inicializar um Repositório
Inicia um novo repositório Git em um diretório existente.

```bash
git init
```

## 3. Clonar um Repositório
Clona um repositório Git existente para sua máquina local.

```bash
git clone <URL_DO_REPOSITÓRIO>
```

## 4. Verificar Status
Mostra o estado atual do repositório (arquivos modificados, preparados para commit, etc.).

```bash
git status
```

## 5. Adicionar Arquivos ao Stage
Adiciona arquivos ou diretórios ao stage para serem preparados para commit.

```bash
git add <ARQUIVO>
# Adiciona todos os arquivos modificados
git add .
```

## 6. Fazer um Commit
Registra as mudanças adicionadas ao stage com uma mensagem descritiva.

```bash
git commit -m "Sua mensagem de commit"
```

## 7. Ver Histórico de Commits
Exibe o histórico de commits no repositório.

```bash
git log
```

## 8. Sincronizar Repositório com o GitHub

### 8.1. Adicionar um Repositório Remoto
Adiciona um repositório remoto (como o do GitHub) ao seu repositório local.

```bash
git remote add origin <URL_DO_REPOSITÓRIO>
```

### 8.2. Enviar Mudanças (Push)
Envia as mudanças locais para o repositório remoto.

```bash
git push origin main
```

## 9. Baixar Mudanças (Pull)
Baixa as mudanças mais recentes do repositório remoto para seu repositório local.

```bash
git pull origin main
```

## 10. Criar e Alternar Branches

### 10.1. Criar um Novo Branch
Cria um novo branch para trabalhar em uma funcionalidade separada.

```bash
git branch <NOME_DO_BRANCH>
```
```bash
git checkout -b <NOME_DO_BRANCH>
```

### 10.2. Alternar para um Branch
Muda para um branch específico.

```bash
git checkout <NOME_DO_BRANCH>
```

## 11. Mesclar Branches
Mescla o branch selecionado ao branch atual.

```bash
git merge <NOME_DO_BRANCH>
```

## 12. Excluir um Branch
Remove um branch local após ele ter sido mesclado ou não ser mais necessário.

```bash
git branch -d <NOME_DO_BRANCH>
```

## 13. Ver Branches
Lista todos os branches locais no repositório.

```bash
git branch
```

## 14. Clonar um Repositório
Se você quer clonar (copiar) um repositório para sua máquina local.

```bash
git clone <URL_DO_REPOSITÓRIO>
```

## 15. Reverter um Commit
Desfaz um commit local. Isso pode ser útil se você quiser desfazer um erro.

```bash
git reset --hard <HASH_DO_COMMIT>
```

## 16. Verificar Diferenças
Mostra as diferenças entre o diretório de trabalho e o último commit.

```bash
git diff
```

## 17. Stash de Mudanças
Guarda temporariamente as mudanças que ainda não estão prontas para commit.

```bash
git stash
```

## 18. Recuperar Mudanças do Stash
Aplica mudanças que foram guardadas com o comando `git stash`.

```bash
git stash pop
```

## 19. Ver Logs do Stash
Mostra uma lista de stashes que foram salvos.

```bash
git stash list
```


## 20. Abrir editor dentro do VScode
Clicando `.` no seu repositorio, ele abrirá o editor online no github
