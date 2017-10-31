# letras_numeros



def numeros_impares():
    impares = 1
    while True:
        yield impares
        impares = impares + 2


if __name__ == "__main__":
    generador = numeros_impares()
    print(next(generador))

    numeros= numeros_impares()
    for n in numeros:
        print(n)
        if n > 100:
            break
