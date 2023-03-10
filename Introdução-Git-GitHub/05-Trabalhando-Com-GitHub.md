# Trabalhando com o GitHub (repositório remoto)

 - Criar um novo repositório vazio no GitHub:
```
Repositories > New
```

- adicionar a origem do repositório remoto no repositório local (terminal):
```
git remote add origin https://github.com/usuario/repositorio.git
```

- verificar o repositório remoto adicionado:
```
git remote -v
```

- empurrar (*push*) as alterações do repositório local (Git) para o remoto (GitHub):
```
git push -u origin main
```
**Local Repository** {`git push`} >> **Remote Repository**

- puxar/integrar (*pull*) as alterações do repositório remoto (GitHub) para o local (Git):
```
git pull origin main
```

**Remote Repository** {`git pull`} >> **Local Repository**

