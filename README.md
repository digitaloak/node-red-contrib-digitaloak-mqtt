### MQTT input node & MQTT unsubscibe
Based on core Node-RED "mqtt in" and "mqtt-broker" nodes. 

#### Known use case
Keep REST API req/res sync when doing async work

#### Description
digitaloak-mqtt-in allows you subscribe dynamically to different topics via msg.topic and output msgs from subscribed topics.
digitaloak-mqtt-unsubscribe allows you to manually unsubscribe from topic.

When box checked "Unsubscribe from topic after first message received" for digitaloak-mqtt-in, node will immediately unsubscribe after receiving first msg. If you want uncheck this option, use digitaloak-mqtt-unsubscribe to unsubscribe manually.

Example is available here: https://flows.nodered.org/flow/3003f194750b0dec19502e31ca234847

#### Installation (Node-RED in docker)
1. Go to Node-RED modules directory - /data/node_modules
2. Run `git clone git@github.com:digitaloak/node-red-contrib-digitaloak-mqtt.git`
3. `cd node-red-contrib-digitaloak-mqtt`
4. `npm install`
5. Restart Node-RED
 

