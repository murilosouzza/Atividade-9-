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

# Cenário 1 – Sistema de Compras Online
O sistema permite que clientes comprem produtos pela internet, acompanhem pedidos e avaliem as compras. Os administradores podem gerenciar produtos no estoque, processar pedidos, responder avaliações e se comunicar com os clientes. O sistema também aceita diferentes formas de pagamento e garante segurança dos dados.

# Requisitos Funcionais (RF)
1. O sistema deve permitir que os clientes filtrem produtos por categoria, preço, marca e avaliação.

2. O sistema deve permitir várias formas de pagamento: Pix, boleto, débito e crédito (à vista ou parcelado).

3. O sistema deve permitir que clientes avaliem suas compras com texto, imagem ou vídeo (desde que a compra tenha sido confirmada).

4. O sistema deve permitir que administradores adicionem e removam produtos do catálogo.

5. O sistema deve permitir o cadastro e login de usuários.

6. O sistema deve permitir que administradores respondam às avaliações dos clientes.

7. O cliente deve poder cadastrar um endereço de entrega e solicitar cancelamento de pedido.

# Requisitos Não Funcionais (RNF)
1. A aplicação deve funcionar 24/7 com tolerância de até 1 hora de instabilidade em manutenção.

2. O sistema deve suportar até 50.000 acessos simultâneos sem travar.

3. Todas as transações devem seguir as diretrizes da LGPD.

4. O tempo de resposta para qualquer ação não deve ultrapassar 2 segundos.

# Requisitos de Domínio (RD)
1. Todas as empresas cadastradas devem ter CNPJ e comprovar regularidade com a Receita Federal.

2. Os dados pessoais e financeiros dos usuários devem ser protegidos e criptografados conforme a LGPD.

# Atores
- Cliente
- Administrador

# Casos de Uso
# 1. Compra de produtos
- Ator : Cliente
- Objetivo: Realizar a compra de um ou mais produtos.
## Pré-condições: 
- Cliente precisa ter conta ativa e estar logado.
## Fluxo Principal:
- Cliente escolhe os produtos.
- Vai para o carrinho.
- Seleciona o endereço e a forma de pagamento.
- Confirma a compra.
- Recebe confirmação de pedido.

## Fluxo Alternativo:
- Cliente não logado.
- Produto fora de estoque.
- Sistema fora do ar.

## Pós-condições: 
- Pedido feito com sucesso, aguardando processamento.

# 2. Acompanhamento de pedido
## Ator: 
- Cliente
## Objetivo: 
- Permitir que o cliente acompanhe o status e o rastreamento da entrega.
## Pré-condições: 
- Cliente logado e com pedido já confirmado.
## Fluxo Principal:
- Cliente acessa seu histórico de pedidos.
- Clica no pedido.
- Acompanha o rastreamento no site da transportadora via código.
## Fluxo Alternativo:
- Cliente sem pedidos realizados.
- Código de rastreio não gerado ainda.
- Sistema fora do ar.

## Pós-condições: 
- Cliente consegue visualizar o status da entrega.
# 3. Avaliação de produto
## Atorres: 
- Cliente, Administrador
## Objetivo: 
- Avaliar produto recebido e permitir que administrador responda.
## Pré-condições: 
- Produto entregue
- cliente com conta ativa.
## Fluxo Principal:
- Cliente acessa o histórico.
- Seleciona o produto.
- Escreve a avaliação (texto, imagem ou vídeo).
- Administrador visualiza e responde se quiser.
## Fluxo Alternativo:
- Produto ainda não entregue.
- Administrador deslogado.
- Sistema fora do ar.

## Pós-condições: 
- Avaliação registrada e, se for o caso, respondida.

# 4. Cadastro de forma de pagamento
## Ator: 
- Cliente
## Objetivo: 
- Salvar uma forma de pagamento preferida.
## Pré-condições: 
- Cliente com conta ativa.
## Fluxo Principal:
- Cliente acessa perfil de pagamento.
- Escolhe entre Pix, cartão, boleto etc.
- Cadastra os dados.
- Sistema valida e confirma.

## Fluxo Alternativo:
- Cartão vencido.
- Forma não aceita pela loja.
- Sistema fora do ar.

## Pós-condições:
- Forma de pagamento salva com sucesso.
# 5. Cancelamento de pedido
## Atores: 
- Cliente, Administrador
## Objetivo: 
- Cancelar um pedido conforme a política da loja.
## Pré-condições: 
- Pedido precisa estar em fase que permite cancelamento.
# Fluxo Principal:
- Cliente solicita cancelamento pelo painel.
- Administrador analisa conforme regras.
- Aprova ou recusa o pedido.

## Fluxo Alternativo:
- Produto já enviado ou entregue.
- Pedido fora do prazo de cancelamento.
- Sistema fora do ar.

## Pós-condições: 
- Pedido cancelado ou recusa informada ao cliente.

# 6. Administração de produtos
## Ator: 
- Administrador
## Objetivo: 
- Adicionar ou remover produtos do catálogo.
## Pré-condições:
- Administrador deve estar logado.
## Fluxo Principal:
- Acessa o painel de produtos.
- Adiciona ou remove produto.
- Sistema atualiza o catálogo visível aos clientes.
- Fluxo Alternativo:
- Produto sem estoque.
- Horário de pico não permite alteração.
- Sistema fora do ar.

## Pós-condições: 
-Produto atualizado no sistema.





# Cenário 2 - Sistema de Reservas de Hotel: 
Um sistema de reservas de hotel permite que os hóspedes reservem quartos online, que os 
funcionários do hotel gerenciem as reservas e que o gerente do hotel gere relatórios de ocupação. 
Os hóspedes podem visualizar os quartos disponíveis e cancelar suas reservas. Os funcionários 
podem confirmar e cancelar reservas. O gerente pode visualizar relatórios de ocupação e receita.
# Requisitos Funcionais (RF)
1. O sistema deve permitir que hóspedes vejam os quartos disponíveis.

2. – O sistema deve permitir que o hóspede realize reservas online.

3. – O sistema deve permitir que o hóspede cancele sua reserva.

4. – O sistema deve permitir que funcionários confirmem reservas feitas por hóspedes.

5. – O sistema deve permitir que funcionários cancelem reservas quando necessário.

6. – O sistema deve permitir que o gerente visualize relatórios de ocupação e receita.
# Requisitos Não Funcionais (RNF)
1. – A aplicação deve funcionar 24 horas por dia, 7 dias por semana, com até 1h de manutenção por semana.

2. – O sistema deve suportar até 10 mil acessos simultâneos sem perda de desempenho.

3. – A interface deve ser acessível via desktop e mobile.

4. – O tempo de resposta das ações deve ser de até 2 segundos.

# Requisitos de Domínio (RD)
1. – Todos os dados dos hóspedes devem ser protegidos de acordo com a LGPD.

2. – O sistema só pode operar com hotéis legalmente cadastrados e licenciados pelo órgão responsável da região.

# Atores
- Hóspede
- Funcionário
- Gerente

# Casos de Uso
# 1. Realizar Reserva de Quarto
## Ator: 
- Hóspede

## Objetivo: 
- Permitir que o hóspede reserve um quarto online.

## Pré-condições: 
- O hóspede precisa ter uma conta criada no sistema.

## Fluxo Principal:
- O hóspede acessa o sistema.
- Consulta a disponibilidade de quartos por data.
- Seleciona o quarto desejado.
- Preenche os dados da reserva.
- Confirma e finaliza a reserva.

## Casos de exceção:
- O sistema está fora do ar.
- Não há quartos disponíveis para as datas escolhidas.
## Pós-condições: 
- A reserva foi feita com sucesso e está registrada no sistema.

# 2. Cancelar Reserva
## Ator: 
- Hóspede

## Objetivo: 
- Permitir que o hóspede cancele uma reserva já feita.

## Pré-condições: 
- O hóspede deve ter uma reserva ativa no sistema.

## Fluxo Principal:
- O hóspede acessa o sistema.
- Vai até a área de reservas.
- Seleciona a reserva que deseja cancelar.
- Confirma o cancelamento.

## Casos de exceção:
- A reserva já passou da data do check-in.
- O sistema está fora do ar.

## Pós-condições:
- A reserva foi cancelada com sucesso.

# 3. Confirmar Reserva
## Ator: 
- Funcionário

## Objetivo: 
- Confirmar uma reserva feita por um hóspede.

## Pré-condições: 
- O funcionário deve estar logado e a reserva deve estar pendente.

## Fluxo Principal:
- O funcionário acessa o painel de reservas.
- Localiza a reserva pendente.
- Verifica os dados da reserva.
- Confirma a reserva no sistema.

## Casos de exceção:
- A reserva foi cancelada pelo hóspede antes da confirmação.
- O sistema está fora do ar.

## Pós-condições: 
- A reserva foi oficialmente confirmada e o quarto reservado.

# 4. Cancelar Reserva como Funcionário
## Ator: 
- Funcionário

## Objetivo:
- Cancelar uma reserva feita, por motivos operacionais.

## Pré-condições: 
- O funcionário deve estar logado. 
- Reserva deve estar ativa.

## Fluxo Principal:
- O funcionário acessa o painel.
- Localiza a reserva a ser cancelada.
- Insere o motivo do cancelamento.
- Confirma o cancelamento.
## Casos de exceção:
- O hóspede já realizou o check-in.
- O sistema está fora do ar.

## Pós-condições: 
- A reserva foi cancelada e o hóspede notificado.

# 5. Visualizar Quartos Disponíveis
## Ator: 
-Hóspede

## Objetivo: 
- Permitir que o hóspede veja os quartos disponíveis por data.

## Pré-condições: 
- O hóspede deve ter uma conta ativa.

## Fluxo Principal:
- O hóspede acessa o sistema.
- Informa as datas desejadas.
- O sistema mostra os quartos disponíveis.

## Casos de exceção:
- Não há quartos disponíveis.
- O sistema está fora do ar.

## Pós-condições: 
- O hóspede consegue ver os quartos disponíveis.

# 6. Acessar Relatórios Gerenciais
## Ator: 
- Gerente
## Objetivo:
- Permitir que o gerente visualize relatórios de ocupação e receita.

## Pré-condições: 
- O gerente deve estar logado e possuir permissão administrativa.

## Fluxo Principal:
- O gerente acessa o painel administrativo.
- Escolhe o tipo de relatório que quer ver.
- Define o período da análise.
- O sistema exibe o relatório.
## Casos de exceção:
- O sistema está fora do ar.
- O gerente não tem permissão para o relatório solicitado.

## Pós-condições: 
- O gerente conseguiu visualizar os dados solicitados.

# Cenário 3 - Sistema de Gerenciamento de Restaurante:
Um sistema de gerenciamento de restaurante permite que os clientes façam reservas de mesas e 
façam pedidos online, que os garçons gerenciem os pedidos e que o gerente do restaurante gere 
relatórios de vendas e controle o cardápio.
# Requisitos Funcionais (RF)
1. O sistema deve permitir que clientes reservem mesas online.

2. O sistema deve permitir que clientes façam pedidos online, direto pelo cardápio.

3. O sistema deve permitir que garçons vejam, aceitem e atualizem o status dos pedidos.

4. O sistema deve permitir que o gerente edite o cardápio (incluir/remover itens).

5. O sistema deve gerar relatórios de venda diários, semanais e mensais para o gerente.

6. O sistema deve permitir que o cliente avalie os pedidos e o atendimento.

7. O sistema deve enviar notificação para o cliente quando o pedido estiver pronto.

# Requisitos Não Funcionais (RNF)
1. O sistema deve estar disponível todos os dias, das 8h às 0h, sem travar ou cair.

2. O tempo de resposta do sistema deve ser de no máximo 2 segundos por operação.

3. O sistema precisa funcionar bem tanto em desktop quanto em celular.

4. Os dados dos clientes devem estar seguros e criptografados de acordo com a LGPD.

# Requisitos de Domínio (RD)
- Todos os funcionários (garçons, gerente) devem estar registrados no sistema com CPF e cargo definido.
- Todos os pedidos devem estar vinculados a uma mesa ou pedido online validado pelo cliente.

# Atores
- Cliente
- Garçom
- Gerente

# Casos de Uso
# 1. Fazer reserva de mesa
## Ator: 
- Cliente
## Objetivo: 
- Reservar uma mesa para um determinado dia e hora.
## Pré-condições: 
- O cliente deve estar cadastrado no sistema.
## Fluxo Principal:
- Cliente acessa o sistema.
- Escolhe data, hora e número de pessoas.
- Seleciona uma mesa disponível.
- Confirma reserva.
## Fluxo Alternativo:
-O horário desejado está cheio.
- O cliente não está logado no sistema.

## Pós-condições: 
- A reserva foi confirmada e salva no sistema.
# 2. Fazer pedido online
## Ator: 
- Cliente
## Objetivo: 
- Pedir comida sem ajuda do garçom, direto pelo sistema.
## Pré-condições: 
- O cliente deve estar com mesa ativa.
- O cliente dve estar com o pedido online liberado.
## Fluxo Principal:
- Cliente acessa o cardápio.
- Escolhe os pratos e bebidas.
- Envia pedido para cozinha.
- Recebe confirmação do pedido.
## Fluxo Alternativo:
- A cozinha está com sistema fora do ar.
- Item escolhido está indisponível.

## Pós-condições: 
- Pedido foi enviado para cozinha e cliente recebeu confirmação.
# 3. Gerenciar pedidos
## Ator: 
- Garçom
## Objetivo: 
- Ver, aceitar e atualizar o status dos pedidos.
## Pré-condições: 
- Garçom deve estar logado no sistema.
## Fluxo Principal:
- Garçom acessa painel de pedidos.
- Visualiza novos pedidos.
- Atualiza o status (em preparo, pronto, entregue).
## Fluxo Alternativo:
- Sistema caiu no meio da atualização.
- Pedido não chegou corretamente no painel.
## Pós-condições: 
- Pedido atualizado corretamente com novo status.
# 4. Editar cardápio
## Ator: 
- Gerente
## Objetivo: 
- Adicionar, remover ou editar itens do cardápio.
## Pré-condições: 
- Gerente deve estar logado com permissão de edição.
## Fluxo Principal:
- Gerente acessa painel de cardápio.
- Clica em “adicionar” ou “editar” item.
- Insere nome, descrição, preço e foto.
- Salva as alterações.

## Fluxo Alternativo:
- Item já existe com mesmo nome.
- Descrição inválida.
## Pós-condições: 
- Cardápio foi atualizado no sistema.
# 5. Gerar relatório de vendas
## Ator: 
- Gerente
## Objetivo: 
- Ver relatório financeiro do restaurante.
## Pré-condições: 
- Gerente deve estar logado com acesso a relatórios.
## Fluxo Principal:
- Gerente entra no painel de relatórios.
- Escolhe intervalo de tempo (dia, semana, mês).
- Sistema gera relatório com dados de vendas, pratos mais pedidos, ticket médio.
## Fluxo Alternativo:
- Sistema sem dados suficientes.
- Erro ao carregar relatório.
## Pós-condições: 
- Relatório é exibido na tela e pode ser exportado.
# 6. Avaliar pedido
## Ator: 
- Cliente
## Objetivo: 
- Avaliar o pedido e atendimento recebido.
## Pré-condições: 
- Cliente precisa ter finalizado um pedido.
## Fluxo Principal:
- Cliente recebe notificação para avaliar.
- Acessa tela de avaliação.
- Dá nota, escreve comentário e pode anexar foto.
## Fluxo Alternativo:
- Cliente não logado.
- Pedido ainda em andamento.

## Pós-condições: A
- Avaliação fica salva e disponível para consulta pelos gerentes.


# Cenário 4 - Sistema de Gerenciamento de Cursos Online 
Uma plataforma de cursos online permite que os estudantes se inscrevam em cursos, assistam às 
aulas e submetam trabalhos. Os instrutores podem criar cursos, gerenciar conteúdo e avaliar os 
trabalhos submetidos. O administrador da plataforma gerencia os usuários (estudantes e 
instrutores) e gera relatórios sobre a utilização da plataforma.
## Requisitos Funcionais (RF)
1. O sistema deve permitir que estudantes se cadastrem e acessem sua conta.

2. O sistema deve permitir que estudantes se inscrevam em cursos disponíveis.

3. O sistema deve liberar acesso ao conteúdo das aulas para os estudantes inscritos.

4. O sistema deve permitir que os instrutores publiquem, editem ou removam conteúdos dos cursos.

5. O sistema deve permitir que estudantes enviem trabalhos diretamente pela plataforma.

6. O sistema deve permitir que instrutores avaliem e deixem feedback nos trabalhos enviados.

7. O sistema deve enviar notificações para os usuários sobre prazos, atualizações ou avisos de curso.

# Requisitos Não Funcionais (RNF)
1. A plataforma deve funcionar 24 horas por dia, todos os dias.

2. A interface deve ser responsiva e funcionar em PC, celular e tablet.

3. O sistema deve criptografar os dados dos usuários.

4. O tempo de carregamento das páginas não pode passar de 3 segundos.

# Requisitos de Domínio (RD)
1. Todos os instrutores devem ser validados com CPF e comprovação de formação ou experiência.
2. Todos os cursos precisam de uma carga horária definida e um plano de ensino associado.

# Atores
-Estudante
-Instrutor
-Administrador

# Casos de Uso
# 1. Cadastro de estudante
## Ator: 
- Estudante
## Objetivo: 
- Criar uma conta para usar a plataforma.
## Pré-condições: 
- Ter e-mail válido e CPF.
## Fluxo Principal:
- Estudante acessa página de cadastro.
- Preenche dados pessoais.
- Cria login e senha.
- Confirma cadastro pelo e-mail.
## Fluxo Alternativo:
- E-mail já cadastrado.
- Dados incompletos.

## Pós-condições: 
- Estudante está com conta ativa na plataforma.

# 2. Inscrição em curso
## Ator: 
- Estudante
## Objetivo: 
- Se inscrever em um curso de interesse.
## Pré-condições: 
- Estar logado no sistema.
## Fluxo Principal:
- Estudante entra no catálogo de cursos.
- Escolhe um curso.
- Clica em "Inscrever-se".
- Confirma participação.
## Fluxo Alternativo:
- Curso já lotado.
- Estudante tentando se inscrever sem login.

## Pós-condições: 
- Estudante está inscrito e com acesso ao conteúdo.

# 3. Assistir aula
## Ator: 
- Estudante
## Objetivo: 
- Acessar os vídeos e materiais do curso.
## Pré-condições: 
- Ter se inscrito no curso.
## Fluxo Principal:
- Estudante entra na aba “Meus Cursos”.
- Escolhe o curso que quer assistir.
- Clica na aula desejada.
- O vídeo e os materiais são carregados.

## Fluxo Alternativo:
- Aula indisponível por erro do instrutor.
- Plataforma fora do ar.

## Pós-condições: 
- Estudante teve acesso ao conteúdo da aula.

# 4. Publicar conteúdo do curso
## Ator: 
- Instrutor
## Objetivo: 
- Inserir vídeos, PDFs, links ou tarefas no curso.
## Pré-condições: 
- Instrutor logado e com curso registrado.
## Fluxo Principal:
- Instrutor acessa painel do curso.
- Escolhe aula ou módulo que vai editar.
- Adiciona vídeos, textos ou atividades.
- Salva alterações.
## Fluxo Alternativo:
- Arquivo inválido ou com tamanho excedido.
- Plataforma fora do ar.
## Pós-condições: 
- O conteúdo foi publicado com sucesso e está disponível pros alunos.

# 5.Entrega de trabalho
## Ator: 
- Estudante
## Objetivo: 
- Submeter um trabalho para avaliação do instrutor.
## Pré-condições: 
- O curso deve ter pelo menos uma atividade liberada.
## Fluxo Principal:
- Estudante acessa a tarefa.
- Faz upload do trabalho (PDF, link ou texto).
- Clica em “Enviar”.
- Sistema confirma o envio.

## Fluxo Alternativo:
- Arquivo fora do formato permitido.
- Prazo da atividade já passou (o sistema aceita porém notifica que a tarefa foi entregue atrasada.).
## Pós-condições: 
- O trabalho está salvo no sistema e disponível para o instrutor corrigir.

# 6. Avaliação de trabalho
##  Ator: 
- Instrutor
## Objetivo: 
- Corrigir trabalhos enviados e dar feedback.
## Pré-condições: 
- Ter pelo menos um trabalho entregue por aluno.
## Fluxo Principal:
- Instrutor acessa a lista de entregas.
- Visualiza cada trabalho.
- Deixa nota e comentário.
- Clica em “Concluir avaliação”.
## Fluxo Alternativo:
- Trabalho corrompido ou ilegível.
- Sistema indisponível no momento.
## Pós-condições: 
- Estudante recebe nota e comentário do instrutor.

# 7. Gerar relatório de uso
## Ator: 
- Administrador
## Objetivo: 
- Ver estatísticas de acesso, cursos mais populares, e engajamento dos usuários.
## Pré-condições: 
- Administrador logado na plataforma.
## Fluxo Principal:
- Admin acessa a aba de relatórios.
- Seleciona período e tipo de relatório.
- Clica em “Gerar”.
- Sistema apresenta os dados na tela.

## Fluxo Alternativo:
- Falha no carregamento dos dados.
- Nenhum dado disponível no período escolhido.
## Pós-condições: 
- Relatório pronto para visualização e exportação.


# Cenário 5 - Sistema de Gerenciamento de Eventos: 
Um sistema de gerenciamento de eventos permite que os organizadores criem e gerenciem 
eventos, os participantes se registrem para os eventos e que os administradores gerenciem a 
plataforma e gerem relatórios de participação. Os eventos podem ser conferências, workshops ou 
seminários.
# Requisitos Funcionais (RF)
1. O sistema deve permitir que organizadores cadastrem eventos com data, local e descrição.

2. O sistema deve permitir que participantes se registrem em eventos disponíveis.

3. O sistema deve liberar certificados para participantes após o evento.

4. O sistema deve permitir o envio de notificações para os inscritos (lembretes, atualizações, etc.).

5. O sistema deve permitir que administradores removam ou editem eventos.

6. O sistema deve gerar relatórios de eventos realizados, número de participantes e feedbacks recebidos.

7. O sistema deve permitir que participantes deixem feedback do evento.

# Requisitos Não Funcionais (RNF)
1. A plataforma deve suportar até 10 mil acessos simultâneos sem travar.

2. A aplicação deve ser responsiva e funcionar bem no celular.

3. Os dados dos usuários devem ser criptografados.

4. O tempo de resposta para cada ação deve ser no máximo 2 segundos.

# Requisitos de Domínio (RD)
1. Todos os eventos devem ser registrados com CNPJ ou CPF do organizador.
2. Os certificados devem seguir um modelo padrão e conter nome, data, título do evento e carga horária.

# Atores
- Participante
- Organizador
- Administrador

# Casos de Uso
# 1. Criar evento
## Ator: 
- Organizador
## Objetivo: 
- Cadastrar um novo evento na plataforma.
## Pré-condições: 
- Organizador deve ter conta e estar logado.
## Fluxo Principal:
- Organizador acessa o painel de eventos.
- Clica em “Criar novo evento”.
- Preenche as informações (nome, data, descrição, local).
- Confirma e publica o evento.
## Fluxo Alternativo:
- Dados obrigatórios não preenchidos.
- Data inválida.

## Pós-condições: 
- Evento foi criado e está visível para os participantes.

2. Registro no evento
## Ator: 
- Participante
## Objetivo: 
- Garantir presença no evento escolhido.
## Pré-condições: 
- Participante deve estar com conta ativa e logado.
## Fluxo Principal:
- Participante acessa a lista de eventos.
- Escolhe um evento.
- Clica em “Registrar”.
- Recebe confirmação por e-mail ou no painel.

## Fluxo Alternativo:
- Evento já lotado.
- Participante não está logado.

## Pós-condições: 
- Registro confirmado, participante garantido no evento.

# 3. Envio de certificado
# Atores: 
-Sistema (automático) 
- Administrador
## Objetivo: 
- Enviar certificados após o término do evento.
## Pré-condições: 
- Participante deve ter comparecido ou marcado presença.
## Fluxo Principal:
- Sistema verifica quem participou.
- Gera o certificado em PDF com dados do evento.
- Envia por e-mail ou deixa disponível na conta.
## Fluxo Alternativo:
- Erro no registro de presença.
- Sistema não encontra dados do evento.
## Pós-condições: 
- Participante tem acesso ao certificado.

# 4. Feedback de evento
## Ator: 
- Participante
## Objetivo: 
- Avaliar o evento após a participação.
## Pré-condições: 
- Ter participado de um evento.
## Fluxo Principal:
- Participante acessa o evento no histórico.
- Clica em “Deixar feedback”.
- Escreve comentário e dá uma nota.
- Envia a avaliação.

## Fluxo Alternativo:
- Participante tenta avaliar sem ter comparecido.
- Sistema fora do ar.
- Pós-condições: Feedback salvo e disponível para o organizador/administrador.

## 5. Geração de relatório
## Ator: 
- Administrador
## Objetivo: 
- Ver dados de eventos, participação e feedback.
## Pré-condições: 
- Estar logado com perfil de administrador.
## Fluxo Principal:
- Acessa a área de relatórios.
- Escolhe evento ou período específico.
- Gera o relatório com total de participantes, inscritos e notas dadas.
- Exporta ou visualiza.

## Fluxo Alternativo:
- Falta de dados para o período selecionado.
- Sistema indisponível.
## Pós-condições: 
- Relatório gerado e pronto para análise.

# 6. Cancelamento de evento
## Atores: 
- Organizador
- Administrador
## Objetivo: 
- Remover ou cancelar evento por algum motivo.
## Pré-condições: 
- Estar logado e ser dono do evento (ou administrador).
## Fluxo Principal:
- Organizador acessa o painel de eventos.
- Seleciona o evento.
- Clica em “Cancelar” e confirma ação.
- Sistema notifica os inscritos.

## Fluxo Alternativo:
- Evento já ocorreu, não pode ser cancelado.
- Sistema está fora do ar.

## Pós-condições: 
- Evento cancelado e participantes notificados.

