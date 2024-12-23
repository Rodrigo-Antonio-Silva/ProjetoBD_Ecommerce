# Modelo Conceitual de Banco de Dados para E-commerce

Este repositório contém o modelo conceitual e relacional de um banco de dados desenvolvido para atender às necessidades de um sistema de e-commerce. Ele faz parte do Bootcamp Dio/Suzano para análise de dados. O objetivo desse primeiro desafio é estruturar um esquema eficiente para gerenciar informações relacionadas a produtos, clientes, pedidos, pagamentos, fornecedores, estoque e logística, garantindo consistência, integridade e flexibilidade no armazenamento e manipulação dos dados.

## Contexto do Projeto

Com a crescente demanda por plataformas de e-commerce, é essencial contar com um banco de dados bem estruturado que possa suportar operações complexas, como:

- Cadastro de clientes, fornecedores e vendedores;
- Gerenciamento de produtos e suas respectivas disponibilidades em estoque;
- Controle de pedidos, faturamento e pagamentos;
- Registro de preços, descontos e promoções aplicáveis;
- Rastreamento de fretes e entrega de produtos.

O modelo foi projetado seguindo as melhores práticas de modelagem de banco de dados, priorizando a normalização para evitar redundâncias e assegurar a integridade dos dados.

## Esquema do Banco de Dados

A imagem abaixo ilustra o modelo conceitual do banco de dados:

![Modelo Conceitual de E-commerce](caminho/para/sua/imagem.png)

## Descrição Geral das Entidades

1. **Cliente**: Contém informações pessoais dos clientes cadastrados no sistema, como nome, CPF/CNPJ e endereço. Permite a classificação do tipo de cliente (ex.: pessoa física ou jurídica).
   
2. **Fornecedor**: Gerencia os dados dos fornecedores responsáveis pelo fornecimento de produtos disponíveis no e-commerce.

3. **Produto**: Representa os itens vendidos no e-commerce, incluindo informações como nome, descrição, categoria e preços. Os preços são gerenciados separadamente para permitir flexibilidade em alterações e promoções.

4. **Estoque**: Controla a entrada e saída de produtos no estoque, permitindo rastrear quantidades disponíveis.

5. **Pedido**: Registra as solicitações feitas pelos clientes, incluindo a data, itens do pedido, quantidade e total calculado. Permite o acompanhamento do status do pedido (ex.: aprovado ou pendente).

6. **Fatura**: Relacionada aos pedidos, armazena as informações de faturamento, como data de emissão, método de pagamento e vínculo com o frete.

7. **Frete**: Controla os dados logísticos, como modalidade de envio, valor, código de rastreamento e tempo estimado para entrega.

8. **Forma de Pagamento**: Lista as opções de pagamento disponíveis, como cartão de crédito, boleto, entre outros.

9. **Disponibiliza**: Relaciona os fornecedores aos produtos que eles oferecem, permitindo identificar de onde cada item foi adquirido.

10. **Vendedor**: Representa os vendedores que disponibilizam produtos, com a opção de categorizar se são terceirizados.

11. **Preço**: Gerencia os valores associados a produtos, incluindo preço atual, descontos aplicáveis e preço ajustado.

## Benefícios do Modelo

- **Escalabilidade**: O modelo permite o crescimento do sistema, com possibilidade de inclusão de novos relacionamentos e atributos.
- **Flexibilidade**: A estrutura modular facilita a adaptação para atender a novos requisitos do negócio.
- **Rastreamento**: A gestão detalhada de preços, estoque, pedidos e faturas garante um controle rigoroso das operações.

## Como Usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
