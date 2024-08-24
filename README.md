




Exemplo de desafio de engenharia de dados com foco em bancos de dados NoSQL, especificamente usando o MongoDB, um banco de dados orientado a documentos.

### Desafio: "Análise de Log de Acessos em Tempo Real"

**Cenário**:
Você foi contratado por uma grande plataforma de streaming que armazena grandes volumes de logs de acessos dos seus usuários. O objetivo é construir um pipeline de dados para processar, analisar e fornecer insights sobre esses logs em tempo real. A empresa utiliza MongoDB como banco de dados NoSQL para armazenar esses logs.

Os logs de acessos contêm informações como:
- ID do usuário
- Data e hora do acesso
- Dispositivo utilizado (TV, smartphone, desktop, etc.)
- Tipo de conteúdo acessado (filme, série, documentário)
- Localização geográfica do usuário (país e cidade)
  
**Objetivos do Desafio**:
1. **Ingestão de Dados**:
   - Criar um script que simule a ingestão de dados de logs em tempo real. Esse script deve gerar eventos de acesso simulados a cada segundo e inseri-los no MongoDB.
   
2. **Estrutura do Banco de Dados**:
   - Defina o esquema de documentos no MongoDB para armazenar os logs de acesso. Considere a estrutura flexível, mas que permita consultas eficientes para a análise de dados.
   
3. **Processamento de Dados**:
   - Usando PySpark ou uma ferramenta de streaming (como Apache Kafka ou Apache Spark Streaming), processe os dados em tempo real. O processamento deve incluir:
     - Identificação de picos de acessos por minuto.
     - Agrupamento de acessos por dispositivo e tipo de conteúdo.
     - Monitoramento de acessos por localização geográfica.

4. **Análise de Dados**:
   - Após processar os dados em tempo real, gere relatórios que respondam perguntas como:
     - Quais são os horários de pico de acessos?
     - Quais são os dispositivos mais usados para acessar a plataforma?
     - Qual tipo de conteúdo é mais acessado em diferentes regiões?
   
5. **Visualização dos Dados**:
   - Construa dashboards usando uma ferramenta como Tableau, Power BI ou Grafana para visualizar em tempo real os insights gerados (por exemplo, visualização de acessos por localização e dispositivos).
   
6. **Otimização e Escalabilidade**:
   - Implemente uma solução de sharding no MongoDB para lidar com o aumento no volume de dados, garantindo que o banco de dados possa escalar horizontalmente conforme a plataforma cresce.
   - Discuta como as consultas e agregações podem ser otimizadas para grandes volumes de dados.

### Requisitos Técnicos:
- **MongoDB**: para armazenamento dos logs de acesso.
- **PySpark** ou **Apache Spark Streaming**: para processamento de dados em tempo real.
- **Dashboards**: Tableau, Power BI, ou Grafana para visualização dos insights.
- **Python**: para scripts de ingestão de dados simulados.

### Avaliação:
- Qualidade do esquema de dados no MongoDB.
- Eficiência do pipeline de ingestão e processamento de dados.
- Capacidade de escalar o banco de dados para suportar grandes volumes de dados.
- Clareza e utilidade dos insights gerados.
- Qualidade das visualizações de dados.

### Desafio Extra:
Implemente uma funcionalidade de detecção de anomalias no pipeline, que alerte automaticamente se o número de acessos por minuto ultrapassar um certo limite predefinido, indicando possível comportamento incomum (como um ataque de bot).

Esse desafio combina habilidades de engenharia de dados, big data e visualização, proporcionando uma experiência prática em cenários reais de processamento de grandes volumes de dados.



