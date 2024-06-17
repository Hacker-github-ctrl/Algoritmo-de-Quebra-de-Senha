Olá mundo, meu nome é Wesley, então pra você que é iniciante na área de segurança da informação e hacking, tenho um desafio pra você, todo hacker é um solucionador de problemas e construtor de ferramentas, eles construam scripts pra resolver problemas, ou seja, eles podem resolver desafios diarios pra automatizar tarefas com seus Scripts, aqui tá um exemplo de um Algoritmo de quebra de senha em Python

```
#Algoritmo de Quebra de Senha
import os
import time

def quebra_de_senha(Senha_correto):
    Senha_correto = "Programador123"
    Senha = [ ]
    
    while True:
        #Enquanto o verdadeiro será bloqueado ou continuar
        
        Senha = input("\nDigite a senha correto pra entrar: ")
        if Senha == Senha_correto:           #se senha for igual a senha correto
            print("\nSenha válida. Parabens!")
            break
        else:           #senão...
            print("\nSenha inválida. Tente novamente! ")
            time.sleep(1)
            os.system('cls')
            continue
    return Senha
        
#Imprimir o resultado da Quebra da senha
Senha_correto = "Programador123"
print(quebra_de_senha(Senha_correto))
´´´
