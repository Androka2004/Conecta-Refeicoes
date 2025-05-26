Documento de Visão de Produto (DVP)  
Visão do Produto

Conecta Refeições

# Introdução

O documento de Visão do Produto (DVP) é um documento que descreve o produto de software que será desenvolvido. Ele descreve o problema que será resolvido, as principais necessidades dos stakeholders, as principais funcionalidades do sistema, as restrições do projeto, etc.

# Propósito

O objetivo deste documento é coletar, analisar e definir características e as necessidades de alto nível do Sistema Conecta Refeições.

Ele se concentra nos recursos necessários aos stakeholders e aos usuários, e nas razões que levam a essas necessidades.

Os detalhes de como o Sistema Conecta Refeições atingem essas necessidades são descritos nas especificações de casos de uso e nos requisitos funcionais.

# Abreviações

| Termo | Definição |
| :---: | :---- |
| DVP | Documento de Visão do Produto |
| NFe | Nota Fiscal Eletrônica |
| NFSe | Nota Fiscal de Serviços Eletrônica |
| SRS | Especificação de Requisitos de Software |
| UML | Linguagem de Modelagem Unificada |
| API | Interface de Programação de Aplicações |

# Definições

| Termo | Definição |
| :---: | :---- |
| Cliente | É uma pessoa física ou jurídica que compra um produto ou contrata um serviço. |
| Consumidor | É uma pessoa física que compra um produto ou contrata um serviço. |
| Empresa | É uma pessoa jurídica que compra um produto ou contrata um serviço. |
| Fornecedor | É uma pessoa física ou jurídica que vende um produto ou presta um serviço. |
| Nota Fiscal | É um documento fiscal que ateste a compra de um produto ou serviço. |
| Produto | É um bem ou serviço que é vendido ou prestado. |
| Serviço | É um bem intangível que é prestado. |
| Canteiro de Obras | Local onde está ocorrendo de fato a construção realizada pela Construtora |
| Espelho | Folha utilizada para coletar as assinaturas dos funcionários que pegaram uma refeição |
| Servente | Funcionário que trabalha dentro do canteiro de obras, realizando a construção |
| Gestor de Obras | Responsável por fazer a gestão dentro do Canteiro de Obras, passando possíveis demandas para o setor administrativo |
| Administrador de Obra | Responsável pelo controle de gastos da obra, dar permissão para a compra de materiais para a obra e contatar fornecedores. |
| Nuvem | Serviços de armazenamento na internet |

# Escopo do Produto

O Sistema Conecta Refeições é uma aplicação que visa digitalizar o processo de solicitação e controle de refeições em obras. Permite que colaboradores façam pedidos via celular, que restaurantes recebam e registrem os pedidos, e que gestores acompanhem os dados. O sistema reduz erros e economiza tempo.

# Posicionamento

# Oportunidade de Negócios

O sistema Conecta Refeições apresenta diversas oportunidades de negócios, tais como:

### **1\. Parcerias com restaurantes locais:**

Integrar restaurantes parceiros na plataforma para que recebam pedidos direto por lá, oferecendo mais visibilidade e benefícios para quem entrar no sistema e ajudando a criar uma rede de alimentação voltada para obras.

### **2\. Expansão para outros setores:**

Adaptar o sistema para empresas de outros segmentos que também oferecem refeições aos seus colaboradores, como indústrias, mineradoras, eventos e escolas, aproveitando a mesma lógica de operação com ajustes pontuais.

### **3\. Módulo de auditoria:**

Adicionar funções que permitam acompanhar todas as etapas do pedido (quem fez, quando, onde e qual refeição), criando um histórico para evitar fraudes e facilitar a prestação de contas com fornecedores e gestores a fim de evitar desperdício orçamental.

### **4\. Marketplace de Serviços Complementares**

### Criar um marketplace dentro da plataforma, onde além dos restaurantes, outros serviços possam ser oferecidos para obras, como fornecedores de marmitas, lanches rápidos, cafés, bebidas e até serviços de logística (entrega nas obras).

### 

### **5\. Integração com outras ferramentas**

Oferecer uma API pública que permite integrar o Conecta Refeições com outros softwares, como ERPs, sistemas de gestão de obra, CRMs e aplicativos de comunicação, como WhatsApp e Telegram.

# Descrição dos benefícios 

| Benefícios | Problemas resolvidos  | Afetados |
| :---- | :---- | :---- |
| Automatização dos processos de pedidos  | Todas as partes do processo são feitas manualmente.  | Todos os envolvidos na obra de uma maneira geral.  Os funcionários que pedem a refeição, os gestores, o restaurante que recebe os pedidos  |
| Comunicação entre obra e restaurante facilitada por meios digitais | Problemas de discrepância entre a quantidade de refeições que a construtora registrou ter pedido, com a quantidade de refeições que o restaurante registrou ter  sido pedidos.  | Restaurante e Empresa |
| Integração com ferramentas já usadas na empresa.  | Passar todos os pedidos manualmente para uma planilha do Excel, que é feito manualmente. | Funcionários da obra como gestores de obra e administrador |
| Reduzir chances de erros | Garantir que não seja feito pedidos errados ;  | Todos os envolvidos na obra de uma maneira geral.  Os funcionários que pedem a refeição, os gestores, o restaurante que recebe os pedidos  |

# Descrição dos stakeholders e dos usuários

| Stakeholder | Descrição | Papel |
| ----- | ----- | ----- |
| Construtora | Empresa responsável pela obra que deseja otimizar o processo de solicitação e controle de refeições para seus colaboradores. | Contrata e utiliza o sistema |
| Restaurante | Restaurante que vai ser integrado a aplicação e vai ofertar as refeições | Utiliza e é um dos beneficiados do desenvolvimento do sistema, já que os pedidos  |
| Equipe de Suporte e Desenvolvimento | Profissionais técnicos responsáveis pela manutenção, atualização e suporte do sistema | Garantem que a plataforma funcione sem interrupções, resolvem problemas técnicos e fazem melhorias e atualizações sempre que necessário |

Usuários e atores

| Usuário | Descrição | Responsabilidades | Stakeholders |
| ----- | ----- | ----- | ----- |
| Colaborador da obra | Funcionários que atuam diretamente nas obras e realizam os pedidos de refeições pelo aplicativo. | Utilizam o sistema para escolher e solicitar suas refeições | Construtura |
| Colaborador do restaurante | Funcionário dos restaurantes que recebem e processam os pedidos feitos pelos colaboradores. | Recebem, confirmam e registram os pedidos | Restaurante |
| Gestores de Obras | Profissionais responsáveis pelo acompanhamento da obra, controle de pedidos e etc... | Monitoram os pedidos feitos, gerenciam a distribuição das refeições e conferem os relatórios | Construtora |
| Administrador | Funcionário que cadastra na planilha | Cadastram os dados das assinaturas em planilhas,  | Construtora |

# Descrição do ambiente de uso

## Ambiente de uso

Ambiente dos Colaboradores:  
Neste ambiente, o sistema é utilizado pelos colaboradores das obras para realizar os pedidos de refeições. Eles acessam o sistema principalmente por meio de dispositivos móveis, como smartphones e tablets, utilizando os sistemas operacionais Android ou iOS. 

Ambiente do Restaurante Parceiro:  
Neste ambiente, o sistema é utilizado pelos funcionários dos restaurantes que recebem e processam os pedidos feitos pelos colaboradores. O acesso ocorre de preferência por computadores, permitindo a visualização, confirmação e registro dos pedidos em tempo real. 

Ambiente Administrativo da Construtora:  
Aqui, o sistema é usado pela equipe administrativa responsável por controlar e gerenciar os pedidos de refeições das obras. Eles acessam principalmente pelo computador para gerar relatórios, analisar dados e integrar informações com planilhas Excel. O ambiente conta com acesso restrito para garantir a segurança e a confidencialidade dos dados.

Ambiente de Suporte e Desenvolvimento:  
Aqui a equipe de TI realiza manutenções, testes e melhorias no sistema antes de disponibilizá-lo para os usuários. Funciona em ambientes controlados, com acesso restrito, permitindo testar novas funções e corrigir erros com segurança.

# Necessidades principais quanto ao ambiente

| Necessidade | Prioridade | Interesse | Solução atual | Solução proposta |
| :---- | :---- | :---- | :---- | :---- |
|  **Qualidade:** O sistema deve sempre estar disponível, livre de erros , deve ter uma integração com banco de dados com o fito de analisar os dados. Integração com excel, pois os colaboradores já estão acostumados. | ALTA | Os clientes esperam que o sistema seja capaz de gerenciar mais efetivamente os pedidos e que possa garantir que não haja erro na contagem de pedidos e das refeições entregues. Os clientes desejam que o sistema esteja sempre disponível | Um gestor se encarrega de gerenciar , anotar todos os pedidos e confirmar com os colaboradores se receberam o pedido. | Por meio de uma aplicação os funcionários podem pedir diretamente com o restaurante, confirmar o recebimento do pedido e etc, |
| **Desempenho:** A aplicação deve ter um tempo de resposta rápido.Ser bastante otimizado para suportar dispositivos com poder computacional limitado.  As requisições devem ser atendidas em menos de 2 segundos. O software deve conseguir aguentar diversas requisições ao mesmo tempo ,visto que os usuários vão provavelmente usar ao mesmo tempo nos horário de refeições.  | ALTA | Os clientes querem que o sistema seja capaz de aguentar todas requisições feitas em horários de pico , além disso querem que a aplicação seja otimizada para atender a todo tipo de dispositivo.Essas requisições seriam os pedidos , confirmação dos pedidos e etc.  | N/A | Por meio da aplicação os colaboradores podem pedir.  |
| **Escalabilidade:** A aplicação deve ser capaz de suportar o crescimento no número de empresas parceiras e funcionários. | MODERADA | O cliente deseja que, não importando o número dos colaboradores e empresas parceiras , a aplicação continue funcionando normalmente.  | De acordo com a expansão da obra, a construtora pode contratar auxiliares para o gestor, ou mais de um gestor para a obra. | Implementar medidas de armazenamento em nuvem, otimizar os processos de pedidos para garantir escalabilidade. |
| **Segurança:** O sistema deve ser seguro, protegido contra acesso não autorizado, invasões e roubo de dados | MODERADA | Os clientes esperam que informações pessoais dos seus colaboradores estejam seguras. O cliente espera que diminua as fraudes de pedidos que muitas vezes são feitas por outras pessoas.   | Os administradores registram as notas fiscais e checam manualmente os pedidos, o'que demanda tempo e pode provocar erros  | Implementar medidas criptográficas e de autenticação para garantir que o pedido chegue na pessoa que pediu com o maior sigilo possível e garantir que não haja fraudes. |
| **Usabilidade**: O sistema deve ser fácil de usar e entender, com uma interface intuitiva e amigável ao usuário. | ALTA | Os clientes enfatizaram a importância do sistema ser fácil de usar e que muito efetivo no uso sendo necessário poucos passos para concluir qualquer tarefa. | N/A. Não tem sistema ainda | Implementar telas que sejam acessíveis a maioria do público alvo. Para garantir isso será necessário realizarmos testes de usabilidade com usuários reais , e ir melhorando a interface |

# Visão geral do produto

O sistema de controle de pedidos de refeição foi desenvolvido para automatizar o processo de solicitação de refeições por colaboradores em obras da construção civil. Ele substitui planilhas manuais por uma plataforma digital acessível via celular ou navegador, permitindo que colaboradores façam pedidos com facilidade, restaurantes recebam as informações organizadas e o setor administrativo tenha relatórios e exportações para controle interno.

A solução oferece níveis de acesso personalizados para cada perfil (colaborador, restaurante, administrador), promovendo eficiência, rastreabilidade e transparência em toda a cadeia do processo.

![Diagrama do sistema](../../assets/diagrama.png)

# Custo e venda

 A decisão acerca da viabilidade econômica deste requisito para planejamento de custos e orçamento do projeto dos sistema Conecta Refeições é aplicável ao departamento comercial, gerente de projetos e um futuro cliente.

# Licenciamento e instalação

O sistema Conecta Refeições será licenciado por meio de uma licença de uso corporativa, fornecida pela empresa desenvolvedora do software. A licença concederá à construtora o direito de utilizar o sistema com suporte para centenas de usuários, conforme escopo definido em contrato.

O Conecta Refeições poderá ser instalado localmente nos servidores da construtora ou em ambiente de nuvem fornecido pela equipe de desenvolvimento , cobrando uma assinatura anual. A instalação poderá ser realizada pela equipe técnica da própria construtora ou, alternativamente, pela equipe da empresa desenvolvedora mediante contratação de serviço adicional.

A empresa desenvolvedora será responsável por fornecer o pacote de instalação, manuais técnicos e instruções detalhadas para configuração do sistema e da base de dados. Após a conclusão da instalação, serão disponibilizadas credenciais de acesso administrativo para uso pleno do sistema.

As atualizações corretivas, voltadas à resolução de bugs eventualmente identificados pelos usuários, poderão ser solicitadas diretamente à equipe de suporte técnico. Essas atualizações serão analisadas e implementadas conforme cronograma acordado, garantindo o bom funcionamento e a estabilidade do sistema.

A propriedade intelectual do Conecta Refeições permanecerá integralmente com a empresa desenvolvedora. A construtora será licenciada para uso do sistema, nos limites estabelecidos contratualmente. Qualquer uso não autorizado, como cópias indevidas, distribuição ou sublicenciamento, constituirá infração contratual e estará sujeito às sanções legais aplicáveis.

# Características e funcionalidades de alto nível

1 \- Cadastro e autenticação de usuários  
O sistema permite o cadastro e login de diferentes tipos de usuários: colaboradores, administradores e restaurantes. Cada perfil terá permissões específicas, garantindo segurança e controle de acesso.

2- Solicitar refeição  
Permite que o colaborador faça seu pedido de refeição de forma simples e rápida, com validações que garantem que o pedido seja feito dentro do prazo estipulado pelo restaurante.

3 \- Visualização e gerenciamento de pedidos  
Restaurantes têm acesso aos pedidos recebidos por dia e por obra, podendo visualizar e organizar a produção e entrega das refeições com base nas solicitações recebidas.

4 \- Relatórios administrativos  
Administradores podem gerar relatórios detalhados com filtros por obra, data e restaurante. Esses relatórios ajudam no controle de consumo e planejamento

5 \- Exportação de dados  
O sistema oferece a funcionalidade de exportar os dados de pedidos para o Excel, permitindo maior integração com processos internos da empresa.

# Restrições

1\.**Restrição de orçamento**: O projeto deve ser concluído dentro de um determinado orçamento e não pode excedê-lo.  
2\.**Restrição de tempo**: O sistema deve ser produzido em um determinado tempo , usando metodologias ágeis entregando , partes do produto   
3\. **Restrições de hardware**:O sistema deve atender a diversos tipos de hardware, como smartphones , tablets e computadores, além disso deve ser bastante otimizado para funcionar em todos.  
4\. **Restrições de segurança e privacidade**: O sistema deve atender aos requisitos de segurança, privacidade e proteção de dados do usuário, conforme a Lei Geral de Proteção de Dados (LGPD).  
5\. **Restrições de usabilidade**: O sistema deve ser fácil de usar e acessível para usuários com deficiências visuais, pouca afinidade com tecnologia e etc…  .  
6\. **Restrições de interoperabilidade**: O sistema deve ser capaz de interoperar com outros sistemas e aplicativos , como o excel ou o whatsapp .  
7\. **Restrições de desempenho**: O sistema deve atender aos requisitos de desempenho, como velocidade, escalabilidade e disponibilidade , atender requisições rapidamente .  
8\.**Restrições de linguagem**: O sistema deve ser compatível com os idiomas inglês e português.

