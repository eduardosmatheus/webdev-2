# Atividade 01 - Matheus Eduardo 

## Quest�es

### 1. Quais as duas formas de se obter um reposit�rio Git?
```
$ git init: coloca o diret�rio atual sob controle de vers�o do Git
$ git clone: Faz o clone de um reposit�rio existente
```

### 2. Explique para que serve o comando git status. Use exemplo para complementar a resposta.

#### O comando `git status` serve para exibir o estado do reposit�rio local e remoto no momento.
#### Exibe as seguintes informa��es:

- O branch em que o projeto se encontra. Consequentemente :
    - Se o branch local est� atualizado perante o reposit�rio remoto;
    - Se h� commits prontos para fazer push;
    - Quais arquivos est�o adicionados para commit;
    - Quais arquivos que foram modificados n�o est�o adicionados para commit;
    - Quais arquivos n�o est�o sob controle de vers�o;

#### Exemplo: 
```
$ git status

On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   Atividade01/README.md

no changes added to commit (use "git add" and/or "git commit -a")
```

### A sa�da do comando indica que o arquivo `README.md`, que est� no diret�rio `Atividade01` foi modificado e precisa ser commitado.

### 3. Levando em considera��o commits e branches criados com Git, explique o que representa a imagem abaixo e descreva quais comandos Git foram executados para se obter este estado.

#### Partindo do commit C2:
```
$ git checkout -b iss53
Switched to a new branch iss53

$ git status
On branch iss53
Your branch is up-to-date with 'origin/master'.
nothing to commit, working tree clean

// S�o feitas algumas altera��es

$ git status
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   Atividade01/README.md

no changes added to commit (use "git add" and/or "git commit -a")

$ git add Atividade01/README.md

$ git commit -m "Altera README." // Aqui est� o commit C3
[iss53 ccfc35b] Altera README.
 1 file changed, 2 insertions(+), 2 deletions(-)

$ git pull


$ git status

$ git add {novas altera��es}

$ git commit -m "{mensagem descrevendo a altera��o}" // Aqui est� o commit C5
```

### 4. A imagem a seguir representa um estado posterior � imagem apresentada na quest�o 3. Explique o que representa a imagem e descreva quais comandos Git foram executados para se obter este estado.

### Partindo do commit C5
```
$ git status

```
