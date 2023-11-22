```markdown
# Verificar se um Número é Primo

Neste exemplo, abordaremos como verificar se um número é primo em Python.

```python
def eh_primo(numero):
    # Um número primo é maior que 1 e divisível apenas por 1 e por ele mesmo
    if numero > 1:
        for i in range(2, int(numero**0.5) + 1):
            if (numero % i) == 0:
                return False
        else:
            return True
    else:
        return False

# Testando se o número 13 é primo
numero_teste = 13
if eh_primo(numero_teste):
    print(f"{numero_teste} é um número primo.")
else:
    print(f"{numero_teste} não é um número primo.")
```

### Explicação:

1. **Definição da Função `eh_primo`:** Criamos uma função chamada `eh_primo` que recebe um número como argumento e retorna `True` se o número for primo e `False` caso contrário.
2. **Verificação Primo:** Dentro da função, verificamos se o número é maior que 1 e, em seguida, iteramos de 2 até a raiz quadrada do número para verificar se ele é divisível por algum outro número.
3. **Teste Primo:** Testamos a função com o número 13 e exibimos uma mensagem indicando se é primo ou não usando a função `print()`.

Para executar este código, basta copiá-lo e colá-lo em um ambiente Python adequado. Isso imprimirá uma mensagem indicando se o número de teste (neste caso, 13) é primo ou não.
