# DevStorm
# Guia Colaborativo para GitHub - [Nome do Projeto]

👋 Bem-vindos ao projeto! Como estamos trabalhando em equipe e usando GitHub, este guia traz **boas práticas** e **dicas básicas** para evitar conflitos e manter a organização.

---

## 📚 GitHub Básico (Para Iniciantes)

### O que é GitHub?
- Plataforma para **versionamento de código**: histórico de todas as mudanças no projeto.
- **Repositório (repo)**: "Pasta" do projeto no GitHub (aqui estamos!).
- **Commit**: "Snapshot" de mudanças específicas (como salvar uma versão).
- **Branch**: Ramificação paralela para desenvolver features sem afetar o código principal (`main`/`master`).

---

## ⚙️ Configuração Inicial
1. **Instale o Git**: [Download aqui](https://git-scm.com/)
2. **Configure seu usuário**:
   ```bash
   git config --global user.name "Seu Nome"
   git config --global user.email "seu@email.com"

 ´´´
Clone o repositório:

 ```bash
git clone https://github.com/[usuário]/[repositório].git
```
✅ Boas Práticas para o Time
1. Trabalhe em Branches Separadas
SEMPRE crie uma nova branch para suas tarefas:

````bash
git checkout -b feature/nome-da-sua-feature
````
Exemplo: feature/header-responsivo, fix/botao-login

3. Commits Claros
Mensagens objetivas no imperativo:

git commit -m "Adiciona menu responsivo para mobile"
❌ Evite: "Alterações" ou "Update".

3. Atualize sua Branch Frequentemente
Antes de começar a trabalhar, puxe as mudanças da main:

````bash
git checkout main
git pull origin main
git checkout sua-branch
git merge main
````
4. Pull Requests (PRs)
Sempre crie um PR para mesclar sua branch na main.

Descreva no PR:

O que foi feito

Screenshots (se for HTML/CSS)

Peça revisão a 2 colegas antes de mergear.

5. Resolvendo Conflitos
Se houver conflitos ao mesclar:

Abra os arquivos marcados.

Escolha quais alterações manter (converse com o time se necessário).

Commit as correções.

### 📂 Organização de Arquivos
```bash
project/
├── index.html
├── styles/
│   ├── main.css        # Estilos globais
│   ├── header.css      # Estilos específicos do cabeçalho
│   ├── forms.css       # Estilos de formulários
│   └── responsive.css  # Media queries
└── assets/
    ├── images/         # Todas as imagens
    ├── fonts/          # Fontes customizadas
    └── scripts/        # JavaScript (se necessário)

````
Separação de responsabilidades:

CSS em arquivos separados (ex: forms.css, header.css).

Use comentários para seções (/* === HEADER STYLES === */).

Evite:
Estilos inline no HTML.

Sobrescrever estilos de colegas sem comunicação.

⚡ Fluxo de Trabalho Sugerido
git pull origin main (sincronize antes de começar)

Crie sua branch → trabalhe nos arquivos.

Teste localmente (abra o HTML no navegador!).

Commit + Push para sua branch.

Abra um PR no GitHub e marque revisores.

Após aprovação, delete a branch mesclada.

❌ Erros Comuns a Evitar
Commitar arquivos desnecessários (node_modules, .DS_Store).

Trabalhar diretamente na branch main.

Ignorar conflitos no Git (resolva sempre!).

Commits gigantes (ex: "Update geral" com 20 arquivos).

🔗 Recursos Úteis
GitHub Guides

Git Simulator (prática visual)

HTML/CSS Best Practices

✨ Lembre-se: Comunicação é chave! Combinem padrões de código e usem issues/PRs para discutir mudanças. Vamos juntos! ✨


### Como usar:
1. Substitua `[Nome do Projeto]`, `[usuário]` e `[repositório]` pelos dados do seu projeto.
2. Adicione detalhes específicos do seu fluxo (ex: revisores fixos, padrões de CSS).
3. Inclua links para documentos internos (ex: design system, protótipo).

Isso dá uma base para o time se orientar e reduz erros comuns em projetos colaborativos. 😊

