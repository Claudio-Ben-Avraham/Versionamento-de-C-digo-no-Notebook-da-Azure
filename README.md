# Versionamento de Código em Notebooks do Azure com Microsoft IA

Este repositório demonstra boas práticas de versionamento de código ao trabalhar com **Notebooks do Azure** em projetos de **Inteligência Artificial (IA)** usando serviços da **Microsoft Azure**.

## 🧠 Objetivo

Permitir a rastreabilidade, colaboração e controle de alterações em projetos de ciência de dados e IA, garantindo integridade e reprodutibilidade dos experimentos através de versionamento adequado com Git e Azure DevOps/GitHub.

---

## ⚙️ Tecnologias Utilizadas

- [Azure Machine Learning](https://learn.microsoft.com/azure/machine-learning/)
- [Azure Notebooks / Jupyter Notebooks](https://notebooks.azure.com/)
- [Git](https://git-scm.com/)
- [GitHub](https://github.com/) ou [Azure Repos](https://azure.microsoft.com/services/devops/repos/)
- Python (com bibliotecas como `pandas`, `numpy`, `sklearn`, etc.)

---

## 📁 Estrutura Sugerida do Projeto

```bash
azure-ai-project/
│
├── notebooks/              # Notebooks versionados
│   ├── 01-data-preparation.ipynb
│   ├── 02-model-training.ipynb
│   └── 03-model-evaluation.ipynb
│
├── scripts/                # Scripts auxiliares exportados dos notebooks
├── data/                   # Amostras de dados (ou link para blob storage)
├── models/                 # Modelos treinados salvos
├── requirements.txt        # Dependências do projeto
└── README.md
🔄 Versionamento de Notebooks

Para garantir versionamento eficiente:

    Use checkpoints no Azure Machine Learning Studio.

    Sincronize os notebooks com um repositório GitHub ou Azure Repos.

    Evite grandes diffs exportando trechos de código para .py quando possível.

    Use comentários claros e commits frequentes.

    Utilize ferramentas como:

        nbdime para comparar notebooks

        papermill para parametrizar e executar notebooks

🚀 Como Usar

    Clone este repositório:

git clone https://github.com/seu-usuario/azure-ai-project.git
cd azure-ai-project

Configure seu ambiente (ou use um Compute Instance no Azure ML):

    pip install -r requirements.txt

    Acesse os notebooks pelo Azure Machine Learning Studio ou localmente com Jupyter.

    Salve versões importantes com git commit e envie com git push.

✅ Boas Práticas

    Use branches para testes e novas features (feature/modelo-novo)

    Utilize tags para marcar versões de experimentos

    Integre com Azure ML Experiments para rastrear métricas

    Documente cada notebook com contexto, hipóteses e resultados

📚 Referências

    Microsoft Learn – Azure Machine Learning

    Azure DevOps Docs

    nbdev – Fastai
