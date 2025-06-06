<h1>Requisitos de Software</h1>

<h2>Conecta Refeições</h2>

## Sumário

- [Sumário](#sumário)
- [Introdução](#introdução)
  - [Definições, Acrônimos e Abreviações](#definições-acrônimos-e-abreviações)
- [Usuários identificados](#usuários-identificados)
- [Requisitos funcionais](#requisitos-funcionais)
- [Requisitos não-funcionais](#requisitos-não-funcionais)
  - [Disponibilidade](#disponibilidade)
  - [Privacidade e segurança](#privacidade-e-segurança)
  - [Usabilidade](#usabilidade)
  - [Suportabilidade](#suportabilidade)
  - [Interoperabilidade](#interoperabilidade)
  - [Manutenibilidade](#manutenibilidade)
  - [Desempenho](#desempenho)
  - [Implementação](#implementação)
  - [Implantação](#implantação)
- [Matriz de rastreabilidade](#matriz-de-rastreabilidade)
  - [Rastreabilidade entre NFs e RNFs](#rastreabilidade-entre-nfs-e-rnfs)

---

# Introdução

O objetivo deste documento é apresentar os requisitos de software do produto **Conecta Refeições**

## Definições, Acrônimos e Abreviações

Esta subseção fornece as definições de todos os termos, acrônimos e abreviações necessárias à adequada interpretação do Documento de Requisitos.

- Identificação dos requisitos: por convenção, a referência a requisitos é feita através do identificador de requisitos, de acordo como descrito abaixo:

  `[IDENTIFICADOR DO TIPO DE REQUISITOSidentificador do requisito]`

  O identificador do tipo de requisitos é conforme abaixo:

  - RF – Requisito Funcional
  - RNF – Requisito Não-Funcional

  O identificador do requisito será uma sequência numérica. Esse número sequencial será único para todo o conjunto de tipos de requisitos.

  **Exemplo**: RF0001, RF1234, RNF1234

# Usuários identificados

Os seguintes usuários foram identificados para o sistema:

- Usuário do sistema
  - Usuários comuns
    - Funcionários da obra
        - Gesto de obra
        - Colaborador da obra
    - Colaborador do restaurante
  - Administrador do sistema

# Requisitos funcionais

Os requisitos funcionais são descritos a seguir.

- **[RF001 - RF099]** - Obra
- **[RF100 - 199]** - Restaurante
- **[RF200 - 299]** - Administrador

**Obra**

- **[RF001]** - Como funcionário da obra, gostaria de fazer o login por meio de matrícula e senha.
- **[RF002]** - Como funcinário da obra, gostaria de visualizar o cardápio diário disponível pelos restaurantes parceiros da obra.
- **[RF003]** - Como funcionário da obra, gostaria de selecionar itens do cardápio e confirmar meu pedido de refeição.
- **[RF004]** - Como funcionário da obra, gostaria que o sistema enviasse feedbacks em tempo real sobre a refeição (Ex: Pedido recebido; Pedido enviado...).
- **[RF005]** - Como funcionário da obra, gostaria de poder editar meu pedido após a solicitação, desde que seja antes do prazo limite estabelecido pelo restaurante.
- **[RF006]** - Como funcionário da obra, gostaria de ter como adicionar alguma observação ou solicitação específica ao restaurante na hora do envio do pedido. 
- **[RF007]** - Como funcionário do restaurante gostaria de visualizar meu histórico pessoal de pedidos, com possibilidade de filtro temporal.
- **[RF008]** - Como gestor de obra, gostaria de manter funcionários da obra e colaborador do restaurante.
- **[RF009]** - Como gestor de obra, gostaria de manter resturantes parceiros, atribuindo a suas respectivas obras.
- **[RF010]** - Como gestor de obra, gostaria de visualizar relatórios relacionados a pedidos, com a possibilidade de filtro temporal.
- **[RF011]** - Como gestor de obra, gostaria de exportar relatórios de pedidos para planilhas excel.


**Restaurante**

- **[RF100]** - Como colaborar do restaurante, gostaria de disponibilizar o cardapio diariamente, para que os funcionários das obras parceiras consigam visualizar. 
- **[RF101]** - Como colaborador do restaurante, gostaria de atualizar o status de um pedido (Ex: Pedido aceito, pedido enviado...).
- **[RF102]** - Como colaborador do restaurante gostaria de alterar o cardápio em tempo real, em casos de faltar algum material.
- **[RF103]** - Como colaborador do restaurante, gostaria de estabelecer um horário de prazo limite para alteração de pedidos. 
- **[RF104]** - Como colaborador do restaurante, gostaria de registrar as refeições consumidas pelos funcionários da obra na modalidade self-service, para que tanto a construtora como o restaurante possam ter um controle preciso.
- **[RF105]** - Como colaborador do restaurante, gostaria de visualizar relatórios relacionados a pedidos, com possibilidade de filtro (Temporal, Obra específica).



# Requisitos não-funcionais

Os requisitos não-funcionais são descritos a seguir.

- **[RNF001 - 050]** - Disponibilidade
- **[RNF051 - 100]** - Privacidade e segurança
- **[RNF100 - 150]** - Usabilidade
- **[RNF151 - 200]** - Suportabilidade

# Disponibilidade

- **[RNF001]** - O sistema deve ser desenvolvido de forma que possa ser usado por dispositivos moveis como IOS e Android, e em navegadores web como Google Chrome, Mozilla Firefox, Edge e outros navegadores baseados em chromium.
- **[RNF002]** - O sistema deve ser desenvolvido de forma que possa ser escalável, ou seja, deve ser possível aumentar a capacidade de armazenamento de dados e de processamento de requisições sem que haja perda de desempenho.
- **[RNF020]** - O sistema deve ser verificado quanto ao desempenho mínimo tolerado dos lados servidor e clientes. As especificações sobre pré-requisitos de hardware e software para a execução do sistema devem ser apresentadas em uma página de pré-requisitos, que deve ser acessível a partir do rodapé do site.
- **[RNF]** - O sistema deverá ser robusto e capaz de lidar com falhas de rede ou interrupções parciais sem perda de dados ou degradação significativa do serviço.


## Segurança e confiabilidade

- **[RNF051]** - O sistema deve ser desenvolvido de forma que os dados dos clientes sejam protegidos e não sejam acessíveis por terceiros.
- **[RNF052]** - O sistema deve atender aos requisitos de privacidade da LGPD (Lei Geral de Proteção de Dados).
- **[RNF]** - O sistema deverá garantir a integridade dos dados, evitando discrepâncias entre a quantidade de refeições pedidas e as refeições registradas e entregues.
- **[RNF]** - Deverão existir procedimentos de backup e recuperação de dados para prevenir a perda de informações em caso de desastres.
- **[RNF]** - O acesso às funcionalidades e dados do sistema deverá ser baseado em perfis de usuário, garantindo que cada usuário só possa acessar as informações e realizar as ações para as quais tem permissão.
- **[RNF]** - O sistema deverá registrar logs de atividades importantes, como pedidos realizados, modificações e acessos, para fins de auditoria e rastreabilidade.


## Usabilidade

- **[RNF004]** - O sistema deverá ter uma interface de usuário simples, intuitiva e amigável, com poucos passos para concluir as tarefas principais (ex: realizar um pedido), para garantir uma migração suave do método analógico para o digital.
- **[RNF]** - O sistema deverá ser acessível para usuários com diferentes níveis de habilidade tecnológica, com foco na facilidade de uso em dispositivos móveis.
- **[RNF]** - A interface deverá ter grande visibilidade e legibilidade, especialmente para usuários em ambientes de obra.
- **[RNF019]** - O sistema deve ser desenvolvido de forma que possa ser acessado por pessoas com deficiência visual, auditiva e física.

## Manutenibilidade
- **[RNF008]** - O código do sistema deverá ser bem documentado, modular e fácil de manter, permitindo que a equipe de desenvolvimento realize correções e atualizações de forma eficiente.
- **[RNF009]** - O sistema deverá ser projetado de forma a facilitar a escrita e execução de testes automatizados e manuais, garantindo a qualidade e a detecção precoce de erros.
- **[RNF016]** - O sistema deve ser documentado de forma que possa ser facilmente compreendido por terceiros e para facilitar a manutenção do sistema.

## Desempenho

- **[RNF]** - Tempo de Resposta: As requisições do usuário (ex: carregar cardápio, confirmar pedido) deverão ser atendidas em menos de 2 segundos na maioria dos casos.
- **[RNF]** - A aplicação deverá ser otimizada para suportar dispositivos móveis com poder computacional limitado, garantindo uma experiência fluida mesmo em smartphones mais antigos.
- **[RNF]** - O software deverá conseguir suportar diversas requisições simultâneas (pedidos, confirmações) em horários de pico (ex: horários de refeição), sem degradação perceptível no desempenho.



