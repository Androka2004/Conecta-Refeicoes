# Capa

---

<h1>Requisitos de Software</h1>

<h2>Conecta Refeições</h2>

<small>Versão 1.0</small>

---

## Histórico de revisões

|    Data    | Versão |        Descrição         |                                          Autor                                           |
| :--------: | :----: | :----------------------: | :--------------------------------------------------------------------------------------: |
| 07/06/2025 |  1.0   |   Criação do documento   | Andrey Vasconcelos, João Pedro Rodrigues,  Lucas Emanuel Araujo, Pedro Arthur de Holanda |
| 28/07/2025 |  1.0   | Modificação para módulos |                                   João Pedro Rodrigues                                   |


---

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
  - Administrador do Sistema
  - Usuario comum   
    - Funcionario da Construtora
      - Colaborador da obra
      - Administração da Obra
        - Gestor da obra
    - Colaborador do Restaurante
    


# Requisitos funcionais

Os requisitos foram classificados em 5 módulos descritos a seguir:

- Módulo Geral
- Módulo Refeição  
- Módulo Restaurante  
- Módulo Gestão  
- Módulo Administrador  



### **Módulo Geral**
- **[RF001]** - Como usuário do sistema, gostaria de fazer o login por meio de matrícula ou e-mail e senha.
- **[RF010]** - Como usuário do sistema eu tenho que conseguir definir o tamanho da minha fonte no sistema
- **[RF016]** - Eu como usuário do sistema gostaria de redefinir minha senha.
- **[RF018]** - Como usuário do sistema gostaria que tivesse uma opção "Lembrar de mim" quando logasse no aplicativo

### **Módulo Refeição** 
- **[RF002]** - Como funcionário da construtora, gostaria de visualizar o cardápio diário disponibilizado pelos restaurantes parceiros da obra.
- **[RF003]** - Como funcionário da construtora, gostaria de selecionar itens do cardápio e realizar meu pedido de refeição.
- **[RF004]** - Como funcionário da construtora, gostaria de ter como adicionar alguma observação ou solicitação específica ao restaurante na hora do envio do pedido. 
- **[RF005]** - Como funcionário da construtora, desejo cancelar meu pedido após a solicitação, desde que seja antes do prazo limite estabelecido.
- **[RF006]** - Como funcionário da construtora, gostaria de poder editar meu pedido após a solicitação, desde que seja antes do prazo limite estabelecido pelo restaurante
- **[RF007]** - Como funcionário da construtora, após realizar o meu pedido, gostaria de visualizar o meu pedido atual.
- **[RF008]** - Como funcionário da construtora, após realizar o meu pedido, gostaria de visualizar o status do meu pedido. 
- **[RF011]** - Como funcionário da construtora, gostaria que existisse a possibilidade de escolher receber notificações relacionado ao status do pedido em tempo real(Ex: Pedido recebido; Pedido enviado...).
- **[RF012]** - Como funcionário da construtora, desejo confirmar o recebimento do meu alimento no aplicativo.
- **[RF014]** - Como funcionário da construtora, queria reportar erros no pedido recebido do Restaurante  
- **[RF015]** - Como funcionário da construtora, desejo pedir o café da manhã na noite anterior.
- **[RF017]** - Como funcionário da construtora, gostaria de visualizar meu histórico pessoal de pedidos, com possibilidade de filtro temporal.
- **[RF019]** - Como funcionário da construtora, desejo poder escolher se vou comer na obra ou no restaurante. 

### **Módulo Restaurante** 
- **[RF100]** - Como colaborador do restaurante, gostaria de emitir o cardápio diariamente, para que os funcionários das obras parceiras consigam visualizar.  
- **[RF101]** - Como colaborador do restaurante, gostaria de atualizar o status de pedido (Ex: Pedido aceito, pedido enviado...).
- **[RF102]** - Como colaborador do restaurante gostaria de alterar o cardápio em tempo real, em casos de faltar algum ingrediente. (Pulei por enquanto)
- **[RF103]** - Como colaborador do restaurante, gostaria de estabelecer um horário de prazo limite para alteração de pedidos, se não estabelecer será estabelecido automaticamente por meio do sistema. 
- **[RF104]** - Como colaborador do restaurante, gostaria de registrar as refeições consumidas pelos funcionários da obra quando visitam o restaurante, para que tanto a construtora como o restaurante possam ter um controle preciso.
- **[RF105]** - Como colaborador do restaurante, gostaria de visualizar relatórios relacionados a pedidos, com possibilidade de filtro (Temporal, Obra específica, Pratos pedidos, e etc). <!-- Meio estranho -->
- ~~**[RF106]** - Como colaborador do restaurante, gostaria de negar a edição de um pedido de um colaborador, em eventuais incidentes.~~
- **[RF107]** - Como colaborador do restaurante gostaria de exportar para CSV os pedidos feitos em um dado dia, para cada obra.
<!-- - **[RF108]** - Como colaborador do restaurante deveria ter a opção de importar os pedidos das empresas parceiras. -->
<!-- - **[RF109]** - Como colaborador do restaurante devo visualizar os pratos mais pedidos, para me previnir e comprar mais ingredientes para esse prato. -->
- **[RF110]** - Como colaborador do restaurante, se o funcionário da obra for comer no restaurante presencialmente, deve ser possível autenticar ele por meio de uma autenticação de 2 fatores, afim de não acontecer fraude. 
- **[RF111]** - Como colaborador do restaurante, gostaria de alterar o prazo limite para a solicitação de uma refeição daquele turno depois de estabelecido.
- **[RF112]** - Como colaborador do restaurante, em caso de alguma eventualidade, gostaria de notificar aos funcionários da obra que não sera ofertada refeições naquele dia.
- **[RF113]** - Como colaborador do restaurante, após importar os pedidos da obra gostaria de imprimir para a cozinha. 
- **[RF114]** - Como colaborador do restaurante eu posso manter cardápios, definindo categorias (Proteína, Carboidrato, Bebidas, etc... ) e a quantidade de vezes que pode ser pedida. Não pode existir categorias iguais no mesmo cardápio.
- **[RF115]** - Como colaborador do restaurante posso definir um cardápio para ser disponibilizado em certo dia

### **Módulo Gestão**
- **[RF200]** - Como gestor de obra, gostaria de listar os colaboradores da obra.
- **[RF201]** - Como gestor de obra, gostaria de visualizar relatórios relacionados a pedidos, com a possibilidade de filtro (Temporal, restaurante especifico, obra...).
- **[RF202]** - Como gestor de obra, gostaria de exportar relatórios de pedidos para planilhas Excel.
- **[RF203]** - Como gestor da obra eu posso pedir o prato para um colaborador da obra, em caso que ele não possa fazer o pedido.
- **[RF205]** - Como gestor da obra, quero confirmar os pedidos dos colaboradores da obra e solicitar as refeições para o restaurante antes do prazo limite. 
- **[RF206]** - Eu como gestor da obra desejo avaliar os dados enviados dos colaboradores da obra com o do colaborador do restaurante, para analisar se houver discrepâncias.
- **[RF207]** - Eu como o gestor da obra desejo poder definir os horários de refeição da obra
### **Módulo Administrativo** 
- **[RF300]** - Eu como administrador do sistema gostaria de definir permissões para usuários comuns
- **[RF304]** - Eu como administrador do sistema desejo registrar que uma ou mais obras não terão fornecimento de refeição naquele dia
- **[RF305]** - Eu como administrador do sistema desejo alterar o restaurante fornecedor de uma obra
- **[RF306]** - Eu como administrador do sistema desejo manter os usuários do sistema
 <!-- %% **[RF308]** - Eu como a administração da obra desejo poder definir os horários de refeição da obra %% -->
- **[RF309]** - Como administrador do sistema, gostaria de manter restaurantes parceiros, atribuindo a suas respectivas obras.
- **[RF310]** - Eu como administrador do sistema posso visualizar todos os relatórios gerados do sistema






# Requisitos não-funcionais

Os requisitos não-funcionais são descritos a seguir.

- **[RNF000 - 049]** - Disponibilidade
- **[RNF050 - 099]** - Privacidade e segurança
- **[RNF100 - 149]** - Usabilidade
- **[RNF150 - 199]** - Suportabilidade
- **[RNF200 - 249]** - Interoperabilidade
- **[RNF250 - 299]** - Manutenibilidade
- **[RNF300 - 349]** - Desempenho
- **[RNF350 - 399]** - Implementação
- **[RNF400 - 449]** - Implantação

## Disponibilidade

- **[RNF000]** - O sistema deve ser desenvolvido de forma que possa ser usado por navegador ou dispositivos moveis como IOS (15 ou superior) e Android (11 ou superior).
- **[RNF001]** - O sistema deve ser desenvolvido de forma que possa ser escalável,para poder suportar mais obras e funcionarios e isso sem perder desemepnho.
- **[RNF002]** - O sistema deverá ser robusto e capaz de lidar com falhas de rede ou interrupções parciais sem perda de dados ou degradação significativa do serviço.
- **[RNF003]** - O sistema deverá estar disponivel 24/7 , funcionarios da obra pode fazer pedidos na maioria dos momentos


## Privacidade e segurança

- **[RNF050]** - O sistema deve ser desenvolvido de forma que os dados dos clientes sejam protegidos e não sejam acessíveis por terceiros.
- **[RNF051]** - O sistema deve atender aos requisitos de privacidade da LGPD (Lei Geral de Proteção de Dados).
- **[RNF052]** - O sistema deverá garantir a integridade dos dados, evitando discrepâncias entre a quantidade de refeições pedidas e as refeições registradas e entregues.
- **[RNF053]** - Deverão existir procedimentos de backup e recuperação de dados para prevenir a perda de informações em caso de desastres.
- **[RNF054]** - O acesso às funcionalidades e dados do sistema deverá ser baseado em perfis de usuário, garantindo que cada usuário só possa acessar as informações e realizar as ações para as quais tem permissão.
- **[RNF055]** - O sistema deverá registrar logs de atividades importantes, como pedidos realizados, modificações e acessos, para fins de auditoria e rastreabilidade.
- **[RNF056]** - O sistema deverá criptografar dados sensivéis do usuario do sistema, como sua matricula e senha. De modo de ser impossivel de recuperar os dados originais do criptografamento



## Usabilidade

- **[RNF100]** - O sistema deverá ter uma interface de usuário simples, intuitiva e amigável, com poucos passos para concluir as tarefas principais (ex: realizar um pedido), sendo uma interface  conversacional, para garantir uma migração suave do método analógico para o digital.

- **[RNF101]** - O sistema deverá ser acessível para usuários com diferentes níveis de habilidade tecnológica, com foco na facilidade de uso em dispositivos móveis.

- **[RNF102]** - A interface deverá ter grande visibilidade e legibilidade, especialmente para usuários em ambientes de obra.

- **[RNF103]** - O sistema deve ser desenvolvido de forma que possa ser acessado por pessoas com deficiência visual, auditiva.

- **[RNF104]** - O sistema deverá permitir a configuração de métodos de notificação (ex: e-mail, push notification) para eventos (ex: pedido confirmado, alteração de status) para cada usuário.
- **[RNF105]** - o sistema deverá bloquear os funcionários da obra de fazer pedidos quando o restaurante estiver fechado, a obra estiver parada, ou o restaurante não fornecer à obra correspondente exceto o pedido do café da manhã que pode ser feito na noite anterior
- **[RNF106]** - O sistema deverá notificar os funcionarios da obra quando os pedidos estão saindo para a entrega
- **[RNF107]** - O sistema deve garantir que os funcionarios da obra so possam pedir para a proxima refeição usando como referência os horarios de almoço da empresa, seus pedidos anteriores e o horário de Brasília.

- **[RNF108]** - Após a ação do **[RF213]**, todos os colaboradores da obra que não confirmaram o pedido será enviado uma notificação pedindo que confirmem o recebimento do pedido 
- **[RNF109]** - Quando o gestor confirmar e solicitar a refeição, os colaboradores da obra não podem mais adicionar ou editar pedidos
- **[RNF110]** - Quando chegar o prazo limite estabelecido pelo restaurante, o sistema deve automaticamente confirmar e solicitar as refeições de obras associadas.

## Suportabilidade

- **[RNF150]** - O sistema deverá suportar diferentes navegadores, sendo eles: Google Chrome, Microsoft Edge, Mozilla Firefox e Opera, atraves de computadores com o sistema operacional Windowns, Linux ou Mac OS. Em caso de dispositivo móvel: Android 11 (2020) ou superior / IOS 15 (2021) ou superior.


- **[RNF151]** - A parte mobile do sistema( Para os colaborados da obra ) deve ser desenvolvido de forma que possa ser executado em Android 11 (2020) ou superior ou IOS 15 (2021) ou superior.

## Interoperabilidade

- **[RNF200]** - O sistema deverá exportar relatórios no formato CSV e XLSX.

## Manutenibilidade

- **[RNF250]** - O código do sistema deverá ser bem documentado, modular e fácil de manter, permitindo que a equipe de desenvolvimento realize correções e atualizações de forma eficiente.
- **[RNF251]** - O sistema deverá ser projetado de forma a facilitar a escrita e execução de testes automatizados e manuais, garantindo a qualidade e a detecção precoce de erros.
- **[RNF252]** - O sistema deve ser documentado de forma que possa ser facilmente compreendido por terceiros e para facilitar a manutenção do sistema.
- **[RNF253]** - Deverão ser implementadas ferramentas de monitoramento para acompanhar o desempenho e disponibilidade do sistema em tempo real.
- **[RNF254]** - O sistema deverá ter ferramentas de monitoramento deverão enviar alertas automáticos para a equipe de suporte em caso de anomalias ou falhas críticas.

## Desempenho

- **[RNF300]** - O sistema deverá ter o tempo de resposta menor que 05 segundos.
- **[RNF301]** - A aplicação deverá ser otimizada para suportar dispositivos móveis com poder computacional limitado, garantindo uma experiência fluida mesmo em smartphones mais antigos.
- **[RNF302]** - O software deverá conseguir suportar 500 a 1000 requisições simultaneas (pedidos, confirmações) em horários de pico (ex: horários de refeição), sem degradação perceptível no desempenho, garantindo que o tempo de resposta seja menor que 05 segundos.

## Implementação

- **[RNF350]** - Deverá ser disponibilizada uma central de ajuda ou seção de FAQ dentro do aplicativo ou em um portal dedicado, com informações sobre o uso do sistema.
- **[RNF351]** - Deverá ser fornecido treinamento inicial para Gestores de Obra, Administradores e Colaboradores do Restaurante sobre o uso do sistema.

## Implantação

- **[RNF400]** - O sistema deverá ser implantado em uma infraestrutura de servidores robusta e escalável, preferencialmente em nuvem
- **[RNF401]** - Deverão ser mantidos ambientes separados para desenvolvimento e produção, para garantir testes seguros antes do deploy.
- **[RNF402]** - A infraestrutura do sistema deve ser modularizada para poder rodar em um servidor local do cliente, caso necessário.








