PI-6SEM (Esboço)/
├── data/
│   ├── 01_raw/          (Arquivos originais exportados do Samsung Health)
│   ├── 02_interim/      (Dados consolidados: batimentos e sono no mesmo arquivo)
│   └── 03_processed/    (Dataset final com lags, médias móveis e sem nulos)
├── notebooks/
│   ├── 01_eda_e_limpeza.ipynb        (Exploração de dados, gráficos de distribuição)
│   ├── 02_feature_engineering.ipynb  (Criação de métricas diárias e defasagem temporal)
│   ├── 03_isolation_forest.ipynb     (Modelo não supervisionado: Detecção de Anomalias)
│   └── 04_xgboost_proxy.ipynb        (Modelo supervisionado: Previsão de Frequência Basal e SHAP)
├── src/                 (Scripts Python com funções reutilizáveis)
│   ├── preprocessing.py (Funções para agrupar dias e lidar com dados faltantes)
│   └── features.py      (Funções para criar lags temporais)
├── requirements.txt
└── README.md