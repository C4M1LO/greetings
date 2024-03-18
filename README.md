# Saludos en Go

Este paquete proporciona una forma simple de obtener saludos personalizados en Go

## Instalacion

Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u github.com/C4M1LO/greetings
```

## Uso
Aqui tienes un ejemplo de como utlizar el paquete en tu codigo

```go
package main

import (
	"fmt"
	"log"

	"github.com/C4M1LO/greetings"
)

func main() {
	log.SetPrefix("greetings: ")
	log.SetFlags(0)
	names := []string{"Camilo", "German", "Luis"}
	menssages, err := greetings.Hellos(names)
	if err != nil {
		log.Fatal(err)
	}
	fmt.Println(menssages)
}
```