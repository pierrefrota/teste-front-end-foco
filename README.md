# Teste Prático – Estágio em Front-end – Foco Tecnologia

> Bem-vindo ao teste técnico para a vaga de Estágio em Front-end na Foco Tecnologia.

Estamos ansiosos para conhecer suas habilidades em front-end e ver como você estrutura uma aplicação prática para um setor específico. Siga as instruções atentamente e fique à vontade para mostrar toda sua criatividade e capacidade técnica!

<br>

## Sobre o Desafio

A Foco Tecnologia está ampliando suas atividades e precisa de um sistema para ajudar donos de hotéis a gerenciar as reservas de seus estabelecimentos. Seu desafio será criar uma aplicação que permita aos nossos clientes:

1. Criar, listar, editar e cancelar reservas.
2. Consultar endereços automaticamente para facilitar o cadastro do responsável pela reserva.
3. Buscar quartos disponíveis para check-in.
4. Armazenar as reservas utilizando **localStorage**, garantindo a persistência dos dados entre as sessões e assegurando que as informações permaneçam disponíveis mesmo após o fechamento da aplicação.


<br>

## Objetivo da Solução

Desenvolver uma aplicação prática e intuitiva que permita aos nossos clientes hoteleiros gerenciar reservas de forma eficiente. O sistema deverá oferecer uma experiência organizada, centralizando informações de reservas e possibilitando ações rápidas, como cadastro e edição de dados. Além disso, a aplicação deve ser visualmente agradável e fácil de navegar, com funcionalidades claras que ajudem os gestores a acompanhar a ocupação de seus estabelecimentos de maneira prática e detalhada.

<br>

## Requisitos

Desenvolva as seguintes telas para a aplicação:

### 1. Tela de Cadastro de Reservas  

O fluxo de cadastro de uma nova reserva deve ser intuitivo e incluir as seguintes etapas:

- O usuário preencherá os dados de check-in, check-out e a quantidade de hóspedes.
- Em seguida, será realizada uma **busca pelos quartos disponíveis**. Usando o [JSON Server](https://github.com/typicode/json-server) com a rota `available_rooms` no arquivo `./mock/reserve_data.json`.
- Após selecionar um quarto, abrirá uma modal para preenchimento dos dados do responsável pela reserva.
- O campo de endereço do responsável deve incluir um auto-complete, consultando a API do [ViaCEP](https://viacep.com.br) a partir do CEP informado.
- Ao salvar a reserva, os dados devem ser armazenados no **localStorage**, garantindo que a reserva apareça em primeiro na listagem.
- Deve haver um botão que, ao ser clicado, navegue para a tela de listagem de reservas.

### 2. Tela de Listagem de Reservas  
Nesta tela, o usuário deverá visualizar todas as reservas registradas. A interface deve permitir as seguintes interações:

- **Listagem das reservas:** As reservas serão buscadas no **localStorage** e exibidas na tela.
- **Estrutura dos dados:** Deve seguir a estrutura da chave `reserve_list` no arquivo `./mock/reserve_data.json`
- **Botão de ações:** 
  - **Cancelamento de reservas:** Oferecer a opção de cancelar reservas conforme necessário.
  - **Alteração de status:** Permitir que o usuário mude o status das reservas, facilitando o gerenciamento das operações.

<br>


## Bônus: Tela de Dashboard

Como um diferencial, você pode desenvolver uma **tela de dashboard** que exiba uma visão geral das reservas. Essa tela pode incluir gráficos ou indicadores importantes, como:

- **Número total de reservas** no dia atual.
- **Taxa de ocupação** (porcentagem de quartos ocupados).
- **Status dos quartos**, se está sujo ou limpo.
- **Estatísticas gerais**, como número de reservas concluídas e canceladas.

Os dados da dashboard estará disponível no arquivo `./mock/dashboard.json`.

O dashboard deve ser organizado e visualmente intuitivo, oferecendo uma visão rápida para ajudar na tomada de decisões dos nossos clientes.

<br>

## Layout

- Na pasta `layout`, você encontrará os arquivos responsáveis pelo design e estrutura visual da aplicação, assim como as cores utilizadas. 
- Os ícones utilizados na interface estão armazenados na pasta `assets`.
- Se precisar adicionar mais ícones, poderá utilizar  de libs como Lucide Icons.

<br>

## Tecnologias

Você pode usar as seguintes tecnologias para implementar sua solução:

- **HTML:** Estruturação da aplicação.
- **CSS:** Estilização da interface.
- **JavaScript:** Interatividade e manipulação do DOM.
- **SASS:** Pré-processador CSS para organização e eficiência nos estilos. **(preferível)**
- **Angular ou React:** Frameworks/bibliotecas para a construção de aplicações web escaláveis e componentes reutilizáveis. **(preferível)**

<br>

## Diferenciais

Estes itens não são obrigatórios, mas serão considerados pontos extras:

- HTML semântico
- Boas práticas de SEO
- Código limpo, bem organizado e com boas práticas de lint
- Atenção à acessibilidade
- Animações que melhoram a experiência do usuário
- Uso de TypeScript para tipagem de dados
- Soluções criativas ou inovações que possam complementar a aplicação

<br>

## O que vamos avaliar

Seu trabalho será avaliado com foco em:

- Lógica e organização do código: clareza e organização na implementação.
- Boas práticas: uso de HTML semântico, SEO e acessibilidade.
- Criatividade: funcionalidades adicionais ou ideias inovadoras.

<br>

## Observações importantes

- Dúvidas: Sinta-se à vontade para entrar em contato caso tenha dúvidas sobre o teste.
- Originalidade: Evite copiar código de outras pessoas. Estamos interessados no seu processo de desenvolvimento!

<br>

## Instruções de Entrega

- Crie um repositório no GitHub com o código do projeto.
- Inclua um arquivo README.md com instruções claras sobre como rodar a aplicação e quaisquer dependências necessárias.
- Será interessante se fizer o deploy da aplicação em algum serviço como Netlify ou Vercel.

<br>


## Prazo

- O prazo para a entrega deste teste é de **7 dias** a partir da data de recebimento.

<br>

Boa sorte, e esperamos ver seu talento em ação! 

<br> 