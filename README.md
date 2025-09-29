# 🌐 Git e GitHub — Resumo das Primeiras Práticas  

Este é um registro organizado das minhas primeiras experiências com **Git e GitHub**.  
Aqui anotei, de forma prática e resumida, os principais **comandos**, **conceitos** e **boas práticas** que usei ao criar repositórios locais, salvar arquivos com commits e documentar projetos usando **Markdown**.  

As anotações servem como guia rápido para revisar o fluxo de trabalho no Git e também como material de apoio para futuros estudos.  

---

## 📁 Estrutura de Pastas e Organização

- Criar pasta principal no Desktop:

  ```bash
  mkdir DIO_Git_Github
  cd ~/Desktop/DIO_Git_Github
  ```

- Criar subpasta para repositório (evita conflitos):
  ```bash
  mkdir dio_resumos_git_github
  cd dio_resumos_git_github
  ```

- Inicializar repositório:

  ```bash
  git init
  ```

  🔹 O nome da branch padrão aparecerá (ex: **master** ou **main**), confirmando que a pasta é um repositório Git.

---

## 📄 Criando Arquivos e Documentação

* Criar arquivo vazio:

  ```bash
  touch README.md
  ```

  ➡️ Usado para documentação do projeto em **Markdown**.

* Lembre-se:

  * Criar arquivo ≠ commit realizado.
  * O arquivo precisa ser **adicionado** e **confirmado**.

---

## 🔄 Fluxo Básico de Versionamento

1. **Verificar status**

   ```bash
   git status
   ```

2. **Adicionar arquivo**

   ```bash
   git add README.md
   ```

3. **Fazer commit**

   ```bash
   git commit -m "Meu primeiro commit"
   ```

---

## ⚙️ Configuração Inicial

Se o Git pedir **nome** e **e-mail** antes do commit:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@email.com"
```

---

## 🔍 Comandos Importantes

### 📜 `git log`

Exibe histórico de commits:

* 🔢 Hash único
* 👤 Autor
* 📅 Data
* 📝 Mensagem

Opções úteis:

* `git log --oneline` → resumo compacto
* `git log --graph` → árvore visual
* `git log -p` → diffs de cada commit

---

### 📌 `git status`

* Mostra o estado do repositório.
* Não reconhece **pastas vazias**.
* Exemplo comum: *nothing to commit, working tree clean*.

---

### 📦 `touch`

Cria arquivos vazios.

```bash
touch index.html
```

* Se já existir, apenas atualiza a data de modificação.

---

## 🚫 Ignorando Arquivos/Pastas

* Criar `.gitignore`:

  ```bash
  echo resumos/ > .gitignore
  ```

  ➡️ O Git ignora a pasta `resumos/`.

* Arquivos `.gitkeep` podem aparecer apenas para evitar pastas vazias (já que o Git não rastreia pastas sem arquivos).

---

## 📝 Mini-Guia de Markdown

### 📌 Títulos

```markdown
# Nível 1
## Nível 2
### Nível 3
```

### ✍️ Ênfase

```markdown
*Itálico*  
**Negrito**  
~~Tachado~~
```

### 📋 Listas

```markdown
- Item
1. Item ordenado
```

### 🔗 Links e Imagens

```markdown
[Link](https://exemplo.com)  
![Imagem](https://url.com/img.png)
```

### 📌 Citações

```markdown
> Texto citado
```

### 💻 Código

```markdown
`inline`
```

````markdown
```bash
git status
```
````

### 📐 Tabelas

```markdown
| Nome     | Idade |
|----------|-------|
| Dênimer  | 28    |
```

### ✅ Checklists

```markdown
- [x] Feito
- [ ] Pendente
```

---

## 💡 Dicas Rápidas

* Sempre trabalhe dentro da **subpasta** do repositório (não na pasta principal).
* Um arquivo só faz parte do versionamento após o **git add** + **git commit**.
* Use `.gitignore` para evitar rastrear arquivos desnecessários.
* `git log` ajuda a entender o histórico e rastrear alterações.

---

📚 **Referências**

* [Guia de Markdown no GitHub](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
* [Documentação GitHub](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github)

---

