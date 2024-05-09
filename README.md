# MySQL---Oficina
O banco de dados da oficina mecânica é projetado para armazenar informações sobre clientes, veículos, mecânicos, ordens de serviço (OS), serviços realizados e peças utilizadas. Ele fornece uma plataforma para controlar e gerenciar a execução de ordens de serviço na oficina.

#Entidades:

    Cliente:
    Armazena informações sobre os clientes da oficina, incluindo nome, endereço e detalhes de contato.

    Veículo:
    Registra detalhes sobre os veículos dos clientes, como marca, modelo, ano e placa do veículo. Cada veículo está associado a um cliente.

    Mecânico:
    Mantém registros dos mecânicos da oficina, incluindo nome, endereço e especialidade.

    Ordem de Serviço (OS):
    Representa uma ordem de serviço emitida para um veículo específico por um cliente. Contém informações como número da OS, data de emissão, valor total, status e data de conclusão. Cada OS está associada a um cliente e um veículo.

    Serviço:
    Descreve os serviços realizados na oficina, incluindo uma descrição do serviço e seu valor. Cada serviço é associado a uma ordem de serviço e a um mecânico responsável.

    Peça:
    Representa as peças utilizadas durante os serviços na oficina, incluindo uma descrição da peça e seu valor. Cada peça está associada a uma ordem de serviço.

#Relacionamentos:
    - Um cliente pode ter vários veículos, mas cada veículo pertence a apenas um cliente.
    - Cada ordem de serviço é emitida para um único veículo por um cliente.
    - Um mecânico pode realizar vários serviços, e cada serviço é realizado por um único mecânico.
    - Uma ordem de serviço pode conter vários serviços e várias peças.
