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

---

# Introdução

O objetivo deste documento é apresentar os requisitos de software do produto **Conecta Refeições**

## Definições, Acrônimos e Abreviações

Esta subseção fornece as definições de todos os termos, acrônimos e abreviações necessárias à adequada interpretação do Documento de Requisitos.

- Identificação dos requisitos: por convenção, a referência a requisitos é feita através do identificador de requisitos, de acordo como descrito abaixo:

  `[IDENTIFICADOR DO TIPO DE REQUISITOS]`

  O identificador do tipo de requisitos é conforme abaixo:

  - RF – Requisito Funcional
  - RNF – Requisito Não-Funcional

  O identificador do requisito será uma sequência numérica. Esse número sequencial será único para todo o conjunto de tipos de requisitos.

  **Exemplo**: RF0001, RF1234, RNF1234

# Usuários identificados

Os seguintes usuários foram identificados para o sistema:

- Usuário do sistema
  - Usuário Comum
    - Colaborador da Obra
    - Colaborador do restaurante
  - Administrador
    - Gestor da obra
  


# Requisitos funcionais

Os requisitos funcionais são descritos a seguir.

- **[RF001 - RF099]** - Obra
- **[RF100 - 199]** - Restaurante

**Obra**

- **[RF001]** - Como funcionário da obra, gostaria de fazer o login por meio de matrícula e senha.
- **[RF002]** - Como funcinário da obra, gostaria de visualizar o cardápio diário disponível pelos restaurantes parceiros da obra.
- **[RF003]** - Como funcionário da obra, gostaria de selecionar itens do cardápio e confirmar meu pedido de refeição.
- **[RF004]** - Como funcionário da obra, gostaria que o sistema enviasse feedbacks em tempo real sobre a refeição (Ex: Pedido recebido; Pedido enviado...).
- **[RF005]** - Como funcionário da obra, gostaria de poder editar ou cancelar meu pedido após a solicitação, desde que seja antes do prazo limite estabelecido pelo restaurante.
- **[RF006]** - Como funcionário da obra, gostaria de ter como adicionar alguma observação ou solicitação específica ao restaurante na hora do envio do pedido. 
- **[RF007]** - Como funcionário do restaurante gostaria de visualizar meu histórico pessoal de pedidos, com possibilidade de filtro temporal.
- **[RF008]** - Como gestor de obra, gostaria de manter funcionários da obra e colaborador do restaurante.
- **[RF009]** - Como gestor de obra, gostaria de manter resturantes parceiros, atribuindo a suas respectivas obras.
- **[RF010]** - Como gestor de obra, gostaria de visualizar relatórios relacionados a pedidos, com a possibilidade de filtro (Temporal, restaurante especifico, obra...).
- **[RF011]** - Como gestor de obra, gostaria de exportar relatórios de pedidos para planilhas excel.


**Restaurante**

- **[RF100]** - Como colaborar do restaurante, gostaria de disponibilizar o cardapio diariamente, para que os funcionários das obras parceiras consigam visualizar. 
- **[RF101]** - Como colaborador do restaurante, gostaria de atualizar o status de pedido (Ex: Pedido aceito, pedido enviado...).
- **[RF102]** - Como colaborador do restaurante gostaria de alterar o cardápio em tempo real, em casos de faltar algum material.
- **[RF103]** - Como colaborador do restaurante, gostaria de estabelecer um horário de prazo limite para alteração de pedidos. 
- **[RF104]** - Como colaborador do restaurante, gostaria de registrar as refeições consumidas pelos funcionários da obra na modalidade self-service, para que tanto a construtora como o restaurante possam ter um controle preciso.
- **[RF105]** - Como colaborador do restaurante, gostaria de visualizar relatórios relacionados a pedidos, com possibilidade de filtro (Temporal, Obra específica).



# Requisitos não-funcionais

Os requisitos não-funcionais são descritos a seguir.

- **[RNF001 - 050]** - Disponibilidade
- **[RNF051 - 100]** - Privacidade e segurança
- **[RNF101 - 150]** - Usabilidade
- **[RNF151 - 200]** - Suportabilidade
- **[RNF201 - 250]** - Interoperabilidade
- **[RNF251 - 300]** - Manutenibilidade
- **[RNF301 - 350]** - Desempenho
- **[RNF351 - 400]** - Implementação
- **[RNF401 - 450]** - Implantação

## Disponibilidade

- **[RNF001]** - O sistema deve ser desenvolvido de forma que possa ser usado por navegador ou dispositivos moveis como IOS e Android.
- **[RNF002]** - O sistema deve ser desenvolvido de forma que possa ser escalável, ou seja, deve ser possível aumentar a capacidade de armazenamento de dados e de processamento de requisições sem que haja perda de desempenho.
- **[RNF]** - O sistema deverá ser robusto e capaz de lidar com falhas de rede ou interrupções parciais sem perda de dados ou degradação significativa do serviço.


## Privacidade e segurança

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
- **[RNF]** - O sistema deverá permitir a configuração de métodos de notificação (ex: e-mail, push notification) para eventos (ex: pedido confirmado, alteração de status) para cada usuário.

## Suportabilidade

- **[RNF151]** - O sistema deverá suportar diferentes navegadores, sendo eles: Google Chrome, Microsoft Edge, Mozilla Firefox e Opera. Em caso de dispositivo móvel: Android 11 (2020) ou superior / IOS 15 (2021) ou superior.

## Interoperabilidade

- **[RNF]** - O sistema deverá exportar relatórios no formato CSV e XLSX.

## Manutenibilidade

- **[RNF008]** - O código do sistema deverá ser bem documentado, modular e fácil de manter, permitindo que a equipe de desenvolvimento realize correções e atualizações de forma eficiente.
- **[RNF009]** - O sistema deverá ser projetado de forma a facilitar a escrita e execução de testes automatizados e manuais, garantindo a qualidade e a detecção precoce de erros.
- **[RNF016]** - O sistema deve ser documentado de forma que possa ser facilmente compreendido por terceiros e para facilitar a manutenção do sistema.
- **[RNF]** - Deverão ser implementadas ferramentas de monitoramento para acompanhar o desempenho e disponibilidade do sistema em tempo real.
- **[RNF]** - O sistema deverá ter ferramentas de monitoramento deverão enviar alertas automáticos para a equipe de suporte em caso de anomalias ou falhas críticas.

## Desempenho

- **[RNF]** - Tempo de Resposta: As requisições do usuário (ex: carregar cardápio, confirmar pedido) deverão ser atendidas em menos de 2 segundos na maioria dos casos.
- **[RNF]** - A aplicação deverá ser otimizada para suportar dispositivos móveis com poder computacional limitado, garantindo uma experiência fluida mesmo em smartphones mais antigos.
- **[RNF]** - O software deverá conseguir suportar diversas requisições simultâneas (pedidos, confirmações) em horários de pico (ex: horários de refeição), sem degradação perceptível no desempenho.

## Implementação

- **[RNF]** - Deverá ser disponibilizada uma central de ajuda ou seção de FAQ dentro do aplicativo ou em um portal dedicado, com informações sobre o uso do sistema.
- **[RNF]** - Deverá ser fornecido treinamento inicial para Gestores de Obra, Administradores e Colaboradores do Restaurante sobre o uso do sistema.

## Implantação

- **[RNF]** - O sistema deverá ser implantado em uma infraestrutura de servidores robusta e escalável, preferencialmente em nuvem
- **[RNF]** - Deverão ser mantidos ambientes separados para desenvolvimento e produção, para garantir testes seguros antes do deploy.








