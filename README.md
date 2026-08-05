# 🦜 Bem-vindo ao Repositório do Papuguinho!

Este documento é a sua porta de entrada. Aqui estão as regras da nossa casa, como organizamos o código e como trabalhamos juntos no repositório. Leia com atenção antes de começar o seu primeiro código!

---
## 🔄 1. O Passo a Passo do Git (Fluxo de Trabalho)

Nós temos uma regra de ouro inquebrável: **Ninguém faz commits direto na branch `main`.** 
A `main` reflete o que está em produção. O sistema está configurado para bloquear qualquer push direto para ela.

### Passo 1: O Setup Inicial (Faça isso apenas na primeira vez)
Para baixar o projeto para o seu computador, abra o terminal na pasta onde deseja guardar os seus projetos e rode:

```bash
# Clone o repositório para a sua máquina
git clone <COLE_O_LINK_DO_REPOSITORIO_AQUI>

# Entre na pasta do projeto
cd <NOME_DA_PASTA_DO_PROJETO>
```

### Passo 2: O Dia a Dia (Para cada nova tarefa)
Antes de começar a programar, garanta que você está na base atualizada e crie a sua ramificação de trabalho:

```bash
# Vá para a branch principal
git checkout main

# Puxe as atualizações mais recentes da nuvem
git pull origin main

# Crie uma nova branch para a sua tarefa e mude para ela
git checkout -b <prefixo>/<nome-da-tarefa>
```

---

## 📝 2. Padrão de Commits (Conventional Commits)

Nós utilizamos a especificação do **[Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0/)**. Isso mantém nosso histórico legível e profissional. 

Todo commit deve obrigatoriamente começar com um destes prefixos:

| Prefixo | Quando usar |
| :--- | :--- |
| `feat:` | Quando você adiciona uma funcionalidade nova. |
| `fix:` | Quando você resolve um bug ou erro. |
| `refactor:` | Quando você reescreve um código antigo sem mudar o que ele faz (melhoria técnica). |
| `chore:` | Tarefas de manutenção (ex: atualizar dependências, arrumar configuração). |
| `docs:` | Alterações apenas em documentação (como este README). |

### Passo 3: Salvando o Código
Quando terminar a tarefa, adicione e "commit" os arquivos usando o padrão:

```bash
# Adicione todos os arquivos modificados
git add .

# Crie o commit explicando a mudança
git commit -m "fix: resolve erro de padding na tela inicial"
```

---

## 🚀 4. Subindo o Código e Code Review

Para que a equipe veja o seu código, você precisa enviá-lo para o GitHub e solicitar a aprovação.

### Passo 4: O Envio (Push)
```bash
# Envie a sua branch para o repositório remoto
git push -u origin <nome-da-sua-branch>
```

### Passo 5: O Pull Request (PR)
1. Abra a página do repositório no GitHub.
2. Você verá um botão verde escrito **"Compare & pull request"**. Clique nele.
3. Descreva o que você fez de forma clara.
4. Aguarde a revisão (Code Review). Se tudo estiver certo, o seu código será aprovado e mesclado na `main`!

---

## 💡 Exemplo Prático Completo

Imagine que você assumiu uma issue do projeto para resolver problemas de segurança atualizando o Firebase. O seu fluxo no terminal seria exatamente este:

```bash
git checkout main
git pull origin main
git checkout -b fix/upgrade-firebase-v13
# ... você atualiza os pacotes e resolve os erros de segurança no código ...
git add .
git commit -m "fix: atualiza para Firebase v13 e resolve erros de segurança"
git push -u origin fix/upgrade-firebase-v13
```
*(Depois disso, é só abrir o Pull Request no GitHub!)*

Bem-vindo ao time e bom código!
