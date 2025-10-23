# Fashion‑MNIST — CNN (TensorFlow)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hugo-42/fashion-mnist-cnn-tf/blob/main/Fashion_MNIST_portfolio.ipynb)

**Projet portfolio** : classification d'images de vêtements (10 classes, 28×28) avec un **réseau de neurones convolutionnel (CNN)** sous **TensorFlow/Keras**.

- 🌐 **Demo (GitHub Pages)** : https://hugo-42.github.io/fashion-mnist-cnn-tf/
- 📓 **Notebook sur GitHub** : https://github.com/hugo-42/fashion-mnist-cnn-tf/blob/main/Fashion_MNIST_portfolio.ipynb

---

## Objectif
Construire un CNN compact et reproductible pour reconnaître les classes du dataset **Fashion‑MNIST**, avec un notebook exécutable en un clic dans **Google Colab**.

## Données
- Source : `tensorflow.keras.datasets.fashion_mnist`
- Format : images 28×28 (niveaux de gris), 10 classes
- Split standard entraînement/test fourni

## Modèle
- Blocs : **Conv → ReLU → MaxPool** (×2), **Dropout**
- Couches **Denses (FC)** → **Softmax (10)**
- Optimiseur : **Adam** • Perte : `sparse_categorical_crossentropy`

## Résultats (référence)
- Accuracy validation : **91%**
- Accuracy test : **90%**
> Les résultats varient selon le matériel et les versions des bibliothèques.

---

## Démarrer

### 1) Google Colab (recommandé)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hugo-42/fashion-mnist-cnn-tf/blob/main/Fashion_MNIST_portfolio.ipynb)

### 2) Local
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```
Ouvrez **Fashion_MNIST_portfolio.ipynb** et exécutez les cellules.

---

## Aperçus
![Courbes d'apprentissage](assets/learning_curves.png)
![Matrice de confusion](assets/confusion_matrix.png)

---

## Structure suggérée du dépôt
```
fashion-mnist-cnn-tf/
├─ Fashion_MNIST_portfolio.ipynb
├─ requirements.txt
├─ README.md
├─ LICENSE
├─ docs/
│  └─ index.html        # Page GitHub Pages
└─ assets/
   ├─ learning_curves.png
   └─ confusion_matrix.png
```

---

## Licence
[MIT](LICENSE)

---

## Auteur
- GitHub : [hugo-42](https://github.com/hugo-42)
