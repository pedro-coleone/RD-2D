# Guia de instalação helios-base

ATENÇÃO: Esse é um guia básico para instalação do repositório, para mais informações sobre a configuração e resoluções de possíveis problemas acesse e leia atentamente os links dispostos durante o guia.

## Instalações necessárias

Utilizando Ubuntu 16.04 ou superior, começe instalando as seguintes bibliotecas:

```
sudo apt update
sudo apt install build-essential libboost-all-dev
```

Depois disso, é necessário instalar a librcsc, que pode ser encontrada no seguinte link: https://github.com/helios-base/librcsc

Primeiro, clone o repositório com o comando:

```
git clone https://github.com/helios-base/librcsc.git
```

Após isso, instale as dependências necessárias:

```
sudo apt update
sudo apt install build-essential libboost-all-dev autoconf automake libtool
```

Agora, é necessário fazer a build da biblioteca:

```
./bootstrap
./configure --disable-unit-test
make
```

Finalmente, utilize o comando para completar a instalação da librcsc no local padrão:

```
sudo make install
```

## Clonando o repositório

O repositório pode ser acessado no seguinte endereço: https://github.com/Red-Dragons-UFSCar/2D-RCSS

E, para clonar na sua máquina use o seguinte código:

```
git clone https://github.com/Red-Dragons-UFSCar/2D-RCSS.git
```

## Build e run

Agora, vamos ao repositório helios, onde iremos fazer a build:

```
./bootstrap
./configure
make
```

Após isso, o código pode ser rodado através do seguinte script:

```
./start.sh
```