# Entendendo o funcionamento do Git

### Git
Sistema de controle de versionamento de código distribuído

### SHA1
A sigla SHA significa Secure Hash Algorithm (Algoritmo de Hash Seguro), é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA).
A encriptação gera um conjunto de caracteres identificador de 40 dígitos.
É uma forma curta de representar o estado de um arquivo, a partir da Hash gerada pelo SHA1.

Rodar o comando abaixo no terminal para gerar uma Hash usando SHA1:
```
echo "ola mundo" | openssl sha1
```

### Objetos fundamentais
Três tipos básicos de objetos do Git responsáveis pelo versionamento do código:
 - **Blobs**: armazena metadados dos arquivos;
 - **Trees (árvores)**: uma tree aponta para os blobs e também outras trees; portanto armazena a informação de toda a estrutura de diretórios e arquivos;
 - **Commits**: armazena meta dados como autor, mensagem, carimbo de timestamp e o commit parente (commit anterior), encapsulando toda a estrutura de trees e blobs para um commit realizado.

Para cada objeto (Blob, Tree, Commit) é gerada uma hash SHA1 controlando as alterações em cada um deles.

**Commit** (*SHA1 + metadados*) -> **Tree** (*SHA1 + metadados*) -> **Blob** (*SHA1 + metadados*)

### Sistema distribuído
Possibilidade de diferentes colaboradores espalhados trabalhando em um mesmo projeto.

### Segurança
A segurança é inerente ao Git pela forma como ele é estruturado.

