

# Criar um DataFrame com os resultados fictícios da pesquisa
data = {
    'Cliente': ['Cliente 1', 'Cliente 2', 'Cliente 3', 'Cliente 4', 'Cliente 5'],
    'Satisfação': [4, 5, 3, 2, 4],
    'Facilidade de Uso': [4, 3, 5, 2, 4],
    'Suporte ao Cliente': [3, 4, 2, 5, 3]
}

df = pd.DataFrame(data)

# Calcular médias de satisfação, facilidade de uso e suporte ao cliente
media_satisfacao = df['Satisfação'].mean()
media_facilidade = df['Facilidade de Uso'].mean()
media_suporte = df['Suporte ao Cliente'].mean()

# Plotar um gráfico de barras com as médias
fig, ax = plt.subplots()
medias = [media_satisfacao, media_facilidade, media_suporte]
labels = ['Satisfação', 'Facilidade de Uso', 'Suporte ao Cliente']
ax.bar(labels, medias)
ax.set_ylabel('Média')
ax.set_title('Média de Satisfação do Cliente')

# Mostrar o gráfico
plt.show()


