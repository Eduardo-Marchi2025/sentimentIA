# Sentiment Analysis B2W Reviews

## 📌 Sobre o Projeto
Este projeto aplica **técnicas de Processamento de Linguagem Natural (NLP)** e **Machine Learning** para realizar **análise de sentimentos** em avaliações de clientes.  
O objetivo é classificar automaticamente as reviews como **positivas** ou **negativas**, auxiliando na compreensão da percepção dos consumidores.

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
- **Pandas / NumPy** para manipulação de dados
- **Scikit-learn** para modelagem e vetorização (TF-IDF)
- **NLTK / SpaCy** para pré-processamento de texto
- **Flask** para disponibilizar o modelo via API
- **Jupyter Notebook** para experimentação

---

## 🚀 Como Executar o Projeto

### 1. Clonar o repositório
```bash
git clone https://github.com/seu-usuario/sentiment-analysis-b2w-reviews.git
cd sentiment-analysis-b2w-reviews
```

### 2. Criar ambiente virtual e instalar dependências
```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

pip install -r requirements.txt
```

### 3. Explorar os notebooks
- Experimentos: `notebooks/experiments/`
- Versão final: `notebooks/final/SentimentAnalysis_B2W_FINAL.ipynb`

### 4. Rodar a API
```bash
cd api
python app.py
```
A API estará disponível em: `http://127.0.0.1:5000/`

---

## 📊 Dataset
O dataset utilizado contém avaliações de clientes da B2W.  
Arquivo: `data/B2W-Reviews01.csv`  
Cada linha corresponde a uma review com seu respectivo rótulo de sentimento.

---

## 📈 Resultados
- Modelo baseado em **TF-IDF + Classificador (Logistic Regression / SVM)**  
- Métricas principais:
  - **Acurácia:** ~XX%  
  - **Precisão / Recall / F1-score:** disponíveis nos notebooks de experimentos

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
