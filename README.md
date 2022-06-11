# Desafio do Projeto sobre Git/Hub da DIO
Desafio de Projeto sobre Git/Hub

## Links Úteis
[Sintaxe Básica Markdown](https://www.markdownguide.org/basic-syntax/)

Comandos Básicos windows
* cd = navegar entre as pastas
* cd / vai para raiz so c:
* cd .. comando para voltar um nível
* cls - limpar terminal
* dir = comando para listar os diretorios(dentro da apsta que estamos navegando)
* mkdir = comando para criar pasta
* tab -> auto completa o comando
* echo hello > hello.txt criar arquivo dentro da pasta
* del (+ nome do arquivo) = para deletar arquivos

Outros Comandos
* rmdir workspace /s /q (comando para remover a pasta e tudo que estiver nela)
* git --version = versão do git
* ls -a mostra arquivos ocultos

##### COMO O GIT FUNCIONA

* SHA1
É a criptografia do arquivo - é feito um embaralhamento do arquivo
A encriptação gera um conjunto de characteres identificador de 40 digitos.
Esse conjunto é único e serve como identificação.

##### Comando para criptografar o arquivo

$ openssl sha1 nome-do-arquivo.txt

##### Obs importante, se alterar um caracter ou adicionar qualquer caracter ou remover/excluir qualquer caracter a mudança é imediata na chave criptrografada, mas se retornar a condição original a chave é mantida pois ela é dinâmica a qualquer alteração.

#### Informações pertinentes sobre a estrutura do GIT
* OBJETOS FUNDAMENTAIS
	###### BLOBS -> Contem metadados do git(tipo do objeto, tamanho da string, 	tamanho do arquivo, etc...)
	###### TREES -> armazena blobs e commits(guarda o nome do arquivo) sera 	responsavel por montar toda a estrutura de onde esta os arquivos, as arvores 	podem apontar para outras arvores ou para os blobs.
	###### COMMITS -> Mais importante de todos é o objeto que vai juntar tudo, o comit 	tambem tem o sha1. comit grava autor, a hora, emnsagem, parente.
	uma vez que altera um arquivo altera toda a estrutura.

* SISTEMA DISTRIBUÍDO 
	É um sistema distribuido seguro, por tudo o que foi falado sobre criptografia no tema anterior.

##### SEGURANÇA

CHAVE SSH E TOKEN
Quando vou inserir meu código para o github vou precisar me autenticar.
Nome de usuario e senha, ficaram obsoletos esse tipo de autenticação foi desligada.
