# Atividade Prática - Git e GitHub

**Aluno:** Bruno Ruthes Pinheiro De Oliveira
**Instituição:** FATEC - Cuiabá/MT
**Data:** 21/10/2025
**Repositório:** https://github.com/bruyen72/aulagithubbruno.git

---

## Objetivos da Atividade

Demonstrar domínio dos conceitos fundamentais de Git e GitHub através de uma atividade prática que inclui:

- Criação e configuração de repositório Git local
- Trabalho com branches (feature/html e feature/css)
- Commits seguindo boas práticas
- Push para repositório remoto no GitHub
- Merge de branches
- Organização de código HTML e CSS em branches separadas

---

## Passo a Passo Executado

### 1. Configuração Inicial do Repositório

```bash
# Inicializar repositório Git
git init

# Adicionar repositório remoto
git remote add origin https://github.com/bruyen72/aulagithubbruno.git
```

**Evidência:** Repositório criado em `C:\Users\bruno.ruthes\Downloads\brunopp`

---

### 2. Branch feature/html - Estrutura HTML

```bash
# Criar e trocar para branch feature/html
git checkout -b feature/html
```

**Arquivo criado:** `index.html`

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aula de Git e GitHub</title>
</head>
<body>
    <h1>Bem-vindo à Aula de Git e GitHub!</h1>
</body>
</html>
```

```bash
# Adicionar ao staging
git add .

# Fazer commit
git commit -m "Add index.html com h1 de boas-vindas"

# Push para GitHub (primeira vez nesta branch)
git push -u origin feature/html
```

**Commit Hash:** `bca8592`
**Branch no GitHub:** ✅ feature/html publicada

---

### 3. Branch feature/css - Estilos

```bash
# Criar e trocar para branch feature/css
git checkout -b feature/css
```

**Arquivo criado:** `style.css`

```css
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    margin: 0;
    padding: 20px;
}

h1 {
    color: #333;
    text-align: center;
    padding: 20px;
    background-color: #4CAF50;
    color: white;
    border-radius: 5px;
}
```

**Arquivo modificado:** `index.html` (adicionado link do CSS)

```html
<link rel="stylesheet" href="style.css">
```

```bash
# Adicionar ao staging
git add .

# Fazer commit
git commit -m "Add estilo CSS e link no HTML"

# Push para GitHub
git push -u origin feature/css
```

**Commit Hash:** `7e7363f`
**Branch no GitHub:** ✅ feature/css publicada

---

### 4. Merge das Branches na Main

```bash
# Criar branch main
git checkout -b main

# Merge da branch feature/html
git merge feature/html

# Merge da branch feature/css
git merge feature/css

# Push da main para GitHub
git push -u origin main
```

**Resultado:** ✅ Todas as alterações integradas na branch main

---

## Estrutura Final do Projeto

```
brunopp/
├── index.html          # Estrutura HTML com h1 e link para CSS
├── style.css           # Estilos para body e h1
└── README.md           # Documentação da atividade
```

---

## Histórico de Commits

```
* 7e7363f Add estilo CSS e link no HTML
* bca8592 Add index.html com h1 de boas-vindas
```

---

## Branches no GitHub

1. **main** - Branch principal com código integrado
2. **feature/html** - Branch com implementação HTML
3. **feature/css** - Branch com implementação CSS

---

## Comandos Git Utilizados

| Comando | Descrição |
|---------|-----------|
| `git init` | Inicializar repositório local |
| `git remote add origin <URL>` | Adicionar repositório remoto |
| `git checkout -b <branch>` | Criar e trocar para nova branch |
| `git add .` | Adicionar arquivos ao staging |
| `git commit -m "mensagem"` | Criar commit com mensagem |
| `git push -u origin <branch>` | Enviar branch para GitHub (primeira vez) |
| `git merge <branch>` | Fazer merge de branch |
| `git log --oneline --graph --all` | Ver histórico de commits |

---

## Conceitos Aplicados

### Working Directory × Staging × Repository
- ✅ Editei arquivos no Working Directory
- ✅ Usei `git add .` para mover para Staging
- ✅ Usei `git commit` para salvar no Repository local
- ✅ Usei `git push` para enviar ao GitHub (remoto)

### Branches
- ✅ Criei branches separadas para HTML e CSS
- ✅ Trabalhei isoladamente em cada funcionalidade
- ✅ Fiz merge para integrar tudo na main

### Boas Práticas
- ✅ Commits com mensagens claras e descritivas
- ✅ Uma funcionalidade por branch
- ✅ Uso correto de `git push -u` na primeira vez

---

## Evidências de Autoria

**Informações do Git Config:**
- Name: Bruno Ruthes Pinheiro De Oliveira - FATEC - Cuiaba/MT
- Email: bruno.r.oliveira12@aluno.senai.br

**Commits assinados com:**
```
Committer: Bruno Ruthes Pinheiro De Oliveira - FATEC - Cuiaba/MT <bruno.r.oliveira12@aluno.senai.br>
```

**Link do Repositório:** https://github.com/bruyen72/aulagithubbruno

---

## Conclusão

Esta atividade demonstra compreensão completa do fluxo de trabalho Git/GitHub, incluindo:
- Gerenciamento de branches
- Commits organizados
- Push para repositório remoto
- Merge de funcionalidades
- Documentação adequada

Todos os arquivos estão disponíveis no GitHub e podem ser verificados pelo professor a qualquer momento.

---

**Data de Conclusão:** 21/10/2025
**Assinatura Digital:** Commits verificáveis no GitHub com credenciais FATEC
