# Projeto de Construção de Imagens Docker

## Descrição

Este projeto tem como objetivo demonstrar o processo de construção de imagens Docker para um ambiente de desenvolvimento completo, incluindo um front-end em React e um back-end em Node.js com integração ao banco de dados MySQL. O projeto está configurado para utilizar GitHub Actions para automação de build e testes, garantindo que todas as alterações no código sejam verificadas automaticamente.

## Estrutura do Projeto

- **front-end/**: Contém o código do front-end desenvolvido em React.
- **back-end/**: Contém o código do back-end desenvolvido em Node.js.
- **Dockerfile**: Arquivo de configuração para construção da imagem Docker do MySQL.
- **.github/workflows/**: Contém os workflows do GitHub Actions para build e testes automatizados.

## Processo de Construção das Imagens

1. **Configuração do MySQL**: O Dockerfile do MySQL é configurado com as variáveis de ambiente necessárias para inicializar o banco de dados.
2. **Build do Front-end**: Utilizando o Node.js, as dependências são instaladas e o front-end é construído.
3. **Testes do Back-end**: As dependências do back-end são instaladas e os testes são executados utilizando o Jest.
4. **Automação com GitHub Actions**: O workflow do GitHub Actions é configurado para executar os passos de build e teste automaticamente em cada push ou pull request na branch `develop`.

## Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
   ```

2. Construa e inicie os contêineres Docker:
   ```bash
   docker-compose up --build
   ```

3. Acesse o front-end em `http://localhost:3000` e o back-end em `http://localhost:5000`.

## Contribuição

Sinta-se à vontade para contribuir com o projeto. Faça um fork do repositório, crie uma nova branch para suas alterações e envie um pull request.

## Licença

Este projeto está licenciado sob a Licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
