Aqui está um README.md para o seu projeto Arduino. Ele explica de forma clara o que o código faz, como funciona e como montar:


---

🚗 Sistema de Controle com Sensor Ultrassônico, Motor e Buzzer

Este projeto utiliza um Arduino, um sensor ultrassônico HC-SR04, motores DC com ponte H, LEDs e um buzzer para criar um sistema de detecção de distância com resposta sonora e visual.

Quando um objeto é detectado a uma certa distância, o sistema ativa motores, LEDs e buzzer de acordo com a lógica programada.
Além disso, há um botão que liga/desliga o sistema.


---

⚙️ Funcionalidades

Botão de Liga/Desliga: Ativa ou desativa todo o sistema.

Sensor Ultrassônico: Mede a distância de obstáculos em centímetros.

Controle de Motores: Ajusta a direção e velocidade dos motores conforme a distância detectada.

Alerta Sonoro: O buzzer emite som quando o objeto está muito próximo.

Sinalização Visual:

LED Vermelho acende quando o objeto está perto.

LED Verde acende quando o caminho está livre.




---

🔧 Componentes Utilizados

1x Arduino Uno

1x Sensor Ultrassônico HC-SR04

2x Motores DC (controlados pela ponte H)

1x Módulo Ponte H (L298N ou similar)

1x Buzzer

1x Botão (com resistor pull-up interno)

1x LED Vermelho

1x LED Verde

Jumpers e protoboard



---

📌 Ligações Principais

HC-SR04

Trigger → pino 5

Echo → pino 3


Ponte H / Motores

IN1 → pino 6

IN2 → pino 11

IN3 → pino 9

IN4 → pino 10

ENA → pino 2


Buzzer → pino 8

Botão → pino 7 (com INPUT_PULLUP)

LED Vermelho → pino 4

LED Verde → pino 12



---

📊 Lógica de Funcionamento

Objeto entre 0 e 30 cm

Buzzer toca (alarme).

LED vermelho acende.

Motores giram em uma direção com potência média.


Objeto entre 30 e 40 cm

(Espaço reservado – pode adicionar lógica personalizada).


Objeto entre 40 e 100 cm

Buzzer desligado.

LED verde aceso.

Motores giram em outra direção.


Sistema Desligado (botão)

Motores desligados.

Buzzer e LEDs apagados.




---

▶️ Como Usar

1. Monte o circuito conforme os pinos acima.


2. Carregue o código no Arduino via Arduino IDE.


3. Pressione o botão para ligar/desligar o sistema.


4. Aproximando objetos do sensor, observe a resposta dos motores, LEDs e buzzer.




---

📽️ Demonstração

👉 (Aqui você pode inserir fotos ou vídeos do protótipo em funcionamento no futuro)


---

📜 Licença

Este projeto é livre para uso educacional e pessoal.


---

Quer que eu escreva também uma seção de “Possíveis Melhorias” no README, com ideias como PWM progressivo conforme distância, ou integração com display LCD para mostrar os centímetros?

