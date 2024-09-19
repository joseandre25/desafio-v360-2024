## Requisitos Funcionais
Esta seção detalha os requisitos funcionais organizados por recursos principais do sistema.

### **RF01** – Agendamento de Entregas
O sistema deve permitir que os usuários agendem entregas no Centro de Distribuição (CD), com a
possibilidade de selecionar a data e horário de entrega. Esse agendamento deve incluir o nome do
fornecedor, o tipo de material a ser entregue e a quantidade correspondente.

**Justificativa:**  
Permitir o agendamento antecipado de entregas garante organização e previsibilidade no fluxo de
caminhões no CD, facilitando a alocação de espaço e recursos.

**Critérios de Aceitação:**<br>
- O usuário deve poder inserir a data, o horário, o fornecedor, o tipo de material e a quantidade a ser
entregue.<br>
- O sistema deve exibir uma confirmação de sucesso ou erro ao final do processo.

---

### **RF02** – Validação de Capacidade do Pátio e Docas
O sistema deve validar se há espaço disponível no pátio e nas docas para confirmar um agendamento de
entrega. Caso não haja espaço, o sistema deve sugerir um novo horário ou data para a entrega.

**Justificativa:**  
Evitar congestionamentos e falta de espaço, promovendo a otimização dos recursos físicos do CD.

**Critérios de Aceitação:**<br>
- O sistema deve verificar automaticamente a disponibilidade de docas e espaço no pátio antes de
confirmar o agendamento.<br>
- Se não houver espaço, o sistema deve sugerir ao usuário novos horários possíveis para o
agendamento.

---

### **RF03** – Visibilidade em Tempo Real de Capacidade
O sistema deve exibir em tempo real a capacidade atual das docas e do pátio, mostrando quais áreas estão
ocupadas e quais estão disponíveis para novas entregas.

**Justificativa:**  
Facilitar o gerenciamento da ocupação do CD, permitindo decisões rápidas e assertivas sobre a logística do
pátio e docas.

**Critérios de Aceitação:**<br>
- A capacidade do pátio e das docas deve ser atualizada em tempo real, com um atraso máximo de 2
segundos.<br>
- O sistema deve mostrar visualmente a ocupação do pátio e docas.

---

### **RF04** – Notificações Automáticas
O sistema deve enviar notificações automáticas para os usuários responsáveis (equipe de recebimento,
logística e suprimentos) sempre que houver alterações nos horários de entrega, cancelamentos ou qualquer
mudança relevante.

**Justificativa:**  
Manter todos os envolvidos atualizados sobre mudanças de cronograma ajuda a reduzir erros e evitar
impactos negativos no fluxo de trabalho.

**Critérios de Aceitação:**<br>
- O sistema deve enviar notificações por e-mail ou SMS em caso de alterações de agendamento.<br>
- O sistema deve permitir configurar quais eventos geram notificações e para quais usuários.

---

### **RF05** – Priorização de Entregas
O sistema deve permitir que os usuários atribuam prioridades às entregas, com base na urgência e na
importância dos materiais, para garantir que materiais críticos sejam recebidos de forma prioritária.

**Justificativa:**  
Priorizar entregas críticas assegura que a produção da fábrica não seja interrompida devido à falta de
materiais essenciais.

**Critérios de Aceitação:**<br>
- O usuário deve poder marcar entregas como "prioritárias" ao agendar.<br>
- O sistema deve organizar a ordem de descarga com base nas prioridades atribuídas.

---

### **RF06** – Geração de Relatórios de Utilização
O sistema deve gerar relatórios periódicos sobre a utilização do pátio e das docas, incluindo métricas como
tempo médio de espera dos caminhões, ociosidade das docas e número de entregas realizadas.

**Justificativa:**  
Esses relatórios permitem uma análise de desempenho do CD, ajudando na identificação de gargalos e na
otimização das operações logísticas.

**Critérios de Aceitação:**<br>
- O sistema deve gerar relatórios mensais e sob demanda.<br>
- Os relatórios devem incluir dados sobre tempo de espera, número de caminhões atendidos e
utilização do espaço.

---

### **RF07** – Definição de Janelas de Horários Permitidos
O sistema deve permitir a configuração de janelas de horário permitidas para entrega, respeitando o horário
de funcionamento do CD, com a possibilidade de bloquear agendamentos fora do expediente ou solicitar
aprovação especial.

**Justificativa:**  
Evitar custos extras com horas adicionais e garantir que o CD opere de maneira eficiente e dentro de seu
horário regular de trabalho.

**Critérios de Aceitação:**<br>
- O sistema deve bloquear automaticamente agendamentos fora das janelas de horário permitidas.<br>
- O sistema deve solicitar aprovação especial para agendamentos fora do expediente.

---

### **RF08** – Reorganização da Fila de Entregas
O sistema deve reorganizar a fila de entregas conforme as prioridades estabelecidas pelos usuários.
Entregas com maior prioridade devem ser tratadas com maior urgência, e o sistema deve ajustar a ordem de
descarregamento automaticamente.

**Justificativa:**  
Permitir uma melhor gestão das entregas com base em prioridades críticas garante que os recursos sejam
alocados de forma eficiente, evitando impactos na produção.

**Critérios de Aceitação:**<br>
- O sistema deve reorganizar a fila de descarregamento automaticamente com base na prioridade
atribuída a cada entrega.<br>
- O sistema deve permitir visualização da ordem de entrega reorganizada em tempo real.

---

### **RF09** – Relatórios de Entregas Atrasadas ou Fora do Horário
O sistema deve gerar relatórios sobre entregas que ocorreram fora do horário agendado ou que chegaram
com atraso, incluindo o impacto financeiro causado por horas extras ou outras medidas corretivas.

**Justificativa:**  
Esses relatórios fornecem visibilidade sobre os problemas operacionais e ajudam a identificar áreas que
precisam de melhorias, além de fornecer informações valiosas para minimizar custos extras.

**Critérios de Aceitação:**<br>
- O sistema deve gerar relatórios mensais e sob demanda sobre entregas atrasadas ou fora do
horário.<br>
- Os relatórios devem incluir o impacto financeiro estimado, como custos de horas extras.

---

### **RF10** – Consulta e Monitoramento de Entregas Programadas
O sistema deve permitir que os usuários consultem uma lista de todas as entregas programadas, com a
possibilidade de visualizar o status de cada uma (pendente, em trânsito, entregue, atrasada, etc.) e
acompanhar em tempo real.

**Justificativa:**  
Facilitar o monitoramento do fluxo de entregas permite uma melhor organização e controle do recebimento
de materiais, evitando imprevistos e otimizando a gestão do CD.

**Critérios de Aceitação:** <br>
- O sistema deve exibir uma lista de entregas programadas com o status atualizado em tempo real. <br>
- O sistema deve permitir filtrar as entregas por status, fornecedor, data ou prioridade.
