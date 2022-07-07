## Criando repositório local

Na pasta/diretório que você deseja versionar, digite:

```
git init
```



------

## Ver estado do Git

```
git status
```



Use esse comando **sem** moderação.

------

## Adicionando seus arquivos ao Git

```
git add nome_do_arquivo
```



ou para adicionar todos os arquivos de uma só vez:

```
git add *
```



Agora é preciso fazer o **commit** para que o **Git** possa rastrear suas modificações:

```
git commit -m 'seu comentário sobre seus arquivos aqui'
```



<img src="https://pythonacademy.com.br/assets/posts/fluxo-git/fluxo-git.png" style="zoom: 85%;" />



------

## Atualizando commit de arquivo modificado

```
git commit -am 'digite sua mensagem aqui'
```



------

## Ligando seu repositório local a sua nuvem

```
git remote add origin link_para_o_repositório_do_seu_projeto
```



No meu caso:

```
git remote add origin https://github.com/vtrx1992/teste.git
```



------

## Enviando suas alterações

Pela primeira vez:

```
git push -u origin master
```



Nas próximas vezes basta

```
git push
```



------

## Copiando um repositório

```
git clone link_para_o_repositório_que_deseja_copiar
```



Exemplo:

```
git clone https://github.com/vtrx1992/teste.git
```



------

## Criando branches

```
git checkout -b nome_do_branch
```



Para voltar ao branch master:

```
git checkout master
```



O comando:

```
git checkout nome_do_branch
```



faz a troca entre os branches.

Seus branches locais não estarão na nuvem a menos que você os envie.

```
git push origin nome_do_branch
```



------

## Unindo branches

```
git merge nome_do_branch
```



------

## Atualizando seu repositório local

Pega as modificações que foram feitas no repositório remoto.

```
git pull
```



------

## Desfazendo commits

```
git revert chave_do_commit
```



A chave do commit é encontrada através do comando:

```
git log
```



------

## Entendendo o fluxo do Git

- working directory: sua pasta/diretório.
- index (staging area): a sala de espera do Git. Para onde vão os commits antes do push.
- master: branch principal. O branch padrão do Git.
- HEAD: por padrão, aponta para o último commit recebido dentro do repositório.