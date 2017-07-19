---
layout: page
title: Segurança Web Básica
permalink: /seguranca-web-basica/
---

Para encarar esta temática de segurança na internet (ou cibersegurança) é necessário [conhecer os riscos][preocupacoes] que se correm, para poder ponderar o nível de segurança adequado a cada situação. Por exemplo: como proceder em relação à palavra-passe do portal do banco não tem de ser necessariamente a mesma forma para um site de música. Não quer isto dizer que não se deva baixar a segurança de um lado, mas pelo menos tem de haver alguma consistência no nível mínimo de segurança.

Há que perceber se vale a pena perder algum conforto de utilização para ter mais segurança, e em que situações isso acontece.

## Dicas gerais para uma navegação mais segura

* Manter o *browser* e as extensões/*plugins* atualizados;

* Não manter sessões ligadas quando não se está a utilizar (fazer *logout* sempre);

* Utilizar opções de limpeza de *cookies* no *browser* ao fechar;

* Não aceitar *cookies* de sites não visitados;

* Por defeito, bloquear o acesso aos dispositivos do computador (*webcam*, microfone, etc..) em todos os sites;

* Bloquear a execução de *plugins*/*flash* também por defeito;

* Utilizar a [proteção contra monitorização][trackingprotection] do *browser* para todos os sites;

* Utilizar extensões no *browser* para bloquear monitorização e redes de publicidade;

* Se possível (em casos mais avançados) limitar a execução de *javascript* nos sites;

* Não utilizar redes públicas desconhecidas;

* Não utilizar redes públicas para aceder a serviços importantes;

* Não fazer fazer login em dispositivos que não sejam de confiança;

## Gestão de palavras-passe

Um dos temas mais debatidos na área de cibersegurança é a autenticação de utilizadores: por um lado existe a discussão de como proteger os serviços contra o roubo/exposição das credenciais dos utilizadores; por outro lado existe o debate sobre o que é uma boa palavra-passe e como fazer a gestão das nossas palavras-passe.

A primeira questão sendo mais técnica e tendo outro público alvo, não faz sentido apresentar aqui, a segunda questão, virada para o utilizador, é a que se vai explorar.

### O que é uma boa palavra-passe?

Antes de responder à pergunta vamos enumerar o que é uma má palavra-passe:

* Palavra-passe comum: fácil de adivinhar por outra pessoa (exemplo: '123456789');

* Relacionado com algo pessoal: fácil de adivinhar por outra pessoa (exemplo: data de nascimento, ou nome de um familiar);

* Palavra-passe com poucos caracteres: fácil de descobrir via computador em caso de exposição;

* Palavra-passe reutilizada: se for exposta por um dos serviços todos os outros ficam comprometidos;

* Palavra-passe derivada de outra: é fácil de descobrir estas variações hoje em dia, caso uma delas seja exposta.

Posto isto, uma palavra-passe que não seja comum, não seja reutilizada (única), não seja relacionada com algo pessoal, que não seja derivada de outras palavras-passe deverá ser uma boa palavra-passe. Por outras palavras, [uma boa palavra-passe é imemorável][securepassword].

Normalmente, uma palavra-passe segura, deve ser gerada aleatoriamente utilizando números, símbolos, letras maiúsculas e minúsculas, sempre diferente para cada aplicação ou serviços diferentes.

### Como fazer a gestão de palavras-passe?

Visto que as boas palavras-passe são imemoráveis, normalmente a gestão das mesmas é feita por aplicações dedicadas como [LastPass][lastpass] ou [1Password][onepassword] (entre outras) que permitem criar novas palavras-passe, fazer *login* em *websites*, etc. No entanto, é necessário confiar nestes serviços e nas suas implementações de armazenamento e transferência das nossas palavras-passe.

Existem também soluções *offline* como [KeePass][keepass] (ou [KeePassX][keepassx]) em que a base de dados que contém as credenciais é da responsabilidade do utilizador e pode ser armazenada, transferida, de acordo com as preferências de cada um.

A recomendação neste caso será para [LastPass][lastpass] ou similar, pela facilidade de utilização e plataformas suportadas.

## Autenticação em 2 passos

A autenticação de um utilizador pode ser feita por 3 vias:

1. Utilizando algo que ele sabe (palavra-passe, código pin, etc.);

2. Algo que ele tem ([RSA token][token], cartão [RFID][rfid], etc.);

3. Ou utilizando "algo que ele é" (dados biométricos como impressão digital).

No dia a dia, a escolha por conveniência é a via 1, e [como se sabe][nadaseguro] existe sempre um compromisso entre segurança e conveniência/usabilidade. Neste caso, algo que o utilizador saiba não quer dizer que mais ninguém o saiba, e não é possível determinar com certeza quem se está a autenticar.

Para aumentar a segurança (à custa de alguma conveniência) pode, em maior parte dos serviços, utilizar-se autenticação em 2 passos, que utiliza outra via (geralmente algo que o utilizador tem) para além da primeira.

Uma das formas de realizar este processo, é enviando uma mensagem ([SMS][sms]) ao utilizador após validar a palavra-passe, com um código PIN que terá de ser introduzido pelo utilizador. Mais recentemente, existe, por parte de muitos serviços, o suporte à aplicação *Google Authenticator* ([iOS][gaios] e [Android][gaandroid]) que gera PINs de 6 dígitos (temporários) que podem ser utilizados durante a autenticação.

## Comunicações privadas

## Compras Online


[trackingprotection]: https://support.mozilla.org/pt-PT/kb/protecao-contra-monitorizacao-na-navegacao-privada
[securepassword]: https://www.troyhunt.com/only-secure-password-is-one-you-cant/
[lastpass]: https://www.lastpass.com/
[onepassword]: https://1password.com/
[keepass]: http://keepass.info/
[keepassx]: https://www.keepassx.org
[token]: https://en.wikipedia.org/wiki/RSA_SecurID
[rfid]: https://en.wikipedia.org/wiki/Radio-frequency_identification
[gaios]: https://itunes.apple.com/us/app/google-authenticator/id388497605
[gaandroid]: https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2
[sms]: https://pt.wikipedia.org/wiki/Servi%C3%A7o_de_mensagens_curtas
[preocupacoes]: {{ site.baseurl }}/com-o-que-me-devo-preocupar
[nadaseguro]: {{ site.baseurl }}/nada-e-seguro/#segurancavsusabilidade
