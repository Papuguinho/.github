# 🦜 Bem-vindo Desenvolvedor do Papuguinho!

Este documento é a sua porta de entrada. Aqui estão as regras da nossa casa, como organizamos o código e como trabalhamos juntos no repositório. Leia com atenção antes de começar o seu primeiro código!

---
## 🔄 1. Fluxo de Trabalho e Git (Como enviar código)

Temos uma regra de ouro inquebrável: **Ninguém faz commits direto na branch `main`.** 
A `main` é sagrada e reflete o que os usuários estão usando em produção. O próprio GitHub está configurado para **bloquear** qualquer `push` direto para lá.

### Passo a Passo para contribuir:

**1. Clone o repositório e atualize sua máquina**
Sempre tenha certeza de que você está trabalhando com a versão mais recente:
```bash
git checkout main
git pull origin main
```

**2. Crie uma branch para a sua tarefa**
Nunca codifique na `main`. Crie uma branch com um nome que explique o que você vai fazer:
*   `feat/`: Para novas funcionalidades.
*   `fix/`: Para conserto de bugs.
*   `refactor/`: Para reescrever códigos antigos sem mudar o comportamento.
```bash
git checkout -b feat/nome-da-sua-tarefa
```

**3. Faça seus Commits (Padrão Semântico)**
Seja claro no que você fez, use o **Convetional Commits** para escrever mensagem diretas e organizadas. <br>
<a href="https://www.conventionalcommits.org/en/v1.0.0/">Convetional Commits</a>

```bash
git add .
git commit -m "feat: adiciona botao de retorno na home"
```

**4. Suba sua branch para o GitHub**
```bash
git push -u origin nome-da-sua-branch
```

**5. Abra o Pull Request (PR)**
Vá até a página do GitHub e clique em "Compare & pull request". Descreva o que você fez para facilitar a vida de quem vai revisar o seu código (Code Review). Se tudo estiver certo, seu código será aprovado e mesclado (merge) na `main`!

---

## 💡 3. Exemplo Prático do Fluxo

Para ilustrar, imagine que você assumiu a issue para resolver as exigências de versão do Firebase v13 e arrumar os erros de segurança. Seu fluxo seria exatamente este:

1. `git checkout main`
2. `git pull origin main`
3. `git checkout -b fix/firebase-v13-security`
4. *(Você atualiza os pacotes e arruma o código no VS Code)*
5. `git add .`
6. `git commit -m "fix: atualiza para Firebase v13 e resolve erros de segurança"`
7. `git push -u origin fix/firebase-v13-security`
8. Abre o PR no GitHub e aguarda a aprovação!

Bem-vindo ao time e bom código! 🚀
