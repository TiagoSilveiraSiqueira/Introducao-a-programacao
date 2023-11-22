# Verificar se um Número é Primo

def eh_primo(numero): <br>
    # Um número primo é maior que 1 e divisível apenas por 1 e por ele mesmo<br>
    if numero > 1:<br>
        for i in range(2, int(numero**0.5) + 1):<br>
            if (numero % i) == 0:<br>
                return False<br>
        else:<br>
            return True<br>
    else:<br>
        return False<br>

# Testando se o número 13 é primo<br>
numero_teste = 13<br>
if eh_primo(numero_teste):<br>
    print(f"{numero_teste} é um número primo.")<br>
else:<br>
    print(f"{numero_teste} não é um número primo.")<br>

Explicação:<br>

Definição da Função eh_primo: Criamos uma função chamada eh_primo que recebe um número como argumento e retorna True se o número for primo e False caso contrário.<br>
Verificação Primo: Dentro da função, verificamos se o número é maior que 1 e, em seguida, iteramos de 2 até a raiz quadrada do número para verificar se ele é divisível por algum outro<br> número.
Teste Primo: Testamos a função com o número 13 e exibimos uma mensagem indicando se é primo ou não usando a função print().
