# Projeto Git & GitHub - Estudo de Versionamento

Repositório criado por Marcel em colaboração com a empresa devmarcelfcampos, com o objetivo de praticar e documentar os principais comandos e fluxos de trabalho com Git e GitHub. Este projeto faz parte de um estudo de versionamento de código, controle de branches, commits, push/pull,merge e GitHub Flow e colaboração entre equipe utilizando GitHub como plataforma central.

---

##  Objetivos

- Entender o funcionamento do Git
- Versionar código localmente e remotamente
- Criar, alternar e excluir branches
- Fazer commits significativos e rastreáveis
- Realizar push/pull no GitHub
- Trabalhar com merge e resolução de conflitos
- Simular fluxo de trabalho em equipe (GitHub Flow)

---

##  Comandos utilizados

```bash
# Inicializar repositório
git init

# Verificar status
git status

# Adicionar arquivos ao stage
git add .

# Fazer commit
git commit -m "mensagem"

# Criar branch
git checkout -b nome-da-branch

# Trocar de branch
git switch nome-da-branch

# Enviar para o GitHub
git push origin nome-da-branch

# Atualizar com mudanças remotas
git pull origin nome-da-branch

# Deletar branch local
git branch -D nome-da-branch

# Deletar branch remota
git push origin --delete nome-da-branch

---

/////// Estrutura Projeto ///////

/formacao-git-github
├── README.md
├── index.html
├── assets/
│   ├── images/
│   │   └── logo.png
│   └── fonts/
│       └── fonts.ttf
├── css/
│   └── style.css
├── js/
│   └── script.js
├── pages/
│   ├── sobre.html
│   └── contato.html

---

/////// branch de feature ///////

feature/estrutura-site
Essa branch vai incluir todas as páginas: index.html, contato.html, sobre.html, etc.

---

/////// Fluxo recomendado ///////

# Crie a branch única
git checkout -b feature/estrutura-site

# Trabalhe nas páginas normalmente
# Ex: crie e edite index.html, contato.html, sobre.html

# Adicione e commite suas mudanças
git add .
git commit -m "Adiciona estrutura inicial das páginas do site"

# Envie para o GitHub
git push origin feature/estrutura-site

---

/////// Nome sugerido para o commit: ///////

"Cria estrutura inicial do site com páginas: index, contato e sobre"


---

/////// Fluxo de colaboração para quando o time crescer no projeto: ///////

Modelo básico de fluxo Git para equipes (Git Flow simplificado)
1. Branch principal (main)
* Contém o código estável e pronto para produção.
* Nunca faça commits diretos nela.

2. Branch de desenvolvimento (develop)
* Aqui acontece o desenvolvimento ativo.
* Branch onde as features são integradas para testes.

3. Branches de feature (feature/)
* Cada desenvolvedor cria sua branch de feature a partir de develop.
* Nomes claros e semânticos, ex: feature/page-index, feature/user-auth.
* Após finalizar a feature, abre-se um Pull Request (PR) para mesclar em develop.

4. Branches de release (opcional)
* Quando o código em develop estiver pronto para lançar, cria-se uma branch release/x.y.
* Permite corrigir bugs e preparar o deploy.

5. Branches hotfix
* Para corrigir problemas urgentes diretamente na main.
* Depois mesclada em develop.

---

/////// Passo a passo para um colaborador: ///////

# Atualizar develop local
  git checkout develop
  git pull origin develop

# Criar branch feature
  git checkout -b feature/nome-da-feature

# Trabalhar, adicionar e commitar
  git add .
  git commit -m "Descrição clara da feature"

# Enviar para remoto
  git push origin feature/nome-da-feature

# Abrir Pull Request no GitHub para merge em develop

  Benefícios:
      * Código principal (main) sempre estável.
      * Organização clara das funcionalidades.
      * Facilita revisão de código com Pull Requests.
      * Evita conflitos e bugs em produção.

---

✍️ Autor
Marcel Ferreira Campos
Desenvolvedor em formação • Git & GitHub na prática
🔗 github.com/devmarcelfcampos

📚 Licença
Este repositório é parte de um curso educacional e não possui licença de uso comercial.



Criando projeto-git-github - Entre Marcel e Empresa devmarcel (Estudo comandos git-github)
