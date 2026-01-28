# Sistema de Recomendação por Imagens Digitais

Este projeto implementa um modelo de Deep Learning capaz de classificar e recomendar imagens por similaridade visual, simulando o comportamento de sistemas de e-commerce modernos.

## 📋 Descrição do Desafio
O objetivo é criar um sistema que, ao receber a imagem de um produto, indique itens relacionados baseando-se estritamente na aparência física (formato, cor e textura), ignorando dados textuais como marca ou preço.

## 🛠️ Tecnologias Utilizadas
- **Linguagem:** Python 3.
- **Modelo:** VGG16 (Transfer Learning da ImageNet) para extração de vetores de características.
- **Métrica de Proximidade:** Similaridade de Cosseno para comparar os *embeddings* das imagens.
- **Dataset:** `tf_flowers` (TensorFlow Datasets) para simulação de catálogo.

## 🚀 Como Funciona
1.  **Extração de Características:** A rede VGG16 converte cada imagem em um vetor numérico que representa suas propriedades visuais.
2.  **Busca por Similaridade:** Quando um usuário "busca" um item, o sistema calcula a distância matemática entre o vetor desse item e todos os outros no catálogo.
3.  **Resultado:** O sistema retorna os produtos com a menor distância (maior similaridade) visual.

## 📌 Requisitos de Execução
Desenvolvido inteiramente no Google Colab, sem necessidade de downloads de datasets externos, utilizando apenas as bibliotecas padrão de Deep Learning.
