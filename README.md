# Tibia Session Tracker

## Instalação

```bash
npm install
```

## Rodar local

```bash
npm run dev
```

## Banco de dados

Execute no Supabase:

```sql
CREATE TABLE sessions (
  id BIGSERIAL PRIMARY KEY,
  created_at TIMESTAMP DEFAULT NOW(),
  session_date DATE,
  raw_xp_gain BIGINT,
  xp_gain BIGINT
);
```

## Deploy

Suba no GitHub e importe na Vercel.