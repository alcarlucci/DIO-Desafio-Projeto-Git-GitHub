# Chave SSH e Token

É portanto necessário, o Git ter formas de autênticação com os repositórios remotos, como o GitHub.
*GitHub*: plataforma em nuvem que servirá de repositório remoto de código versionado pelo Git.

### Chave SSH
De maneira resumida, é uma forma de estabelecer uma conexão segura e encriptada entre dois hosts (máquinas), por ex.: conexão entre nossa máquina local e o repositório remoto no GitHub. Isso é feio por meio de um par de chaves (pública/privada).
 - gerar chave SSH no terminal da máquina local:
```
ssh-keygen -t ed25519 -C seu_email@email.com
```
 - copiar o conteúdo da chave pública gerada:
```
cat  ~/.ssh/id_ed25519.pub
```
 - configuração da chave SSH no GitHub:
```
Settings > SSH and GPG keys > SSH keys: New SSH key
```
(*colar o conteúdo da chave pública em "key"*)
 - iniciar o processo do ssh-agent no terminal da máquina local:
```
eval $(ssh-agent -s)
```
 - passar a chave (privada) gerada para o ssh-agent:
```
ssh-add  ~/.ssh/id_ed25519
```

### Token
Uma alternativa à autenticação por chave SSH seria utilizando um Token de acesso pessoal.
 - configuração de Token de acesso pessoal no GitHub:
```
Settings > Developer settings > Personal access tokens > Tokens: Generate new token
```
Após gerar o Token de acesso pessoal no GitHub, copie esse token apresentado no GitHub ao final do processo de criação, e salve em um arquivo num local seguro da sua máquina local. Esse token será solicitado em futuras autênticações com o GitHub.
