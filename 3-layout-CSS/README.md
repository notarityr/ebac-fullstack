# 3-layout-CSS

## A entrega desse exercício consiste em:

Criar mais duas seções no layout previamente criado durante o módulo. </br>
</br>
Exemplo: entretenimento e tecnologia, as novas seções devem conter outras notícias e diferentes cores;

## Passo a passo realizado: 

1. Criação de um novo diretório na branch `exercicios-ebac`:

```bash
mkdir 3-layout-CSS
```
2. Criação das seções `Tecnologia` e `Entretenimento`:
- Adicionadas as imagens referentes aos novos artigos na pasta `./imagens`
- Adicionados os textos das imagens para acessibilidade `<img src="./imagens/tecnologia.png" alt="Mão robótica" />`
- Adicionados os títulos dos artigos `<h3>Uso de inteligência artifical já faz parte das empresas</h3>`

```HTML
<section> //criação da seção
        <h2>Tecnologia</h2> //título
        <article> //início do artigo
            <img src="./imagens/tecnologia.png" alt="Mão robótica" /> //criação da alt
            <header>
                <time>13/07/2026 às 15:38</time>
            </header>
            <h3>Uso de inteligência artifical já faz parte das empresas</h3> //adição dos títulos
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                Tenetur consequuntur doloremque totam labore architecto. 
                Corporis adipisci optio placeat quibusdam totam iure veritatis quam, ullam tenetur error? 
                Laborum, modi itaque. Sunt.
            </p>
            <a href="#" title="Leia a notícia completa">Ler mais</a>
        </article> //fim do artigo
        </section> //fim da seção
```

3. Adicionadas as novas seções na lista de navegação:

```HTML
<nav>
            <ul> 
               <!-- ... -->
                <li>
                    <a href="#technology" title="Ir para a seção de tecnologia">Tecnologia</a>
                </li>
                <li>
                    <a href="#entertainment" title="Ir para a seção de entretenimento">Entretenimento</a>
                </li>
            </ul>
        </nav>
```

4. Inserindo identificadores nas seções correspondentes:

```HTML
<section id="entertainment">
        <h2>Entretenimento</h2>
        <article>
```

5. Criação do arquivo `main.css`:
- Utilizando os identificadores inseridos para criar âncoras `id="tecnology`, `#technology`
- Mudando o estilo dos headers `<h2>` com alteração de suas cores `color: rgb`

```CSS
#technology h2 {
    color: rgb(255, 30, 0); 
}

#entertainment h2 {
    color:rgb(55, 0, 255)
}
```

6. Envio da branch para o GitHub:

```bash
   git add .
   git commit -m "layout completado com requisitos"
   git push origin exercicios-ebac
```

Os arquivo "main.css" pode ser visualizado dentro deste diretório. </br>
As novas imagens podem ser visualizadas dentro do diretório `./imagens`.
