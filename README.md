# Projeto Integrador - Modelo

Um modelo para o desenvolvimento do Projeto Integrador do Curso de Técnico em Desenvolvimento de Sistemas para a Internet Integrado ao Ensino Médio do IFC - Campus Araquari.

Professores: [Marco André Mendes](github.com/marcoandre) e [Alann Perini](https://github.com/AlannKPerini).

Links do projeto:

-   [Documentação (esse documento)](github.com/marcoandre/pi-modelo)
-   [Backend](github.com/marcoandre/pi-backend)
-   [Frontend](github.com/marcoandre/pi-frontend)

# Como usar esse modelo para o Projeto Integrador

1. Faça um fork desse repositório para a sua conta do GitHub.
2. Clone o repositório para o seu computador.
3. Abra o arquivo README.md no seu editor de texto favorito (recomendamos o [Visual Studio Code](https://code.visualstudio.com/)).
4. Tenha instalada a extensão [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) no seu editor de texto.
5. Edite o arquivo README.md com as informações do seu projeto.

# Desenvolvimento

-   As equipes serão avaliadas por cada etapa da documentação e entregas realizadas.
-   Cada equipe deverá escolher um sistema para o desenvolvimento das atividades, a partir dos modelos apresentados.

# Modelos de Sistemas

## 1- Ponto de Vendas (PDV)

Tivemos a ideia de criar uma paródia do site de compras e vendas da Amazon, ou de qualquer outra empresa na qual se identifique;

A escolha desse sistema foi pelo fato de ja estarmos "acostumados" com o tema e ja estar com a ideia montada.


# Situação Problema

-   **Introdução**: O mercado Arco-Íris, é um estabelecimento que está no ramo a alguns anos, mas o gerente do mercado sempre teve problemas em definir o que precisava comprar, o lucro de suas vendas e os produtos que estão em estoque.

-   **Situação-problema**: Pelo fato de não ter algo que possa o ajudar a visualizar as coisas que acontecem com os produtos no mercado, ele não consegue definir exatamente o lucro sobre os seus produtos durante o mês e/ou ano, todos os itens em estoque e nas prateleiras e principalmente os produtos que deve comprar para que haja sempre na sua loja.

-   **Conclusão**: Portanto, ao efetuar qualquer venda ele deveria poder visualizar e automáticamente ver também quais itens que foram vendidos e se possuí em estoque e também a quantidade do mesmo.

# Descrição da proposta 

-   **Qual o foco de ação do software:** O foco do software é fazer com que o    administrador visualizar os itens vendidos e os itens em estoque para que possa haver a compra de mais produtos para a venda do mercado.

    No caso, dos clientes, que estarão cadastrados na loja, terão acesso a um aplicativo do estabelecimento em que será possível visualizar todos os itens disponíveis para compra no mercado e também possível visualizar se o item está em estoque ou não.

    Para um cliente efetuar o cadastro na loja, poderá se dirigir ao caixa, onde será oferecido a fazer a sua conta (Será necessário: CPF, RG, E-mail e senha)
    para poder acessar o aplicativo da loja.

-   **Os níveis de usuário do sistema:** Administrador, Cliente, Usuário

-   **O que poderá ser feito no software:** No caso do administrador, será possível visualizar os itens em estoque e as vendas que ocorreram durante o mês e/ou ano.

Entretanto no caso dos usuários, eles poderão apenas visualizar os produtos que estão no mercado.
  
-   **Se houver mais de um nível de usuário:** 

-       Administrador: responsável pela manutenção do site e o banco de dados, na qual também poderá visualizar o banco para ter ideia do que é necessário.

-       Usuário: O usuário terá acesso ao aplicativo onde poderá ver os itens que estão a venda e em estoque; E também poderá efetuar as compras na loja.

-       Cliente: O cliente, diferente do usuário, não terá acesso ao aplicativo da loja, mas poderá efetuar compras no estabelecimento

# Regras de negócios

-   **RN001 -** O administrador poderá visualizar a quantidade de itens vendidos durante o mês e/ou ano.
-   **RN002 -** O administrador poderá visualizar a quantidade e itens que estão em estoque.
-   **RN003 -** Os clientes precisam fazer o cadastro para acessar o aplicativo.
-   **RN004 -** O cliente poderá fazer o cadastro no caixa.
-   **RN005 -** Para efetuar o cadastro é necessário: CPF, RG, Email e uma senha.
-   **RN006 -** O cliente e o usuário poderá fazer compras na loja.
-   **RN007 -** O caixa poderá aceitar cartões de crédito e/ou débito.
-   **RN008 -** O relatório do fluxo do caixa, deverá emitir a contabilidade dos produtos e do dinheiro.

# Requisitos Funcionais

-   **RF001 - Fazer cadastro na loja:** O usuário deverá fazer o      cadastro para poder utilizar o aplicativo da loja. 
-   Dados Necessários: Nome Completo, CPF, RG, Senha e Número de celular
-   Usuários: Clientes
-   **RF002 - Autenticação do usuário:** O sistema vai autenticar o cadastro do cliente, verificando se ele pode acessar a sua conta no aplicativo e caso possa, ele poderá usar o aplicativo.
-   Dados Necessários: Nome Completo, Senha e permissão
-   Usuários: Todos os clientes cadastrados
-   **RF003 - Visualização dos itens disponíveis:** O sistema vai providenciar todos os itens que estarão disponíveis na loja, apenas visível para os usuários cadastrados.
-   Dados Necessários: Itens em estoque
-   Usuários: Todos os clientes cadastrados
-   **RF004 - Visualização da quantidade de itens:** O sistema vai providenciar a quantidade de cada item disponível na loja, apenas visível para os usuários cadastrados.
-   Dados Necessários: Itens em estoque, Quantidade de itens
-   Usuários: Todos os clientes cadastrados
-   **RF005 - Relatório de vendas:** O sistema vai providenciar para o gerente da loja, o relatório de produtos vendidos no dia e mês, através dos produtos passados pelo caixa.
-   Dados Necessários: Itens em estoque, Quantidade de itens
-   Usuários: Gerente

# Requisitos não Funcionais

-   **RNF001 - Escalabilidade:** O sistema deve ser capaz de aumentar ou diminuir conforme necessário.
-   **RNF002 - Compatibilidade:** O sistema deve ser compatível com outros sistemas mobile.
-   **RNF003 - Confiabilidade:** O sistema deve ser confiável e atender aos requisitos do usuário.
-   **RNF004 - Segurança:** O sistema não deve permitir pessoas não cadastradas de usarem o aplicativo da loja. 
-   **RNF005 - Segurança:** O sistema não deve fornecer dados de outras pessoas.
-   **RNF006 - Manutenção:** O sistema não deverá ficar fora do ar em atualizações e/ou em resoluções de problemas no aplicativo.
-   **RNF007 - Banco de Dados:** O sistema será implementado com o banco de dados MySQL.
-   **RNF008 - Legais:** O sistema deve atender às exigências da LGPD (Leis Gerais da Proteção de Dados).
-   **RNF009 - Técnologia Front-End:** Para a exibição em front-end, o software utilizará o CSS3 e o React Native, além das bibliotecas de Javascript.
-   **RNF010 - Técnologia Back-End:** O software será desenvolvido pela linguagem de programação Django.