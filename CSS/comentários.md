# Comentários

    * Não irá afetar o seu código 
    * Ajuda a lembrar dos blocos de cógidos
    * Deixa dicas para leitura 
    * Ajuda outros a entenderem 
    * Nunca esqueça de fechar um comentário aberto 
    * Podemos utilizar o comentário para desabilitar partes do código

    Comentários começam com /* e terminam com */

```CSS

/* Básico */
/* ------------------------------------------------------- */

body {
    font: 1em/150% Helvetica, Arial, sans-serif;
    padding: 1em;
    margin: 0 auto;
    max-width: 33em;
}

@media (min-width:  70em) {
    body {
        font-size: 130%;
    }
}


/* Elementos Específicos */
/* ------------------------------------------------------- */

div p, #id:first-line {
    background-color: red;
    border-radius: 3px;
}

div p {
    margin: 0;
    padding: 1em;
}

div p + p {
    padding-top: 0;
}

p {
    color: blue;
}

```