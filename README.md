# Predição da Vida Útil de Motores Aeronáuticos (RUL)

Este projeto tem como objetivo desenvolver um modelo preditivo para estimar a vida útil remanescente (RUL - Remaining Useful Life) de motores aeronáuticos, com base em sensores operacionais, configurações de voo e ciclos de operação. A partir de técnicas de aprendizado de máquina e validação cruzada, é possível antecipar falhas críticas, otimizar a manutenção e aumentar a segurança operacional.

## Objetivo

Prever a quantidade de ciclos restantes até a falha de cada motor com alta precisão, utilizando dados sensoriais e operacionais reais. O modelo proposto visa contribuir para a redução de custos com manutenção não planejada e melhoria da eficiência operacional.

## Metodologia

1. Pré-processamento:
   - Leitura e análise do dataset PM_train
   - Cálculo da variável alvo RUL (Remaining Useful Life)
   - Eliminação de sensores com baixa variabilidade estatística
   - Padronização das variáveis preditoras

2. Modelagem:
   - Random Forest Regressor com otimização de hiperparâmetros (GridSearchCV)
   - Validação cruzada por grupo (GroupKFold) respeitando os motores individuais
   - Avaliação com MAE, RMSE e R²

3. Visualização:
   - Gráficos de dispersão real vs previsto
   - Análises de ciclo final por motor
   - Interpretação da distribuição da vida útil

## Bibliotecas Utilizadas

pandas  
numpy  
matplotlib  
seaborn  
plotly  
scikit-learn  

## Execução

O notebook já está com os resultados executados e documentados.  
Pode ser aberto diretamente em qualquer ambiente compatível com Jupyter Notebook para exploração dos dados e adaptação do modelo.

## Estrutura

predicao-rul-motores/  
├── notebooks/  
│   └── Pred_motores_aeronauticos.ipynb  
├── README.md  
└── LICENSE

## Autor

Heitor Tonet  
Engenheiro de Controle e Automação e Cientista de Dados, com foco em aplicações industriais, mobilidade inteligente e modelagem preditiva aplicada ao mundo físico.

## Licença

Este projeto está sob a licença MIT.
