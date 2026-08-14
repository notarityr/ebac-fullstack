# 2-formulario-HTML

## A entrega desse exercício consiste em:

A entrega desse exercício consiste em:

Criar um arquivo HTML que contenha um formulário de cadastro, com os campos nome, e-mail e senha e a existência de um botão para realizar o cadastro;
- foi criado o arquivo chamado "index.html" com o formulário e suas especificações

Adicionar também uma label para cada campo e referenciar essa label ao ID que será atribuído ao campo;
- adicionadas as labels e IDs

Enviar esse arquivo para o Github em uma branch chamada exercício_html;
- enviado para a branch chamada exercicios-ebac

## Passo-a-passo realizado

1. Criação do repositório `ebac-fullstack` no GitHub, realizado previamente.

2. Dentro dele foi criado um novo diretório na branch `exercicios-ebac`:

```bash
  mkdir 2-formulario-HTML
```

3. Adição do arquivo `index.html` com o formulário:

```bash
   touch index.html
   git add index.html
   git commit -m "adicionando formulário de cadastro em HTML"
```

4. Desenvolvimento do HTML:

```HTML
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Formulário de Cadastro</title>
</head>
<body>
    <h1>Cadastro</h1> 
    //criando formulário com 'form'
    <form> 
        //conectando label ao id com 'for/id'
        <label for="nome">Nome:</label> 
        //criando caixa de texto com identificador 'name' e preenchimento obrigatório 'required'
        <input type="text" id="nome" name="nome" required> 
        <br><br>

        <label for="email">E-mail:</label>
        //verifica se o input tem formato de e-mail com 'type email'
        <input type="email" id="email" name="email" required>  
        <br><br>

        <label for="senha">Senha:</label>
        //ocultando os caracteres digitados com 'type password'
        <input type="password" id="senha" name="senha" required> 
        <br><br>
        //criando botão de cadastro com 'button'
        <button type="submit">Cadastrar</button>
    </form>
</body>
</html>
```
   
5. Envio da branch para o GitHub:

```bash
   git push origin exercicios-ebac
```

O arquivo "index.html" pode ser visualizado dentro deste diretório.
