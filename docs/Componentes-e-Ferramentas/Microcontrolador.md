---
parent: Componentes e Ferramentas  # Título da página pai como definido no index.md
nav_order: 20  # Ordem que vai aparecer no menu à esquerda
title: Microcontrolador  # O que vai aparecer no menu à esquerda
has_children: false  # Se possui sub-páginas
---

# Comparação entre Arduino Uno, Arduino Nano, ESP32 e ESP8266


Os microcontroladores são pequenos computadores em um único chip. Eles contêm processadores, memória e interfaces de entrada/saída (I/O). Estes são usados em muitos produtos eletrônicos, pois são pequenos, baratos e consomem pouca energia. Por exemplo, o ATmega328P é o microcontrolador encontrado no Arduino Uno e Nano, enquanto o ESP32 e o ESP8266 são os microcontroladores nas suas respectivas placas.

Os kits de desenvolvimento, também conhecidos como devkits, são placas que contêm um microcontrolador e uma variedade de componentes adicionais que facilitam o uso do microcontrolador. Estes podem incluir reguladores de voltagem, osciladores, interfaces USB, GPIOs (General Purpose Input/Output) e outras interfaces de I/O, e até mesmo funcionalidades de comunicação sem fio, como WiFi e Bluetooth no caso dos devkits do ESP32 e ESP8266.

Ao projetar um produto final, é possível usar somente o microcontrolador. No entanto, os devkits são especialmente úteis para o desenvolvimento e a prototipagem, pois simplificam o processo de configuração e uso do microcontrolador.

Agora, vamos dar uma olhada mais detalhada nos diferentes microcontroladores e seus kits de desenvolvimento.

## Comparação entre os diferentes microcontroladores e devkits

| Propriedade | Arduino Uno | Arduino Nano | ESP32 | ESP8266 |
| :--------: | :---------: | :----------: | :---: | :-----: |
| Microcontrolador | ATmega328P | ATmega328P | ESP32 | ESP8266 |
| Clock Speed | 16 MHz | 16 MHz | Até 240 MHz | 80 MHz |
| Memória Flash | 32 KB | 32 KB | Externa (varia com o módulo) | Externa (varia com o módulo) |
| SRAM | 2 KB | 2 KB | 520 KB | 160 KB |
| EEPROM | 1 KB | 1 KB | Não possui (emulação via Flash) | Não possui (emulação via Flash) |
| GPIOs | 14 | 14 | 34 | 16 |
| ADC | 6 Canais | 8 Canais | Até 18 Canais | 1 Canal |
| DAC | Não possui | Não possui | 2 Canais | Não possui |
| WiFi | Não | Não | Sim | Sim |
| Bluetooth | Não | Não | Sim | Não |
| Preço no Brasil |  |  |  |  |
| Preço na China (AliExpress) |  |  |  |  |

## Microcontroladores e suas propriedades

### Arduino Uno

![Arduino Uno](https://www.arduino.cc/en/uploads/Main/ArduinoUno_R3_Front_450px.jpg)

O Arduino Uno é talvez a placa Arduino mais usada devido à sua grande compatibilidade e facilidade de uso. É baseado no microcontrolador ATmega328P.

- **Preço no Brasil:** 
- **Preço na China (AliExpress):** 

#### Especificações

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

### Arduino Nano

![Arduino Nano](https://www.arduino.cc/en/uploads/Main/ArduinoNanoFront_3_lg.jpg)

O Arduino Nano é uma versão compacta do Arduino Uno, tornando-o uma escolha adequada para projetos que exigem um fator de forma menor.

- **Preço no Brasil:** 
- **Preço na China (AliExpress):** 

#### Especificações

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

### ESP32

![ESP32](https://www.espressif.com/sites/default/files/product/esp32/overview/esp32-pico-d4_main.jpg)

O ESP32 é um microcontrolador com Wi-Fi e Bluetooth integrados, tornando-o uma escolha popular para projetos IoT.

- **Preço no Brasil:** 
- **Preço na China (AliExpress):** 

#### Especificações

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

### ESP8266

![ESP8266](https://www.espressif.com/sites/default/files/product/esp-wroom-02/overview/esp-wroom-02-wifi-module.jpg)

O ESP8266 é um microcontrolador com capacidades Wi-Fi integradas. É amplamente utilizado em projetos IoT devido ao seu baixo custo e recursos.

- **Preço no Brasil:** 
- **Preço na China (AliExpress):** 

#### Especificações

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

## Conclusão

Esperamos que este guia tenha ajudado você a entender melhor as diferenças entre o Arduino Uno, Arduino Nano, ESP32 e ESP8266, bem como a diferença entre um microcontrolador e um kit de desenvolvimento. Cada um desses microcontroladores e kits de desenvolvimento tem seus próprios pontos fortes, e a escolha entre eles depende das suas necessidades específicas para o seu projeto.

