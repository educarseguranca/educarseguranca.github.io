---
layout: post
title: Nada é seguro!
permalink: /Nada-E-Seguro/
---

Nada é 100% seguro! Ter isto em mente é fundamental quando se trata de segurança.

Um sistema dito seguro é aquele que procura sempre melhorar em termos de segurança, consegue identificar e responder rapidamente em caso de falhas, e tenha redundância suficiente para prevenir uma falha total.
Neste caso sistema pode significar várias coisas: sistemas operativos, aplicações, processos pessoais <sup>1</sup>; etc. Basicamente tudo onde segurança faça sentido.
Costumo avaliar o grau de segurança de um sistema, pelo esforço necessário que uma entidade maliciosa teria de fazer para conseguir quebrar a segurança do mesmo. É uma questão simples de custo/benefício (como em tudo na vida): aumentando o custo de quebrar a segurança de um sistema, reduz-se o número de possíveis entidades maliciosas que vão tentar fazê-lo, e o retorno no benefício torna-se menor.


<sup>1</sup> <sub>Um exemplo é a forma como gerimos as nossas palavras-passe pessoais. Desde memorizar até utilizar um bloco de notas ou um gestor de palavras-passe, tudo pode ser visto nesta perspetiva.</sub>


### Como surgem então os problemas?

Muitos dos casos de "falha de segurança" em que um site ou uma aplicação perde dados, ou de onde são roubados dados dos utilizadores, não se trata (na minha opinião) de uma falha de segurança, trata-se sim de uma [não existência de segurança][link0]. Penso que não se pode dizer que a causa é uma falha de segurança se nunca houve investimento nesse sentido. Seria o mesmo que dizer que é uma falha de segurança quando um banco tem o cofre aberto, na rua, e descobrem que desapareceu dinheiro.


Outro [grande][link1] [número][link2] de [casos][link3] surgem do facto de [não serem feitas][link4] [atualizações][link5] das aplicações e ferramentas que se utilizam. Por vezes os custos de atualizar são grandes, mas geralmente não são tidos em conta os custos de recuperar de uma falha de segurança que surge da falta dessas mesmas atualizações.


É fácil ser-se alvo de um ataque (no ponto de vista dos sistemas) à medida que o número de utilizadores cresce, e quando se pensa em proteção para que estes ataques não tenham sucesso, é necessário proteger todas as possíveis "portas de entrada", de todo o tipo de ataques conhecidos. Porque para quem ataca, basta encontrar um elo fraco ou "porta de entrada" para se poder ultrapassar toda a segurança do sistema.


Um ponto que vale a pena mencionar no que toca à segurança de um sistema é que as pessoas são (invariavelmente) o [elo mais fraco][link6]. Por exemplo numa empresa por muito que se invista na segurança da infraestrutura e em processos seguros, o elo mais fraco continua a ser o humano que utiliza essa infraestrutura. Basta que um dos utilizadores faça o download de um ficheiro malicioso, ou faça clique num link de um e-mail malicioso e pode deitar por terra todo o esforço até aí investido pela empresa.


### Como identificar possíveis problemas?

Para grandes sistemas ou aplicações existe normalmente (num caso onde existe esta preocupação claro) monitorização da utilização, de acessos a dados, logins, etc. E alguns serviços dão a conhecer ao utilizador quando algum alerta é gerado: [por exemplo a Google envia um email][imageLoginAlert], para os e-mails de segurança configurados, a alertar para o facto dessa conta Google ter feito login num dispositivo desconhecido ou pouco utilizado.
[Existem também alguns serviços][hibp] disponibilizados [a título individual][TroyHunt] que alertam os seus utilizadores em caso de falhas de segurança nos serviços mais utilizados na web.


Claro que, no caso de processos pessoais, cabe a cada um tentar perceber os riscos que corre, e no caso de haver alguma suspeita tentar investigar na medida do possível se existem realmente problemas. É um dos compromissos da não utilização de ferramentas de terceiros, ter a responsabilidade de monitorizar e investigar em caso de suspeita se houver esta preocupação com segurança.


### Como reagir em caso de falha de segurança?

Neste caso sem saber a causa e efeitos do problema em causa é difícil determinar o melhor caminho a seguir. No entanto é possível fazer um plano e tentar seguir da melhor forma possível:

* Tentar adquirir o máximo de informação possível acerca do tipo problema;
* Tentar saber se se aplica ao nosso caso específico;
* Seguir instruções gerais para o tipo de problema em causa.

Exemplo: se for o caso de roubo de credenciais de um site ou aplicação da quais somos utilizadores, normalmente o melhor curso é terminar as sessões abertas, esperar pela indicação dos responsáveis do site que o problema foi identificado/contido, e mudar a palavra-passe depois desta indicação. No caso desta palavra-passe ser utilizada noutros sites (má prática a ser discutida noutro tópico) mudar as palavras-passe nos outros sites onde é utilizada.

## Segurança versus Usabilidade

> "É possível ter aplicações ou processos mais seguros? Então porque não se fazem aplicações mais seguras?"

Acerca deste tópico o que há a saber é que existe sempre um compromisso entre segurança e usabilidade, e os serviços tentam oferecer o melhor equilíbrio possível ao utilizador (ou deveriam) e por vezes dão a possibilidade de melhorar a segurança com a perda de um pouco de conforto (ou usabilidade) - como é o caso da autenticação em dois passos.

Como o objetivo não é a segurança (na maior parte dos casos), têm de se eliminar os obstáculos que podem pôr em causa o objetivo (na maior parte dos casos é mais utilizadores que se traduz em mais lucros) e facilitar a aderência dos utilizadores. Claro que com o nível de segurança suficiente para que estes não abandonem o serviço.

[Por vezes os serviços complicam][link7] e existe mesmo a perda de usabilidade e redução de segurança, com base em decisões antiquadas ou mesmo erradas.



[link0]: https://arstechnica.com/security/2017/03/firefox-gets-complaint-for-labeling-unencrypted-login-page-insecure
[link1]: https://www.publico.pt/2017/05/13/tecnologia/noticia/europol-ciberataque-foi-de-um-nivel-sem-precedentes-1772033
[link2]: https://www.rtp.pt/noticias/mundo/ciberataque-mundial-e-ainda-uma-ameaca-presente_a1002046
[link3]: https://www.rtp.pt/noticias/pais/portugal-telecom-confirma-ter-sido-alvo-de-ciber-ataque_a1001323
[link4]: https://www.publico.pt/2017/05/15/tecnologia/noticia/perguntas-e-respostas-sobre-o-ciberataque-1772266
[link5]: https://technet.microsoft.com/en-us/library/security/ms17-010.aspx
[link6]: https://pt.wikipedia.org/wiki/Phishing
[link7]: https://www.troyhunt.com/the-cobra-effect-that-is-disabling/
[imageLoginAlert]: ../images/google_login_alert.png
[hibp]: https://haveibeenpwned.com/
[TroyHunt]: https://www.troyhunt.com/about/
