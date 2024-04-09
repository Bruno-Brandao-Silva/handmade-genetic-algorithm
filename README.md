# Projeto de Algoritmo Genético em Python

Este é um projeto em Python que implementa um algoritmo genético para otimização de funções. O algoritmo inclui uma estrutura de seleção por torneio, reprodução por cruzamento, mutação, elitismo e operações genéticas para evoluir uma população em direção a valores ótimos de uma função de maximização ou minimização.

## Funcionalidades Implementadas

### 1. Representação de Indivíduos

- Os indivíduos são representados como listas de bits, onde cada bit codifica um número em ponto flutuante dentro de um intervalo especificado.
- Funções auxiliares permitem codificar e decodificar números em ponto flutuante para sua representação binária.

### 2. Funções de Fitness Implementadas

- **Quartic Function (`objective_Q1`)**: Uma função de múltiplas dimensões que visa minimizar o valor de acordo com a fórmula de quartic.
- **Ackley Function (`objective_Q2`)**: Uma função de múltiplas dimensões que visa minimizar o valor de acordo com a fórmula de Ackley.

### 3. Algoritmo Genético

- **Inicialização da População**: Gera uma população inicial de indivíduos com valores aleatórios dentro de um intervalo especificado.
- **Seleção por Torneio**: Implementa a seleção por torneio para manter a diversidade na população.
- **Cruzamento (Crossover)**: Realiza o cruzamento entre indivíduos para gerar novos descendentes.
- **Mutação**: Introduz mutações nos indivíduos para explorar novas regiões do espaço de busca.
- **Elitismo**: Mantém o melhor indivíduo da geração anterior na próxima geração para garantir convergência.

### 4. Execução do Algoritmo

- O algoritmo evolui a população por um número máximo de gerações ou até atingir um critério de convergência.
- Durante a evolução, são exibidos dados estatísticos sobre a população, como melhor indivíduo, pior indivíduo, média e desvio padrão.

## Como Executar

1. **Requisitos**
   - Python 3.x
   - Bibliotecas: `numpy`, `matplotlib`, `pandas`, `IPython`

2. **Instruções**
   - Clone este repositório para sua máquina local.
   - Certifique-se de ter os requisitos instalados.
   - Execute os scripts Python `genetic_algorithm.py` para executar o algoritmo genético para ambas as funções (`objective_Q1` ou `objective_Q2`), conforme necessário.

## Parâmetros de Configuração

- Os parâmetros do algoritmo genético, como tamanho da população, número máximo de gerações, probabilidade de mutação, intervalos de valores para os cromossomos, etc., podem ser configurados no início do script Python.

## Observações

- Os resultados e estatísticas da execução do algoritmo genético são exibidos no console.
- Você pode modificar as funções objetivo ou adicionar novas funções implementando-as e substituindo nas chamadas do algoritmo.
