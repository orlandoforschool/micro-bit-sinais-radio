# micro-bit-sinais-radio
Projeto micro:bit sinais rádio para 3 dispositivos

Para garantir que estou a comunicar no mesmo canal, defini o grupo de rádio para o mesmo número. Sendo assim, no editor MakeCode, separador Radio, posso definir um bloco para o grupo de microbits comunicar. pode ser qualquer número entre 0 e 255. Tem de ser o mesmo número.

A ideia do projeto é ter 3 dispositivos micro:bit. Anexei snapshots do código para cada um dos 3 micro:bit. No código partilhado tenho tudo junto. 

O primeiro micro:bit, define o grupo de radio como 255. Envia o número 1. Além disso, é exibido o número 1, para saber que a mensagem foi enviada. Este micro:bit quando receber a string "heart", mostra o ícone do coração, faz uma pausa e limpa o ecrã.


O segundo micro:bit, define o grupo de rádio com o mesmo número 255. Usei a opção no rádio receivedString. Testo se a string recebido é "1", então, mostro o número 2, faço uma pausa e envio a string "2".

Assim, quando agito o primeiro micro:bit, o segundo micro:bit deve mostrar o número 2.

O terceiro micro:bit, define o grupo de rádio com o mesmo número 255. Quando receber a string "2", mostra os leds em forma de "coração", envia a string "heart". faz uma pausa e limpa o ecrã.
