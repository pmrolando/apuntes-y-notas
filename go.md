# Go

https://golang.org/

Variables

Conversión de Tipos

Operadores

Condicionales
Ciclos
Funciones
Arreglos
Slides
Make
Append
Copy
Punteros
Structures
Métodos
Interfaces
Go routines
Archivos



package saludar

import "fmt"

// MeVes es para utilizar desde otro paquete
var MeVes string        // Publico
var noMeVes string      // Privado

// Saludar saluda una persona

func Saludar(nombre string) {
    fmt.Println("Hola", nombre)
}

func noVisible() {
    fmt.Println("No me ven desde otro paquete")
}

