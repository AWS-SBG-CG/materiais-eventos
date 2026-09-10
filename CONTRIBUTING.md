# 🛠️ Guia de Contribuição — Materiais de Eventos

Ficamos muito felizes pelo seu interesse em contribuir com o repositório oficial do **AWS Student Builder Group - UEPB Campina Grande**! 🚀

Toda contribuição é bem-vinda: seja adicionando dicas práticas, corrigindo um slide, compartilhando roteiros de código, sugerindo temas ou compartilhando referências que ajudaram nos seus estudos.

---

## 🧭 Como Funciona o Fluxo de Contribuição

Para garantir a qualidade, segurança e integridade do repositório, adotamos o fluxo padrão de **Fork e Pull Request**:

```text
[Repositório Principal] (AWS-SBG-CG/materiais-eventos)
         │
         ▼  (1) Fork
[Seu Repositório Pessoal] (seu-usuario/materiais-eventos)
         │
         ▼  (2) Criação de branch local: git checkout -b feat/minha-dica
[Suas Alterações & Commits]
         │
         ▼  (3) Push para o seu fork: git push origin feat/minha-dica
[Seu Fork no GitHub]
         │
         ▼  (4) Abertura de Pull Request (PR)
[Análise & Aprovação pelo Core Team] ➔ Merge na branch principal (main)!
```

---

## 👣 Passo a Passo Prático

### 1. Faça um Fork do Repositório
No canto superior direito deste repositório, clique no botão **Fork** para criar uma cópia dele na sua conta pessoal do GitHub.

### 2. Clone o seu Fork localmente
```bash
git clone https://github.com/SEU_USUARIO/materiais-eventos.git
cd materiais-eventos
```

### 3. Crie uma Branch para a sua alteração
Use nomes descritivos e em minúsculas com hifens:
```bash
git checkout -b feat/adiciona-referencia-s3-evento-01
# ou
git checkout -b fix/corrige-comando-aws-cli
```

### 4. Faça suas melhorias
Adicione suas dicas, novos materiais ou correções na pasta correspondente ao evento:
- Se for material de um evento específico: `eventos/XX-nome-do-evento/`
- Se for guia geral ou links: `materiais-complementares/`

### 5. Regras Críticas de Segurança ⚠️
> **NUNCA faça commit de:**
> - Chaves de acesso AWS (`AKIA...`) ou chaves secretas.
> - Arquivos de credenciais (`~/.aws/credentials` ou `.env`).
> - Certificados privados (`.pem`, `.key`).
> 
> Repositórios públicos são varridos em tempo real por bots; qualquer credencial exposta na internet é imediatamente comprometida.

### 6. Faça o Commit e Push
```bash
git add .
git commit -m "docs(evento-01): adiciona guia de boas práticas para IAM"
git push origin feat/adiciona-referencia-s3-evento-01
```

### 7. Abra o Pull Request (PR)
1. Vá até o repositório oficial: `https://github.com/AWS-SBG-CG/materiais-eventos`
2. O GitHub exibirá um aviso sugerindo **Compare & pull request**. Clique nele!
3. Preencha o template do PR com a descrição da sua mudança e confira o checklist de segurança.
4. Clique em **Create Pull Request**.

---

## 🔍 Como o Core Team Analisa os Pull Requests

Nossos organizadores recebem uma notificação e analisam cada PR submetido:
1. **Verificação de Segurança:** Garantir ausência total de credenciais ou links maliciosos.
2. **Relevância Técnica:** O material condiz com as boas práticas da AWS e com a temática do evento?
3. **Clareza Didática:** A explicação está acessível para estudantes de todos os níveis?

Se tudo estiver aprovado, faremos o **Merge** e sua contribuição passará a fazer parte do acervo público oficial da comunidade! 🎉
