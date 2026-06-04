# 🌸 Iris Species Classifier — Machine Learning Demo

Projeto de Machine Learning que treina um modelo para identificar a espécie de uma flor Iris com base em suas medidas físicas.

## 📋 Sobre o Projeto

Este projeto foi desenvolvido como parte do curso de **Oracle Cloud Infrastructure (OCI)** e demonstra o processo completo de Machine Learning, desde o carregamento dos dados até a realização de previsões.

## 🔄 Fluxo do Projeto

```
Carregar Dados → Pré-processar → Treinar Modelo → Avaliar → Prever
```

## 📊 Dataset

O dataset utilizado é o famoso **Iris Dataset**, contendo 150 amostras de flores de 3 espécies diferentes:

- 🌸 *Iris Setosa*
- 🌺 *Iris Versicolor*
- 🌼 *Iris Virginica*

Cada amostra possui 4 características:

| Feature | Descrição |
|---|---|
| `sepal_length` | Comprimento da sépala (cm) |
| `sepal_width` | Largura da sépala (cm) |
| `petal_length` | Comprimento da pétala (cm) |
| `petal_width` | Largura da pétala (cm) |

## 🛠️ Tecnologias Utilizadas

- **Python 3.13**
- **Pandas** — manipulação de dados
- **Scikit-learn** — modelo de Machine Learning
- **Jupyter Notebook** — ambiente de desenvolvimento

## ⚙️ Como Executar

### 1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/ml-iris-demo.git
cd ml-iris-demo
```

### 2. Instale as dependências
```bash
conda install pandas scikit-learn
```

### 3. Abra o notebook
```bash
jupyter notebook MLDemo1.ipynb
```

### 4. Execute todas as células em ordem

> O dataset `iris.csv` é baixado automaticamente pelo notebook, não é necessário baixar manualmente.

## 🤖 Modelo

O algoritmo utilizado é a **Regressão Logística**, um classificador que aprende os padrões dos dados de treinamento e consegue prever a espécie de flores novas.

```python
model = LogisticRegression(max_iter=200)
model.fit(X, y)
```

## 🔮 Exemplo de Previsão

```python
nova_flor = pd.DataFrame([[5.1, 3.5, 1.4, 0.2]], 
              columns=['sepal_length', 'sepal_width', 'petal_length', 'petal_width'])

model.predict(nova_flor)
# Resultado: array(['setosa'])
```

## 📁 Estrutura do Projeto

```
ml-iris-demo/
├── MLDemo1.ipynb   # Notebook principal
├── iris.csv        # Dataset
└── README.md       # Este arquivo
```

## 👨‍💻 Autor

Desenvolvido durante o curso de Oracle Cloud Infrastructure (OCI).
