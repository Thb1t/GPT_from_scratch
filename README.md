# 🤖 My Language Models from Scratch  

![Python](https://img.shields.io/badge/python-3.9%2B-blue.svg)  
![PyTorch](https://img.shields.io/badge/PyTorch-1.12%2B-red.svg)  
![License](https://img.shields.io/badge/license-MIT-green.svg)  
![Contributions](https://img.shields.io/badge/contributions-welcome-orange.svg)  

Welcome to **GPT from Scratch**!  
The goal of this project is to **implement a Transformer model step by step**, inspired by the architecture behind **GPT (Generative Pre-trained Transformer)**.  

This repository shows how to go from **a simple Bigram model** ➡️ to **a multi-layer Transformer** capable of generating text in French 🇫🇷 and English 🇬🇧 for example.  

---

## 📚 Inspirations  
This project is based on:  
- 🎥 [Andrej Karpathy – Let's build GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY)  
- 📄 The scientific paper ["Attention is All You Need"](https://en.wikipedia.org/wiki/Attention_Is_All_You_Need) 
- 🧠 OpenAI’s GPT-2 / GPT-3 and [nanoGPT](https://github.com/karpathy/nanoGPT)  

---

## ⚙️ How it works
- 📖 Read a text dataset (Victor Hugo or Harry Potter, multilingual)
- 🔢 Create a mapping between **characters ↔ integers**
- 🧩 Build **encoders/decoders** to switch between text and numbers
- ✂️ Split the dataset into **training (90%)** and **validation (10%)**
- 📦 Process text into **blocks** (context windows) and **batches**
- 🏗️ Implement a **Bigram Language Model**
- 🚀 Train the model using **PyTorch** (`AdamW` optimizer)
- ✨ Generate new text sequences and have fun 😆 !!!

---

## 📂 Repository structure  
- `Bigram.py` → Bigram model + first experiments  
- `Transformer.py` → Full Transformer implementation  
- `text/` → Training corpora (Victor Hugo, Harry Potter, …)  

---

## 🏋️ Training Example  


After just **5,000 iterations**, the model starts producing French-like words (though not meaningful sentences yet):


<custom-element data-json="%7B%22type%22%3A%22table-metadata%22%2C%22attributes%22%3A%7B%22title%22%3A%22Exemple%20avec%20d%C3%A9filement%22%7D%7D" />

<custom-element data-json="%7B%22type%22%3A%22table-metadata%22%2C%22attributes%22%3A%7B%22title%22%3A%22Texte%20g%C3%A9n%C3%A9r%C3%A9%20apr%C3%A8s%205%20000%20it%C3%A9rations%22%7D%7D" />

| Description        | Example                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|--------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Generated Text** | <div style="height: 300px; overflow-y: auto; white-space: pre-wrap;">L'homme a vie Vient pared »<br> Et leurs pas, ébranlant les arches colossales, Troublent les morts couchés sous le pavé des salles.<br> « Oui, nous triomphons ! Venez, sœurs en toutes la foules échoses,<br> D'où fut notre prend notre tout fincens.  Le vent les dérité ! cerf, s'édiffrer leur ma des voix ;<br> Et le parles mourents sourirs le profondée, Mour !<br> Mère du bois ils Dieu la vise ent l'air fait des blancs de mains croisées, Triste, tous entière flots que jour passe ;<br> Il pour leur verra qui son ne ferait cette dans la mière ;<br> Le jour est tête en jour, ils sont là sour ma nombre,<br> Ne velous tra. Qu'on noir mon sangla ! Pierme qu'il nous dans les femmes ?<br> Ils ne s'en vont travailler quinze heures sous dont les tiffles ; Il profond des de l'enfini qui sortes astères,<br> La femme sous luille avec le noir poit.<br> Sans le vers main mauglant, filets attenant ; L'horreur bon est comte le vieille ; L'inge nous pare ; le maître ; leurs mes bleaux ; S'il me vol branche l'amour, regarde, et la nuit.<br> La pauvre montagne homme a Va degrés ! »<br> Le vol plus à cert la porte fix sont qui le partie : La maine se valle, Pour les bouche pritaint en pleint frilleur,<br> Et vous êtes l'homme un flot de l'empire à leur bouille !<br> Qui pourre mon cherveux qui rapportez, dans ce chacun !<br> Par à peine ces deux enfants, couvres Ainsi qu'un pour toute heure ;<br> Parvu qu'il elle, frappe elle lible, Temble, à dérans les coiffres qu'un regarde en tremblant son coeur,<br> Je coupens saint le vert d'enfant mennuit pleur moment.<br> Son bis non sang qu'on chevaiement plus frappé.<br> Car vous êtes pous l'ombre de l'amour même ! Vous êtes l'oasis qu'on le luit mour conde et tout fini.<br> Oui, a regarde et de la petite flamme Son au son aeuil s'aira ces ondeul !<br> Car dans le borouche, âme en pyréche à la mal !<br> Couris à la la penit ses cartant pas, L'ondre effroi de sa démon pable à voix !<br> Si ma triste, S'ai je double qui pleur main et voleur !<br> Il vit, qui fui voulez : Chantez, ples mortes,  Cette foule qui fait ce que mure vous</div> |


---
## Schema 
Here you can find the schema of a Transformer Model :
![Transformer Schema](img/Encoder-Decoder.png)

Here is a cool schema I found ! It is a realy clear explanation of the different dimension :
![Dimension Schema](img/dimension.png)
