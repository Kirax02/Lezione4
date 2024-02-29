Quando un dispositivo, in questo caso il laptop-PT0 (192.168.100.100), invia uno o piu pacchetti ad un altro dispositivo situato in un altra rete, in questo caso il laptop-PT2 (192.168.200.100) succede che il pacchetto parte dal laptop e arriva nello switch che lo instrada al router utilizzando il MAC address (layer 2 del modello ISO/OSI) poi il router controlla la sua tabella di routing e instrada il pacchetto ad uno switch presente nella rete dell'IP address di destinazione (layer 3 del modello ISO/OSI) e in fine lo switch instrada il pacchetto al laptop di destinazione sempre utilizzando il MAC address. Invece se ci dobbiamo collegare ad un servizio il pacchetto avra anche il layer 4 del modello ISO/OSI ovvero quello del trasporto che utilizza dei protocolli, i piu fondamentali sono il TCP e l'UDP, quindi l'header del pacchetto oltre ad avere l'IP di destinazione che identifica la macchina avrà anche la porta di destinazione che identifica il servizio che verra utilizzato. Esempio se con il laptop-PT0 noi ci collegassimo al server0 (192.168.200.101) una volte che il router avra instradato il pacchetto allo switch appartente alla rete del server, lo switch controllera la porta di destinazione che in questo caso è la porta 80.
