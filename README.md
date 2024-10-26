# *CÓDIGO PARA ANÁLISE DE DADOS DA API ASTEROIDES NEOWS* 📊


## LINGUAGEM UTILIZADA PARA FAZER ESSE PROJETO:

  * Python

## BIBLIOTECAS UTILIZADAS:

  * Requests: para realizar a solicitação HTTP;
  * Json: utilizada para troca de dados entre os sistemas;
  * Pandas: usada para a manipulação e análise dos dados por meio de uma DataFrame
    ![WhatsApp Image 2024-10-25 at 23 05 12](https://github.com/user-attachments/assets/1531c0d4-41ef-464a-be0b-10b57aacf168)
  * Matplotlib.pyplot: útil na criação do gráfico gerado com as informações extraídas da API.
    ![WhatsApp Image 2024-10-26 at 00 02 21](https://github.com/user-attachments/assets/77981538-7220-4506-8f11-b9cbbf49148a)
    
## FONTES DE PESQUISA:

#### Fonte dos dados:
  * https://api.nasa.gov/
    
#### Inteligência Artificial:
  * https://gemini.google.com/app/961166ade42b33a7?hl=pt-BR

#### Canais do Youtube:
  * https://www.youtube.com/watch?v=s54N3QuLdKc
  * https://www.youtube.com/watch?v=C0aj3FjN5e0
  * https://www.youtube.com/watch?v=dPb4acFiaYs

#### Sites:
  * https://www.alura.com.br/artigos/criando-graficos-no-python-com-a-matplotlib
  * https://www.alura.com.br/artigos/o-que-e-json

## FUNCIONAMENTO DO CÓDIGO

Para esse código funcionar será necerrário que o utilizador gere uma chave pessoal, os dados requisitados pelo site da NASA (https://api.nasa.gov) são nome, sobrenome e email, após a realização dessa etapa, a chave será enviada pelo email apresentado. Quando o desenvolvedor obter a chave, ele deve copiá-la e colá-la no campo "CHAVEAPI" da URL presente no código que faz a requisição para o site permitir acesso aos dados sobre os asteroides no intervalo de tempo 03-09-2003 e 10/09/2003.

É possível mudar esse intervalo de tempo apenas alterando as datas desejadas, mas a NASA só oferece informações de dados com até 7 dias entre o espaço de tempo e esses dados são adquiridos por datas que já ocorreram. Exemplo, se o desenvolvedor desejar ver dados entre 11/12/2004 e 15/12/2004, ele deverá usar esse formato: https://api.nasa.gov/neo/rest/v1/feed?start_date=2004-12-11&end_date=2004-12-15&api_key=CHAVEAPI

Eu utilizei os recursos da DataFrame que expõe os primeiros dados dos asteroides (df.head()) e os últimos dados (df.tail()) por preferência pessoal, mas fica a critério do desenvolvedor que for experimentar o código. 

As cores do gráfico foram escolhidas com base no propósito que desenvolvi esse código, mas a mudança pode ser feita apenas substituindo o "orange" pela cor que mais agrade o interessado.

**Em condições de funcianamento do código sem erros, ele deve fazer a requisição para o site da NASA e gerar DataFrames que mostram os seguintes dados dos asteroides que passaram perto da Terra no intervalo de tempo: id, nome e grau de perigosidade. Também deve ser gerado um gráfico em barras com eixo x sendo o nome do asteroide e o eixo y sendo o grau de perigosidade, com ele é possível a visualização da diferença entre as ocorrênci
as de asteroides perigosos e não perigosos.**
    
    
