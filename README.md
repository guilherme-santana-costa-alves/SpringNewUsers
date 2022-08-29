# SpringNewUsers
#### Construindo uma API REST com banco de dados usando Java e Spring Boot

**Pré-requisitos:**
 - Lógica de programação (qualquer linguagem)
 - Programação orientada a objetos (qualquer linguagem)
 - Ferramentas
 - Spring Tool Suite (STS)
 - Postman

**Visão geral do sistema**
Vamos construir um sistema (API REST) de usuários e departamentos, com os seguintes casos de uso:

 - Buscar todos usuários
 - Buscar um usuário pelo seu id
 - Inserir um novo usuário

![image](https://user-images.githubusercontent.com/53286067/187309375-d5a402cc-bf24-4a82-b2aa-791321b42247.png)

**Desenvolvimento moderno: relacional -> objeto -> json**

![image](https://user-images.githubusercontent.com/53286067/187309425-cf7d28aa-0bcb-4d76-b35d-f112619d28da.png)

**Configuração do Maven Resources Plugin**

```
<plugin>
	<groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-resources-plugin</artifactId>
	<version>3.1.0</version>
</plugin>
```

**Configurações do banco de dados**

```
# Dados de conexão com o banco H2
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.username=sa
spring.datasource.password=

# Configuração do cliente web do banco H2
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console

# Configuração para mostrar o SQL no console
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```
