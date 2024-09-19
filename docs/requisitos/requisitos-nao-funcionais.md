## Requisitos Não Funcionais
Esta seção descreve os requisitos não funcionais, que são atributos de qualidade e restrições que o sistema deve atender para garantir sua eficácia e eficiência em ambiente produtivo.

### **RNF01** – Desempenho
**Descrição:**  
O sistema deve ser capaz de processar agendamentos e exibir atualizações de status em tempo real com um tempo de resposta máximo de 2 segundos por operação.

**Justificativa:**  
A velocidade de resposta é crucial para garantir que as operações logísticas não sejam prejudicadas e para proporcionar uma experiência de usuário fluida, principalmente em momentos de alta demanda.

**Critérios de Aceitação:**<br>
- O tempo de resposta do sistema para consultas e atualizações não deve exceder 2 segundos. <br> 
  - O sistema deve ser capaz de processar até 500 agendamentos simultâneos sem degradação de performance.

---

### **RNF02** – Disponibilidade
**Descrição:**  
O sistema deve estar disponível para uso na maior parte do tempo, com janelas de manutenção programadas fora do horário comercial do CD.

**Justificativa:**  
Alta disponibilidade é essencial para suportar a operação contínua do Centro de Distribuição, minimizando interrupções que possam afetar a logística e o planejamento das entregas.

**Critérios de Aceitação:**  <br>
- O sistema deve ter uma taxa de disponibilidade mínima de 99,9%.  <br>
  - As janelas de manutenção devem ser programadas e notificadas com pelo menos 24h de antecedência.

---

### **RNF03** – Escalabilidade
**Descrição:**  
O sistema deve ser escalável, suportando o crescimento no número de agendamentos e o aumento na quantidade de usuários simultâneos, sem comprometer a performance.

**Justificativa:**  
O volume de entregas e a quantidade de usuários pode aumentar com o tempo, e o sistema deve ser capaz de lidar com essa expansão sem queda no desempenho.

**Critérios de Aceitação:**  <br>
- O sistema deve suportar o dobro da carga inicial (número de usuários e agendamentos) sem perda de desempenho.  <br>
  - Deve ser possível adicionar novos servidores e recursos sem reconfiguração significativa do sistema.

---

### **RNF04** – Segurança
**Descrição:**  
O sistema deve garantir a segurança das informações por meio de autenticação de usuários, criptografia de dados sensíveis e registro de atividades (logs), para evitar acessos não autorizados e garantir a rastreabilidade das ações.

**Justificativa:**  
A proteção de dados, especialmente sobre fornecedores, entregas e informações do CD, é essencial para evitar fraudes, acessos indevidos e garantir a conformidade com normas de segurança da informação.

**Critérios de Aceitação:**  <br>
- O sistema deve implementar autenticação via login e senha com regras de segurança (mínimo de 8 caracteres, uso de números e caracteres especiais).  <br>
- Todos os dados sensíveis (agendamentos, fornecedores, usuários) devem ser criptografados.  
  - O sistema deve manter logs de todas as ações de usuários por um período determinado.

---

### **RNF05** – Usabilidade
**Descrição:**  
O sistema deve ter uma interface de usuário intuitiva e de fácil utilização, com treinamentos mínimos necessários. Deve ser acessível em desktops e dispositivos móveis, garantindo responsividade.

**Justificativa:**  
Usuários com diferentes níveis de familiaridade com tecnologia precisam usar o sistema de forma eficiente, e ele deve ser intuitivo o suficiente para minimizar erros operacionais.

**Critérios de Aceitação:**  <br>
- O sistema deve ser acessível tanto em desktop quanto em dispositivos móveis, com uma interface responsiva.  <br>
- Testes de usabilidade devem demonstrar que 90% dos usuários conseguem completar uma operação básica (ex.: agendar entrega) sem auxílio técnico.
