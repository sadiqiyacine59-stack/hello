Graphique des ventes par produit
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

sns.set(style="whitegrid")

# Exemple de données fictives
data = {
    'produit': ['Produit A', 'Produit B', 'Produit C', 'Produit D'],
    'quantité': [120, 80, 150, 60],
    'prix_unitaire': [10, 15, 7, 20]
}

df = pd.DataFrame(data)

# Graphique des ventes par produit
plt.figure(figsize=(8,5))
sns.barplot(data=df, x='produit', y='quantité', palette='viridis')
plt.title("Ventes par produit")
plt.xlabel("Produit")
plt.ylabel("Quantité vendue")
plt.xticks(rotation=45)
plt.show()


