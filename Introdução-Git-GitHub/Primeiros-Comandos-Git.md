# Primeiros comandos com Git
Rodar no terminal os comandos abaixo dentro da pasta que servirá de repositório.

### Configurações iniciais do Git
 - Configurar o nome de usuário do Git para todos os repositórios no computador:
```
git config --global user.name 'Nome Usuario'
```
 - Configurar o endereço de e-mail para todos os repositórios no computador:
```
git config --global user.email 'email@example.com'
```
 - Verificar as configurações do git:
```
git config -l
```

### Iniciar o Git
 - Iniciar o repositório Git dentro da pasta:
```
git init
```
 - Verificar o repositório iniciado:
```
git status
```

### Iniciar o versionamento
 - Após criar os arquivos dentro da pasta (repositório):
```
git add .
```

### Criar um Commit
 - Comitar os arquivos criados/alterados dentro da pasta (repositório):
```
git commit -m "comentários das alterações"
```

