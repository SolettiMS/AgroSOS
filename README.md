# AgroSOS

MVP do AgroSOS, uma plataforma emergencial de peças agrícolas inspirada no fluxo do iFood para situações críticas no campo.

## Stack

- Next.js 14 com App Router
- TypeScript estrito
- Tailwind CSS
- Lucide React
- Prisma

## Rodando localmente

```bash
npm install
npm run dev
```

Acesse:

```text
http://127.0.0.1:3000
```

## Scripts

```bash
npm run dev
npm run build
npm run lint
npm run prisma:generate
```

## Banco de dados

O schema Prisma está em `prisma/schema.prisma`.

Crie um arquivo `.env` baseado em `.env.example` e configure `DATABASE_URL` antes de usar Prisma com um banco real.

## Fluxo do MVP

- Home do produtor com busca textual e upload de foto para simulação de IA.
- API mock de visão que identifica a peça `HXE21132`.
- API de busca que calcula distância com Haversine e ordena por menor tempo de entrega.
- Tela comparativa com logos reais das lojas e destaque para entrega mais rápida.
- Rastreamento do pedido com status automático a cada 4 segundos.
