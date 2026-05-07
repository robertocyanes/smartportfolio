🟡 SmartPortfolio

SmartPortfolio é uma API REST de investimentos desenvolvida com Java 21 + Spring Boot, focada no gerenciamento de carteira, simulação de rentabilidade e organização de ativos financeiros.

A aplicação permite criar, consultar e simular investimentos de forma simples, estruturada e escalável.

🔗 Repositório: https://github.com/robertocyanes/smartportfolio

🎯 Objetivo

Este projeto foi desenvolvido com foco em:

Prática de Spring Boot moderno (v3+)
Uso de Java 21
Construção de API REST
Aplicação de boas práticas de arquitetura em camadas
Implementação de testes unitários
Estrutura pronta para QA e automação de testes
Simulação de cenários reais de investimentos
🟡 Funcionalidades
📊 Cadastro de investimentos
💰 Simulação de retorno financeiro
🟡 Consulta de carteira
🔄 Atualização de ativos
❌ Remoção de investimentos
🟡 Stack Tecnológica
Java 21
Spring Boot 3.5.6
Spring Web
Spring Data JPA
H2 Database (ambiente de testes/dev)
Maven
Lombok
JUnit 5
Spring Boot Test
🧪 Testes
🟡 Testes Unitários

O projeto utiliza JUnit 5 + Spring Boot Test, cobrindo:

Inicialização do contexto da aplicação (contextLoads)
Validação básica de configuração Spring
Base pronta para expansão de testes de Service e Controller

Exemplo atual:

@SpringBootTest
class SmartPortfolioApplicationTests {

    @Test
    void contextLoads() {
    }
}
🧪 Evolução dos Testes (Recomendado)

Estrutura pronta para expansão:

Tests de Service (Mockito)
Tests de Controller (MockMvc)
Tests de regras de negócio
Testes de cálculo financeiro
🧱 Arquitetura

O projeto segue arquitetura em camadas:

Controller → Service → Repository → Database

Separação clara de responsabilidades:

Controller → expõe API REST
Service → regras de negócio
Repository → acesso ao banco
Entity/Model → estrutura de dados
⚙️ Configuração do Projeto
🟡 Maven (pom.xml)

Projeto configurado com:

Spring Boot 3.5.6
Java 21
UTF-8 encoding garantido
Lombok para redução de boilerplate
H2 para ambiente local/testes
🚀 Como rodar o projeto
git clone https://github.com/robertocyanes/smartportfolio.git
cd smartportfolio
mvn spring-boot:run
🧪 Rodar testes
mvn test
🟡 Banco de Dados

O projeto usa H2 Database (in-memory) por padrão:

Ideal para testes
Sem necessidade de instalação
Reset automático a cada execução
📬 Exemplo de API
Criar investimento
POST /investments
{
  "name": "Tesouro Direto",
  "amount": 1000,
  "rate": 0.12
}
🟡 QA (Quality Assurance)

O projeto já está preparado para QA:

✔ Testes Manuais
Postman
Validação de status HTTP
Cenários positivos e negativos
✔ Testes Automatizados (estrutura futura)
JUnit (backend)
Mockito (mock de serviços)
Cypress (fluxos de API/integração futura)
🟡 Melhorias Futuras
🔐 Autenticação JWT
📈 Dashboard com gráficos
🟡 Docker
⚙️ CI/CD com GitHub Actions
🟡 Cobertura de testes (JaCoCo)
🧪 Testes automatizados com Cypress completo
🟡 Deploy em nuvem
🟡 Observação final

Este projeto está estruturado como base profissional de API Spring Boot com foco em evolução contínua, testes e boas práticas de engenharia de software.

Autor:
Roberto César Yanes
