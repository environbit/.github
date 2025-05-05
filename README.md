# Serviços

 ## Service Mesh
 - [main-api](https://gitlab.com/environbit/service-mesh/main-api)
   A Main API tem por objetivo ser um "gateway" de comunicação entre interfaces externas, como por exemplo o front end, com isso podemos alterar os contratos de APIs internas sem que o front end ou aplicações que utilizem nossos serviços de API sofram com possiveis breaking changes. Além disso para aspiraçoes futuras a main api pode vir a ser utilizado como um sidecar, dando assim o real sentido de utilizarmos a palavra "service mesh" em nosso contexto de arquitetura.

 - [improve-service](https://gitlab.com/environbit/service-mesh/improve-service)
  Entende se por Improve Service o microserviço responsável encapsular funções que estejam especificamente relacionados à enriquecimento de dados.

# Arquitetura e Padrões

## Conventional Commit e SemVer
O Conventional Commit é um padrão de mensagem de commit que visam ajudar a manter a história do código de um projeto de software organizada e coesa. As mensagens de commit seguindo este padrão consistem em um tipo, um escopo opcional e uma descrição curta. O tipo pode ser uma das seguintes opções: "feat" (nova funcionalidade), "fix" (correção de bug), "docs" (mudanças na documentação), entre outras. O escopo opcional é usado para especificar em qual parte do projeto a mudança foi feita. A descrição curta fornece uma breve explicação da mudança realizada.

Usar o Conventional Commit tem várias vantagens. Primeiro, ajuda a manter a história do código organizada e fácil de entender, já que as mensagens de commit seguem um padrão consistente. Isso também facilita o uso de ferramentas de automação, como geradores de changelog ou ferramentas de versionamento automático. Além disso, o Conventional Commit é compatível com o padrão SemVer (Semantic Versioning), o que significa que as mudanças nas mensagens de commit podem ser usadas para gerar automaticamente novas versões do software.

- Disclaimer: Recomendamos a utilização de libs que forcem o uso do conventional commit para garantir que o padrão esteja sendo aplicado e para que nâo quebre o fluxo de versionamento automatico.

- Referência: [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/#summary)

## Service Mesh
Um service mesh é uma camada de software que se coloca entre os serviços de uma aplicação e a rede de comunicação. Ele gerencia a comunicação entre os serviços de uma aplicação distribuída, fornecendo funcionalidades como roteamento de tráfego, balanceamento de carga, monitoramento, segurança e outras.

Em um contexto de microsserviços, um service mesh é uma opção útil para gerenciar a complexidade de comunicação entre vários serviços pequenos e independentes. Ele permite que cada serviço se concentre em sua própria funcionalidade, enquanto o service mesh cuida da comunicação entre os serviços e da infraestrutura necessária para isso.

O uso de um service mesh também pode simplificar a implantação e a manutenção de uma aplicação distribuída, pois todas as configurações de comunicação são centralizadas e gerenciadas pelo service mesh. Além disso, um service mesh pode fornecer uma visão mais clara da comunicação entre os serviços, facilitando o monitoramento e a depuração de problemas.

- Referência: [Artigo](https://www.redhat.com/pt-br/topics/microservices/what-is-a-service-mesh)

## Divisão por módulos
Organizar uma aplicação por módulos também é importante para manter o código organizado e de fácil manutenção. Dividir o código em módulos separados permite que os desenvolvedores trabalhem em partes específicas do projeto de forma independente, sem afetar o resto da aplicação. Além disso, isso também facilita a reutilização de código em outros projetos.

- Referência: [TAO OF Node)](https://alexkondov.com/tao-of-node/)

## Serverless
Uma arquitetura serverless é uma forma de construir e executar aplicativos e serviços sem ter que se preocupar com a infraestrutura de servidor. Em vez disso, os desenvolvedores podem simplesmente escrever código e deixar que a plataforma se preocupe com a execução e escalabilidade do aplicativo. Isso pode ser mais eficiente do ponto de vista de custo e pode permitir que os desenvolvedores se concentrem mais no código da aplicação em si, em vez de se preocuparem com a configuração e manutenção da infraestrutura de servidor.

- Referência: [Docs](https://www.serverless.com/framework/docs/providers/aws/guide/intro)

## MVC
MVC é um padrão de arquitetura de software que divide uma aplicação em três camadas principais: modelo, visualização e controlador. O objetivo é separar os aspectos de lógica de negócios, interface do usuário e de controle de fluxo de uma aplicação em componentes independentes.

A camada do modelo representa os dados e a lógica de negócios da aplicação. Ela é responsável por acessar e manipular os dados, como por exemplo realizar consultas a um banco de dados ou fazer cálculos.

A camada da visualização representa a interface do usuário da aplicação, ou seja, como os dados são apresentados para o usuário final. Ela pode ser implementada como páginas HTML, componentes de interface de usuário em uma aplicação desktop ou tela de um aplicativo mobile.

A camada do controlador é responsável por gerenciar o fluxo de trabalho da aplicação, recebendo as solicitações do usuário, chamando o modelo para obter os dados necessários e passando os dados para a visualização para serem exibidos.

- Referência: [Artigo](https://www.codecademy.com/article/mvc)

## Infraestrutura as a Code (IaC)
Infrastructure as Code (IaC) é uma prática de gerenciamento de infraestrutura de TI que consiste em tratar a configuração da infraestrutura de um sistema de computadores, como código. Isso significa que, em vez de configurar manualmente os componentes da infraestrutura (como servidores, redes e armazenamento), essa configuração é especificada em um arquivo de código, que pode ser versionado, testado e gerenciado de forma semelhante ao código de uma aplicação.

O objetivo da IaC é tornar o gerenciamento da infraestrutura mais automatizado, repetível e confiável. Isso pode ajudar a reduzir erros humanos, diminuir o tempo gasto com configuração manual e facilitar a implantação e a manutenção de sistemas. Além disso, a IaC também pode ser usada para documentar e compreender melhor a configuração da infraestrutura de um sistema.
