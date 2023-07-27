---
parent: Componentes e Ferramentas  # Título da página pai como definido no index.md
nav_order: 20  # Ordem que vai aparecer no menu à esquerda
title: Ponte H  # O que vai aparecer no menu à esquerda
has_children: false  # Se possui sub-páginas
---
# 


# Estudo sobre Ponte H 
## Índice
1. [Introdução](#Introdução)
2. [Modelos](#Modelos)
3. [Prós e contras](#Prós-e-contras)
4. [Guia de uso](#Guia-de-uso)
5. [Cuidados](#Cuidados)
6. [SMD](#SMD)


## Introdução 

As pontes H são circuitos eletrônicos que permitem que um motor DC (Corrente Contínua) possa girar em ambas as direções, horária e anti-horária. São chamadas de "pontes H" por causa da típica configuração do esquema eletrônico, que se assemelha a uma letra "H".

Esses circuitos são muito utilizados em robótica e em qualquer sistema que necessite controlar o sentido de rotação de motores de corrente contínua. Uma ponte H é composta geralmente por 4 interruptores (transistores, relés ou outros dispositivos semelhantes) que, ao serem acionados corretamente, permitem alterar o sentido da corrente que passa pelo motor.

As pontes H são fundamentais em muitos dispositivos do dia a dia, desde brinquedos a automóveis. Existem diversos modelos de pontes H, desde os mais simples até os mais complexos, com capacidades para suportar diferentes voltagens e correntes. Além disso, algumas pontes H incorporam características adicionais como proteção contra sobrecarga, circuitos de controle PWM (Pulse Width Modulation) para controle de velocidade e até mesmo capacidade para fornecer feedback sobre o estado atual do motor.

As pontes H de pequeno porte são especificamente projetadas para lidar com motores de baixa potência, normalmente usados em pequenos robôs ou brinquedos. Estes componentes são compactos, eficientes e muitas vezes projetados para serem facilmente integrados com microcontroladores como o Arduino.

Portanto, entender as pontes H e suas aplicações é fundamental para o projeto e a construção de sistemas que requerem controle de motores de corrente contínua. Seja em uma escala menor, como em brinquedos controlados por rádio, ou em uma escala maior, como em veículos elétricos, a ponte H é uma peça fundamental da engenharia eletrônica moderna.

## Modelos 

### L298N
O modelo mais comumente vendido de ponte H para uso em Arduino é o L298N porém não costumamos ultiliza-la nos projetos a mais de 6 anos.  Está pornte h é excessivamente grande e possui muita perda de potencia em forma de calor, além de não possuir vantagens econômicas em relação as outras.

### DRV8833
É uma ótima opção pequena e barata, conseguimos comprar da china por 3 reais e no Brasil por 25, sua maior limitação esta na tensão entre  2,7 a 10,8 volts porém usualmente conseguimos usar até 12v.

### TB6612
É uma opção melhor em relação a DVR8833 pois trabalha com uma tensão de até 13,5V. Mas seu custo é 3x maior na china por volta de 7 reais e aqui no Brasil quase 5x mais caro chegando a 70 reais.

### TB9051FTG
É uma ponte H muito boa que foi importada da Pololu para o seguidor de linha, possui feedback de corrente, trabalha em uma boa faixa de tensão, a melhor que já usamos, mas seu custo de compra e de importação ficam muito longe de justificar o seu uso.
  
 

| Característica | L298N | TB6612 | DRV8833 | TB9051FTG |
|---------------|-------|--------|---------|-----------|
| Tensão de Operação (V) | 5 - 35 | 2.7 - 5.5 | 2.7 - 10.8 | 4.5 - 28 |
| Corrente de Pico por Canal (A) | 2 (até 3 por curto período) | 1.2 (até 3.2 por curto período) | 1.5 (até 2 por curto período) | 5 (até 6 por curto período) |
| Corrente Contínua por Canal (A) | ~2 | ~1.2 | ~1.5 | ~2.6 |
| Número de Canais | 2 | 2 | 2 | 1 |
| Modulação por Largura de Pulso (PWM) | Sim | Sim | Sim | Sim |
| Proteção Térmica | Não | Sim | Sim | Sim |
| Indicador de Erro | Não | Não | Não | Sim |
| Regulação de Corrente | Não | Não | Sim | Não |
| Modo de Standby/Desligamento | Não | Sim | Sim | Sim |
| Proteção contra Inversão de Polaridade | Não | Não | Não | Sim |

# Pros e contras

| Módulo | Prós | Contras |
|--------|------|---------|
| L298N  | Alta tensão de operação. Fácil de usar e bastante popular, o que significa muitos recursos e exemplos online. | Comparativamente ineficiente. Não tem proteção térmica. Maior em tamanho comparado aos outros módulos. |
| TB6612 | Mais eficiente que o L298N. Possui proteção térmica. | Corrente máxima menor que o L298N. |
| DRV8833 | Baixa tensão de operação torna-o ideal para pequenos robôs. Suporta regulação de corrente. | Corrente máxima é menor comparada a outros módulos. |
| TB9051FTG | Alta corrente de pico. Possui indicador de erro e proteção contra inversão de polaridade. | Possui apenas um canal, enquanto os outros possuem dois.|
