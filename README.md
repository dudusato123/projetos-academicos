# projetos-academicos
criando repositório para projetos 
# 🧮 Calculadora de IMC

Este é um projeto simples feito em Python para calcular o Índice de Massa Corporal (IMC) com base no peso e altura do usuário.

## 📌 O que o projeto faz?

- Solicita ao usuário seu peso (em kg) e altura (em metros)
- Calcula o IMC utilizando a fórmula: `IMC = peso / (altura ^ 2)`
- Classifica o resultado: Abaixo do peso, Normal, Sobrepeso, etc.

## ▶️ Como usar

1. Clone o repositório
2. Execute o script no terminal com:
   ```bash
   python imc_calculadora.py



def calcular_imc(peso, altura):
    imc = peso / (altura ** 2)
    return imc

def classificar_imc(imc):
    if imc < 18.5:
        return "Abaixo do peso"
    elif imc < 24.9:
        return "Peso normal"
    elif imc < 29.9:
        return "Sobrepeso"
    elif imc < 34.9:
        return "Obesidade grau 1"
    elif imc < 39.9:
        return "Obesidade grau 2"
    else:
        return "Obesidade grau 3 (mórbida)"

def main():
    print("Calculadora de IMC")
    peso = float(input("Digite seu peso (kg): "))
    altura = float(input("Digite sua altura (m): "))

    imc = calcular_imc(peso, altura)
    classificacao = classificar_imc(imc)

    print(f"\nSeu IMC é {imc:.2f} — {classificacao}.")

if __name__ == "__main__":
    main()
