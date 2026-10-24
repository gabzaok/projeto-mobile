# 3️⃣ Amanda

> ⚠️ Espere o **Renan** avisar no grupo que fez o push.

## 1. Atualize o projeto oficial

Na pasta do projeto oficial (`blog-educacional-backend`):

```powershell
git checkout fase-04-mobile
git pull
```

## 2. Copie a sua pasta

Abra a pasta **`parte-3-amanda`**, aperte **Ctrl+A** e depois **Ctrl+C**.

 Obs: Não incluir a pasta `parte-3-amanda`, somente o conteudo dentro dela.

## 3. Cole no projeto oficial

Abra a pasta do projeto oficial e aperte **Ctrl+V**.
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
git push
```

## 5. Avise no grupo

> "Fiz o push, o projeto está completo!"
