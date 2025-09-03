
# Deploy do Frontend (Vercel) - passo a passo

1. Crie um repositório no GitHub com a pasta `sistema/frontend`.
2. Acesse https://vercel.com e conecte sua conta GitHub (use a conta que preferir).
3. Clique em "New Project" e selecione o repositório do frontend.
4. Defina as variáveis de ambiente no Vercel (Settings > Environment Variables):
   - REACT_APP_API_URL -> URL do backend (ex.: https://seu-backend.onrender.com)
5. Deploy automático será feito a cada push no GitHub.
6. Após deploy, acesse a URL pública gerada pelo Vercel.
