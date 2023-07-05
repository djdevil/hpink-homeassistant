Assicurati di avere Home Assistant e HACS correttamente installati e funzionanti.

Visita la pagina del repository GitHub dell'integrazione HP PRINTER su https://github.com/elad-bar/ha-hpprinter.

Nella scheda "Integrazioni", cerca e installa le dipendenze "Paper Buttons Row" e "browser mod". Segui le istruzioni per l'installazione di queste dipendenze.

Installa l'integrazione tramite HACS e configura la stampante nei dispotivi.

Fai clic sul pulsante verde "Code" e seleziona "Download ZIP" per scaricare il file ZIP dell'integrazione.

Estrai il contenuto del file ZIP in una posizione facilmente accessibile sul tuo computer.

All'interno della cartella estratta, troverai un file chiamato hpink.yaml. Copia questo file.

Apri il file hpink.yaml cerca la seguente riga di codice:


service: notify.mobile_app_iphonedavide
Questa riga di codice specifica il servizio di notifica predefinito utilizzato nell'integrazione hp printer. Per sostituire questo servizio di notifica con il tuo servizio personalizzato, segui questi passaggi:

Sostituisci notify.mobile_app_iphonedavide con il nome del tuo servizio di notifica personalizzato nel seguente formato:

service: notify.nome_del_tuo_servizio_di_notifica

Assicurati di mantenere la struttura notify.nome_del_tuo_servizio_di_notifica e di sostituire correttamente "nome_del_tuo_servizio_di_notifica" con il nome effettivo del tuo servizio di notifica.

Salva il file dopo aver apportato questa modifica. 

Accedi al tuo server Home Assistant e individua la cartella "packages". Di solito si trova nella directory principale di Home Assistant.

Incolla il file hpink.yaml nella cartella "packages".

Riavvia Home Assistant per applicare le modifiche.

Dopo il riavvio, apri l'interfaccia di Home Assistant nel tuo browser e vai alla pagina del frontend.


Nella pagina del frontend, cerca l'entità chiamata "HP Printer Printer" nella lista delle entità disponibili. Dovresti vederla elencata come una delle entità integrate dopo aver installato l'integrazione hp printer tramite HACS.

Importante: Se non vedi l'entità "HP Printer Printer" nell'elenco delle entità, assicurati di aver seguito correttamente i passaggi precedenti e che l'integrazione sia stata installata correttamente.

Una volta individuata l'entità "HP Printer Printer", fai clic su di essa e rinominala in "sensor.hp_envy_5540_total_pages_printed_xml".

Nota: Assicurati di mantenere la struttura "sensor.hp_envy_5540_total_pages_printed_xml" per evitare eventuali problemi di compatibilità con il resto della configurazione.

Salva le modifiche e continua con gli altri passaggi indicati nella guida.

Torna alla tua installazione di HACS in Home Assistant.



Ora, crea o apri il file card.yaml nella vista in cui desideri visualizzare la card dell'integrazione hp printer.

Copia e incolla il codice specificato nel file card.yaml del repository hp printer nella tua vista. Salva il file dopo l'incollaggio.

Riavvia Home Assistant per applicare tutte le modifiche.

Dopo il riavvio, dovresti essere in grado di vedere la card dell'integrazione hp printer nella tua vista specificata. Assicurati di seguire attentamente i passaggi e verificare che tutte le dipendenze siano state correttamente installate.


Per configurare la data di rinnovo dell'abbonamento HP Instant Ink e le informazioni sulle pagine stampate, inclusi i costi aggiuntivi, segui questi passaggi:

Assicurati di aver installato correttamente la card nell'interfaccia di Home Assistant seguendo la guida precedente.

Nella vista in cui hai aggiunto la card dell'integrazione hp printer, cerca l'icona delle impostazioni associata alla card. Di solito è rappresentata da un'icona a forma di ingranaggio o da tre punti verticali.

Fai clic sull'icona delle impostazioni per aprire il pannello di configurazione della card.

All'interno del pannello di configurazione, dovresti trovare opzioni per impostare la data di rinnovo dell'abbonamento HP Instant Ink, il numero di pagine incluse mensilmente, le pagine già stampate e le pagine extra con il relativo costo.

Segui le istruzioni fornite nel pannello di configurazione per inserire le informazioni richieste. Potresti dover inserire le date nel formato corretto, specificare le pagine stampate e i costi associati.

Assicurati di salvare le modifiche apportate nella configurazione della card.

Una volta completati questi passaggi, la card dell'integrazione hp printer visualizzerà le informazioni correttamente configurate, come la data di rinnovo dell'abbonamento, le pagine incluse, le pagine già stampate e le pagine extra con i relativi costi. Sarai in grado di visualizzare e monitorare queste informazioni direttamente nella vista di Home Assistant.

Ricorda che le opzioni di configurazione potrebbero variare leggermente a seconda della specifica implementazione della card hp printer che hai installato. Assicurati di leggere attentamente le istruzioni fornite con la card per ottenere una corretta configurazione.


