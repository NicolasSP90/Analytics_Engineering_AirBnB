## Engenharia de Dados e Garantia de Qualidade no Conjunto de Dados do Airbnb Rio de Janeiro

### Descrição do Projeto
Este projeto visa construir um pipeline de dados para o conjunto de dados do Airbnb sobre hospedagens na cidade do Rio de Janeiro. O objetivo é estruturar, limpar e validar os dados para criar uma base confiável para análises avançadas e insights de negócio.

O projeto utiliza uma arquitetura em camadas (Bronze, Silver e Gold) para armazenar dados brutos, processados e prontos para análise. Para isso, são aplicadas técnicas de engenharia de dados, garantindo a qualidade e a integridade dos dados em cada fase.

### Dados
O conjunto de dados <a href="http://insideairbnb.com/">"Inside Airbnb"</a>, fornece informações valiosas sobre:

**Listing (Listagem):** Detalhes de propriedades, incluindo tipo, preço, localização e comodidades.

**Reviews (Avaliações):** Avaliações de hóspedes, incluindo data, identificador da propriedade e comentários.

**Calendar (Calendário):** Disponibilidade das propriedades com datas e preços por dia.


### Estrutura do Projeto
### Camada Bronze
- Aquisição e Armazenamento de Dados:
- Baixar e estruturar os dados brutos (Listing, Reviews e Calendar) em PostgreSQL.
- Armazenar os dados brutos nas tabelas correspondentes no banco de dados.
  
### Camada Silver
**Data Clean:**
- Lidar com valores ausentes, duplicados e outliers.
- Padronizar os nomes das colunas e limpar campos textuais, removendo caracteres especiais e erros.

**Garantia da Qualidade dos Dados:**
- Definir métricas de qualidade para garantir integridade, precisão e consistência.
- Implementar verificações de qualidade contínuas.
- Testes Automatizados de Qualidade com Great Expectations:

Criar testes para validar as expectativas de dados e garantir conformidade com regras de negócios.
- Utilizar dbt para transformar e preparar os dados para análise.
- Carregar e armazenar os dados transformados no PostgreSQL.
- Validação de Expectativas com Great Expectations:

### Camada Gold
- Utilizar dbt para realizar agregações e criar uma camada otimizada para análises.
- Armazenar os dados, prontos para consultas analíticas.

### Tecnologias Utilizadas

