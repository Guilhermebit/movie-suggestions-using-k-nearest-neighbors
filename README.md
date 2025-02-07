<p align="center">
  <img src="https://img.shields.io/badge/python-3.11+-blue" alt="Python version" />
</p>

## Objetivo
Este projeto implementa um sistema de recomendação de filmes utilizando o algoritmo de Machine Learning K-Nearest Neighbors (KNN). A ideia é sugerir filmes para um usuário com base nas avaliações de outros usuários com interesses semelhantes através do cálculo da distância euclidiana. 
A análise foi realizada usando o conjunto de dados do [MovieLens](https://grouplens.org/datasets/movielens/latest/) **ml-latest-small.zip**.

## Tecnologias
- Python 3.x
- Pandas
- NumPy
- Matplotlib

## 🔍 Como funciona o KNN?  

O **K-Nearest Neighbors (KNN)** é um algoritmo de aprendizado de máquina baseado em instâncias, usado para classificação e regressão. Ele funciona da seguinte forma:  

1. Dado um ponto de entrada, o algoritmo busca os **K vizinhos mais próximos** com base em uma métrica de distância.  
2. No caso da recomendação de filmes, esses vizinhos são usuários com preferências semelhantes.  
3. Os filmes mais bem avaliados por esses vizinhos são recomendados ao usuário-alvo.  

No nosso caso, utilizamos a **distância euclidiana** para medir a semelhança entre os usuários.  

---

## 📏 O que é a Distância Euclidiana?  

A **distância euclidiana** mede o quão longe dois pontos estão em um espaço multidimensional. Ela é definida pela fórmula:  

<div align="center">
  <img src="https://github.com/user-attachments/assets/6ceac1af-6b79-4246-a262-45bfba86b4b6" alt="Euclidean Distance Formula" width="300">
</div>


Onde:  
- \( A \) e \( B \) são vetores representando dois usuários.  
- \( n \) é o número de filmes avaliados.  
- Quanto menor a distância, maior a similaridade entre os usuários.  

No contexto deste projeto, a distância entre usuários representa o grau de similaridade entre suas preferências. Quanto menor a distância entre um usuário e seus vizinhos mais próximos, mais semelhantes são seus gostos.
