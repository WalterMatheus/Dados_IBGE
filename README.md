# Dados IBGE
População por estado e projeção de crescimento

## 1. Introdução e Contexto do Projeto

### Problema/Oportunidade
Dados demográficos brutos, embora ricos em informações, são complexos e de difícil interpretação para um público não técnico. A capacidade de extrair, transformar e visualizar esses dados de forma clara e interativa é um desafio comum em análises de grande volume. Este projeto serve como uma demonstração prática da minha habilidade em transformar grandes volumes de dados públicos (IBGE) em insights visuais e compreensíveis utilizando técnicas avançadas de análise de dados. Ao focar na distribuição populacional por sexo e idade e nas projeções de crescimento, o projeto não só aborda uma questão de relevância social e econômica, mas também evidencia competências em tratamento de dados e criação de visualizações impactantes (mapas e gráficos) que podem ser replicadas para outros conjuntos de dados complexos.

### Ferramentas Utilizadas
- Python para converter parte dos dados para o formato longo;
- Microsoft Excel para identificação de duplicatas e limpeza dos dados;
- Tableau para visualização;
- GitHub para controle de versão e portfólio.

## 2. Coleta e Aquisição de Dados

### Fonte dos Dados
Dataset do IBGE: https://www.ibge.gov.br/estatisticas/sociais/populacao/9109-projecao-da-populacao.html (tabela "População por sexo e idade simples" xlsx)

### Método de Coleta
Download de arquivos xlsx e utilização de scripts Python para conversão de alguns dados para o formato longo.

## 3. Análise Exploratória de Dados

### Primeiras Observações
Não foi encontrado dados duplicados ou campos nulos, porém, foi possível observar que os anos estavam dividos por colunas, sendo necessário converter as colunas dos anos em uma dimensão (coluna) para melhor funcionamento no Tableau.

### Desafios Identificados
- Os locais (estados, regiões e país) não estavam acompanhados de suas respectivas coordenadas, o que pode ser um impedimento de visualização de dados em um mapa para determinadas ferramentas;
- O banco de dados apresenta os anos por coluna, sendo um formato que pode dificultar a visualização.

## 4. Limpeza e Pré-processamento de Dados
   
### Padronização e Transformação
Foi alterada a formatação dos dados que representavam os anos, onde esses foram convertidos para o formado longo, transformando-se as diversas colunas que representavam cada ano em uma única dimensão.

## 5. Modelagem e Organização dos Dados

### Estruturação para o Tableau
Após a conversão das diversas colunas representando os anos foi feito um ajuste visual do comprimento e expessura das linhas e colunas no Microsoft Excel para melhor navegação na tabela.

### Dicionário de Dados

| Nome da Coluna | Tipo de Dado | Descrição                                                   |
| -------------- | ------------ | ----------------------------------------------------------- |
| `IDADE`        | Texto        | Idade dos indivíduos (ex: "4 anos", "25 anos". |
| `SEXO`         | Texto        | Sexo dos indivíduos (ex: "Masculino", "Feminino").          |
| `CÓD.`         | Numérico     | Código do IBGE para a localidade ou município.              |
| `SIGLA`        | Texto        | Sigla da Unidade da Federação (ex: "SP", "RJ").             |
| `LOCAL`        | Texto        | Nome do município ou localidade.                            |
| `ANO`          | Numérico     | Ano de referência da estimativa/aferição populacional.               |
| `POPULAÇÃO`    | Numérico     | Quantidade estimada/aferida de habitantes.                  |

## 6. Visualização e Dashboard no Tableau

### Objetivo da Visualização
Desenvolvimento de dashboards interativos no Tableau para facilitar a visualização da distribuição populacional do Brasil e sua progressão ao longo dos anos.

### Tipos de Gráficos
- Gráficos de linhas para visualização da progressão da população brasileira entre os sexos masculino e feminino.
- Mapa para visualização da distribuição da população ao longo do território brasileiro.
  
### Interatividade
Implementação de filtros dinâmicos por ano, sexo e idade, permitindo que o usuário personalize sua análise.

## 7. Resultados e Insights Obtidos
   
### Principais Descobertas
É possível observar que São Paulo é o estado de maior concentração da população e que conforme avançamos em termos de idade maior fica a diferença entre população feminina e população masculina, podendo ser um indicativo de que mulheres possuem maior expectaviva de vida no Brasil.

### Valor Gerado
O projeto facilita visualização da distribuição da população pelo território brasileiro e sua progressão ao longo dos anos considerando idade e sexo, além disso, o projeto pode facilitar a automatização na geração de novos insights a partir do estabelecimento de uma nova forma da configuração dos dados.

### Resposta ao Problema/Oportunidade
Foi possível desenvolver gráficos para facilitar a visualização da distribuição da população e sua estimativa de progressão ao longo dos anos.

## 8. Próximos Passos 

### Análise por Faixas Etárias Estratégicas
- Envelhecimento Populacional: Onde está concentrada e para onde está crescendo a população idosa? Quais as implicações para saúde, previdência e serviços?
- População Jovem/Adulta: Quais regiões terão mais jovens em idade escolar ou mais adultos em idade economicamente ativa? (Fundamental para educação, mercado de trabalho, consumo).
- Razão de Dependência: Calcular e visualizar a razão de dependência (população de 0-14 anos + 65+ anos / população de 15-64 anos). Isso indica o "peso" da população não economicamente ativa sobre a ativa. Onde essa razão está crescendo/diminuindo?
- Comparação Histórica: Comparar as projeções atuais com o que realmente aconteceu em censos anteriores. Houve desvios significativos? Por quê?

### Correlações
- Economia: Como a projeção populacional se correlaciona com o PIB per capita regional ou com a taxa de desemprego?
- Infraestrutura: Onde a infraestrutura atual (hospitais, escolas, transporte) será mais ou menos sobrecarregada pelas mudanças populacionais?
- Setor Agro: Como as mudanças demográficas nas áreas rurais afetam a disponibilidade de mão de obra e o perfil de consumo/produção?

## 9. Acesso ao Projeto

### Link para o Repositório: 
- Dados IBGE
