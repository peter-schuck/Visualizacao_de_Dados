# Relatório

> [!CAUTION]
>
> - Você <ins>**não pode utilizar ferramentas de IA para escrever este relatório**</ins>.

## Identificação

- **Nome**: Pedro Schuck de Azevedo
- **Cartão UFRGS:** 587553

## Dados utilizados

> [!IMPORTANT]
>
> - Os dados utilizados devem ser informados como **links** para as fontes originais.
> - Se houver mais de um conjunto de dados, liste todos separadamente.
> - Para cada conjunto de dados, inclua também uma **descrição curta** explicando os dados.

1. **Dataset Instituto Nacional de Meteorologia (INMET)**: https://portal.inmet.gov.br/dadoshistoricos
    * **Descrição curta**: Dados meteorológicos com múltiplas variávies (precipitação, umidade, temperatura e etc) de distintos períodos de tempo e locais do Brasil. Especificamente para esta visualização, utilizou-se dados de Porto Alegre do ano de 2024.

## Código-fonte da visualização

> [!IMPORTANT]
>
> - Indique abaixo onde está, dentro deste repositório, o código-fonte usado para gerar a visualização.

- **Arquivo principal**: visualization-project.ipynb
- **Arquivos complementares (se houver)**: dados_climaticos_jardim_botanico.CSV
  - Dados climáticos referentes ao bairro Jardim Botânico usados para gerar a visualização.

## Imagem da visualização gerada

> [!IMPORTANT]
>
> - Insira aqui uma imagem da visualização criada por você. Troque `imagem-da-visualizacao.png` pelo caminho correto do arquivo no repositório. 
> - Se você criou alguma visualização interativa, então descreva aqui como acessá-la. Por exemplo, se for uma página HTML, coloque o link, ou se for uma visualização 3D, descreva como compilar e executar o código. 

Para interagir com a visualização (movimentar o slider ou checar os atributos de cada ponto do scatterplot) basta rodar as células do notebook em qualquer ambiente que possua as bibliotecas pandas e altair de python, desde que os dados do .CSV estejam na mesma pasta que este.

![Visualização resultante](imagem-da-visualizacao.png)

## Descrição da visualização

### Legenda (*caption*)

> [!IMPORTANT]
>
> - Escreva um texto curto explicando como interpretar a visualização. Descreva os elementos visuais, eixos, cores, símbolos ou interações relevantes.
> - Este texto seria a legenda (*caption*) que acompanharia a figura em uma publicação, por exemplo.

Scatterplot com agregação em Bubble chart da temperatura (°C) pela umidade (%) para todos os dias do ano de 2024 no bairro Jardim Botânico de Porto Alegre. Cada ponto representa um dia no scatterplot com a cor referindo-se a quantidade de precipitação (mm) nele ou representa um conjunto de dias no Bubble chart agregado, com a área do círculo representando a contagem da quantidade de dias que correspondem a certa faixa de temperatura e umidade.

### Conclusão demonstrada pela visualização

> [!IMPORTANT]
>
> - Escreva uma conclusão curta sobre os dados com base na visualização.
> - Explique qual insight, padrão ou tendência pode ser observado.

Percebe-se que existe uma leve correlação negativa entre temperatura e umidade, ou seja, dias mais quentes tendem a ser menos úmidos. Fora isso, a precipitação parece ser a causa de alguns dos dias mais úmidos, além de manter as temperaturas perto da faixa de 20 a 22°C. Mantendo o foco na contagem de dias, nota-se que a grande maioria encontra-se nos intervalos de 20 a 26°C de temperatura e 65 a 85% de umidade, indicando uma predominância anual de temperaturas amenas e umidade relativamente alta.
