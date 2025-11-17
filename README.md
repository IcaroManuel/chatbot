# Chatbot (chat-ia)

Projeto frontend de um chatbot baseado em Next.js — interface e integração com APIs de IA.

## Visão geral

Este repositório contém a aplicação frontend do chatbot (`chatbot`). A app é construída com Next.js 13 e integra bibliotecas de IA para comunicação com modelos (ex.: `openai-edge`, `ai`). O objetivo é fornecer uma interface moderna para conversas com um modelo de linguagem.

## Tecnologias

- Next.js 13
- React 18
- TypeScript
- Tailwind CSS
- openai-edge / ai
- Radix UI (componentes)

Essas dependências estão listadas em `package.json`.

## Pré-requisitos

- Node.js (recomenda-se 18+)
- npm ou pnpm

## Instalação

No WSL (ou terminal de sua preferência), a partir da pasta `chatbot`:

```bash
# instalar dependências
npm install

# ou, se usar pnpm
# pnpm install
```

## Scripts úteis

- `npm run dev` — executa a aplicação em modo de desenvolvimento (Next.js).
- `npm run build` — cria a versão de produção.
- `npm run start` — inicia o servidor a partir do build.
- `npm run lint` — executa o linter (ESLint).

Exemplo para rodar em desenvolvimento:

```bash
npm run dev
# Acesse http://localhost:3000
```

## Variáveis de ambiente

A aplicação provavelmente precisa de chaves para acessar APIs de IA (por exemplo, OpenAI). Crie um arquivo `.env.local` na raiz de `chatbot` com as variáveis necessárias, por exemplo:

```
# Exemplo
OPENAI_API_KEY=sk-... 
# Ajuste os nomes das variáveis conforme o código do projeto
```

Verifique o diretório `src/app/api` (ou outro local) para confirmar nomes exatos das variáveis.

## Estrutura do projeto (resumo)

- `src/` — código fonte do app Next.js
  - `app/` — rotas e páginas (Next 13)
  - `components/` — componentes reutilizáveis
  - `lib/` — utilitários
- `public/` — ativos estáticos
- `package.json` — scripts e dependências

(A estrutura completa pode ser vista na árvore do repositório.)

## Boas práticas e dicas

- Mantenha a chave da API em segredo; não a comite.
- Para deploy, o Vercel funciona bem com Next.js e já provê integração para variáveis de ambiente.
- Use `npm run build` e `npm run start` para rodar a versão de produção localmente.

## Como contribuir

1. Fork e clone este repositório.
2. Crie uma branch com a sua feature: `git checkout -b feat/minha-feature`.
3. Abra um Pull Request descrevendo a mudança.

## Licença

Este repositório está com licença MIT por padrão. Ajuste conforme necessário.

---

Se quiser, posso: adicionar exemplos de variáveis de ambiente específicas, documentar as rotas de API encontradas em `src/app/api`, ou traduzir/expandir seções (ex.: deployment, testes). Quer que eu inclua alguma informação específica do projeto?