## Integrantes:
Leonardo Fernandes Mesquita, RM:559623
https://github.com/leoGitFiap
Marco Antonio Caires Freire, RM:559256
https://github.com/MACF77
Guilherme Augusto Caseiro, RM:559765
https://github.com/Guiitens2005

# Projeto: Sistema de Monitoramento de Ambiente com IoT

##  Objetivo do Projeto
Desenvolver uma solução de Edge Computing capaz de monitorar condições ambientais (temperatura, umidade, luminosidade) usando sensores conectados a microcontroladores. Os dados serão processados localmente e enviados para uma plataforma de IoT no back-end, sendo visualizados por meio de um aplicativo web.

##  Especificações Técnicas dos Componentes
- **Microcontrolador**: ESP32
- **Sensores**:
  - DHT22 (Temperatura e Umidade)
  - LDR (Sensor de Luminosidade)
- **Atuadores**:
  - LED indicador de condição crítica
- **Back-end**:
  - Plataforma IoT: ThingsBoard / AWS IoT / Node-RED
- **Aplicação (Front-end)**:
  - Web App responsivo usando React.js para visualização dos dados.
  
##  Arquitetura em Camadas

### 1. IoT (Dispositivos)
- **Microcontrolador**: ESP32 responsável pela coleta e envio dos dados.
- **Sensores**: Capturam informações do ambiente.
- **Atuadores**: Reagem a determinadas condições (ex.: acionar LED).

### 2. Back-end (Plataforma IoT)
- **Recebe e armazena dados**.
- **Gerencia dispositivos**.
- **Fornece APIs para integração**.

### 3. Aplicação (Front-end)
- **Dashboard Web**: Interface gráfica para monitoramento em tempo real dos dados coletados.
- **Notificações**: Alertas visuais no app para condições fora dos parâmetros.

##  Descrição do Diagrama

O diagrama apresenta três camadas:
- **IoT Layer**: Microcontrolador conectado a sensores e atuadores.
- **Back-end Layer**: Plataforma que recebe os dados, armazena, e provê API REST.
- **Application Layer**: Aplicativo Web que consome as APIs e exibe as informações ao usuário.

O fluxo principal é:
1. Sensores captam dados - 2. Microcontrolador processa e envia - 3. Back-end armazena e disponibiliza - 4. Aplicativo exibe as informações.

---

Link do Wokwi: https://wokwi.com/projects/429593279758081025
