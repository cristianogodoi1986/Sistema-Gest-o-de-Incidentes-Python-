

---

````markdown
<!-- Banner Superior -->
<div align="center">

# ⚙️ Sistema de Gestão de Incidentes (Python)

![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-blue)
![Python](https://img.shields.io/badge/Python-3.8%2B-yellow)
![License](https://img.shields.io/badge/Licença-MIT-green)
![ITIL](https://img.shields.io/badge/Framework-ITIL4-purple)
![Automação](https://img.shields.io/badge/Automação-Relatórios%20%26%20Gráficos-orange)

</div>

---

## 🧩 Visão Geral

O **Sistema de Gestão de Incidentes** é uma aplicação desenvolvida em **Python** para **analisar, monitorar e gerar relatórios automáticos** sobre incidentes de TI, com base nas práticas do **ITIL4**.  
Ele transforma planilhas de chamados em **dashboards profissionais**, **gráficos JPG**, **relatórios Excel**, **PDFs** e **apresentações PowerPoint**.

---

## 🚀 Funcionalidades

✅ Leitura de planilhas (Excel/CSV)  
✅ Geração automática de gráficos e relatórios (Excel, PDF e PPTX)  
✅ Métricas: SLA, MTTR, volume e reincidência  
✅ Exportação automática organizada por pastas  
✅ Visualização de indicadores ITIL  
✅ Execução local ou via Google Colab  

---

## 🧰 Tecnologias Utilizadas

| Categoria | Ferramentas / Bibliotecas |
|------------|--------------------------|
| Linguagem | Python 3.8+ |
| Manipulação de Dados | Pandas, NumPy |
| Visualização | Matplotlib |
| Arquivos Excel/PDF/PPTX | OpenPyXL, XlsxWriter, Python-PPTX |
| Imagens | Pillow |
| Framework | ITIL4 |

---

## 📦 Dependências (instale antes de rodar)

Se quiser rodar localmente, basta instalar essas bibliotecas:

```bash
pip install pandas numpy matplotlib openpyxl xlsxwriter python-pptx xlrd Pillow
````

> 💡 No Google Colab, a maioria já vem instalada — basta usar `pip install python-pptx xlsxwriter` se precisar.

---

## 📁 Estrutura do Projeto

```
SISTEMA-GESTAO-INCIDENTES/
├── data/                 # Planilhas de entrada (ex: backlog.xlsx)
├── scripts/              # Scripts Python (parte1.py, parte2.py, etc.)
├── graficos/             # Gráficos gerados (.jpg)
├── outputs/              # Saídas (Excel, PDF, PowerPoint)
├── docs/                 # Documentação e imagens
└── README.md             # Este arquivo completo
```

---

## 🧾 Como Usar o Sistema

1️⃣ Coloque sua planilha de incidentes na pasta `data/`.
2️⃣ Execute o script principal (exemplo):

```bash
python scripts/parte2.py
```

3️⃣ O sistema vai gerar automaticamente:

```
/graficos    → Imagens JPG
/outputs     → Excel, PDF e PowerPoint
```

4️⃣ Os relatórios terão nomes como:

* `Analise_Backlog_20251024_101500.xlsx`
* `Relatorio_Backlog_20251024_101500.pdf`
* `Apresentacao_Backlog_20251024_101500.pptx`

---

## 📊 Métricas Geradas

* ⏱ **MTTR (Tempo médio de resolução)**
* 📉 **SLA Compliance (%)**
* 📈 **Volume de incidentes por categoria**
* 🧩 **Taxa de reincidência**
* 👨‍💻 **Performance por solucionador**

---

## 🧠 Como Funciona Internamente

O sistema processa a planilha e identifica automaticamente colunas como:

* `status_operacional`
* `mns_status_ans`
* `solucionador`
* `prioridade`
* `grupo_designado`

> Se sua planilha tiver nomes diferentes, basta ajustar no início do script (`identificar_colunas`).

Após o mapeamento, o código:

1. Cria gráficos (`matplotlib`)
2. Gera um Excel completo (`openpyxl/xlsxwriter`)
3. Exporta relatório em PDF (`reportlab`)
4. Cria slides no PowerPoint (`python-pptx`)

---

## 🧰 Exemplo de Execução

```python
# Exemplo rápido de execução
from sistema_incidentes import gerar_relatorios

gerar_relatorios("data/backlog.xlsx")
```

Saída esperada:

```
✅ Leitura concluída: backlog.xlsx
📈 Gráficos gerados: /graficos
📊 Relatórios criados: /outputs
🎉 Processo finalizado com sucesso!
```

---

## 📸 Exemplo Visual (Dashboard Power BI ou gráfico)

> *(Você pode substituir a imagem abaixo por seu dashboard real)*
> ![Dashboard de Incidentes](https://via.placeholder.com/900x450?text=Exemplo+de+Dashboard+Power+BI)

---

## 🧭 Roadmap (Próximas melhorias)

* [ ] Adicionar API REST (Flask/FastAPI) para incidentes em tempo real
* [ ] Envio automático de relatórios por e-mail
* [ ] Interface web com Streamlit
* [ ] Dashboard interativo no Power BI Service

---

## 🤝 Contribuição

Quer contribuir com melhorias?

1. Faça um **fork** do repositório
2. Crie uma branch `feature/nova-funcionalidade`
3. Faça as alterações e envie um **Pull Request**

---

## 📜 Licença

Este projeto é licenciado sob a **MIT License**.
Você pode usar, modificar e distribuir livremente, mantendo os créditos.

---

## ✉️ Contato

**Cristiano Godoi**
💼 Gestão de Incidentes | 💡 Data Analytics | ⚙️ ITIL4

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://www.linkedin.com/in/cristiano-godoi-franciscano-25508683/)
[![Email](https://img.shields.io/badge/Email-Hotmail-blue?style=for-the-badge\&logo=microsoftoutlook\&logoColor=white)](mailto:cristiano.godoi10@hotmail.com)

---


