import matplotlib.pyplot as plt

# 1. Tendência de Estoque Diário (Gráfico de Linha)
dias = [1, 2, 3, 4, 5, 6, 7]
estoque = [100, 95, 110, 105, 120, 115, 130]

plt.figure(figsize=(8, 5))
plt.plot(dias, estoque, marker='o', color='blue', label='Estoque')
plt.title('Tendência de Estoque Diário')
plt.xlabel('Dia da Semana')
plt.ylabel('Quantidade em Estoque')
plt.legend()
plt.grid(True, linestyle='--', alpha=0.6)
plt.show()

# 2. Comparação de Produtos (Gráfico de Barras)
produtos = ['Teclado', 'Mouse', 'Monitor', 'Webcam']
quantidades = [50, 75, 30, 60]

plt.figure(figsize=(8, 5))
plt.bar(produtos, quantidades, color=['#66b3ff', '#99ff99', '#ffcc99', '#ff9999'])
plt.title('Comparação de Produtos em Estoque')
plt.xlabel('Produto')
plt.ylabel('Quantidade')
plt.grid(axis='y', linestyle='--', alpha=0.6)
plt.show()

# 3. Proporção de Categorias (Gráfico de Pizza)
categorias = ['Eletrônicos', 'Vestuário', 'Alimentos']
valores = [15000, 8000, 5000]

plt.figure(figsize=(6, 6))
plt.pie(valores, labels=categorias, autopct='%1.1f%%', startangle=90, colors=['#66b3ff','#99ff99','#ffcc99'])
plt.title('Proporção do Valor de Estoque por Categoria')
plt.show()

# 4. Preço vs Quantidade (Gráfico de Dispersão)
precos = [50, 120, 300, 80, 20]
estoque_itens = [80, 25, 10, 70, 150]

plt.figure(figsize=(8, 5))
plt.scatter(precos, estoque_itens, color='purple', s=100, alpha=0.7, edgecolors='black')
plt.title('Relação entre Preço Unitário e Quantidade em Estoque')
plt.xlabel('Preço Unitário (R$)')
plt.ylabel('Quantidade em Estoque')
plt.grid(True, linestyle='--', alpha=0.6)
plt.show()
