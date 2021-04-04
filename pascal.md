# Pascal

## Estructura de un programa en Pascal:
```pascal
Program nombreDelPrograma;

Uses
    { Lista de librerias }

Const
    { Lista de constantes }

Type
    { Lista de tipos de datos }

Var
    { Lista de variables }


    { Declaraciónes de Procedimientos y Funciones }

Begin
    { Sentencias de código }
End.
```

## Ejemplo Hola Mundo
```pascal
Program HolaMundo;

Begin
    WriteLn('Hola Mundo');
    ReadLn;
End.
```

## Comentarios
```pascal
{ 
    Comentario 
    de varias 
    líneas 
}

(* 
    Otra forma de 
    un comentario
    multilínea
*)

// Comentario de una sola línea
```

## Tipos de datos

* Integer: 2 bytes. -32768 a 32767
* Real:
* Boolean:
* Char

## Variables
```pascal
Program UsoDeVariables;

{ Declaración de variables }
Var
    { Variable1, Variable2, ..., VariableN : TipoDeDato; }
    Numero1, Numero2: Integer;

Begin
    { Asignación de variables }
    Numero1 := 5;
    Numero2 := 1000;
End.
```

Operadores
| Simbolo | Significado |
| ------- | ----------- |
| =   | Es igual que/a |
| <>  | Es diferente que/a |
| >   | Es mayor que/a |
| <   | Es menor que/a |
| >=  | Es mayor o igual que/a |
| <=   |Es menor o igual que/a |

<!-- Funciones predefinidas -->

### If
```pascal
If CondicionBooleana Then
    { Bloque de código };
```

### If Else
```pascal
If CondicionBooleana Then
    { Bloque de código };
Else
    { Bloque de código };
```

### Case
```pascal
Case  Opcion Of
    ValorConstanteA1, ... ValorConstanteAn: { Bloque de código };
    ValorConstanteB1, ... ValorConstanteBn: { Bloque de código };
    ValorConstanteC1, ... ValorConstanteCn: { Bloque de código };
    ...
    ValorConstanteN1, ..., ValorConstanteNn: { Bloque de código };
Else
    { Bloque de código };
End;
```
### For
Repite un bloque de código un número determinado de veces, desde un valor inicial hasta un valor final, aumentando o disminuyendo el valor del contador.

```pascal
{ Aumenta el valor del contador }
For Contador := ValorInicial To ValorFinal Do
    { Bloque de código };

{ Disminuye el valor del contador }
For Contador := ValorInicial DownTo ValorFinal Do
    { Bloque de código };
```


### While

Repite un bloque de código hasta que una condición se deje de cumplir, mientras se cumpla la condición repetira el bloque.

```pascal
While CondicionBooleana Do
    { Bloque de código };
```

###  Repeat

Repite un bloque de código hasta que se cumpla una condición, mientras no se cumpla se repetira el bloque.

```pascal
Repeat
    { Bloque de código }
Until CondicionBooleana;
```

## Procedimientos

```pascal
Program UsoDeProcedimiento;
    { Declaración de un procedimiento con y sin parametros }

    { Procedimiento sin parametros }
    Procedure ProcedimientoSinParametros;
    Const
        { Lista de constantes del procedimiento }

    Type
        { Lista de tipos de datos del procedimiento }

    Var
        { Lista de variables del procedimiento }

    { Cuerpo del procedimiento }
    Begin
        { Sentencias de código }
    End;

    // Procedimiento con parametros
    Procedure ProcedimientoConParametros(Parametro1, Parametro2: TipoDeDato1; Parametro3 TipoDeDatos2);
    Const
        { Lista de constantes del procedimiento }

    Type
        { Lista de tipos de datos del procedimiento }

    Var
        { Lista de variables del procedimiento }

    { Cuerpo del procedimiento }
    Begin
        { Sentencias de código }
    End;

{ Cuerpo del programa }
Begin
    { Invocación de procedimiento sin parametros }
    ProcedimientoSinParametros;

    { Invocación de procedimiento con parametros }
    ProcedimientoConParametros(ValorParaParam1, ValorParaParam2, ValorParaParam3)
End.
```

## Funciones
```pascal
Program UsoDeFunción;

Var
    ResultadoRetornado: TipoDeDatoSimple;

    { Declaración de una función }
    Function Funcion(Parametro1, Parametro2: TipoDeDato1; Parametro3 TipoDeDatos2 ): TipoDeDatoSimpleComoRetorno;
    Const
        { Lista de constantes de la función }

    Type
        { Lista de tipos de datos de la función }

    Var
        { Lista de variables de la función }

    { Cuerpo de la función }
    Begin
        { Sentencias de código }

        { 
            Para retornar un valor se debe asignar ese valor 
            al nombre de la función 
        }
        Funcion := ValorDevuelto;
    End;

{ Cuerpo del programa }
Begin
    { Invocación de la función }
    ResultadoRetornado := Funcion(ValorParaParam1, ValorParaParam2, ValorParaParam3)
End.
```

