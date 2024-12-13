Avaliação de implementação da cultura devops CALMS


## Cultural

A aplicação tem um histórico de falhas relativamente alto, então seria interessante a equipe realizar uma análise pós-resolução para entender o que aconteceu e como evitar que esse(s) problema(s) ocorram novamente.

## Automação

Dado os processos que a empresa tem, a implementação de automação em diversas partes do processos ajudaria a equipe a diminuir o tempo de deploy, defeitos e o tempo gasto em testes manuais: 

### Esteira de CI

Esteiras automaticas de CI garantiriam que a aplicação está em um estado correto e evitando que aplicações "quebradas" sejam passadas para etapas posteriores. Isso ajudaria a ter uam entrega mais agil das funcionalidades já que a esteira já garantiria o estado correto da aplicação e deixaria ela já apta a ser publicada, ajudaria a evitar que erros de negócio sejam passados a diante já que os testes seriam executados automaticamente na esteira e também diminuiria o tempo gasto pelo time de operação testando manualmente a aplicação.

### Testes automatizados

Adição de testes automatizados diminuiriam o tempo gasto pelo time de operações em testes manuais e correção de aplicação e também diminuiria as chances da aplicação ser publicada com algum erro. Assim, se algum erro aparecer quebrado no processo, o próprio time de desenvolvimento já corrige esses erros, evitando trabalho para o time de operações.

### Esteira de CD

Com uma esteira de CD, a publicação passaria a ser automatica, diminuindo o tempo gasto pelo time de operações no deploy manual e aumentando a velocidade de deploy.

## Lean

Olhando as métricas de desempenho se observa um tempo relativamente grande para o deploy e recuperação assim como números um pouco altos de incidentes. Atacando o tempo de entrega pode ser que o time não esteja entregando valor o tão rápido quanto poderia, então conversar com o time para que passem a focar na entrega MVP(Minimal Viable Product) entregando o maior valor com o menor tempo possível somado as outras melhorias mencionadas ajudariam a diminuir esse tempo consideravelmente.

Dado o número de incidentes, a aplicação de análises pós-resolução do problema para entender o que aconteceu em conjunto com as outras melhorias mencionadas, traria um entendimento do que deu errado e como evitar isso.

A taxa de sucesso de deploys pode ser atacada com a automação das etapas de desenvolvimento como esteira de CI/CD e monitoramento através da garantia que a aplicação que está em deploy está até certo ponto "correta", fazendo o deploy automatico da aplicação e com monitoramento para poder acompanhar e ter informações da aplicação no decorrer da sua aplicação para ter mais informações na tomada de decisões e também identificar possiveis problemas.

O tempo de recuperação pode ser melhorado de maneira semelhante a taxa de sucesso, com a utilização de CD para a publicação rápida de versões da aplicação(seja rollback ou novas versões) como o monitoramento que ajudaria a ter um diagnostico mais preciso do problema.

## Mensuração

A mensuração é um componente muito importante, com ele podendo monitorar a saúde de diversos componentes da aplicação como banco de dados e aplicações individuais, como também coletar logs das aplicações que ajudariam a identificar as causas de eventuais problemas que venham a ocorrer.


# Tres maneiras


## Primeira maneira

Utilizar ferramentas para se ter uma maior visibilidade das tarefas em andamento, focando em entregas menores e com mais valor para o cliente.
Aplicação de automação para aumentar a confiabilidade da aplicação e diminuir o tempo gasto do time em deploys e correção de problemas

## Segunda maneira

Utilização de monitoramento para acompanhar a saúde da aplicação e coleta de logs de forma a identificar mais rápidamente problemas que venham a ocorrer, combinando isso com a automação para a execução de testes automatizados na esteira. 


## Terceira maneira

Criar uma cultura de aprendizado e compartilhamento para que membros do time estejam sempre aprendendo e trazendo conhecimentos/novas práticas para a empresa. Com recursos como 