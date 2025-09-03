
# Deploy do Backend (Render) - passo a passo

1. Crie um repositório no GitHub com a pasta `sistema/backend` (ou suba tudo em um repo principal).
2. No Render (https://render.com) crie um novo **Web Service** – conecte sua conta GitHub e selecione o repositório.
3. Configure o build command (se necessário): `npm install && npm run build` (o esqueleto não tem build).
4. Configure o start command: `npm start`
5. Variáveis de ambiente (Environment):
   - PORT (opcional)
   - MYSQL_HOST, MYSQL_PORT, MYSQL_USER, MYSQL_PASSWORD, MYSQL_DATABASE
   - JWT_SECRET
   - SMTP_HOST, SMTP_PORT, SMTP_USER, SMTP_PASS
6. Se o banco MySQL não estiver disponível externamente, crie um serviço de banco (Render tem add-ons) ou use um banco gerenciado (PlanetScale, ClearDB, Amazon RDS, etc).
7. Depois do deploy, importe `sistema/database/schema.sql` e `sistema/database/seed.sql` no seu banco de produção.
8. Teste as rotas (por exemplo: GET /health, POST /auth/login).
