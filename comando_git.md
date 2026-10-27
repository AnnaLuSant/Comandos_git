
# 💻 Comandos Git para Iniciantes

Este guia reúne os principais comandos do **Git**, organizados por categorias, com explicações e exemplos práticos para facilitar o aprendizado.

O objetivo é auxiliar iniciantes a compreender como utilizar o Git para versionar arquivos, gerenciar branches e colaborar em projetos de desenvolvimento de software.

## 📑 Sumário



1. [Configuração inicial](#️-1-configuração-inicial)
2. [Criação e inicialização de repositórios](#-2-criação-e-inicialização-de-repositórios)
3. [Gerenciamento de arquivos e commits](#-3-gerenciamento-de-arquivos-e-commits)
4. [Trabalhando com branches](#-4-trabalhando-com-branches)
5. [Sincronização com o GitHub](#️-5-sincronização-com-o-github)
6. [Boas práticas](#-6-boas-práticas)

---

##  1. Configuração inicial

Antes de começar a utilizar o Git, é importante configurar o nome e o e-mail que serão associados aos commits.

### `git --version`

Verifica a versão do Git instalada no computador.

```bash
git --version
```

### `git config --global user.name`

Define o nome do usuário que será identificado nos commits.

```bash
git config --global user.name "Seu Nome"
```

Configura o endereço de e-mail associado aos commits.

```bash
git config --global user.email "seuemail@exemplo.com"
```


## 2. Criação e inicialização de repositórios

Um repositório Git é o ambiente no qual os arquivos e o histórico de alterações de um projeto são gerenciados.

### `git init`

Inicializa um novo repositório Git na pasta atual.

```bash
git init
```

Cria uma cópia local de um repositório remoto, incluindo seu histórico de versionamento.

```bash
git clone https://github.com/usuario/repositorio.git
```


Exibe a situação atual do repositório, identificando arquivos modificados, novos arquivos e alterações preparadas para commit.

```bash
git status
```

---

##  3. Gerenciamento de arquivos e commits

#### Os commits representam registros das alterações realizadas em um projeto, permitindo acompanhar sua evolução.

### `git add`

Adiciona arquivos à área de preparação (*staging area*), indicando quais alterações farão parte do próximo commit.

**Para adicionar um arquivo específico:**

```bash
git add arquivo.txt
```

**Para adicionar todas as alterações da pasta atual e suas subpastas:**

```bash
git add .
```

### `git commit`

Registra as alterações preparadas no histórico do repositório.

```bash
git commit -m "Adiciona um comentário na alteração"
```


##  4. Trabalhando com branches

As **branches** são ramificações do projeto que permitem desenvolver funcionalidades, realizar testes e corrigir problemas sem modificar diretamente a linha principal de desenvolvimento.

### `git branch`

Lista as branches locais existentes no repositório.

```bash
git branch
```

**Para criar uma nova branch:**

```bash
git branch nova-funcionalidade
```

### `git switch`

Alterna entre branches existentes.

```bash
git switch nova-funcionalidade
```

**Para criar uma branch e acessá-la imediatamente:**

```bash
git switch -c nova-funcionalidade
```

### `git branch -m`

Renomeia a branch atual.

```bash
git branch -m novo-nome
```
--- 

### `git branch -d`

Exclui uma branch local que já foi integrada ao desenvolvimento.

```bash
git branch -d nova-funcionalidade
```

>  **Atenção:** Antes de excluir uma branch, verifique se suas alterações importantes foram integradas.

---

##  5. Sincronizando com o GitHub

Os repositórios remotos permitem compartilhar projetos e sincronizar alterações entre diferentes computadores e desenvolvedores.

### `git remote add origin`

Associa um repositório remoto ao projeto local.

```bash
git remote add origin https://github.com/usuario/repositorio.git
```

### `git remote -v`

Exibe os endereços dos repositórios remotos configurados.

```bash
git remote -v
```

### `git push`

Envia os commits locais para um repositório remoto.

```bash
git push origin main
```

**Para publicar uma nova branch e configurar seu acompanhamento remoto:**

```bash
git push -u origin nova-funcionalidade
```
> **Atenção:** Antes de dar um push na branch, verifique se suas alterações e se está commitando na branch correta.

### `git pull`

Busca e integra as atualizações de um repositório remoto à branch local.

```bash
git pull
```


## 6. Boas práticas

Além de conhecer os comandos, é importante adotar hábitos que contribuam para a organização e a manutenção dos projetos.

- **Escreva mensagens de commit descritivas:** facilite a identificação das alterações realizadas.
- **Realize commits regularmente:** registre mudanças pequenas e relacionadas entre si.
- **Utilize branches:** mantenha o desenvolvimento de novas funcionalidades separado da branch principal.
- **Consulte o `git status`:** verifique os arquivos modificados antes de realizar commits.
- **Utilize `.gitignore`:** evite versionar arquivos temporários, dependências geradas e informações sensíveis.
- **Mantenha seu repositório atualizado:** sincronize as alterações remotas antes de integrar trabalhos colaborativos.

---

##  Referências e documentação

Para aprofundar seus conhecimentos, consulte a documentação oficial:

- [Git — Documentação oficial](https://git-scm.com/doc)
- [Git — Livro Pro Git](https://git-scm.com/book/pt-br/v2)
- [GitHub Docs](https://docs.github.com/pt)

---

**📖 Bons estudos e bons commits! ^_^** 
