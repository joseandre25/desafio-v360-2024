### Personas

O sistema foi projetado para atender as necessidades de diferentes usuários envolvidos no processo de recebimento e logística do Centro de Distribuição (CD). As principais personas são:

- **João, Supervisor de Recebimento**: Responsável por garantir a organização do pátio e das docas, e pela eficiência no descarregamento dos caminhões.
- **Maria, Analista de Suprimentos**: Encargada de assegurar que todos os materiais para a produção sejam entregues no prazo, evitando custos extras e interrupções.
- **Carlos, Coordenador de Logística**: Gerencia o fluxo logístico do CD, garantindo que as entregas sejam feitas de forma organizada e sem congestionamentos no pátio.

Essas personas enfrentam desafios que o sistema busca resolver por meio de funcionalidades específicas para melhorar a visibilidade, organização e eficiência no processo de agendamento e recebimento de entregas.


### Associações Temáticas de Problemas com Requisitos Funcionais

| **Problema**                                   | **Usuários Relacionados**                            | **Requisitos Funcionais que Resolvem**                                                                                  |
|------------------------------------------------|------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
| **Falta de controle e agendamento de entregas** | João, Maria, Carlos                                  | RF01 – Agendamento de Entregas (FT01), RF10 – Consulta e Monitoramento de Entregas Programadas (FT10)                   |
| **Congestionamento no pátio e docas**           | João, Carlos                                         | RF02 – Validação de Capacidade do Pátio e Docas (FT02), RF03 – Visibilidade em Tempo Real de Capacidade (FT03)           |
| **Falta de visibilidade de entregas futuras**   | Maria, Carlos                                        | RF03 – Visibilidade em Tempo Real de Capacidade (FT03), RF10 – Consulta e Monitoramento de Entregas Programadas (FT10)   |
| **Falta de comunicação sobre mudanças**         | João, Maria                                          | RF04 – Notificações Automáticas (FT04)                                                                                 |
| **Priorização de entregas críticas**            | João, Maria, Carlos                                  | RF05 – Priorização de Entregas (FT05), RF08 – Reorganização da Fila de Entregas (FT08)                                  |
| **Atrasos e custos extras com entregas fora do horário** | Maria, Carlos                                | RF07 – Definição de Janelas de Horários Permitidos (FT07), RF09 – Relatórios de Entregas Atrasadas ou Fora do Horário (FT09) |
| **Ociosidade ou uso ineficiente do pátio**      | João, Carlos                                         | RF06 – Geração de Relatórios de Utilização (FT06), RF09 – Relatórios de Entregas Atrasadas ou Fora do Horário (FT09)     |

### Explicação

1. **Falta de controle e agendamento de entregas**: Todos os usuários mencionam a ausência de um sistema que permita organizar as entregas no CD. O RF01 resolve isso com um sistema de agendamento, e o RF10 dá visibilidade de entregas futuras.
2. **Congestionamento no pátio e docas**: João e Carlos destacam problemas com congestionamento. O RF02 valida a capacidade antes de agendar, e o RF03 dá visibilidade em tempo real para uma gestão eficiente.
3. **Falta de visibilidade de entregas futuras**: Maria e Carlos mencionam a necessidade de saber quando as entregas serão feitas para melhor planejamento. O RF03 e RF10 resolvem isso mostrando a capacidade do pátio e a lista de entregas.
4. **Falta de comunicação sobre mudanças**: Maria e João destacam a falta de atualizações automáticas sobre mudanças nas entregas. O RF04 resolve isso com notificações automáticas.
5. **Priorização de entregas críticas**: Todos os usuários mencionam a importância de gerenciar entregas críticas. O RF05 e RF08 tratam da priorização de entregas e reorganização automática da fila.
6. **Atrasos e custos extras com entregas fora do horário**: Maria e Carlos destacam o impacto de entregas fora do horário. O RF07 previne isso configurando horários permitidos, e o RF09 gera relatórios sobre atrasos e custos.
7. **Ociosidade ou uso ineficiente do pátio**: João e Carlos mencionam a ineficiência do uso do pátio, resolvido com o RF06, que gera relatórios de uso, e o RF09, que analisa entregas fora do horário.
