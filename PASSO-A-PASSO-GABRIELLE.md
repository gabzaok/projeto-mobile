# 1️⃣ Gabrielle

> ✅ Você é a primeira. Pode começar agora.

## 1. Baixe o projeto oficial numa pasta nova

```powershell
git clone https://github.com/RenanVenturini/blog-educacional-backend.git blog-oficial
cd blog-oficial
git checkout fase-04-mobile
```

## 2. Copie a sua pasta

No **Explorador de Arquivos do Windows** (não use o VS Code), abra a pasta **`parte-1-gabrielle`**, aperte **Ctrl+A** e depois **Ctrl+C**.

 Obs: Não incluir a pasta `parte-1-gabrielle`, somente o conteudo dentro dela.

## 3. Cole no projeto oficial

Ainda no **Explorador de Arquivos**, abra a pasta **`blog-oficial`** e aperte **Ctrl+V**.
Se o Windows perguntar, clique em **"Substituir os arquivos no destino"**.

## 4. Envie

Rode um bloco de cada vez, na ordem:

```powershell
git add .dockerignore .env.example .gitignore docker-compose.yml frontend/Dockerfile frontend/nginx.conf frontend/.dockerignore
git commit -m "chore: adiciona docker do front-end e atualiza configurações"
```

```powershell
git add src/routes/postsRoutes.js src/controllers/postsController.js src/controllers/comentariosController.js src/services/comentariosService.js src/middlewares/postMiddleware.js src/models/postsModel.js
git commit -m "feat(api): adiciona comentários dos alunos e resposta do professor"
```

```powershell
git add index.js src/app.js src/config/database.js src/middlewares/errorMiddleware.js src/routes/materiasRoutes.js src/services/authService.js
git commit -m "refactor(api): separa a montagem da API e cria as tabelas novas"
```

```powershell
git add mobile/.env.example mobile/.gitignore mobile/app.json mobile/package.json mobile/package-lock.json mobile/tsconfig.json mobile/assets mobile/src/config.ts mobile/src/theme.ts mobile/src/types mobile/src/services/api.ts mobile/src/services/storage.ts mobile/src/utils mobile/src/components/Botao.tsx mobile/src/components/Campo.tsx mobile/src/components/Estados.tsx mobile/src/components/Formulario.tsx mobile/src/app/_layout.tsx mobile/src/app/inicio.tsx "mobile/src/app/(tabs)/_layout.tsx"
git commit -m "feat(mobile): cria a estrutura do app e a tela inicial"
```

```powershell
git add mobile/src/services/postsService.ts mobile/src/components/ListaPostagens.tsx mobile/src/components/PostCard.tsx mobile/src/components/Comentarios.tsx mobile/src/app/aluno.tsx "mobile/src/app/(tabs)/index.tsx" "mobile/src/app/posts/[id]/index.tsx"
git commit -m "feat(mobile): adiciona lista, busca e leitura de posts com comentários"
```

```powershell
git add mobile/src/components/PostForm.tsx mobile/src/app/posts/novo.tsx "mobile/src/app/posts/[id]/editar.tsx" "mobile/src/app/(tabs)/admin.tsx"
git commit -m "feat(mobile): adiciona criação, edição e exclusão de posts"
```

Confira que não sobrou nada (tem que aparecer "nothing to commit") e envie:

```powershell
git status
git push
```

## 5. Avise no grupo

> "Fiz o push, Renan pode começar."
