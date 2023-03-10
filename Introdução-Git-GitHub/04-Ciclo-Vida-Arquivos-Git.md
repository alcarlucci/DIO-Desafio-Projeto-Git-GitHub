# Ciclo de vida dos arquivos no Git

### Arquivos Untracked (não rastreados pelo Git):
 - **New file**: novos arquivos adicionados ou criados no repositório

### Status dos arquivos Tracked (rastreados pelo Git):
 - **Unmodified**: arquivo não modificado (após um commit por ex.)
 - **Modified**: edição de um arquivo unmodified
 - **Staged**: arquivo em "Stage", preparado para o commit

### Organização dos repositórios - Local e Remoto:
**Ambiente de desenvolvimento (local)**:
 - Working directory
 - Staging area
 - Local Repository (Git)

**Servidor (remoto)**:
 - Remote Repository (GitHub por exemplo)

**Working directory** {`git add`} >> **Staging area** {`git commit`} >> **Local Repository**

