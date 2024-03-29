---
parent: VSSS
nav_order: 20
---
# Instalação e execução do SSL Vision  

## Introdução  

No passado, as regras da RoboCup Small Size League permitiam que cada equipe configurasse o seu próprio sistema de visão global como um sensor primário. Esta opção trouxe várias limitações organizacionais e custos para as equipes, prejudicando o andamento do campeonato. Além disso, a maioria das equipes convergiu para soluções semelhantes e produziu poucos resultados de pesquisa significativos para esse problema de visão global nos últimos anos.

Em 2009, os comitês da liga decidiram migrar para um sistema de visão compartilhada (incluindo hardware) que pudesse ser usado por todos os times. Este sistema - denominado SSL-Vision - é atualmente desenvolvido por voluntários das equipes participantes. Foi desenvolvido somente para Linux.

Esse é um guia básico de instalação e execução do software. Caso tenha algum problema de incompatibilidade/execução, visite [**requirements**](https://github.com/RoboCup-SSL/ssl-vision/wiki/requirements) na wiki do repositório original. 

  **Repositório original do SSL Vision:** https://github.com/RoboCup-SSL/ssl-vision

 
## Guia de instalação

### Sistemas Operacionais

O software foi desenvolvido para Linux, com a distribuição de referência **Ubuntu 20.04 LTS**.
### Obtendo o SSL Vision
Para obter a versão mais atualizada usando git:

```bash
git clone https://github.com/RoboCup-SSL/ssl-vision.git
```

### Instalando dependências

Ubuntu/Debian a partir de 22.04 (pacote libdc1394-22 não utilizado nessas versões):
```bash
apt-get install -qq g++ qtdeclarative5-dev libqt5multimedia5 libeigen3-dev protobuf-compiler libprotobuf-dev cmake libv4l-0 libopencv-dev freeglut3-dev
```

Ubuntu/Debian 21.10 e anteriores: `./InstallPackagesUbuntu.sh`
    
Archlinux: `./InstallPackagesArch.sh`

### Compilação
Após verificar o código, o programa pode ser compilado com: `make`

### Execução
Após compilar com sucesso, haverão os três binários dentro do diretório `./bin` , que devem ser executados a partir do root do repositório:

-   `./bin/vision`   - SSL-Vision application
-   `./bin/client`  - Simple sample client
-   `./bin/graphicalClient` - Graphical sample client
