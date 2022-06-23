# Analisador Léxico && Sintático da linguagem Lugosi, feito com JavaCC!!!

## Descrição (Depois de ter gerado o compilador):
- Input: Arquivo *.lug* que é compilado para uma linguagem intermediária
- Output: Arquivo de saida *.java* de mesmo nome que arquivo .lug

## Build && Run

### Requiments:
- Javac (JDK)
- Javacc

### Windows && Linux:
> Gerando o Compilador:
- `> javacc Lugosi.jj`
- `> javac *.java`
> Usando o Compilador:
- `> java Lugosi <source_file_name>.lug`
- `> java <source_file_name>.java`

## Lugosi File Example:

```Java
main
{
    var int x;
    var float y;
    var float z;

    var float zz;

    x := 10;
    y := 20;
    z := 30;

    zz := sqrt(z);

    if((x > 20))
    {
        y := (x + 20);
    };

    while((y > 1)) do
    {
        z := (zz + y);
        y := (y - 1);
    };

    print(z);
}

function float sqrt(float n)
{
    return (n * n);
}
```
