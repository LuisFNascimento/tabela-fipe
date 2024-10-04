# Tabela FIPE - Consulta de Veículos
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/LuisFNascimento/tabela-fipe/blob/main/LICENSE)

Este projeto faz consultas à API da Tabela FIPE para buscar informações sobre carros, motos e caminhões, incluindo marcas, modelos e valores de avaliação. Ele foi desenvolvido em Java e faz uso de uma interface de linha de comando para interação com o usuário.

## Funcionalidades

* Consulta de marcas de veículos (carros, motos e caminhões).
* Busca de modelos de veículos por marca.
* Filtragem de modelos por trecho do nome.
* Exibição dos valores de avaliação dos veículos em diferentes anos.
* Estrutura do Projeto
## Pacotes:
* br.com.alura.TabelaFipe.principal: Contém a classe principal que gerencia o fluxo da aplicação.
* br.com.alura.TabelaFipe.model: Contém as classes que representam os dados retornados pela API, como Dados, Modelos, e Veiculo.
* br.com.alura.TabelaFipe.service: Contém as classes que realizam o consumo da API e a conversão dos dados.
## Classe Principal: Principal.java
 Esta classe é responsável por:
* Exibir o menu de opções para o usuário escolher entre carro, moto ou caminhão.
* Consultar a API FIPE e retornar as marcas disponíveis com base na opção selecionada.
* Permitir ao usuário filtrar modelos por trecho do nome.
* Exibir uma lista dos veículos e seus respectivos valores de avaliação, filtrados por ano.
## Serviços:
* ConsumoApi: Classe responsável por fazer as requisições à API da Tabela FIPE.
* ConverteDados: Classe responsável por converter os dados recebidos em JSON para objetos Java utilizáveis.
## Tecnologias Utilizadas
* Java 8+
* API REST: API Tabela FIPE
* Biblioteca de JSON: Utilizada para manipulação e conversão dos dados da API.
## Como Executar o Projeto
Clone o repositório:

bash
Copiar código
git clone https://github.com/seuusuario/nome-do-repositorio.git
Compile o projeto:

bash
Copiar código
javac -d bin -sourcepath src src/br/com/alura/TabelaFipe/principal/Principal.java
Execute o projeto:

bash
Copiar código
java -cp bin br.com.alura.TabelaFipe.principal.Principal
O programa exibirá o menu de opções para você escolher entre carro, moto ou caminhão.

Exemplo de Execução
csharp
Copiar código
*** OPÇÕES ***
Carro
Moto
Caminhão

Digite uma das opções para consultar:
Carro

[Exibição de marcas de carros]

Informe o código da marca para consulta:
1

[Exibição de modelos da marca escolhida]

Digite um trecho do nome do veículo a ser buscado:
Civic

[Exibição dos modelos filtrados]

Digite o código do modelo para buscar os valores de avaliação:
12345

[Exibição dos veículos com seus valores de avaliação por ano]
Contribuições
Contribuições são bem-vindas! Fique à vontade para abrir issues ou enviar pull requests.

Licença
Este projeto está licenciado sob a licença MIT - veja o arquivo LICENSE para mais detalhes.
