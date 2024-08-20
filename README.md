# Exercício Prático: Introdução ao Git

## Objetivo
Este exercício tem como objetivo familiarizar você com os conceitos e comandos básicos do Git, incluindo a criação de repositórios, trabalho com branches e a simulação de um fluxo de colaboração.

## Passo a Passo

### 1. Criar um Repositório Local
1. **Inicialize um repositório Git vazio:**

   No terminal, navegue até o diretório onde deseja criar o repositório e execute o comando:
   ```bash
   git init
   ```
   Isso criará um repositório Git vazio no diretório atual.

### 2. Criar a Branch principal
1. **Crie uma nova branch chamada `main`:**
   ```bash
   git checkout -b main # ou git checkout -b master
   ```
   Agora, você está trabalhando na branch `main`.

### 3. Publicar o Repositório em uma Plataforma de Hospedagem
1. **Crie um novo repositório no GitHub/GitLab:**
   - Acesse GitHub/GitLab e crie um novo repositório.
   - Copie o URL do repositório remoto.

2. **Adicione o repositório remoto:**
   ```bash
   git remote add origin <URL-do-repositório>
   ```

3. **Envie as alterações para o repositório remoto:**
   ```bash
   git push -u origin main  # ou git push -u origin master
   ```

### 4. Criar uma Branch e Fazer um Commit
1. **Crie uma nova branch chamada `feature-x`:**
   ```bash
   git checkout -b feature-x
   ```
   Agora, você está trabalhando na branch `feature-x`.

2. **Crie um arquivo `README.md`:**

   No editor de texto de sua escolha, crie um arquivo chamado `README.md` e adicione o seguinte conteúdo:

   ```markdown
   # Projeto de Exemplo

   Este é um projeto de exemplo para praticar o uso do Git.
   ```

3. **Adicione o arquivo ao staging area:**
   ```bash
   git add README.md
   ```

4. **Faça o commit das alterações:**
   ```bash
   git commit -m "Adiciona README.md"
   ```

### 5. Mesclar a Branch `feature-x` na Branch Principal
1. **Volte para a branch principal (`main` ou `master`):**
   ```bash
   git checkout main  # ou git checkout master
   ```

2. **Mescle as alterações da branch `feature-x`:**
   ```bash
   git merge feature-x
   ```

   Isso integrará as alterações da branch `feature-x` na branch principal.

### 6. Criar um Pull Request (PR)
1. **No GitHub/GitLab, crie um Pull Request:**
   - Acesse o repositório remoto e crie um PR da branch `feature-x` para a branch principal.

2. **Descreva o PR:**
   - No PR, descreva as alterações feitas e por que elas devem ser mescladas na branch principal.

### 7. Revisão do Exercício
- **Verifique as mudanças:**
   - Veja as alterações que foram mescladas na branch principal.
   - Discutir possíveis problemas e soluções.

## Conclusão
Este exercício básico abrangeu os fundamentos do Git, como trabalhar com branches, fazer commits, e colaborar através de um Pull Request. Agora você está mais preparado para utilizar o Git em projetos reais!

