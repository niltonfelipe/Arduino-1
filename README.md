Núcleo Arduino para chips WiFi ESP8266
===========================================

Este projeto traz suporte para chips ESP8266 para o ambiente Arduino. Ele permite que você escrever esboços usando funções e bibliotecas familiares Arduino, e executá-los diretamente sobre ESP8266, não microcontrolador externo necessário.

ESP8266 Arduino núcleo vem com bibliotecas de se comunicar através de Wi-Fi usando TCP e UDP, configurar HTTP, mDNS, SSDP, e servidores de DNS, faça atualizações OTA, use um sistema de arquivos em memória flash, o trabalho com cartões SD, servos, SPI e periféricos I2C .

### Instando com Boards Manager ###

Começando com 1.6.4, Arduino permite a instalação de pacotes da plataforma de terceiros usando o Gerenciador Boards. Temos pacotes disponível para Windows, Mac OS e Linux (32 e 64 bits).

Instale Arduino 1.6.5 do website Arduino.
Arduino e abra Preferências janela Iniciar.
Digite http://arduino.esp8266.com/stable/package_esp8266com_index.json em *Additional Board Manager URLs* field. Você pode adicionar vários URLs, separando-os com vírgulas.
- Abrir Boards Manager do menu Ferramentas> > Board menu e instalar esp8266 plataforma (e não se esqueça de selecionar sua placa ESP8266 de menu Ferramentas> Board após a instalação).

#### Versões disponíveis

##### Versão estável ![](http://arduino.esp8266.com/stable/badge.svg)
Boards manager link: `http://arduino.esp8266.com/stable/package_esp8266com_index.json`

Documentação:: [Reference](http://arduino.esp8266.com/stable/doc/reference.html)

##### Staging version ![](http://arduino.esp8266.com/staging/badge.svg)
Boards manager link: `http://arduino.esp8266.com/staging/package_esp8266com_index.json`

Documentação: [Reference](http://arduino.esp8266.com/staging/doc/reference.html)


### Construindo versão mais recente da fonte [![Linux build status](https://travis-ci.org/esp8266/Arduino.svg)](https://travis-ci.org/esp8266/Arduino)

```
$ git clone https://github.com/esp8266/Arduino.git
$ cd Arduino/build
$ ant dist
```

Documentação para última versão de desenvolvimento:

- [Reference](hardware/esp8266com/esp8266/doc/reference.md)
- [Supported boards](hardware/esp8266com/esp8266/doc/boards.md)
- [Change log](hardware/esp8266com/esp8266/doc/changes.md)

### Questões e apoio ###

O melhor lugar para fazer perguntas relacionadas a este núcleo é fórum da comunidade ESP8266: http://www.esp8266.com/arduino. Se você encontrar o fórum útil, por favor considerar apoiar-lo com uma doação.
[![Donate](https://img.shields.io/badge/paypal-donate-yellow.svg)](https://www.paypal.com/webscr?cmd=_s-xclick&hosted_button_id=4M56YCWV6PX66)

Se você encontrar um problema, você está convidado a apresentá-lo aqui no Github: https://github.com/esp8266/Arduino/issues. Forneça o máximo possível de contexto: a versão que você está usando (você pode verificá-lo no Fórum Manager), seu código esboço, saída serial, modelo da placa, configurações IDE (seleção bordo, tamanho flash, etc).

### Contributing

Para pequenas correções de código e documentação, vá em frente e envie uma solicitação de recebimento.

Mudanças maiores (reescrever partes do código existente a partir do zero, adicionando novas funções para o núcleo, adicionando novas bibliotecas) geralmente deve ser discutido [no chat](https://gitter.im/esp8266/Arduino) primeiro.

Ramos especiais com lotes de pequenos commits (especialmente intitulado "oops", "fix erro de digitação", "esqueceu-se de adicionar o arquivo", etc.) deve ser esmagado antes de abrir uma solicitação de recebimento. Ao mesmo tempo, por favor, abster-se de colocar várias alterações independentes em uma única solicitação de recebimento.

### License and credits ###

Arduino IDE é desenvolvido e mantido pela equipe de Arduino. O IDE é licenciado sob a GPL.

ESP8266 núcleo inclui um conjunto de ferramentas gcc xtensa, que também está sob a GPL.

Esptool escrito por Christian Klippel é licenciado sob a GPLv2, atualmente mantido por Ivan Grokhotkov: https://github.com/igrr/esptool-ck.

Espressif SDK incluídos nesta compilação está sob Espressif MIT License.

Arquivos principais ESP8266 está licenciado sob a LGPL.

[SPI Flash File System (SPIFFS)](https://github.com/pellepl/spiffs) escrito por Peter Andersson é usado neste projeto. Ele é distribuído sob a licença MIT.
