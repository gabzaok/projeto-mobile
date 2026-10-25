# 3️⃣ Amanda

> ⚠️ Espere o **Renan** avisar no grupo que fez o push.

## 1. Atualize o projeto oficial e crie a sua branch

Na pasta do projeto oficial (`blog-educacional-backend`), entre na branch do Renan e crie a sua a partir dela:

```powershell
git fetch
git checkout feature/fase4-renan
git pull
git checkout -b feature/fase4-amanda
```

Confira que está na sua branch (tem que aparecer `feature/fase4-amanda`):

```powershell
git branch --show-current
```

## 2. Copie a sua pasta

No **Explorador de Arquivos do Windows** (não use o VS Code), abra a pasta **`parte-3-amanda`**, aperte **Ctrl+A** e depois **Ctrl+C**.

 Obs: Não incluir a pasta `parte-3-amanda`, somente o conteudo dentro dela.

## 3. Cole no projeto oficial

Ainda no **Explorador de Arquivos**, abra a pasta do projeto oficial e aperte **Ctrl+V**.
Se o Windows perguntar, clique em **"Substituir os arquivos no destino"**.

## 4. Envie

Rode um bloco de cada vez, na ordem:

```powershell
git add src/services/alunosService.js src/controllers/alunosController.js src/routes/alunosRoutes.js src/app.js
git commit -m "feat(api): adiciona cadastro, edição, listagem e exclusão de alunos"
```

```powershell
git add "mobile/src/app/(tabs)/alunos.tsx" mobile/src/app/alunos
git commit -m "feat(mobile): adiciona telas de alunos"
```

```powershell
git add tests package.json package-lock.json
git commit -m "test: adiciona testes automatizados da API"
```

```powershell
git add .github/workflows/Main.yml
git commit -m "ci: roda os testes e gera as imagens docker no GitHub Actions"
```

```powershell
git add README.md mobile/README.md
git commit -m "docs: atualiza a documentação para a fase 4"
```

Confira que não sobrou nada (tem que aparecer "nothing to commit") e envie:

```powershell
git status
git push -u origin feature/fase4-amanda
```

## 5. Abra o Pull Request

No GitHub do projeto oficial, clique em **"Compare & pull request"** e confira:

- **base:** `fase-04-mobile`
- **compare:** `feature/fase4-amanda`

Depois clique em **"Create pull request"**.

## 6. Avise no grupo

> "Fiz o push na branch feature/fase4-amanda, o projeto está completo!"
