
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
### 5.1 Resetando Arquivo Adicionado

```bash
git reset <ARQUIVO>
```

## 6. Fazer um Commit
Registra as mudanças adicionadas ao stage com uma mensagem descritiva.

```bash
git commit -m "Sua mensagem de commit"
```

### 6.1 Em uma BRANCH e precisar comentar o commit
Aqui está uma explicação mais detalhada do processo de como realizar um commit no Git utilizando a interface do editor Vim:

    1. **Executar o comando de commit**:

    ```bash
    git commit
    ``` 
    
    Esse comando inicia o processo de commit, abrindo o editor de texto configurado no seu terminal (geralmente o Vim).

    2. **Entrar no modo de inserção (Insert Mode)**:
    - Quando o editor Vim abrir, você estará no modo normal (Normal Mode).
    - Para começar a editar o texto, pressione a tecla **`i`** no teclado. Isso ativa o modo de inserção, permitindo que você digite o texto da mensagem de commit.

    3. **Escrever a mensagem de commit**:
    - Digite a mensagem que descreve as alterações realizadas. Recomenda-se que a mensagem seja clara e concisa. Por exemplo:
       
        Adiciona função de cálculo de média no módulo de estatísticas
       
    - A primeira linha deve ser um resumo breve (50 caracteres ou menos). Caso deseje adicionar detalhes adicionais, pule uma linha e forneça mais informações.

    4. **Sair do modo de inserção e voltar para o modo normal**:
    - Pressione a tecla **`Esc`** para sair do modo de inserção e retornar ao modo normal.

    5. **Salvar as alterações e sair do editor**:
    - Digite **`:wq`** e pressione **Enter**.
        - **`:w`** salva as mudanças.
        - **`:q`** fecha o editor.

    Depois disso, o commit será concluído e registrado no histórico do Git.

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
### 10.2. Criando e entrando na Branch direto
```bash
git checkout -b <NOME_DO_BRANCH>
```

### 10.3. Alternar para um Branch
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
### 13.1 mostrando todas as Branches
```bash
git branch --all
```
### 14. Dando push na branch

```bash
git push -u origin <NOMEDOARQUIVO>
```
## 15. Clonar um Repositório
Se você quer clonar (copiar) um repositório para sua máquina local.

```bash
git clone <URL_DO_REPOSITÓRIO>
```

## 16. Reverter um Commit
Desfaz um commit local. Isso pode ser útil se você quiser desfazer um erro.

```bash
git reset --hard <HASH_DO_COMMIT>
```

## 17. Verificar Diferenças
Mostra as diferenças entre o diretório de trabalho e o último commit.

```bash
git diff
```

## 18. Stash de Mudanças
Guarda temporariamente as mudanças que ainda não estão prontas para commit.

```bash
git stash
```

## 19. Recuperar Mudanças do Stash
Aplica mudanças que foram guardadas com o comando `git stash`.

```bash
git stash pop
```

## 20. Ver Logs do Stash
Mostra uma lista de stashes que foram salvos.

```bash
git stash list
```


## 21. Abrir editor dentro do VScode
Clicando `.` no seu repositorio, ele abrirá o editor online no github
