## Visão de Produto

# 1. Introdução

## 1.1 Finalidade
A finalidade desta Especificação de Requisitos de Software (SRS) é detalhar os requisitos funcionais e não funcionais do sistema de Controle de Agendamentos de Entregas no Centro de Distribuição (CD). O objetivo principal é descrever de forma completa o comportamento esperado do sistema, incluindo funcionalidades que permitem o agendamento, monitoramento e controle das entregas, além de requisitos de desempenho, segurança e usabilidade. Este documento é voltado tanto para desenvolvedores quanto para testadores, garantindo uma visão abrangente e detalhada do que o sistema deve realizar.

## 1.2 Escopo
O sistema de Controle de Agendamentos de Entregas será responsável por gerenciar e otimizar o processo de recepção de mercadorias no CD, garantindo que as entregas sejam agendadas de forma eficiente, respeitando a capacidade do pátio e das docas. Ele permitirá o agendamento de entregas, monitoramento em tempo real da ocupação, priorização de materiais críticos, geração de relatórios e envio de notificações automáticas. Este SRS abrange todas as funcionalidades que asseguram o bom funcionamento do processo de agendamento, desde a entrada de dados até o controle de priorização e geração de relatórios.

## 1.3 Definições, Acrônimos, e Abreviações
- **CD**: Centro de Distribuição.
- **RF**: Requisito Funcional.
- **RNF**: Requisito Não Funcional.
- **SRS**: Especificação de Requisitos de Software.
- **Agendamento**: Processo de reserva de data e hora para a entrega de materiais no CD.
- **Docas**: Áreas de descarga de caminhões no CD.
- **Pátio**: Espaço físico no CD onde os caminhões aguardam para descarregar.
- **Prioridade**: Nível de urgência atribuído a uma entrega, que pode influenciar a ordem de descarregamento.

# 2. Descrição Geral

## 2.1 Perspectiva do Produto
O sistema de Controle de Agendamentos de Entregas faz parte do ambiente operacional do CD e interage diretamente com os processos logísticos da empresa. Ele será implementado como um sistema web acessível por diferentes dispositivos, permitindo a visualização e controle das entregas. O produto deve integrar-se a outros sistemas internos de gestão logística e permitir a interação tanto de usuários internos (equipe de recebimento e logística) quanto externos (fornecedores).

## 2.2 Funções do Produto
O sistema deve:<br>
- Permitir o agendamento de entregas, incluindo data, hora, tipo de material e fornecedor.<br>
- Verificar a disponibilidade de espaço no pátio e nas docas antes de confirmar um agendamento.<br>
- Monitorar em tempo real a ocupação do CD e a fila de descarregamento.<br>
- Priorizar entregas críticas conforme indicado pelos usuários.<br>
- Gerar relatórios de utilização e desempenho do CD.<br>
- Enviar notificações automáticas para os usuários sobre alterações ou cancelamentos.<br>
- Reorganizar a fila de entregas conforme as prioridades estabelecidas.

## 2.3 Características dos Usuários <br>
Os principais usuários do sistema são:<br>
- **Equipe de Logística**: Responsável por gerenciar as entregas e a ocupação do CD. Eles usarão o sistema para monitorar o fluxo de caminhões e tomar decisões operacionais.<br>
- **Fornecedores**: Responsáveis por agendar as entregas no CD, garantindo que seus caminhões cheguem dentro dos horários permitidos.<br>
- **Equipe de Recebimento**: Atuará na priorização de entregas e reorganização da fila de descarregamento com base em critérios de urgência e disponibilidade.
