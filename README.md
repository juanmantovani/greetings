#Saludos en Go
Este paquete proporciona una forma simple de obtener saludos personalizados en Go.

##Instalacion
Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u https://github.com/juanmantovani/greetings
```

##Uso
Aquí tiees un ejemplo de cómo utilizar el paquete en tu código

```go
package main

import (
	"fmt"
	"log"

	"github.com/juanmantovani/greetings"
)

func main() {
    message, err := greetings.Hello("Juan")
	
    if err != nil {
		log.Fatal(err)
	}
	
    fmt.Println(message)
}

```