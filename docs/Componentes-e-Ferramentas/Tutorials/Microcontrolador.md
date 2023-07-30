---
parent: Componentes e Ferramentas  # Título da página pai como definido no index.md
nav_order: 20  # Ordem que vai aparecer no menu à esquerda
title: Microcontrolador  # O que vai aparecer no menu à esquerda
has_children: false  # Se possui sub-páginas
---
# Comparação entre Arduino Uno, Arduino Nano, ESP32 e ESP8266

Os Arduino Uno, Arduino Nano, ESP32 e ESP8266 são algumas das placas de microcontroladores mais populares utilizadas para o desenvolvimento de projetos IoT. Eles diferem em vários aspectos, desde suas especificações técnicas até seus preços.

## Arduino Uno

![Arduino Uno](https://www.arduino.cc/en/uploads/Main/ArduinoUno_R3_Front_450px.jpg)

O Arduino Uno é talvez a placa Arduino mais usada devido à sua grande compatibilidade e facilidade de uso. É baseado no microcontrolador ATmega328P.

- **Preço no Brasil:** 
- **Preço na China (AliExpress):** 

### Especificações

- Microcontrolador: ATmega328P
- Tensão operacional: 5V
- Entradas/saídas digitais I/O: 14 (das quais 6 fornecem saída PWM)
- Entradas analógicas: 6
- Corrente DC por I/O Pin: 20 mA
- Corrente DC para Pin de 3.3V: 50 mA
- Memória Flash: 32 KB (ATmega328P) dos quais 0.5 KB são usados pelo bootloader
- SRAM: 2 KB (ATmega328P)
- EEPROM: 1 KB (ATmega328P)
- Velocidade do relógio: 16 MHz

## Arduino Nano

![Arduino Nano](https://www.arduino.cc/en/uploads/Main/ArduinoNanoFront_3_lg.jpg)

O Arduino Nano é uma versão compacta do Arduino Uno, tornando-o uma escolha adequada para projetos que exigem um fator de forma menor.

- **Preço no Brasil:** 
- **Preço na China (AliExpress):** 

### Especificações

- Microcontrolador: ATmega328P
- Tensão operacional: 5V
- Entradas/saídas digitais I/O: 14 (das quais 6 fornecem saída PWM)
- Entradas analógicas: 8
- Corrente DC por I/O Pin: 40 mA
- Corrente DC para Pin de 3.3V: 50 mA
- Memória Flash: 32 KB dos quais 2 KB são usados pelo bootloader
- SRAM: 2 KB
- EEPROM: 1 KB
- Velocidade do relógio: 16 MHz

## ESP32

![ESP32](https://www.espressif.com/sites/default/files/product/esp32/overview/esp32-pico-d4_main.jpg)

O ESP32 é um microcontrolador com Wi-Fi e Bluetooth integrados, tornando-o uma escolha popular para projetos IoT.

- **Preço no Brasil:** 
- **Preço na China (AliExpress):** 

### Especificações

- Dual-core Xtensa® 32-bit LX6
- Até 240MHz de clock
- 520 KB SRAM
- Wi-Fi 802.11 b/g/n
- Bluetooth 4.2 e BLE
- 34 pinos GPIO
- Interfaces de periféricos: SPI, I²C, I²S, UART
- Conversor ADC de 12 bits até 18 canais
- 2 conversores DAC de 8 bits
- 10 sensores touch capacitivos

## ESP8266

![ESP8266](https://www.espressif.com/sites/default/files/product/esp-wroom-02/overview/esp-wroom-02-wifi-module.jpg)

O ESP8266 é um microcontrolador com capacidades Wi-Fi integradas. É amplamente utilizado em projetos IoT devido ao seu baixo custo e recursos.

- **Preço no Brasil:** 
- **Preço na China (AliExpress):** 

### Especificações

- Tensilica L106 32-bit micro controller
- 80 MHz clock speed
- 64 KB de memória de boot ROM
- 64 KB de memória de instrução RAM
- 96 KB de memória de dados RAM
- Memória Flash externa - 16 MB máx.
- IEEE 802.11 b/g/n Wi-Fi
- 16 pinos GPIO
- Interfaces de periféricos - SDIO, SPI, UART
- Conversor ADC de 10 bits

Cada um desses microcontroladores tem suas vantagens e desvantagens, por isso, a escolha entre eles geralmente depende do projeto específico em que você está trabalhando.


# Comparação entre Arduino Uno, Arduino Nano, ESP32 e ESP8266

| Característica | Arduino Uno | Arduino Nano | ESP32 | ESP8266 |
| --- | --- | --- | --- | --- |
| Microcontrolador | ATmega328P | ATmega328P | Xtensa® 32-bit LX6 | Tensilica L106 32-bit |
| Clock Speed | 16 MHz | 16 MHz | Até 240 MHz | 80 MHz |
| SRAM | 2 KB | 2 KB | 520 KB | 96 KB |
| Flash Memory | 32 KB | 32 KB | (External) 16 MB max | (External) 16 MB max |
| GPIO Pins | 14 | 14 | 34 | 16 |
| ADC | N/A | N/A | 12-bit | 10-bit |
| DAC | N/A | N/A | 2x 8-bit | N/A |
| Preço Brasil | - | - | - | - |
| Preço China (AliExpress) | - | - | - | - |

Os preços são variáveis e podem mudar com o tempo e localização, por isso é necessário verificá-los individualmente em cada local.

Para o Arduino Uno e Arduino Nano, as bibliotecas de suporte, a comunidade de código aberto e a facilidade de uso são pontos fortes. O ESP32 e ESP8266, por outro lado, são ótimos para aplicativos IoT devido aos seus recursos integrados de Wi-Fi e (no caso do ESP32) Bluetooth.

