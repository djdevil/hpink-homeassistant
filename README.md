<a href="https://www.buymeacoffee.com/divil17F"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=divil17F&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff" /></a>

# Guida all'installazione e alla configurazione di HP Printer per Home Assistant

Questa guida ti fornirà i passaggi necessari per installare e configurare correttamente l'integrazione HP Printer Ink Status in Home Assistant utilizzando HACS.

**Prerequisiti:**
- Avere Home Assistant e HACS correttamente installati e funzionanti.

1. Visita la pagina del repository GitHub dell'integrazione HP Printer su [https://github.com/elad-bar/ha-hpprinter](https://github.com/elad-bar/ha-hpprinter).
2. Nella scheda "Integrazioni", cerca e installa le dipendenze "Paper Buttons Row" e "browser mod" seguendo le istruzioni fornite nella documentazione del repository.
3. Installa l'integrazione HP Printer tramite HACS seguendo le istruzioni fornite nella documentazione del repository.
4. Fai clic sul pulsante verde "Code" nella pagina del repository e seleziona "Download ZIP" per scaricare il file ZIP dell'integrazione.
5. Estrai il contenuto del file ZIP in una posizione facilmente accessibile sul tuo computer.
6. Troverai un file chiamato `hpink.yaml` all'interno della cartella estratta. Copia questo file.
7. Accedi al tuo server Home Assistant e individua la cartella "packages". Di solito si trova nella directory principale di Home Assistant.
8. Incolla il file `hpink.yaml` nella cartella "packages".
9. Riavvia Home Assistant per applicare le modifiche.
10. Apri l'interfaccia di Home Assistant nel tuo browser e vai alla pagina del frontend.
11. Nella pagina del frontend, cerca l'entità chiamata "HP Printer Printer" nella lista delle entità disponibili. Dovresti vederla elencata come una delle entità integrate dopo aver installato l'integrazione HP Printer tramite HACS.
    - **Nota:** Se non vedi l'entità "HP Printer Printer" nell'elenco delle entità, assicurati di aver seguito correttamente i passaggi precedenti e che l'integrazione sia stata installata correttamente.
12. Una volta individuata l'entità "HP Printer Printer", fai clic su di essa e rinominala in "sensor.hp_envy_5540_total_pages_printed_xml".
    - **Nota:** Assicurati di mantenere la struttura "sensor.hp_envy_5540_total_pages_printed_xml" per evitare eventuali problemi di compatibilità con il resto della configurazione.
13. Salva le modifiche e continua con gli altri passaggi indicati nella guida.
14. Torna alla tua installazione di HACS in Home Assistant.
15. Crea o apri il file `card.yaml` nella vista in cui desideri visualizzare la card dell'integrazione HP Printer.
16. Copia e incolla il codice specificato nel file `card.yaml` del repository HP Printer nella tua vista. Salva il file dopo l'incollaggio.
17. Riavvia Home Assistant per applicare tutte le modifiche.
18. Dopo il riavvio, dovresti essere in grado di vedere la card dell'integrazione HP Printer nella tua vista specificata. Assicurati di seguire attentamente i passaggi e verifica che tutte le dipendenenze siano state correttamente installate.

**Configurazione delle informazioni sull'abbonamento HP Instant Ink e le pagine stampate:**

1. Assicurati di aver installato correttamente la card nell'interfaccia di Home Assistant seguendo la guida precedente.
2. Nella vista in cui hai aggiunto la card dell'integrazione HP Printer, cerca l'icona delle impostazioni associata alla card. Di solito è rappresentata da un'icona a forma di ingranaggio o da tre punti verticali.
3. Fai clic sull'icona delle impostazioni per aprire il pannello di configurazione della card.
4. All'interno del pannello di configurazione, troverai opzioni per impostare la data di rinnovo dell'abbonamento HP Instant Ink, il numero di pagine incluse mensilmente, le pagine già stampate e le pagine extra con il relativo costo.
5. Segui le istruzioni fornite nel pannello di configurazione per inserire le informazioni richieste. Potresti dover inserire le date nel formato corretto, specificare le pagine stampate e i costi associati.
6. Assicurati di salvare le modifiche apportate nella configurazione della card.

Una volta completati questi passaggi, la card dell'integrazione HP Printer visualizzerà le informazioni correttamente configurate, come la data di rinnovo dell'abbonamento, le pagine incluse, le pagine già stampate e le pagine extra con i relativi costi. Sarai in grado di visualizzare e monitorare queste informazioni direttamente nella vista di Home Assistant.

Ricorda che le opzioni di configurazione potrebbero variare leggermente a seconda della specifica implementazione della card HP Printer che hai installato. Assicurati di leggere attentamente le istruzioni fornite con la card per ottenere una corretta configurazione.

Spero che questa guida ti sia stata utile! Se hai ulteriori domande, non esitare a chiedere.


ENGLISH


# HP Printer Integration Installation and Configuration Guide for Home Assistant

This guide will provide you with the necessary steps to properly install and configure the HP Printer integration in Home Assistant using HACS.

**Prerequisites:**
- Have Home Assistant and HACS properly installed and functioning.

1. Visit the GitHub repository page for the HP Printer integration at [https://github.com/elad-bar/ha-hpprinter](https://github.com/elad-bar/ha-hpprinter).
2. In the "Integrations" tab, search for and install the dependencies "Paper Buttons Row" and "browser mod" following the instructions provided in the repository's documentation.
3. Install the HP Printer integration through HACS following the instructions provided in the repository's documentation.
4. Click on the green "Code" button on the repository page and select "Download ZIP" to download the integration's ZIP file.
5. Extract the contents of the ZIP file to an easily accessible location on your computer.
6. You will find a file named `hpink.yaml` within the extracted folder. Copy this file.
7. Access your Home Assistant server and locate the "packages" folder. It is usually found in the main directory of Home Assistant.
8. Paste the `hpink.yaml` file into the "packages" folder.
9. Restart Home Assistant to apply the changes.
10. Open the Home Assistant interface in your browser and navigate to the frontend page.
11. In the frontend page, search for the entity named "HP Printer Printer" in the list of available entities. You should see it listed as one of the integrated entities after installing the HP Printer integration through HACS.
    - **Note:** If you don't see the "HP Printer Printer" entity in the list of entities, make sure you have followed the previous steps correctly and that the integration has been successfully installed.
12. Once you locate the "HP Printer Printer" entity, click on it and rename it to "sensor.hp_envy_5540_total_pages_printed_xml".
    - **Note:** Make sure to maintain the structure "sensor.hp_envy_5540_total_pages_printed_xml" to avoid any compatibility issues with the rest of the configuration.
13. Save the changes and proceed with the other steps mentioned in the guide.
14. Go back to your HACS installation in Home Assistant.
15. Create or open the `card.yaml` file in the view where you want to display the HP Printer integration card.
16. Copy and paste the specified code from the HP Printer repository's `card.yaml` file into your view. Save the file after pasting.
17. Restart Home Assistant to apply all the changes.
18. After the restart, you should be able to see the HP Printer integration card in your specified view. Make sure to carefully follow the steps and verify that all dependencies have been properly installed.

**Configuration of HP Instant Ink Subscription Renewal Date and Printed Pages Information:**

1. Make sure you have successfully installed the card in the Home Assistant interface following the previous guide.
2. In the view where you added the HP Printer integration card, look for the settings icon associated with the card. It is usually represented by a gear-shaped icon or three vertical dots.
3. Click on the settings icon to open the card's configuration panel.
4. Inside the configuration panel, you will find options to set the HP Instant Ink subscription renewal date, the number of monthly included pages, the already printed pages, and the extra pages with their respective costs.
5. Follow the instructions provided in the configuration panel to enter the required information. You may need to enter the dates in the correct format, specify the printed pages, and associated costs6. Be sure to save the changes made in the card's configuration.

Once you have completed these steps, the HP Printer integration card will display the correctly configured information, such as the subscription renewal date, included pages, printed pages, and extra pages with their respective costs. You will be able to view and monitor this information directly in the Home Assistant view.

Please note that the configuration options may vary slightly depending on the specific implementation of the HP Printer card you have installed. Make sure to carefully read the instructions provided with the card to achieve a proper configuration.

I hope this guide has been helpful to you! If you have any further questions, feel free to ask.

<a href="https://www.buymeacoffee.com/divil17F"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=divil17F&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff" /></a>


