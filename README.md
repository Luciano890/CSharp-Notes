# CSharp-Notes
Notas del lenguaje de programación C#

# Menú

- [Excepciones](#Excepciones)
  - [when](#when)
- [POO](#POO)
- [Herencia](#Herencia)
- [Clases Abstractas](#Clases-Abstractas)

---

## Excepciones

<p align="center">
<img src="https://thatcsharpguy.github.io/postimages//aprende-c-sharp/ex/diagram.png" alt="Herencia de excepciones" />
</p>

```c#
try
{
    /*Algo de Código*/
}
catch (FormatException e) /*Deben ir las excepciones especifica siempre de primeras*/
{
    /*Algo de Código*/
}
catch (Exception e) /*Excepcion General*/
{
    Console.WriteLine(e.Message); /*Ver cual excepcion fue arrojada*/
}
```

### when

otra forma de capturar excepciones especificas

```c#
try
{
    /*Algo de Código*/
}            
catch (Exception e) when ((e.GetType() != typeof(FormatException))) /*Todas las excepciones menos FormatException*/
{
    Console.WriteLine(e.Message); /*Ver cual excepcion fue arrojada*/
}
catch (FormatException e)
{
    /*Algo de Código*/
}
```

---

## POO

---

## Herencia

---

## Clases Abstractas

---
