## VALID CARD
#### Contenido:
1. Diagrama de flujo validCard.
2. Pseudocódigo validCard.
3. Ejecución del código en JS.
4. Explicación del código.
- - - - -- -

### 1. DIAGRAMA DE FLUJO

![DFcifradoCesar](DFcifradoCesar.png "Diagrama Flujo CifradoCesar")

### 2. PSEUDOCÓDIGO

        INICIO PROCESO
          var message, option, arr;

        hacer
          leer opciones  

            enCasoDe(true)

              caso(option == 1):                  
                escribir message  
                si ( longitugMessage == 0 ó tipoDeDato_message  == 'number')
                  leer 'ERROR'
                sino cipher <-- message
              parar

              caso(option == 2):
                escribir message  
                  si ( longitugMessage == 0 ó tipoDeDato_message  == 'number')
                    leer 'ERROR'
                  sino descipher <-- message
              parar

              caso(option == 3):
              parar

              default: mostrar ('No hay esa opción')

        mientras((option != 1) && (option != 2) && (option != 3));

        FIN PROCESO

        -----------------------------------------------------------------------------

        INICIO subProceso

          función cipher <--- (message)
            message = messageMayuscula

            para ( var i = 0; i < longitudMessage; i++)
              array[i] = valorUnicodeMessage
              array[i] = formulaCifradoCesar // (( arr[i] - 65 + n ) % 26 + 65)
              array[i] = devolverletraValorUnicode

          retorna mostrar message cifrado

        FIN subProceso

        ------------------------------------------------------------------------------

        INICIO subProceso

          función cipher <--- (message)
            message = messageMayuscula

            para ( var i = 0; i < longitudMessage; i++)
              array[i] = valorUnicodeMessage
              array[i] = formulaDescifradoCesar // (( arr[i] + 65 - n ) % 26 + 65)
              array[i] = devolverletraValorUnicode

          retorna mostrar message cifrado

        FIN subProceso



        
