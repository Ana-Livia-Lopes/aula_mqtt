# aula_mqtt
README - MQTT Publisher e Subscriber

Requisitos:
  Antes de executar os scripts, certifique-se de ter o Python instalado em seu sistema. Além disso, será necessário instalar a biblioteca paho-mqtt.

Instalação do MQTT:
  Execute o seguinte comando para instalar a biblioteca necessária ->
pip install paho-mqtt

Descrição dos Arquivos:
  publisher.py: Publica mensagens em um tópico MQTT.
  subscriber.py: Inscreve-se em um tópico MQTT e recebe mensagens publicadas nele.

Configuração do Ambiente
  Os scripts utilizam o broker público HiveMQ ("broker.hivemq.com") na porta 1883.
O tópico MQTT usado nesse projeto é senai/dev.

Como Testar:
  1. Executar o Subscriber:
Abra um terminal e execute ->
python subscriber.py
Isso inscreverá o cliente no tópico e aguardará mensagens.
  2. Executar o Publisher
Em outro terminal, execute ->
python publisher.py
  Digite mensagens e pressione Enter para publicá-las no tópico.

3. Verificar a Comunicação
As mensagens enviadas pelo publisher.py devem aparecer no terminal onde o subscriber.py está sendo executado.
