# Git Course

### Setar usuário
* git config --global user.name "Leonardo Comelli"

### Setar email
* git config --global user.email leonardo@software-ltda.com.br

### Listar configurações
* git config --list

### Adicionar um arquivo em específico
* git add meu_arquivo.txt

### Comitar informando mensagem
* git commit meuarquivo.txt -m "minha mensagem de commit"

### Remover arquivo
* git rm meu_arquivo.txt

### Remover diretório
* git rm -r diretorio

### Exibir histórico
* git log

### Exibir resumo do histórico (hash completa, autor, data, comentário e qtde de alterações (+/-))
* git log --stat

### Este comando deve ser utilizando enquanto o arquivo não foi adicionado na staged area.
* git checkout -- meu_arquivo.txt

### Este comando deve ser utilizando quando o arquivo já foi adicionado na staged area.
* git reset HEAD meu_arquivo.txt
####    Se o resultado abaixo for exibido, o comando reset não alterou o diretório de trabalho.
#### Unstaged changes after reset:
#### M	meu_arquivo.txt

### A alteração do diretório pode ser realizada através do comando abaixo:
* git checkout meu_arquivo.txt

## Repositório Remoto

### Exibir os repositórios remotos
* git remote / git remote -v

### Vincular repositório local com um repositório remoto
* git remote add origin git@github.com:leocomelli/curso-git.git

### Vincular repositório local com um repositório remoto
* git remote add origin git@github.com:leocomelli/curso-git.git

### Renomear um repositório remoto
* git remote rename origin curso-git
### Desvincular um repositório remoto
* git remote rm curso-git

### Enviar arquivos/diretórios para o repositório remoto
#### O primeiro push de um repositório deve conter o nome do repositório remoto e o branch.
* git push -u origin master

#### Os demais pushes não precisam dessa informação
* git push

## Atualizar repositório local de acordo com o repositório remoto
### Atualizar os arquivos no branch atual
* git pull

### Buscar as alterações, mas não aplica-las no branch atual
* git fetch

### Clonar um repositório remoto já existente
*git clone git@github.com:leocomelli/curso-git.git