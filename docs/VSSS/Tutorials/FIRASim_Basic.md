# Instalação e execução do FIRASim

## Introdução

FIRASim é o Software oficial de simulação de partidas virtuais da VSSS Brasil, e, utilizado juntamente com o Docker, permite que equipes compitam virtualmente à distância.

O Software foi desenvolvido no **Ubuntu 18.04**, escrito em C++ e feito pela equipe de competição RoboCin.

O repositório contendo o código fonte e os manuais de instalação estão contidos no [repositório original do FIRASim](https://github.com/robocin/FIRASim).

**Atenção: As instruções de instalação contidas nesse documento são uma versão resumida e traduzida das instruções contidas no repositório original. Caso o seu sistema operacional seja MAC OS, busque a opção de baixar alguma dependência através de seu source code. Caso tenha tido algum problema com este guia, vá para o material original e siga suas instruções.**

## Requisitos de sistema
  
O FIRASim foi desenvolvido e testado em **Ubuntu 18.04**, mas é capaz de compilar e rodar em sistemas Windows, Linux e MacOS, de 32 e 64 bits. 

Caso seja usuário Linux, é importante que o driver de sua placa de vídeo esteja devidamente instalado. Seguem os guias oficiais de instalação para: [NVIDIA](https://docs.nvidia.com/datacenter/tesla/tesla-installation-notes/index.html) e [AMD](https://www.amd.com/en/support/kb/faq/gpu-643)

## Dependências 
  
O FIRASim depende de: 
  
- [C++](https://en.cppreference.com/w/)
- [CMake](https://cmake.org/) version 3.5+
- [OpenGL](https://www.opengl.org)
- [Qt5 Development Libraries](https://www.qt.io)
- [Open Dynamics Engine (ODE)](http://www.ode.org)
- [VarTypes Library](https://github.com/jpfeltracco/vartypes) forked from [Szi's Vartypes](https://github.com/szi/vartypes)
- [Google Protobuf 3](https://github.com/google/protobuf)
- [Boost development libraries](http://www.boost.org/) (needed by VarTypes)

## Instalação em Ubuntu
  
Primeiramente, abra um terminal e instale as dependências já citadas:

```bash 
sudo apt-get install git build-essential cmake qt5-default libqt5opengl5-dev libgl1-mesa-dev libglu1-mesa-dev libprotobuf-dev protobuf-compiler libode-dev libboost-dev 
 ``` 
 
 Compile e instale VartTypes de seu source, usando git:
  
 ```bash 
 $ cd /tmp 
 $ git clone https://github.com/jpfeltracco/vartypes.git 
 $ cd vartypes 
 $ mkdir build 
 $ cd build 
 $ cmake .. 
 $ make 
 $ sudo make install 
 ``` 
  
Clone o FIRASim para o diretório de sua preferência.

 ```bash 
 $ cd /path/to/firasim_ws 
 $ git clone https://github.com/robocin/FIRASim.git 
 $ cd FIRASim 
 ``` 
 
 Crie um diretório dentro da pasta do projeto chamado "build" (Ignorado pelo gitignore) e entre nela:
  
 ```bash
 $ mkdir build 
 $ cd build 
 ``` 
 
 Execute o Cmake dentro de 'build' para gerar a makefile
  
 ```bash 
 $ cmake .. 
 ``` 
 
 Compile o programa:
  
 ```bash 
 $ make 
 ``` 
 
 O binário(Executável) é copiado para a pasta '../bin' depois de ter compilado o código.
 
 Para rodar o programa, execute-o como qualquer outro programa em C('./FIRASim' dentro da pasta do binário), ou, mais recomendado, dentro da pasta 'build' inserir no terminal './../bin/FIRASim'.
 
 Podes executar o programa com algumas flags, sendo elas e suas utilidades:
 - "-H": para rodar o software sem a interface gráfica;
 - "-atkfault": para ativar a detecção de dois robôs adversários dentro da áre
 - "-xlr8": para usar uma função mais rápida e menos precisa da ODE
