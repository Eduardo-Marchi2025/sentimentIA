 # PROJETO SENTIMENTAPI: Análise Automatizada de Sentimentos

## 📌 Sobre o Projeto
O presente projeto tem como objetivo o desenvolvimento de uma solução automatizada para classificação de sentimentos em textos.
A solução desenvolvida consiste em um pipeline completo de classificação de sentimentos, capaz de receber textos escritos por clientes 
e classificá-los de forma binária como **Positivos** ou **Negativos**, possibilitando sua integração com aplicações externas por meio de uma API simples.
Foram aplicadas técnicas de **Processamento de Linguagem Natural (NLP)** e **Machine Learning** para realizar **Análise de Sentimentos** em avaliações reais de clientes,
por meio do dataset **B2W Reviews**.  

---

## 📁 Estrutura do Projeto

```text
sentiment-analysis-b2w-reviews/
│
├── data/
│   └── B2W-Reviews01.csv
│
├── notebooks/
│   ├── final/
│   │   └── SentimentAnalysis_B2W_FINAL.ipynb
│   │
│   └── experiments/
│       ├── Ajustes_TFIDF.ipynb
│       ├── Testes_Acuracia.ipynb
│       └── Versoes_Intermediarias.ipynb
│
├── models/
│   ├── modelo_sentimental.joblib
│   └── vectorizer_tfidf.joblib
│
├── api/
│   └── app.py
│
├── docs/
│   └── explicacao_projeto.pdf
│
└── README.md
```

---

## ⚙️ Tecnologias Utilizadas
- **Python 3.9+**
- **Pandas / NumPy**
- **matplotlib** 
- **Scikit-learn** 
- **NLTK** 
- **Jupyter Notebook** 
- **Joblib e ONNX**
  
---

## ▶️ Como Executar o Projeto no Google Colab

### 1️⃣ Abrir o Notebook:

- Acesse este repositório no GitHub  
- Clique no arquivo **`.ipynb`**  
- Clique em **“Open in Colab”**  
  ou abra manualmente em:  
  [https://colab.research.google.com](https://colab.research.google.com/drive/1-SYVnlF0YSwYr3pq0gcc9TxUHoVJApLU?usp=sharing)

---

### 2️⃣ Instalar Dependências

Execute a primeira célula do notebook para instalar as bibliotecas necessárias:

```python
!pip install pandas numpy scikit-learn nltk

````

### 3️⃣ Upload do Dataset

No Google Colab:

- Clique no ícone de pastas (barra lateral esquerda)

- Faça upload do arquivo .csv

- Verifique se o caminho do arquivo corresponde ao usado no notebook

Exemplo:
```python
df = pd.read_csv('/content/dataset.csv')
```

### 4️⃣ Execução do Notebook

Execute todas as células em ordem, de cima para baixo

O notebook está organizado nas seguintes etapas:

- Carregamento dos dados
- Carregamento e Inspeção Inicial dos Dados
- Seleção e Limpeza dos Dados
- Criação do Rótulo de Sentimento
- Análise Exploratória (EDA)
- Pré-processamento de Texto
- Vetorização com TF-IDF
- Treino e Teste
- Treinamento do Modelo
- Avaliação
- Salvando o Modelo (para API)
- Exemplo de Inferência

---

## 📊 Dataset

O conjunto de dados utilizado é composto por avaliações e comentários reais de clientes extraídos de um dataset da B2W Reviews.

- Dataset: B2W-Reviews01
- Autores: Real, L. , Oshiro, M. Mafra, A.
- Arquivo: `data/B2W-Reviews01.csv`  
- Plataforma: GitHub
- Link: [Repositório do GitHub](https://github.com/b2wdigital/b2w-reviews01)

Este projeto é de caráter educacional, e todos os créditos pelo conjunto de dados pertencem ao seu respectivo autor.


---

## 📈 Resultados
- Acurácia: O resultado foi de aproximadamente 95% (0.9484).

- Precisão (Precision): Para 'Negativo', foi de 0.92, e para 'Positivo', 0.96.

- Recall (Sensibilidade): Para 'Negativo', foi de 0.91, e para 'Positivo', 0.97.

- F1-score: Para 'Negativo', foi de 0.91, e para 'Positivo', 0.96.

 ---

## 📄 Documentação
Mais detalhes sobre o projeto podem ser encontrados em:  
`docs/explicacao_projeto.pdf`

---

## 🤝 Contribuição
Contribuições são bem-vindas!  
1. Faça um fork do projeto  
2. Crie uma branch (`git checkout -b feature/nova-feature`)  
3. Commit suas alterações (`git commit -m 'Adiciona nova feature'`)  
4. Push para a branch (`git push origin feature/nova-feature`)  
5. Abra um Pull Request  

---

## 📜 Licença
Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
