# 🕸️ Graph Theory & Advanced Algorithms in Python

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Algorithms](https://img.shields.io/badge/Algorithms-Graph%20Theory-success.svg)](#algoritmos-e-estruturas-implementadas)
[![Testing](https://img.shields.io/badge/Tests-Unittest%20%7C%20TDD-brightgreen.svg)](tests/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENSE)

Implementação de estruturas de dados e algoritmos clássicos de **Teoria dos Grafos** em Python puro, com foco em eficiência assintótica, modularidade e cobertura de testes unitários (**TDD**).

O repositório contempla implementações completas de grafos direcionados e não-direcionados via **Listas de Adjacência** e **Matrizes de Adjacência**, além de algoritmos de travessia, caminhos mínimos com restrições, fecho transitivo e árvores geradoras mínimas.

---

## 🚀 Algoritmos e Estruturas Implementadas

| Categoria | Algoritmo / Estrutura | Complexidade | Arquivo / Módulo |
| :--- | :--- | :---: | :--- |
| **Estruturas Base** | **Lista de Adjacência** (Vértices, Arestas, Graus, Laços) | Espaço: $O(V + E)$ | `meu_grafo_lista_adj.py` |
| **Estruturas Base** | **Matriz de Adjacência** (Não-direcionada e Dígrafos) | Espaço: $O(V^2)$ | `meu_grafo_matriz_adj_dir.py` |
| **Travessia** | **Busca em Largura (BFS)** | $O(V + E)$ | `bfs()` e reconstrução em árvore |
| **Travessia** | **Busca em Profundidade (DFS)** | $O(V + E)$ | `dfs()` e detecção de conectividade |
| **Topologia** | **Detecção de Ciclos & Conectividade** | $O(V + E)$ | `ha_ciclo()`, `conexo()`, `caminho()` |
| **Fecho Transitivo** | **Algoritmo de Warshall** | $O(V^3)$ | `warshall()` (alcançabilidade em dígrafos) |
| **Árvore Geradora Mínima**| **Algoritmo de Prim** (Padrão e Modificado) | $O(V^2)$ | `prim_nao_modificado()`, `prim_modificado()` |
| **Árvore Geradora Mínima**| **Algoritmo de Kruskal** com Bucket Sort | $O(E \log V)$ | `kruskall_nao_modificado()`, `bucket_sort_kruskall()` |
| **Caminhos Otimizados** | **Dijkstra Customizado para Roteamento** | $O(V^2)$ / $O(E \log V)$ | `dijkstra_drone()` |

---

## 🧪 Qualidade de Código & Test-Driven Development (TDD)

Todas as implementações foram validadas com suítes de testes automatizados utilizando o framework `unittest` padrão do Python, garantindo:

* Verificação rigorosa de casos de borda (grafos desconexos, laços, arestas paralelas e grafos completos).
* Validação de propriedades topológicas (grau de vértices, conectividade e ciclos).
* Correção formal dos algoritmos de menor caminho e peso mínimo de árvores geradoras.

---

## 📂 Organização dos Módulos

graph-algorithms/ ├── 01-adjacency-list/ # Operações fundamentais em Listas de Adjacência ├── 02-bfs-dfs-traversal/ # Travessias em largura e profundidade com árvore geradora ├── 03-cycles-and-connectivity/ # Algoritmos de identificação de ciclos e caminhos máximos ├── 04-undirected-matrix/ # Grafos não-direcionados com Matriz de Adjacência ├── 05-directed-matrix-warshall/ # Dígrafos e Fecho Transitivo de Warshall ├── 06-minimum-spanning-tree/ # Síntese de MST via Prim e Kruskal (com Bucket Sort) └── 07-constrained-routing/ # Roteamento de menor custo e Dijkstra adaptado


---

## 🛠️ Tecnologias

* **Linguagem**: Python 3.8+ (Zero dependências externas / Vanilla Python)
* **Framework de Testes**: `unittest`
* **Paradigma**: Programação Estruturada e Orientada a Objetos com foco em Análise de Algoritmos

---

## 🚀 Como Executar e Testar

### Pré-requisitos
* Python 3 instalado no sistema.

### Executando os Testes Unitários

```bash
# 1. Clone o repositório
git clone https://github.com/caiodantass/GRAFOS.git
cd GRAFOS

# 2. Execute a suíte de testes de qualquer módulo
python -m unittest grafo_lista_adj_test.py

# Ou rode todos os testes do projeto de uma vez:
python -m unittest discover -s . -p "*_test.py"
```
---

## 👨‍💻 Autor

**Caio Lívio Dantas**  
* Engenheiro de Software / Desenvolvedor  
* LinkedIn: [linkedin.com/in/caio-lívio](https://www.linkedin.com/in/caio-l%C3%ADvio/)  
* GitHub: [@caiodantass](https://github.com/caiodantass)
