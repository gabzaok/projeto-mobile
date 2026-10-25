# 2️⃣ Renan

> ⚠️ Espere a **Gabrielle** avisar no grupo que fez o push.

## 1. Atualize o projeto oficial e crie a sua branch

Na pasta do projeto oficial (`blog-educacional-backend`), entre na branch da Gabrielle e crie a sua a partir dela:

```powershell
git fetch
git checkout fase-04-mobile
git pull
git checkout -b feature/fase4-renan
```

Confira que está na sua branch (tem que aparecer `feature/fase4-renan`):

```powershell
git branch --show-current
```

## 2. Copie a sua pasta

No **Explorador de Arquivos do Windows** (não use o VS Code), abra a pasta **`parte-2-renan`**, aperte **Ctrl+A** e depois **Ctrl+C**.

 Obs: Não incluir a pasta `parte-2-renan`, somente o conteudo dentro dela.

## 3. Cole no projeto oficial

Ainda no **Explorador de Arquivos**, abra a pasta do projeto oficial e aperte **Ctrl+V**.
Se o Windows perguntar, clique em **"Substituir os arquivos no destino"**.

## 4. Envie

Rode um bloco de cada vez, na ordem:

```powershell
git add src/services/professoresService.js src/controllers/professoresController.js src/routes/professoresRoutes.js src/middlewares/usuarioMiddleware.js src/app.js
git commit -m "feat(api): adiciona cadastro, edição, listagem e exclusão de professores"
```

```powershell
git add mobile/src/contexts/AuthContext.tsx mobile/src/services/authService.ts mobile/src/app/login.tsx "mobile/src/app/(tabs)/conta.tsx"
git commit -m "feat(mobile): adiciona login e controle de acesso do professor"
```

```powershell
git add mobile/src/services/usuariosService.ts mobile/src/components/UsuarioForm.tsx mobile/src/components/UsuariosLista.tsx "mobile/src/app/(tabs)/professores.tsx" mobile/src/app/professores
git commit -m "feat(mobile): adiciona telas de professores"
```

Confira que não sobrou nada (tem que aparecer "nothing to commit") e envie:

```powershell
git status
git push -u origin feature/fase4-renan
```

## 5. Abra o Pull Request

No GitHub do projeto oficial, clique em **"Compare & pull request"** e confira:

- **base:** `fase-04-mobile`
- **compare:** `feature/fase4-renan`

Depois clique em **"Create pull request"**.

## 6. Avise no grupo

> "Fiz o push na branch feature/fase4-renan, Amanda pode começar."
