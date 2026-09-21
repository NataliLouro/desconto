# 🏷️ Sistema de Desconto Progressivo

Programa em Python desenvolvido para calcular automaticamente o valor final de uma compra com base em faixas de desconto progressivo.

---

## 🛠️ Regras de Desconto

| Valor da Compra (R$) | Percentual de Desconto |
| :--- | :---: |
| Menor que R$ 200,00 | **5%** |
| Entre R$ 200,00 e R$ 299,99 | **10%** |
| Maior ou igual a R$ 300,00 | **15%** |

---

## 💻 Código-Fonte (`desconto_progressivo.py`)

```python
# Programa de Sistema de Desconto Progressivo para Loja Online

# 1. Entrada de dados
valor_compra = float(input("Digite o valor total da compra (R$): "))

# 2. Estrutura condicional para determinar a taxa de desconto
if valor_compra < 200.00:
    taxa_desconto = 0.05   # 5% de desconto
elif valor_compra < 300.00:
    taxa_desconto = 0.10   # 10% de desconto
else:
    taxa_desconto = 0.15   # 15% de desconto

# 3. Processamento/Cálculos
valor_desconto = valor_compra * taxa_desconto
valor_final = valor_compra - valor_desconto

# 4. Saída de dados
print("\n--- RESUMO DA COMPRA ---")
print(f"Valor original: R$ {valor_compra:.2f}")
print(f"Porcentagem de desconto: {int(taxa_desconto * 100)}%")
print(f"Valor do desconto: R$ {valor_desconto:.2f}")
print(f"Valor final a pagar: R$ {valor_final:.2f}")
```
