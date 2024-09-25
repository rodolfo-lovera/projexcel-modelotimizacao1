# Projeto de Otimização - Compra de Insumos para produção de Suco 

Este repositório contém um projeto de otimização baseado na compra de insumos para a produção de suco de laranja, com o objetivo de realizar a compra otimizada de diversos fornecedores, levando em consideração preço, qualidade e restrições logísticas. O modelo de otimização levou em conta um objetivo, decisões de negócio e algumas restrições, separadas por abas.

## :floppy_disk: Arquivos

- **c4_Modelootimizacao.xlsx**: Arquivo principal em Excel contendo todo o modelo de otimização. Esse arquivo está dividido em 6 abas, cada uma com uma etapa específica do processo de otimização.
- **Pasta Screenshots**: Imagens que mostram o modelo e a configuração do Solver em cada etapa.

## :boom: Habilidades e Conhecimentos Desenvolvidos
### 1. Conceitos de Programação Linear
Entendimento dos princípios básicos da programação linear, como funções objetivo, variáveis de decisão e restrições.
Compreensão da estrutura de um modelo de otimização e como formulá-lo de forma matemática.

### 2. Técnicas de Modelagem
Aprendizado sobre como modelar problemas do mundo real em termos matemáticos.
Habilidade em traduzir restrições e objetivos de um problema para um formato que possa ser solucionado por algoritmos de otimização.

### 3. Decisão Baseada em Dados
Habilidade em tomar decisões informadas com base em dados quantitativos, considerando trade-offs entre custo e qualidade.
Desenvolvimento de uma mentalidade orientada por dados ao abordar problemas de negócios.

### 4. Resolução de Problemas Complexos
Capacidade de dividir problemas complexos em partes gerenciáveis e abordá-los sistematicamente.
Habilidade em aplicar métodos matemáticos e lógicos para resolver problemas.

### 5. Interpretação de Resultados
Competência para interpretar os resultados da otimização e comunicar suas implicações de forma clara para diferentes públicos.
Habilidade em transformar dados brutos em insights práticos que podem ser usados na tomada de decisão.

## :factory: Estrutura do Arquivo Excel

### 1. Aba: Specs
Contém os dados dos fornecedores, incluindo preços e índices de qualidade como:
- Acidez
- Adstringência
- Cor
- Índice Brix

Esses dados são a base para o modelo de otimização.

![Specs](https://github.com/rodolfo-lovera/projexcel-modelotimizacao1/blob/main/Screenshots/Cap4%20(1).PNG)

### 2. Aba: Optimization Model
Primeiro modelo de otimização que busca atender as restrições de qualidade e fornecimento, com base no fornecedor Florida Valencia. Aqui são estabelecidos o objetivo, as variáveis de decisão e as restrições iniciais.

![Optimization Model](https://github.com/rodolfo-lovera/projexcel-modelotimizacao1/blob/main/Screenshots/Cap4%20(2).PNG)

### 3. Aba: Relaxamento de Qualidade
Modelo de otimização focado na redução de preço, com relaxamento dos índices de qualidade. Esse modelo permite avaliar o impacto da redução de custos na qualidade final do suco.

![Relaxamento de Qualidade](https://github.com/rodolfo-lovera/projexcel-modelotimizacao1/blob/main/Screenshots/Cap4%20(3).PNG)

### 4. Aba: Análise de Redução de Qualidade
Aqui, realizei uma análise detalhada da redução de qualidade em função da diminuição do preço de compra. São calculadas as percentagens de relaxamento para diferentes parâmetros de qualidade.

![Análise de Redução de Qualidade](https://github.com/rodolfo-lovera/projexcel-modelotimizacao1/blob/main/Screenshots/Cap4%20(4).PNG)

### 5. Aba: Minimax
Neste modelo, é implementada uma otimização minimax, cujo objetivo é minimizar o impacto do maior relaxamento nos índices de qualidade. O Solver ajusta automaticamente a maior restrição relaxada.

![Minimax](https://github.com/rodolfo-lovera/projexcel-modelotimizacao1/blob/main/Screenshots/Cap4%20(5).PNG)

### 6. Aba: BIG M - Restrição de 4 Fornecedores
Modelo com a implementação de restrição de até 4 fornecedores utilizando a técnica "Big M". Nessa aba, o Solver limita a compra a no máximo quatro fornecedores, garantindo que o modelo respeite essa nova regra logística.

![BIG M](https://github.com/rodolfo-lovera/projexcel-modelotimizacao1/blob/main/Screenshots/Cap4%20(6).PNG)

## Instruções

1. Abra o arquivo `c4_Modelootimizacao.xlsx`.
2. Cada aba representa uma etapa do processo de otimização descrito acima.
3. O Solver está configurado para otimizar os modelos. Para executar o Solver, siga os passos:
   - Abra a aba relevante.
   - Vá em **Dados > Solver**.
   - Pressione **Solucionar**.

## Screenshots

Imagens de apoio do modelo e da configuração do Solver podem ser encontradas na pasta **Screenshots**.


## 📧 Contato

Para mais informações ou dúvidas, entre em contato:

- LinkedIn: [Rodolfo Lovera](www.linkedin.com/in/rodolfo-lovera)
- E-mail: rodolfo.lovera@gmail.com
