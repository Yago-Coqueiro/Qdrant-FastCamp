# Qdrant FastCamp

Repositório criado para as entregas do FastCamp, com foco em busca semântica vetorial usando o [Qdrant](https://qdrant.tech/).

---

## 📁 Arquivos

### `Qdrant_Aula.ipynb`
Notebook de quick start seguindo o material do FastCamp. Cobre os conceitos fundamentais do Qdrant:
- Instalação do cliente e do fastembed
- Conexão com o Qdrant Cloud
- Criação de collection
- Geração de embeddings e indexação de dados
- Busca semântica por similaridade

> Base de dados: cardápio de restaurante com 30 itens

---

### `Qdrant_Pratica.ipynb`
Aplicação prática desenvolvida de forma independente, utilizando os conceitos do quick start em um contexto de **triagem de pacientes**. O sistema recebe a queixa de um paciente em linguagem natural e retorna os quadros clínicos mais similares.

Diferenciais em relação ao notebook de aula:
- Payload rico com campos estruturados: CID-10, urgência, especialidade e conduta
- Filtros por metadados: urgência mínima e especialidade médica
- Filtros combinados
- Índices de payload para campos numéricos e keyword
- Célula interativa para testes com queixas personalizadas

> Base de dados: 20 quadros clínicos com diferentes níveis de urgência e especialidades

---

## 🛠️ Tecnologias

- [Qdrant](https://qdrant.tech/) — banco de dados vetorial
- [fastembed](https://github.com/qdrant/fastembed) — geração de embeddings
- Modelo: `BAAI/bge-small-en-v1.5` (384 dimensões, similaridade por cosseno)

---

## ▶️ Como executar

Ambos os notebooks foram desenvolvidos no Google Colab. Para rodar, basta clicar no badge abaixo ou abrir diretamente pelo GitHub.

1. Abra o notebook desejado no Colab
2. Substitua a `url` e a `api_key` pelas suas credenciais do Qdrant Cloud
3. Execute as células em ordem

> Conta gratuita disponível em [cloud.qdrant.io](https://cloud.qdrant.io)

---

> ⚠️ O `Qdrant_Pratica.ipynb` é estritamente educacional e não substitui avaliação médica profissional.
