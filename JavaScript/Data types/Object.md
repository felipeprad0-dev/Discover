# Object 

    * Objeto é um tipo de dado estrutural
    * Propriedades / atributos 
    * Funcionalidades / métodos 


    Para declarar um objeto, se abre chaves `{}`:
        
        {}

    Dentro, definimos as propriedades e valores: 

        { propriedade: "valor" }
    
    E podemos adicionar funcionalidades: 

        { propriedade: "valor" 
          function(){}
        }

```JS 

 console.log({
     name: "Felipe",
     age: 25,
     walk: function() {
         console.log("Felipe can walk");
     }
 });

```