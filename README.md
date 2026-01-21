# Tech Challenge - Fase 2

O ToggleMaster é um ecossistema de microsserviços distribuídos. 

A arquitetura da aplicação é composta por 5 microsserviços:   

• **auth-service (Go):** 
Gerencia chaves de API e autenticação. (Banco de Dados: PostgreSQL)

• **flag-service (Python):** 
CRUD das definições das feature flags. (Banco de Dados: PostgreSQL) 

• **targeting-service (Python):** 
Gerencia regras complexas de segmentação. (Banco de Dados: PostgreSQL) 

• **evaluation-service (Go):** 
O "caminho quente" (hot path) de alta performance que retorna a decisão final (true/false). (Cache: Redis) 

• **analytics-service (Python):** 
Consome eventos de uma fila e salva dados de análise. (Fila: AWS SQS, Banco de Dados: AWS DynamoDB)
