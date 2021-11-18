# Uso do Flyway

Para instalar o flyway basta adicionar sua dependência no `pom.xml`, por padrão ele já integra com o Spring, desativando a criação de tabelas padrão do JPA.

## Criação das migrations

Para criação das migrations basta criar o diretório `src/main/resources/db/migration` e criar os arquivos `.sql`, seguindo o seguinte padrão de nome:

- `V1__nome_migration.sql`
- `V2__nome_outra_migration.sql`

OBS: Seguindo esse padrão o próprio Flyway conseguirá rodar os scripts na ordem.
