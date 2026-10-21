# Projeto Integrador - 6º Semestre (PI-6SEM)

## 📁 Estrutura do Projeto

```text
PI-6SEM/
├── data/
│   ├── 01_raw/
│   ├── 02_interim/
│   └── 03_processed/ 
├── notebooks/
│   ├── 01_eda_e_limpeza.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_isolation_forest.ipynb
│   └── 04_xgboost_proxy.ipynb
├── src/
│   ├── preprocessing.py
│   └── features.py    
├── requirements.txt
└── README.md
```

---

## 🚀 Instalação e Configuração

Recomenda-se utilizar um ambiente virtual (`venv`) para isolar as dependências do projeto.

### 1. Criar e ativar o ambiente virtual

No terminal, na raiz do repositório, execute:

```bash
# Cria o ambiente virtual na pasta .venv
python3 -m venv .venv

# Ativa o ambiente virtual (Linux / macOS)
source .venv/bin/activate

# (Se estiver no Windows PowerShell)
# .\.venv\Scripts\Activate.ps1
```

### 2. Instalar as dependências

Com o ambiente virtual ativado, instale os pacotes necessários:

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

---

## 📓 Como Executar os Notebooks

Os notebooks estão localizados no diretório `notebooks/`. Você pode executá-los de duas maneiras:

### Opção 1: Pelo VS Code (Recomendado)

1. Certifique-se de que a extensão **Jupyter** (`ms-toolsai.jupyter`) está instalada no VS Code.
2. Abra o arquivo do notebook desejado (na pasta `notebooks/`).
3. No canto superior direito da janela do notebook, clique em **Select Kernel** (Selecionar Kernel).
4. Escolha **Python Environments...** e selecione o ambiente `.venv` (`./.venv/bin/python`).
5. Execute as células normalmente utilizando `Shift + Enter`.

### Opção 2: Pelo Navegador (JupyterLab ou Jupyter Notebook)

1. No terminal, com o ambiente virtual ativado (`source .venv/bin/activate`), inicie o servidor:
   ```bash
   # Interface JupyterLab
   jupyter lab

   # Ou interface clássica do Jupyter Notebook
   jupyter notebook
   ```
2. O navegador será aberto automaticamente (geralmente em `http://localhost:8888`).
3. Acesse a pasta `notebooks/` e abra o arquivo que deseja executar.