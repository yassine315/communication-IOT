# communication-IOT
<h1>prerequit<h1>
  <p> installer le broker mosquitto clicker <a href="https://mosquitto.org/download/"> ici</a> pour le faire</p>
  <h1>explication</h1>
<p><b>le projet contien deux fichiers un pour l'envoi 'publish.py' et l'autre pour recevoir 'recevoire_ESP' :</b><p>
  <h5>publish.py</h5>
  <p>pour   se connecter au broker : <kbd>mqttc.connect("localhost", 1883, 60)</kbd></p>
  <p>pour envoyer le message msg au topic 'esp/test' on utilise <kbd> mqttc.publish("esp/test", msg, qos=2)</kbd></p>
  <h5>recevoire_ESP</h5>
  <p>on s'ubscribe au topic avec <kbd>client.subscribe("esp/R1");</kbd></p>
  <p>on recupere les message qui sont dans le proker avec <kbd>client.setCallback(callback);</kbd>
    
