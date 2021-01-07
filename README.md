# PLCexercises
PLC (Programmable Logic Controller) using Ladder Diagram Language


Exercício prático 1 - Portão:
Neste exercício, você aplicará seu conhecimento de Ladder para projetar um programa que controlará a porta ProSim-II. 
O sistema de porta inclui um motor reversível, um par de chaves limitadoras e um painel de controle, todos conectados ao seu PLC. 
O programa que você criar irá monitorar e controlar este equipamento enquanto segue os seguintes critérios:
-Neste exercício, os botões Abrir e Fechar serão usados para controlar os movimento da porta. 
O movimento não será mantido quando qualquer um dos interruptores for liberado e, portanto, o interruptor de Stop não é necessário nem usado neste exercício. 
No entanto, todas as outras entradas e saídas disponíveis são empregadas neste exercício.
-Pressionar o interruptor de abertura fará com que a porta se mova para cima (aberta) se não já totalmente aberto. 
A operação de abertura continuará enquanto a chave estiver pressionada. 
Se a chave for liberada, ou se a chave limitadora LS1 abrir,  o movimento da porta irá parar imediatamente.
-Pressionar o botão Fechar fará com que a porta se mova para baixo (feche), se ainda não estiver totalmente fechado. 
A operação de fechamento continuará enquanto a chave for mantida pressionada. 
Se a chave for liberada, ou se a chave limitadora LS2 fechar, o movimento da porta irá parar imediatamente.
-Se a porta já estiver totalmente aberta, pressionar o interruptor de abertura não irá energizar o motor.
-Se a porta já estiver totalmente fechada, pressionar o botão Fechar não energizará o motor.
-Sob nenhuma circunstância o motor deve ser acionado para girar nos dois sentidos simultaneamente.
-A lâmpada aberta acenderá se a porta estiver na posição Totalmente aberta.
-A lâmpada fechada será iluminada se a porta estiver na posição totalmente fechada.

Exercício prático 2 - Portão:
Modifique o programa do exercício anterior para que o CLP mantenha o movimento da porta apropriado, uma vez iniciado por o operador. 
A operação de abertura ou fechamento da porta continuará até a conclusão mesmo que o operador libere o botão que iniciou o movimento. 
O programa irá aderir aos seguintes critérios:
-O movimento da porta irá parar imediatamente quando o Interruptor de Parada for inicialmente pressionado, e permanecerá parado se a chave for liberada.
-Pressionar o interruptor de abertura fará com que a porta se abra, se ainda não estiver totalmente aberta. 
A operação de abertura continuará até a conclusão mesmo que o interruptor seja liberado.
-Pressionar o botão Fechar fará com que a porta feche, se ainda não estiver totalmente fechada. 
A operação de fechamento continuará até a conclusão mesmo se o interruptor for liberado.
-Se a porta já estiver totalmente aberta, pressionar o interruptor de abertura não irá energizar o motor.
-Se a porta já estiver totalmente fechada, pressionar o botão Fechar não energizará o motor.
-Sob nenhuma circunstância os dois enrolamentos do motor serão energizados ao mesmo tempo. 
-A lâmpada AJAR será iluminada se a porta NÃO estiver totalmente fechada ou na posição totalmente aberta. 
-A lâmpada aberta acenderá se a porta estiver na posição Totalmente aberta. Além disso, sempre que a porta estiver se movimentando para abrir, a lâmpada deverá piscar;
-A lâmpada fechada acenderá se a porta estiver na posição Totalmente fechada. Além disso, sempre que a porta estiver se movimentando para fechar, a lâmpada deverá piscar;

Exercício prático 3 - Silo:
O sistema irá posicionar automaticamente as caixas e enchê-las de forma sequencial. Além disso, fazer com que:
-A sequência possa ser parada e reiniciada a qualquer momento usando os botões Start e Stop
-A lâmpada RUN deve permanecer acesa enquanto o sistema estiver funcionando;
-Se o botão Stop for pressionado, tanto a lâmpada RUN, quanto o motor e a válvula devem ser desernegizadas imediatamente;
-A lâmpada FILL deve ficar acesa enquanto a caixa estiver enchendo;
-A lâmpada FULL será energizada quando a caixa estiver cheia e deve permanecer assim até que a caixa mova para longe do sensor de proximidade.

Exercício prático 4 - Semáforo:
Primeira parte
Utilizando um único temporizador, use as instruções de comparação de palavras para controlar o semáforo simulado.
Seu programa deve incorporar um período de 1 segundo (verde atrasado) quando ambas as direções terão apenas suas luzes VERMELHAS acesas. 

Segunda parte
Modifique o seu programa para que as faixas de pedestres também sejam controladas. Seu programa deve operar da seguinte forma:
-Quando pressionado, o botão de faixa de pedestres causará ao Sinal de Caminhada apropriado ser iluminado na próxima ocorrência de uma transição de Vermelho para Verde 
para a direção apropriada;
-Uma vez que o Sinal de Caminhada esteja aceso, ele permanecerá assim durante o Green (do semáforo contrário) sinal.
-Quando a luz amarela (do semáfor contrário) aparece, o Walk Sign começará a piscar On e Off e continue fazendo isso até que o sinal vermelho apareça.
