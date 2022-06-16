title: Terminoloia de alertas - New Relic
theme: jdan/cleaver-retro
author:
  name: Vitor Passarella
  email: vitor.moraes@zup.com.br
output: terminologia_alertas.html
controls: true

--

# Overview da terminologia de alertas do New Relic

--

### Sobre o que falaremos
Nesta pequena apresentação falaremos um pouco sobre a estrutura de alertas que podemos usar no New Relic e a ordem que elas funcionam.

--

### Estrutura de alertas

* Policy: os alertas começam com uma Policy. Uma Policy tem 0 ou mais condições (Condition). Uma boa prática é você ter pelo menos uma condição; 
* Condition: uma Condition é criada para analisar um data source, como um host ou app. Com uma Condition, você quer monitorar um comportamento, como o uso de um CPU em um host, ou algum outro limite (Threshold);
* Threshold: é uma configuração crítica que vai ativar uma violação (Violation);

--

* Violation: um evento que pode causar um incidente. Existem vários tipos de Violation, como Warning Violations, Critical Violations. Uma Critical Violation cria um incidente (Incident);
* Incident: criam notificações (Notification);
* Notification: Mensagem destinada a quem será notificado e como. Exemplos de notificações: via Slack, e-mail, webhooks etc.



