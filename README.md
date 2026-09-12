# **AvvioPC Pro: La Nuova Era del Deployment**

**AvvioPC Pro** rappresenta l'evoluzione definitiva del primordiale *AvvioPC*, nato originariamente come un basilare script batch DOS scritto per semplificare le configurazioni iniziali dei computer in ambito retail. Mentre la prima versione offriva un semplice menù testuale, ed essendo priva di aggiornamenti o funzioni di reportistica era divenuta ormai obsoleto, le alternative commerciali sul mercato si dimostravano troppo generiche, scomode o eccessivamente lente per l'utilizzo quotidiano. Da queste necessità nasce l'ecosistema **AvvioPC Pro**, un installer definitivo e professionale sviluppato e strutturato su tre moduli fondamentali integrati.

L'adozione di questa suite trasforma radicalmente l'operatività del punto vendita: l'automazione spinta azzera i tempi morti e i colli di bottiglia tecnici, garantendo un incremento immediato della produttività. Questo si traduce in una drastica riduzione dei costi occulti di configurazione e in un servizio al cliente impeccabile, elevando gli standard qualitativi e l'efficienza dell'intera azienda.

| Modulo Operativo | Piattaforma Target | Obiettivo Strategico e Funzioni Chiave |
| :--- | :--- | :--- |
| **1. Web App Front-End** | Smartphone / Mobile Browser | Barcode scanner S/N, OCR Product Key, Generazione MSA & PIN client-side |
| **2. USB Zero-Touch** | Notebook / PC in Lavorazione | Bypass OOBE, provisioning offline, installazione silent app & AV, auto-update Cloudflare |
| **3. Demone di Stampa** | PC di Rete / Banco Servizi | Ricezione job da server, generazione automatica e stampa del report di consegna professionale |

## **1. Il Centro di Controllo: Web App di Front-End**

Il fulcro operativo dell'interazione con l'operatore è un'applicazione web PWA installabile su qualsiasi smartphone (Android e iOS), concepita per essere utilizzata in mobilità e direttamente davanti al cliente prima del passaggio in cassa.

[ INSERIRE IMMAGINE WEB APP QUI ]

* **Acquisizione Dati Avanzata:** Integra un lettore barcode tramite fotocamera per associare istantaneamente il Serial Number (S/N) del PC. Include moduli OCR per acquisire i product key delle licenze ed iniettarli in modalità totalmente *unattended* durante il provisioning.
* **Gestione Account Microsoft (MSA):** Dispone di un algoritmo di generazione automatizzata delle credenziali per i nuovi account MSA. L'operatività in presenza del cliente si rivela strategica e indispensabile per ricevere e confermare in tempo reale il PIN di verifica inviato da Microsoft sullo smartphone dell'utente.

## **2. L'Esecutore Silente: Chiavetta USB Zero-Touch**

Il vero motore dell'automazione sul campo è la chiavetta USB di servizio. Il supporto si genera e si aggiorna tramite un web Installer dedicato, scaricabile da un qualsiasi PC espositivo connesso ad Internet.

[ INSERIRE IMMAGINE NOTEBOOK USB QUI ]

* **Configurazione Automatica Zero-Touch:** È sufficiente collegare l'alimentazione al computer da configurare, inserire la chiavetta USB e accendere la macchina per saltare a piè pari tutte le noiose e lunghe schermate OOBE di Microsoft Windows 11.
* **Provisioning Offline Integrato:** Il sistema esegue la disinstallazione pulita degli antivirus dimostrativi e procede all'installazione *unattended* della suite di applicazioni predefinite. Gestisce l'attivazione di Microsoft Office, inietta l'account Microsoft pre-creato e configura l'antivirus commerciale selezionato (Unieuro Everyday Security, Norton 360 o McAfee), forzando all'occorrenza gli aggiornamenti via Windows Update.
* **Sincronizzazione Cloud Autoaggiornante:** Al termine delle lavorazioni, la chiavetta verifica la presenza di nuove release del pacchetto sui server Cloudflare R2 e scarica autonomamente gli aggiornamenti (funzione con bypass rapido in caso di consegne urgenti).

[ INSERIRE IMMAGINE NOTIFICHE WPF QUI ]

* **Diagnostica e Telemetria Visiva:** Una finestra di console monitora l'avanzamento registrando ogni evento in appositi file di log. Eventuali interruzioni o anomalie vengono prontamente segnalate tramite maxi-banner visivi ad alto contrasto, leggibili anche a grande distanza nell'area di lavoro.

## **3. La Prova Tangibile: Il Demone di Stampa**

A chiudere l'architettura della suite interviene un'utility residente e autoaggiornante installata su un computer connesso alla rete locale del negozio.

[ INSERIRE IMMAGINE REPORT CARTACEO QUI ]

* **Flusso di Lavoro Asincrono:** Il demone lavora in background e in modo del tutto silente, rimanendo in ascolto delle chiamate provenienti dalla Web App.
* **Generazione Automatica:** Non appena i dati di configurazione vengono inviati al server centralizzato, il demone elabora la scheda e manda automaticamente in stampa un report sintetico, elegante e professionale.
* **Trasparenza verso il Cliente:** Tale scheda informativa è concepita per essere consegnata al cliente al momento del ritiro, fornendo una prova tangibile, chiara e trasparente di tutte le attività tecniche svolte sul computer.

---

> **▲ Note di Sviluppo & Filosofia Progettuale:**
> Questo intero ecosistema asincrono è stato realizzato dal sottoscritto a titolo completamente gratuito e senza fini di lucro. L'intero progetto è il frutto di innumerevoli ore di sviluppo volontario, guidato esclusivamente da una profonda passione per questo lavoro e dal desiderio concreto di migliorare la quotidianità lavorativa dei team. Alcune limitazioni nell'installazione automatica di software a pagamento derivano dall'impossibilità di acquistare licenze di test, costringendo a verifiche "live" direttamente durante le lavorazioni reali. In ogni caso si è voluto realizzare un prodotto professionale, robusto e intuitivo, nato e sviluppato direttamente sul campo: **da commesso, per i commessi**.
