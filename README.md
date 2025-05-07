# Criando casos de uso
# UNIMAR (Universidade De Marília)
# Professor: Valdir
# Aluno: Murilo Santos Souza
# RA: 2038823 
# Curso: ADS, Turma C, Noturno
# 1° Termo
# Exercícios 
Para cada cenário a seguir, você deve pelo menos 6 requisitos funcionais (RF), 4 não funcionais 
(RNF) e 2 de domínio (RD). Após os requisitos, para cada cenário você deve focar nos casos de 
uso, listando: 
- Todos os atores 
- Pelo menos 6 casos de uso para cada cenário 
- Detalhar por escrito cada caso, trazendo: 
- Título 
- Ator(es) 
- Objetivo 
- Pré-condições 
- Fluxo Principal (etapas) 
- Casos de exceção (fluxo alternativo) 
- Pós-condições
# Cenário 1 - Sistema de Compras Online:
Um sistema de compras online permite que os clientes comprem produtos, acompanhem seus 
pedidos e deixem avaliações. Os administradores do sistema podem adicionar ou remover 
produtos, processar pedidos e responder às avaliações dos clientes.

# Requisitos Funcionais (RF)
- O sistema deve permitir que clientes filtrem suas pesquisas conforme suas preferências.
- O sistema deve contar com várias maneiras de efetuação de pagamento, pix, débito, boleto e crédito a vista ou parcelado.
- O sitema deve permitir que o usuário avalie suas compras, seja com vídeo, imagens, ou apenas texto (contanto que a compra seja verificado como verdadeira).
- Os admnistradores do sistema podem adicionar ou remover itens de acordo com o estoque.
- O sistema deve permitir que admnistradores respondam à avaliações feitas por clientes.
- O sistema deve permitir que novos usuários realizem cadastro.
- O sistema deve permitir que antigos usuários acessem sua conta.
# Requisitos NÃO Funcionis (RNF)
- A apllicação deve funcionar 24/7 tolerando até 1 hora de instabilidade caso necessite de manutenção.
- A aplicação deve suportar 50000 acessos simultâneos sem perca de desempenho.
- Todas as transações feitas devem seguir a LGPD.
- O tempo de resposta da aplicação deve ser de no máximo 2 segundos, para qualquer ação executada.
# Requisitos de domínio
- Todas as transações e dados do cliente devem ser protegidas pela LGPD.
- Todas as empreas que atuarem dentro da aplicação devem estar cadastradas com CNPJ e devem apresentar um documento de quitações com a Receita Federal.
# Casos de uso do cenário:
 Ator| Casos de uso |
|---|---|
| *Cliente*  | permir que os clientes comprem produtos, permitir que acompanhem seus pedidos, permitir que deixem avaliações, permitir que cadastrem cartão de crédito ou débito, permitir que o cliente cancele o produto, permitir que o cliente cadastre o lugar de entrega do produto, o cliente pode ter suas avaliações repondidas pelos admnistradores, pode conversar com os admnistradores caso estes mandem mensagem.|
| *Admnistrador* | Os administradores do sistema podem adicionar produtos, os admnistradores podem remover produtos, os admnistradores podem processar pedidos, os admnistradores podem responder às avaliações dos clientes, os admnistradores podem caso necessário mandar mensagem para o cliente, os admnistradores devem conseguir admnistrar cancelamentos de acordo com suas políticas internas.|
# Caso de uso de compra de produtos:
- O cliente deve conseguir realizar compras.
## Ator: 
- Cliente
## Pré condição:
- O cliente deve possuir uma conta criada na aplicação
## Fluxo principal:
- O cliente consegue chegar na aba de checkout.
## Casos de exceção (Fluxo secundário)
- A aplicação está fora do ar.
- O cliente não possuí uma conta criada.
## Pós condições:
- O cliente consegue realizar sua compra
# Caso de uso, acompanhamento de pedido:
- O cliente deve conseguir rastreas seus pedidos.
## Ator: 
- Cliente
## Pré condição:
- O cliente deve possuir uma conta criada na aplicação
- O cliente deve possuir um produto comprado
- O cliente deve possuir um código de rastreio
## Fluxo principal:
- O usuário usa se códido de rstreio para rastrear o produto no site do frete.
## Casos de exceção
- O cliente não possui uma conta criada
- O cliente não possui produtos comprados
- A aplicação está fora do ar
## Pós condições:
- O cliente consegue realizar o rastreio do seu produto
# Caso de uso de avaliação
- O cliente deve conseguir realizar avaliações na aplicação
- Os admnistradores dvem poder responder às avaliações
## Atores:
- Cliente
- Admnistradores
## Pré Condições
- O cliente deve possuir uma conta cadastrada na aplicação
- O cliente deve ter comprado um produto
- O produto deve ter chegado nas mão do clientes e o mesmo assinado um termo de entrega
- Os admnistradores devem possuir sua loja cadastrada na aplicação
- Os admnistradores devem conseguir checar se o dito cliente realizou a compra do produto
# Fluxo principal:
- O usuário consegue realizar sua avaliação pela aplicação
- Os admnistradores conseguem responder as avaliações feitas pelos clientes.
## Casos de exceção (Fluxo secundário)
- A aplicação está fora do ar
- O produto ainda não chegou na casa do cliente
- Os admnistradores estão deslogados do sistema
## Pós condições:
- O cliente conseguiu realizar sua avaliações
- Os admnistradores conseguiram responder a avaliação do cliente.
# Cenário de cadastro de meios de pagamentos
- O sistema deve permitir o cadastro do meio de pagamento de preferência do cliente.
## Ator:
- Cliente
## Pré condições:
- O cliente dve possuir uma conta criada na aplicação
- O meio de pagamento deve estar disponível na aplicação
- O meio de pagamento deve ser válido
## Fluxo principal:
- O cliente consegue cadastrar os dados do seu meio de pagamento de preferência.
## Casos de exceção (Fluxo secundário)
- A aplicação está fora do ar
- O meio usado pelo cliente está vencido ou não é autorizado pela aplicação.
## Pós condição:
- O cliente obteve êxito em cadastrar sua forma de pagamento.
#  Cenário de cancelamento de produto
- O cliente deve conseguir cancelar suas compras.
- Os admnistradores devem avaliar o cancelamento de acordo com suas políticas internas.
## Atores:
- Clientes
- Admnistradores
##  Pré condições:
- O cliente deve possuir uma conta criada na aplicação
- Deve existir um produto com a compra efetuada
- Os admnistradores devem estar logado na aplicação
- Os admnistradores devem cosneguir analisar às consições de cancelamento
## Fluxo principal:
- O Cliente conseguiu solicitar o cancelamento da compra aos admnistradores
- Os admnistradores conseguiram ver a análisar o pedido de cancelamento do produto.
## Fluxo secundário:
- O sistema está fora do ar.
- O caso de cancelamento não está dentro dos padrões de política da empresa.
- O produto já foi entregue
## Pós condições:
- O cliente conseguiu cancelar o produto
- Os admnistradores aceitaram o cancelamento do produto
# Cenário cadastro de entrega
- O cliente deve conseguir cadastrar o lugar de entrega do produto
## Atores
- Cliente
## Pré condição:
- O cliente deve possuir cadastro na aplicação.
- O endereço dever ser válido e estar dentro do território nacional.
## Fluxo principal:
- O cliente conseguiu válidar seu endereço de entrega.
## Fluxo secundário:
- A aplicação está fora do ar.
- O endereço cadastrado não é valido.
## Pós condições:
- O cliente conseguiu cadastrar o endereço de entrega.
# Cenário de uso adicionar produtos:
- A aplicação deve permitir que os admnistradores adicionem seus produtos.
## Ator:
- Admnistrador
## Pré condição:
- O produto adicionado deve estar disponível no estoque
- O admnistrador deve estar logado na aplicação
## Fluxo principal:
- O admnistrador consegue cadastrar um produto na sua loja.
## Fluxo secundário
- A aplicação está fora do ar
- O produto não está disponível no estoque
## Pós condição:
- O produto foi adicionado com êxito pelos admnistradores
# Cenário de remoção de produtos
- Os admnistradores devem conseguir remover produtos de sua loja
## Ator
- Admnistrador
## Pré condição
- O admnistrador deve estar logado na aplicação
- O produto retirado da loja não estar no estoque
- O produto deve possuir um cadatro no sistema
- Deve ser feito apenas em momentos de baixo fluxo de clientes
## Fluxo principal:
- O admnistrador consegue acessar as opções de produto
## Fluxo secundário:
- A aplicação está fora do ar
- Ainda existem produtos no estoque
- O horário não permite alteração do produto

## Pós condições
- O produto foi retirado da aba da loja.

# Cenário de processamento de pedidos:
- Os admnistradores devem conseguir processar o pedido
## Atores:
- Cliente
- Admnistrador
## Pré condição
- O admnistrador deve estar logado na aplicação
- Deve existir um produto sendo comprado
- O meio de pagamento deve ter sido aprovado
- O cliente deve possuir uma conta cadastrada
- O cliente deve possuir um meio de pagamento válido
- Porduto deve estar em estoque
- Deve existir um endereço de entrega válido
## Fluxo principal:
- O admnistrador com todos os dados em mão consegue processar o pedido do cliente.
## Fluxo secundário
- A aplicação está fora do ar
- O produto não está em estoque
- Meio de pagamento não aprovado
- Não existe um produto para ser processado
- Local de entrega inválido
## Pós condição
- O admnistrados conseguiu processar o produto e enviar para a entrega
# Cenário resposta de avaliação de clientes
- Admnistradores devem conseguir responder avaliações
- Clientes devem conseguir avaliaro produto
## Atores:
- Cliente
- Admnistrador
## Pré condição
- O admnistrador deve estar logado na aplicação
- O cliente deve possuir uma conta cadastrada
- Deve haver um produto comprado
- O produto deve ter chegado ao cliente
## Fluxo principal:
- O cliente com o produto em mão pode avalia-lo
- A empresa com uma avaliação válida pode responder caso deseje
## Fluxo secundário
- A aplicação está fora do ar
- Não existem produtos comprados
- O produto ainda não foi entegue
## Pós condição
- O cliente avalia o produto
- Os amnistradores respondem à avaliação
# Cenário mensagem para o cliente
## Atores
- Cliente
- Admnistrador
## Pré condição
- Os clientes devem possuir uma conta cadastrada
- O admnistrador deve estar logado
- Deve haver um produto comprado ou no carrinho
## Fluxo principal
- O admnistrador entra em contato com o cliente para discutir possíveis problemas no produto ou sanar dúvidas quanto a funcionalidades do mesmo
- O cliete recebe a mensagem do admnistrador
## Fluxo secundário
- A aplicação está fora do ar
## Pós condição:
- O admnistrador conseguiu sanar dúvidas ou realizar uma troca de produto
- Os clientes responderam as mensagens recebidas
# Cenário de admnistração de cancelamentos.
- Os admnistradores devem conseguir analisar solicitações de cancelamentos de produtos
- Os clientes devem conseguir solicitar cancelamento do produto
## Atores:
- Clientes
- Admnistradores
## Pré condições
- Deve existir um produto comprado
- O admnistrador deve estar logado
- O admnistrador deve conseguir acessar a solicitação de cancelamento
- O cliente deve ter solicitado cancelamnto
- O cliente deve possuir uma conta cadastrada
## Fluxo principal:
- O cliente solicita o cancelamento da compra do produto
- O admnistrador analisa o pedido de acordo com as pplíticas da empresa
## Fluxo secundário:
- O sistema está fora do ar
- O produto já foi entregue
- O cancelamento não se enquadra nas políticas da empresa
## Pós condição:
- O admnistrador cancelou o produto do cliente
- O produto foi cancelado






# Cenário 2 - Sistema de Reservas de Hotel: 
Um sistema de reservas de hotel permite que os hóspedes reservem quartos online, que os 
funcionários do hotel gerenciem as reservas e que o gerente do hotel gere relatórios de ocupação. 
Os hóspedes podem visualizar os quartos disponíveis e cancelar suas reservas. Os funcionários 
podem confirmar e cancelar reservas. O gerente pode visualizar relatórios de ocupação e receita.
# Cenário 3 - Sistema de Gerenciamento de Restaurante:
Um sistema de gerenciamento de restaurante permite que os clientes façam reservas de mesas e 
façam pedidos online, que os garçons gerenciem os pedidos e que o gerente do restaurante gere 
relatórios de vendas e controle o cardápio.
# Cenário 4 - Sistema de Gerenciamento de Cursos Online 
Uma plataforma de cursos online permite que os estudantes se inscrevam em cursos, assistam às 
aulas e submetam trabalhos. Os instrutores podem criar cursos, gerenciar conteúdo e avaliar os 
trabalhos submetidos. O administrador da plataforma gerencia os usuários (estudantes e 
instrutores) e gera relatórios sobre a utilização da plataforma.
# Cenário 5 - Sistema de Gerenciamento de Eventos: 
Um sistema de gerenciamento de eventos permite que os organizadores criem e gerenciem 
eventos, os participantes se registrem para os eventos e que os administradores gerenciem a 
plataforma e gerem relatórios de participação. Os eventos podem ser conferências, workshops ou 
seminários.
