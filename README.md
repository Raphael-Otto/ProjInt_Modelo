# Projeto Integrador - Mercado Arco-Íris

Um modelo para o desenvolvimento do Projeto Integrador do Curso de Técnico em Desenvolvimento de Sistemas para a Internet Integrado ao Ensino Médio do IFC - Campus Araquari.

Professores: [Marco André Mendes](github.com/marcoandre) e [Alann Perini](https://github.com/AlannKPerini).


Equipe:

Links do projeto:

-   [Documentação (esse documento)](github.com/marcoandre/pi-modelo)
-   [Backend](github.com/marcoandre/pi-backend)
-   [Frontend](github.com/marcoandre/pi-frontend)


# Situação Problema

O mercado Arco-Íris, é um estabelecimento que está no ramo há alguns anos, mas o gerente do mercado sempre teve problemas em definir o que precisava comprar, o lucro de suas vendas e os produtos que estão em estoque.

Por não haver um gerenciamento adequado do estoque, há uma difuculdade em definir exatamente o lucro sobre os produtos durante o mês e ano. Também é difícil determinar os itens em estoque e nas prateleiras. Por fim, é difícil definir os produtos a comprar, para que haja sempre na sua loja.

Portanto, ao efetuar qualquer venda ele deveria poder visualizar e automaticamente ver também quais itens que foram vendidos e se possui em estoque e também a quantidade do mesmo.

# Descrição da proposta 

O foco do software é fazer com que o administrador visualize os itens vendidos e os itens em estoque para que possa haver a compra de mais produtos para a venda do mercado.

No caso dos clientes cadastrados na loja, eles terão acesso a um aplicativo do estabelecimento em que será possível visualizar todos os itens disponíveis para compra no mercado e também possível visualizar se o item está em estoque ou não.

Para um cliente efetuar o cadastro na loja, poderá se dirigir ao caixa, onde será oferecido a fazer a sua conta para poder acessar o aplicativo da loja.

O sistema terá 3 níveis de usuário: Gerente, Cliente, Caixa.

TODO: REFAZER!!!

No caso do administrador, será possível visualizar os itens em estoque e as vendas que ocorreram durante o mês e/ou ano.

Entretanto no caso dos usuários, eles poderão apenas visualizar os produtos que estão no mercado.
  
Administrador: responsável pela manutenção do site e o banco de dados, na qual também poderá visualizar o banco para ter ideia do que é necessário.

Usuário: O usuário terá acesso ao aplicativo onde poderá ver os itens que estão a venda e em estoque; E também poderá efetuar as compras na loja.

Cliente: O cliente, diferente do usuário, não terá acesso ao aplicativo da loja, mas poderá efetuar compras no estabelecimento

# Regras de negócios

FIXME: COLOCAR NOMES NAS REGRAS E RENUMERAR

-   **RN001 -** O gerente poderá visualizar a quantidade de itens vendidos durante o mês e/ou ano.
-   **RN002 -** O gerente poderá visualizar a quantidade e itens que estão em estoque.
-   **RN003 -** Os clientes precisam fazer o cadastro para acessar o aplicativo.
-   **RN004 -** O cliente poderá fazer o cadastro no caixa.
-   **RN005 -** No caso do cliente não querer se cadastrar, será usado um Cliente genérico.
-   **RN007 -** O caixa poderá aceitar cartões de crédito e/ou débito.
-   **RN008 -** O Gerente poderá acessar um relatório do fluxo do caixa de um período determinado.
-   **RNF004 - Segurança:** O sistema não deve permitir pessoas não cadastradas de usarem o aplicativo da loja. 

# Requisitos Funcionais

FIXME: SEPARAR EM ENTRADA, PROCESSAMENTO E SAÍDA

FIXME: REFORMATAR

**ENTRADA**

-   **RF001 - Cadastro de usuário:** O usuário deverá fazer o cadastro para poder utilizar o aplicativo da loja. 
    -   **Dados Necessários:** Nome Completo, CPF, RG, Senha e Número de celular
    -   **Usuários:** Clientes

- CADASTRO DE PRODUTOS ???

**PROCESSAMENTO**

-   **RF002 - Autenticação do usuário:** O sistema vai autenticar o cadastro do cliente, verificando se ele pode acessar a sua conta no aplicativo e caso possa, ele poderá usar o aplicativo.
    -   **Dados Necessários:** Nome Completo, Senha e permissão
    -   Usuários: Todos os clientes cadastrados

VENDA???

PAGAMENTO??

**SAÍDA**

-   **RF003 - Visualização dos itens disponíveis:** O sistema vai providenciar todos os itens que estarão disponíveis na loja, apenas visível para os usuários cadastrados.
-   **Dados Necessários:** Itens em estoque
-   Usuários: Todos os clientes cadastrados
-   **RF004 - Visualização da quantidade de itens:** O sistema vai providenciar a quantidade de cada item disponível na loja, apenas visível para os usuários cadastrados.
-   **Dados Necessários:** Itens em estoque, Quantidade de itens
-   Usuários: Todos os clientes cadastrados
-   **RF005 - Relatório de vendas:** O sistema vai providenciar para o gerente da loja, o relatório de produtos vendidos no dia e mês, através dos produtos passados pelo caixa.
-   **Dados Necessários:** Itens em estoque, Quantidade de itens
-   Usuários: Gerente

# Requisitos não Funcionais

-   **RNF001 - Escalabilidade:** O sistema deve ser capaz de aumentar ou diminuir conforme necessário.
-   **RNF002 - Compatibilidade:** O sistema deve ser compatível com outros sistemas mobile.
-   **RNF003 - Confiabilidade:** O sistema deve ser confiável e atender aos requisitos do usuário.
-   **RNF005 - Segurança:** O sistema não deve fornecer dados dos clientes para terceiros.
-   **RNF006 - Manutenção:** O sistema não deverá ficar fora do ar em atualizações e/ou em resoluções de problemas no aplicativo.
-   **RNF007 - Banco de Dados:** O sistema será implementado com o banco de dados MySQL.
-   **RNF008 - Legais:** O sistema deve atender às exigências da LGPD (Leis Gerais da Proteção de Dados).
-   **RNF009 - Tecnologia de front-end web:** Para a exibição em front-end, será utilizado CSS3, HTML5 e o framework de Javascript VueJS.
- Tecnologia para desenvolvimento front-end mobile: REACT Native.
-   **RNF010 - Tecnologia Back-End:** O software será desenvolvido utilizando o framework Django com o DRF.
- Navegadores???
- Plataformas de smartphones??