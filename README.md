
# BlueGuard: Monitoramento Ambiental em Tempo Real com Arduino e LCD
O BlueGuard é um sistema de monitoramento ambiental que utiliza um Arduino para coletar dados de temperatura, umidade e luminosidade em tempo real. Os dados são exibidos em um display LCD, facilitando o acompanhamento das condições do ambiente. Este projeto é ideal para monitorar ambientes internos, como casas, estufas, laboratórios, entre outros.

# Funcionalidades
- Monitoramento de Temperatura: Mede a temperatura do ambiente usando um sensor DHT22 e exibe no display LCD.
- Monitoramento de Umidade: Mede a umidade relativa do ar usando o sensor DHT22 e exibe no display LCD.
- Monitoramento de Luminosidade: Mede a intensidade da luz ambiente usando um LDR (Light Dependent Resistor) e exibe no display LCD.
- Alertas: Exibe mensagens de alerta no display LCD quando a temperatura ou umidade ultrapassam os limites definidos.

# Hardware Necessário
- Arduino Uno (ou compatível)
- Sensor DHT22 (temperatura e umidade)
- LDR (sensor de luz)
- Display LCD I2C 16x2
- Resistor (para o LDR)
- Jumpers

# Bibliotecas Utilizadas
- LiquidCrystal_I2C: Para controlar o display LCD I2C.
- DHT: Para ler os dados do sensor DHT22.
- Wire: Para comunicação I2C com o display LCD.

# Esquema de Conexão
Arduino     DHT22      LCD I2C     LDR
-------     -------     -------     ---
5V          VCC        VCC        -
GND         GND        GND        GND
2 (D2)       DATA       SDA        -
A0          -          SCL        Sinal
-           -          -          VCC (via resistor)

# Instruções de Uso
1. Conecte os componentes conforme o esquema de conexão.
2. Instale as bibliotecas LiquidCrystal_I2C e DHT no Arduino IDE.
3. Carregue o código sketch.ino no Arduino.
4 .Observe os valores de temperatura, umidade e luminosidade no display LCD.
5. Verifique as mensagens de alerta caso os limites sejam ultrapassados.

# Personalização
Você pode ajustar os valores de okThreshold e alertThreshold no código para definir os limites de luminosidade desejados.
Você pode personalizar as mensagens exibidas no display LCD.
Simulação
Você pode simular o projeto no Wokwi usando o link: https://wokwi.com/projects/396275444597834753

# Próximos Passos
Expandir o projeto: Adicione outros sensores para monitorar diferentes parâmetros ambientais (qualidade do ar, CO2, etc.).
Conectar à internet: Envie os dados para a nuvem para monitoramento remoto e análise.
Criar um sistema de alerta: Envie notificações por e-mail ou SMS quando os limites forem ultrapassados.

# Equipe
- Bento Rangel - RM559124 
- Daniel Vieira - RM556275
