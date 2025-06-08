# 🌊 AbrigAPP - Previsão Inteligente de Riscos com IA

Projeto desenvolvido para a disciplina **Disruptive Architectures: IoT, IoB & Generative IA** da Global Solution FIAP 2025.

---

## 📌 Descrição do Projeto

Este projeto simula sensores ambientais e aplica técnicas de **Inteligência Artificial (IA)** para prever o **nível de risco de enchentes** com base em dados climáticos. A proposta está integrada ao app **AbrigAPP**, voltado ao apoio da população em eventos extremos.

A solução substitui o uso de hardware físico (Arduino/ESP32) por **simulações no Google Colab**, conforme autorizado pelo professor, mantendo foco na **comunicação IoT + análise preditiva** com Machine Learning.

---

## 🎯 Objetivo

Criar um sistema inteligente capaz de:

- Simular sensores IoT: nível de água, chuva, umidade do solo e temperatura.
- Prever automaticamente o risco de enchente (baixo, médio, alto).
- Exportar os resultados em JSON, prontos para consumo por apps ou APIs de alerta.
- Visualizar os dados e decisões do modelo com dashboards e gráficos.

---

## 🔧 Tecnologias Utilizadas

- 🧠 **Python + Scikit-learn** (Machine Learning)
- 📊 **Pandas / Matplotlib / Seaborn** (visualização de dados)
- 💻 **Google Colab** (execução do projeto)
- 📦 **Joblib** (salvamento de modelo)
- 🧾 **JSON** (formato de integração IoT)
- 🔐 **LabelEncoder** (tratamento de categorias)

---

## 🧪 Como Executar

1. Acesse o notebook pelo Colab ou clone este repositório:
2. Execute as células em ordem:
   - Simulação dos dados de sensores
   - Treinamento do modelo de IA
   - Visualizações
   - Previsão com novos dados simulados
   - Exportação da resposta como JSON

---

## 🗂️ Estrutura dos Arquivos

| Arquivo                         | Descrição                                               |
|--------------------------------|----------------------------------------------------------|
| `GS_AbrigAPP.ipynb`         | Notebook principal com todo o fluxo da solução          |
| `modelo_risco_enchente.pkl`    | Modelo treinado (Random Forest)                         |
| `label_encoder_risco.pkl`      | Encoder para transformar labels de risco                |
| `simulated_data.csv`           | Dados simulados de sensores (opcional)                  |
| `README.md`                    | Este documento                                           |

---

## 📊 Exemplo de Previsão (JSON)

```json
{
  "dados_sensores": {
    "nivel_agua_cm": 140,
    "chuva_mm": 95,
    "umidade_solo_pct": 90,
    "temperatura_C": 26
  },
  "risco_previsto": "alto"
}
