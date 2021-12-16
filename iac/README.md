# Desafio _Infrastructure-as-code_

## Motivação
Recursos de infraestrutura em nuvem devem ser criados utilizando gerenciadores de configuração, tais como [Cloudformation](https://aws.amazon.com/cloudformation/), [Terraform](https://www.terraform.io/) ou outros, garantindo que todo recurso possa ser versionado e recriado de forma facilitada.

## Objetivo
- Criar uma instância **t2.micro** (AWS) Linux utilizando **Terraform** ou **Cloudformation**.
- A instância deve ter somente às portas **80** e **443** para todos os endereços da internet.
- A porta SSH (**22**) deve estar acessível somente para um _range_ IP definido.
- **Inputs:** A execução do projeto deve aceitar dois parâmetros:
    - O IP ou _range_ necessário para o acesso da porta SSH
    - A região da _cloud_ em que será provisionada a instância
- **Outputs:** A execução deve imprimir o IP público da instância

## Extras
- Pré-instalar o docker na instância e subir a imagem do [Apache](https://hub.docker.com/_/httpd/), tornando a página padrão da ferramenta visível ao acessar o IP público da instância.

## Notas
- Todos os recursos devem ser criados usando os créditos gratuitos da AWS.
- Não esquecer de destruir os recursos após criação e testes do desafio para não haver cobranças ou esgotamento dos créditos.
