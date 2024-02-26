import networkx as nx
import matplotlib.pyplot as plt

# Criar um objeto de grafo
G = nx.Graph()

# Adicionar nós
G.add_node(1)
G.add_node(2)
G.add_node(3)
G.add_node(4)
G.add_node(5)

# Adicionar arestas
G.add_edge(1, 2)
G.add_edge(1, 3)
G.add_edge(2, 3)
G.add_edge(3, 4)
G.add_edge(4, 5)
G.add_edge(1, 5)

# Plotar o grafo
nx.draw(G, with_labels=True, node_color='skyblue', node_size=800, font_size=10, font_weight='bold')
plt.show()
