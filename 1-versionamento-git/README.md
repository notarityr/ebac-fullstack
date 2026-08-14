# 1-versionamento-git

## A entrega desse exercício consiste em:

Criar um repositório no Github, por exemplo: curso_ebac_frontend;
- foi criado um repositório chamado "ebac-fullstack".

Criar uma branch chamada exercicio_git no repositório recém-criado;
- foi criada uma branch chamada "exercicios-ebac".

Na branch exercício_git deverá ser adicionado um arquivo nome.txt com o seu nome completo;
- foi criado através do comando `echo "Túlio Cícero Wiles Notari" > nome.txt`

## Passo-a-passo realizado

1. Criação do repositório `ebac-fullstack` no GitHub.

2. Dentro dele foi criado um novo diretório:
```bash
  mkdir 1-versionamento-git
```
3. Clonagem do repositório para a máquina local:
```bash
   git clone https://github.com/notarityr/ebac-fullstack
```
   
4. Criação da branch `exercicio_git`:
```bash
   git checkout -b exercicios-ebac
```
   
5. Adição do arquivo `nome.txt` com meu nome completo:

```bash
   echo "Túlio Cícero Wiles Notari" > nome.txt
   git add nome.txt
   git commit -m "Adicionando arquivo nome.txt com meu nome completo"
```
   
6. Envio da branch para o GitHub:
```bash
   git push origin exercicios-ebac
```
O arquivo "nome.txt" pode ser visualizado dentro deste diretório.
