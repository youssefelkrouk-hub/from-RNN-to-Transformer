# Activité pratique n°4 – Architecture Transformer

Notebook PyTorch qui compare **RNN, LSTM et Transformer** sur la prédiction d'une série temporelle (`sin(x)`), puis présente **GPT** et **BERT** avec des modèles pré-entraînés (Hugging Face).

📓 Notebook : `AP4_Architecture_Transformer.ipynb`

---

## 1. Contexte : l'IA générative

![État de l'art](attention%20is%20all%20you%20need/Stateofart.jpg)

---

## 2. Avant 2017 : les RNN

![RNN](attention%20is%20all%20you%20need/RNN.jpg)

---

## 3. L'architecture Transformer

![Architecture Transformer](attention%20is%20all%20you%20need/Transformer%20Architecture.jpg)

📄 Article de référence : [`Attention Mechanism 2017.pdf`](attention%20is%20all%20you%20need/Attention%20Mechanism%202017.pdf)

---

## 4. Plan du notebook

![Architecture du notebook](attention%20is%20all%20you%20need/Notebookarch.jpg)

| Partie | Contenu |
|---|---|
| 1 | Série `sin(x)`, fenêtre glissante (longueur 10), DataLoader |
| 2 | RNN (16 unités) |
| 3 | LSTM (16 unités) |
| 4 | Transformer *from scratch* + comparaison des 3 modèles |
| 5 | GPT : attention causale (mini-GPT + `distilgpt2`) |
| 6 | BERT : `fill-mask` (`[MASK] est la capitale du Maroc.`) |

---

## 5. Lancer le projet

```bash
python -m venv venv_ap4
venv_ap4\Scripts\activate        # Windows  (Linux/macOS : source venv_ap4/bin/activate)
pip install torch numpy pandas matplotlib transformers jupyter ipykernel
jupyter notebook
```

Les parties 5 et 6 téléchargent des modèles Hugging Face au premier lancement (connexion internet nécessaire).

## 6. Structure du dossier

```
.
├── AP4_Architecture_Transformer.ipynb
├── README.md
└── attention is all you need/
    ├── Attention Mechanism 2017.pdf
    ├── Notebookarch.jpg
    ├── RNN.jpg
    ├── Stateofart.jpg
    └── Transformer Architecture.jpg
```
