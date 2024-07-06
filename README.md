# WinesQuality
Construção de  uma aplicação em nuvem usando o Amazon sagemaker para o pipeline de machine learning
A ideia
Definir se um vinho é um bom vinho ou não,usando um algoritmo de classificação e o conjunto de dados "Qualidade de vinhos" disponibilizado em UCI Machine Learning Repository, e produzido por Comissão de Viticultura da Região dos Vinhos Verdes (CVRVV) , Porto, Portugal.

O conjunto de dados
Os dois conjuntos de dados estão relacionados com as variantes tinto e branco do vinho "Vinho Verde" português. Devido a questões de privacidade e logística, apenas variáveis ​​físico-químicas (entradas) e sensoriais (saída) estão disponíveis. Esses conjuntos de dados podem ser vistos como tarefas de classificação ou regressão. As classes são ordenadas e não equilibradas.

Features
Variável de entrada:

acidez fixa
acidez volátil
ácido cítrico
açúcar residual
cloretos
dióxido de enxofre livre
dióxido de enxofre total
densidade
pH
sulfatos
álcool Variável de saída (com base em dados sensoriais):
qualidade (pontuação entre 0 e 10)
Citação do dataset
P. Cortez, A. Cerdeira, F. Almeida, T. Matos e J. Reis. Modelagem de preferências de vinho por mineração de dados de propriedades físico-químicas. In Decision Support Systems, Elsevier, 47 (4): 547-553, 2009.

Configuração do laboratório
Apartir da qualidade que é um número na base 10(0 à 10) transforma num número na base 2(0 ou 1) para ter uma clasiificação. 1-Considerado um bom vinho, 2-considerado um vinho ruim. Notas de qualidade igual ou acima de 6 são considerados bons vinhos.

Pipeline no aws sagemaker
Após definido e formulado um problema, e coletado os dados, o próximo passo são:

analisar os dados
definir se as características funcionam para a regra de negócio
implantar o modelo
selecionar o modelo
treinar o modelo
avaliar e fazer os testes
