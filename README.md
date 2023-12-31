<a href="https://www.buymeacoffee.com/divil17F"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=divil17F&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff" /></a>

<a href="https://ibb.co/k9MVgz0"><img src="https://i.ibb.co/k9MVgz0/IMG-9737.png" alt="IMG-9737" border="0"></a> <a href="https://ibb.co/yq2SxYB"><img src="https://i.ibb.co/yq2SxYB/IMG-9738.png" alt="IMG-9738" border="0"></a>

# HP Printer Integration Installation and Configuration Guide for Home Assistant

Assicurati di avere Home Assistant e HACS correttamente installati e funzionanti.

1. Visita la pagina del repository GitHub dell'integrazione HP PRINTER su [https://github.com/elad-bar/ha-hpprinter](https://github.com/elad-bar/ha-hpprinter). E Installa questa integrazione manualmente o tramit HACS

2. Tramite HACS, cerca e installa le dipendenze Frontend "Paper Buttons Row" e "browser mod". Segui le istruzioni per l'installazione di queste dipendenze.

3. Una volta installata l'integrazione tramite HACS  configura la stampante nei dispositivi.

4. Ora scarica il mio codice seleziona "Download ZIP" per scaricare il file ZIP dell'integrazione.

5. Estrai il contenuto del file ZIP in una posizione facilmente accessibile sul tuo computer.

6. All'interno della cartella estratta, troverai un file chiamato hpink.yaml. Copia questo file.

7. Apri il file hpink.yaml e cerca la seguente riga di codice:

   service: notify.mobile_app_iphonedavide

   Questa riga di codice specifica il servizio di notifica predefinito utilizzato nell'integrazione hp printer. Per sostituire questo servizio di notifica con il tuo servizio personalizzato, segui questi passaggi:

8. Sostituisci notify.mobile_app_iphonedavide con il nome del tuo servizio di notifica personalizzato nel seguente formato:

   service: notify.nome_del_tuo_servizio_di_notifica

   Assicurati di mantenere la struttura notify.nome_del_tuo_servizio_di_notifica e di sostituire correttamente "nome_del_tuo_servizio_di_notifica" con il nome effettivo del tuo servizio di notifica.

9. Salva il file dopo aver apportato questa modifica.

10. Accedi al tuo server Home Assistant e individua la cartella "packages". Di solito si trova nella directory principale di Home Assistant.

11. Incolla il file hpink.yaml nella cartella "packages".

12. Riavvia Home Assistant per applicare le modifiche.

13. Dopo il riavvio, apri l'interfaccia di Home Assistant nel tuo browser e vai alla pagina del frontend.

14. Nella pagina del frontend, cerca l'entità chiamata "HP Printer Printer" nella lista delle entità disponibili. Dovresti vederla elencata come una delle entità integrate dopo aver installato l'integrazione hp printer tramite HACS.

   Importante: Se non vedi l'entità "HP Printer Printer" nell'elenco delle entità, assicurati di aver seguito correttamente i passaggi precedenti e che l'integrazione sia stata installata correttamente.

15. Una volta individuata l'entità "HP Printer Printer", fai clic su di essa e rinominala in "sensor.hp_envy_5540_total_pages_printed_xml".

   Nota: Assicurati di mantenere la struttura "sensor.hp_envy_5540_total_pages_printed_xml" per evitare eventuali problemi di compatibilità con il resto della configurazione.

16. Salva le modifiche e continua con gli altri passaggi indicati nella guida.

17. Torna alla tua installazione diHACS in Home Assistant.

18. Ora, crea o apri il file card.yaml nella vista in cui desideri visualizzare la card dell'integrazione hp printer.

19. Copia e incolla il codice specificato nel file card.yaml del repository hp printer nella tua vista. Salva il file dopo l'incollaggio.

20. Riavvia Home Assistant per applicare tutte le modifiche.

21. Dopo il riavvio, dovresti essere in grado di vedere la card dell'integrazione hp printer nella tua vista specificata. Assicurati di seguire attentamente i passaggi e verificare che tutte le dipendenze siano state correttamente installate.

Per configurare la data di rinnovo dell'abbonamento HP Instant Ink e le informazioni sulle pagine stampate, inclusi i costi aggiuntivi, segui questi passaggi:

1. Assicurati di aver installato correttamente la card nell'interfaccia di Home Assistant seguendo la guida precedente.

2. Nella vista in cui hai aggiunto la card dell'integrazione hp printer, cerca l'icona delle impostazioni associata alla card. Di solito è rappresentata da un'icona a forma di ingranaggio o da tre punti verticali.

3. Fai clic sull'icona delle impostazioni per aprire il pannello di configurazione della card.

4. All'interno del pannello di configurazione, dovresti trovare opzioni per impostare la data di rinnovo dell'abbonamento HP Instant Ink, il numero di pagine incluse mensilmente, le pagine già stampate e le pagine extra con il relativo costo.

5. Segui le istruzioni fornite nel pannello di configurazione per inserire le informazioni richieste. Potresti dover inserire le date nel formato corretto, specificare le pagine stampate e i costi associati.

6. Assicurati di salvare le modifiche apportate nella configurazione della card.

Una volta completati questi passaggi, la card dell'integrazione hp printer visualizzerà le informazioni correttamente configurate, come la data di rinnovo dell'abbonamento, le pagine incluse, le pagine già stampate e le pagine extra con i relativi costi. Sarai in grado di visualizzare e monitorare queste informazioni direttamente nella vista di Home Assistant.

Ricorda che le opzioni di configurazione potrebbero variare leggermente a seconda della specifica implementazione della card hp printer che hai installato. Assicurati di leggere attentamente le istruzioni fornite con la card per ottenere una corretta configurazione.



ENGLISH


# HP Printer Integration Installation and Configuration Guide for Home Assistant

Make sure you have Home Assistant and HACS properly installed and functioning.

1. Visit the GitHub repository page for the HP PRINTER integration at [https://github.com/elad-bar/ha-hpprinter](https://github.com/elad-bar/ha-hpprinter).

2. In the "Integrations" tab, search for and install the dependencies "Paper Buttons Row" and "browser mod". Follow the instructions for installing these dependencies.

3. Install the integration through HACS and configure the printer in your devices.

4. Click on the green "Code" button and select "Download ZIP" to download the integration's ZIP file.

5. Extract the contents of the ZIP file to an easily accessible location on your computer.

6. Within the extracted folder, you will find a file named hpink.yaml. Copy this file.

7. Open the hpink.yaml file and locate the following line of code:

   service: notify.mobile_app_iphonedavide
   
   This line of code specifies the default notification service used in the hp printer integration. To replace this notification service with your custom service, follow these steps:

8. Replace notify.mobile_app_iphonedavide with the name of your custom notification service in the following format:

   service: notify.your_notification_service_name
   
   Make sure to maintain the structure notify.your_notification_service_name and replace "your_notification_service_name" with the actual name of your notification service.

9. Save the file after making this modification.

10. Access your Home Assistant server and locate the "packages" folder. It is usually located in the main directory of Home Assistant.

11. Paste the hpink.yaml file into the "packages" folder.

12. Restart Home Assistant to apply the changes.

13. After the restart, open the Home Assistant interface in your browser and navigate to the frontend page.

14. In the frontend page, search for the entity named "HP Printer Printer" in the list of available entities. You should see it listed as one of the integrated entities after installing the hp printer integration through HACS.

   Important: If you do not see the "HP Printer Printer" entity in the list of entities, make sure you have followed the previous steps correctly and that the integration has been installed successfully.

15. Once you locate the "HP Printer Printer" entity, click on it and rename it to "sensor.hp_envy_5540_total_pages_printed_xml".

   Note: Make sure to maintain the structure "sensor.hp_envy_5540_total_pages_printed_xml" to avoid any compatibility issues with the rest of the configuration.

16. Save the changes and continue with the other steps mentioned in the guide.

17. Go back to your HACS installation in Home Assistant.

18. Now, create or open the card.yaml file in the view where you want to display the hp printer integration card.

19. Copy and paste the code specified in the hp printer repository's card.yaml file into your view. Save the file after pasting.

20. Restart Home Assistant to apply all the changes.

21. After the restart, you should be able to see the hp printer integration card in your specified view. Make sure to carefully follow the steps and verify that all dependencies have been properly installed.

**Configuration of HP Instant Ink Subscription Renewal Date and Printed Pages Information:**

To configure the HP Instant Ink subscription renewal date and information about printed pages, including additional costs, follow these steps:

1. Make sure you have successfully installed the card in the Home Assistant interface following the previous guide.

2. In the view where you have added the hp printer integration card, look for the settings icon associated with the card. It is usually represented by a gear icon or three vertical dots.

3. Click on the settings icon to open the card'sconfiguration panel.

4. Inside the configuration panel, you should find options to set the HP Instant Ink subscription renewal date, the number of monthly included pages, the already printed pages, and extra pages with their respective cost.

5. Follow the instructions provided in the configuration panel to input the required information. You may need to enter dates in the correct format, specify printed pages, and associated costs.

6. Make sure to save the changes made in the card configuration.

Once you have completed these steps, the hp printer integration card will display the correctly configured information, such as the subscription renewal date, included pages, already printed pages, and extra pages with their respective costs. You will be able to view and monitor this information directly in the Home Assistant view.

Please note that the configuration options may slightly vary depending on the specific implementation of the hp printer card you have installed. Make sure to carefully read the instructions provided with the card to achieve proper configuration.



I hope this guide has been helpful to you! If you have any further questions, feel free to ask.

<a href="https://www.buymeacoffee.com/divil17F"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=divil17F&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff" /></a>


