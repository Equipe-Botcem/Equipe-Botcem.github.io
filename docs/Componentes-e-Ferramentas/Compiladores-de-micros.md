---
parent: Componentes e Ferramentas  # Título da página pai como definido no index.md
nav_order: 20  # Ordem que vai aparecer no menu à esquerda
title: Compiladores de Micros  # O que vai aparecer no menu à esquerda
has_children: false  # Se possui sub-páginas
---

# Guia Completo de Ambiente de Desenvolvimento para Arduino e ESP32

Neste guia iremos discutir os dois principais ambientes que ultilizamos para programar microcontroladores. Já adiantando que o PlatformIo é fortemente recomendado para uso na equipe junto com o Vscode e Github. 

## Índice

1. [Comparação entre Arduino IDE e PlatformIO](#comparação-entre-arduino-ide-e-platformio)
2. [Instalação e Configuração](#instalação-e-configuração)
    - [Visual Studio Code](#visual-studio-code)
    - [PlatformIO](#platformio)
    - [GitHub](#github)
    - [Arduino IDE](#arduino-ide)

## Comparação entre Arduino IDE e PlatformIO

Ao desenvolver projetos com Arduino ou ESP32, você pode escolher usar a Arduino IDE ou o PlatformIO. Ambos têm suas vantagens e desvantagens.

### Arduino IDE

1. **Facilidade de uso:** Arduino IDE tem uma interface de usuário mais simples e é mais fácil para iniciantes.
2. **Compatibilidade:** Suporta todas as placas Arduino e algumas outras placas compatíveis.
3. **Código aberto:** Arduino IDE é software livre e de código aberto.
4. **Menos recursos:** Comparado ao PlatformIO, o Arduino IDE tem menos recursos avançados.

### PlatformIO

1. **Integração com VS Code:** PlatformIO é integrado ao Visual Studio Code, o que proporciona um ambiente de desenvolvimento mais avançado e completo.
2. **Facilidade para encontrar bibliotecas:** PlatformIO tem uma ferramenta embutida para pesquisar e instalar bibliotecas, o que facilita bastante o processo.
3. **Suporte a múltiplas placas e plataformas:** PlatformIO suporta mais de 30 plataformas diferentes, incluindo Arduino e ESP32.
4. **Controle de versão:** Tem integração com Git e outras ferramentas de controle de versão.
5. **Dependências de gerenciamento:** PlatformIO tem um sistema para gerenciar dependências de bibliotecas e frameworks.
6. **Recursos avançados do VS Code:** Como é integrado ao VS Code, você pode aproveitar todos os plugins e ferramentas disponíveis nesse editor.

## Instalação e Configuração

### Visual Studio Code

O Visual Studio Code é um editor de código leve mas poderoso disponível para Windows, MacOS e Linux. 

#### Como instalar o Visual Studio Code

1. Acesse o [site oficial do Visual Studio Code](https://code.visualstudio.com/).
2. Clique em "Download" e escolha o sistema operacional correto.
3. Siga as instruções de instalação na tela.

### PlatformIO

PlatformIO é uma plataforma de desenvolvimento open-source para IoT.

#### Como instalar e configurar o PlatformIO

1. Abra o Visual Studio Code.
2. Clique na aba "Extensions" ou use o atalho `Ctrl + Shift + X`.
3. Na barra de pesquisa, digite "PlatformIO" e pressione `Enter`.
4. Clique em "Install" no cartão PlatformIO IDE.
5. Após a instalação, o PlatformIO IDE aparecerá na barra lateral. Clique nele.
6. Você pode criar um novo projeto clicando em "New Project" ou importar um projeto existente clicando em "Open Project".
7. Ao criar um novo projeto, você precisa selecionar a placa e o framework.

### GitHub

O GitHub é uma plataforma de hospedagem de código-fonte com controle de versão usando git.

#### Como instalar e configurar o GitHub no Visual Studio Code

1. Acesse o [site do GitHub](https://github.com/).
2. Crie uma conta ou faça login na sua conta existente.
3. No Visual Studio Code, abra a aba "Extensions" ou use o atalho `Ctrl + Shift + X`.
4. Pesquise "GitHub" na barra de pesquisa e instale a extensão "GitHub Pull Requests and Issues".
5. Depois de instalada, abra a aba "Source Control" ou use o atalho `Ctrl + Shift + G`.
6. Clique em "Clone Repository" se quiser trabalhar em um repositório existente, ou em "Initialize Repository" para começar um novo projeto.
7. Siga as instruções na tela para configurar o GitHub.
8. Você pode fazer commit, push e pull diretamente do Visual Studio Code. As solicitações pull e questões do GitHub também são integradas.

### Arduino IDE

O Arduino IDE é um ambiente de desenvolvimento integrado open-source criado pela Arduino.

#### Como instalar o Arduino IDE

1. Acesse o [site oficial do Arduino](https://www.arduino.cc/en/Main/Software).
2. Clique em "Download" e escolha o sistema operacional correto.
3. Siga as instruções de instalação na tela.

---

Esperamos que este guia tenha ajudado a entender as diferenças entre Arduino IDE e PlatformIO e a instalar e configurar o Visual Studio Code, PlatformIO, GitHub e Arduino IDE. Se você tiver alguma dúvida, sinta-se à vontade para perguntar!


@André Luís C Barbado - Oz
