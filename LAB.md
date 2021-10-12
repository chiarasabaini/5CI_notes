# LAB

---

https://slidemodel.com/business-model-canvas/
https://slidemodel.com/how-to-work-breakdown-structure-wbs/

---

## 2021-09-29

![on premise/cloud](res/img/cloud.png)

---

## 2021-09-27

![apps.marconivr.it (CMDB)](res/img/appscmdb.png)

### WEBSERVER
- "problema" dell'orario pubblico
    - soluzione &#x2192; login
        - opzione 1 &#x2192; spaggiari
            - soluzione "migliore"
                - c'è anche l'account genitore
            - incerto, poichè non si sa se è supportato
        - opzione 2 &#x2192; login con altri AAA or no login
            - senza eseguire l'accesso è visibile solo l'orario pubblico (senza alcune info)

**login types**
- spaggiari
- AD
- Google
- DB

![orario](res/img/orario.png)

Access DB &#x2192; contine una checklist che ha tutte le informazioni riguardanti tutti gli utenti

---

## 2021-09-22

![reverse proxy scheme](res/img/reverse_proxy.png)

#### Glossary

**Proxy**
- simula qualcosa
- intermediario -> tutto ciò che sta fuori dalla rete vede il proxy ma non ciò che sta all'interno della rete
![proxy scheme](res/img/proxy.svg)

**Reverse Proxy**
- proxy in ingresso -> ciò che sta all'interno della rete vede il proxy ma non ciò che sta fuori
- solitamente implementati per aumentare la sicurezza, le prestazioni e l'affidabilità
![reverse proxy scheme](res/img/reverse_proxy.svg)

**Rete**
- serve per offrire/usufruire dei servizi

**WSL** <sup>[Windows Subsystem for Linux]</sup>
- consente di eseguire un ambiente GNU/Linux direttamente su Windows, non modificato, senza il sovraccarico di una macchina virtuale tradizionale o di una configurazione dualboot

**Port forwarding**
- applicazione di conversione degli indirizzi di rete che reindirizza una richiesta di comunicazione da una combinazione di IP e port numbers a un'altra mentre i pacchetti attraversano un gateway

**Autenticazione**
- DB
- server AAA
    - servizio dedicato che se ne occupa (es.: LDAP -> AD)
    - **AAA** <sup>[Authentication Authorization Accounting]</sup>
        - Authentication
            - processo di identificazione di un individuo, di solito basato su un nome utente e una password
            - si basa sull'idea che ogni singolo utente avrà informazioni uniche che lo distinguono dagli altri utenti
        - Authorization
            - processo di concessione o negazione di un utente l'accesso alle risorse di rete una volta che l'utente è stato autenticato 
            - la quantità di indormazioni e servizi a cui l'utente ha accesso dipendono dal livello di autorizzazione dell'utente
        - Accounting
            - processo di tenere traccia dell'attività di un utente durante l'accesso alle risorse di rete, compresa la quantità di tempo trascorso in rete, i servizi a cui si accede mentre si è lì e la quantità di dati trasferiti durante la sessione
            - i dati vengono utilizzati per l'analisi delle tendenze, la pianificazione della capacità, la fatturazione, l'auditing e l'allocazione dei costi

**RODC** <sup>[Read Only Domain Controller]
- è un tipo di Domain Controller con partizioni read-only dell'ADDS (Active Directory Domain Services)
- le aziende tendono ad utilizzare il RODC quando:
    - non c'è abbastanza sicurezza fisica per il data center
    - non c'è abbastanza larghezza di banda per stabilire connessioni di rete

**SSO** <sup>[Single Sign On]</sup>
- è una tecnologia che combina diverse schermate di login alle applicazioni in una sola
- un utente deve inserire le proprie credenziali di accesso (nome utente, password, etc.) una sola volta su una singola pagina per accedere a tutte le proprie applicazioni SaaS

**DMZ** <sup>[DeMilitarized Zone]</sup>
- zona non protetta (esposta)
- sottorete fisica o logica che contiene ed espone i servizi rivolti all'esterno di un'organizzazione a una rete non attendibile, in genere più grande (es.: Internet)
- sta venendo sostituita dal *cloud* -> SaaS, PaaS, IaaS

**LAMP** <sup>[Linux, Apache, MySQL, PHP/Perl/Python]</sup>
- XAMPP for Linux
- ogni lettera dell'acronimo rappresenta uno dei suoi quattro elementi costitutivi open source
- uno degli stack di soluzioni più comuni per molte delle applicazioni più popolari del web
- ora si riferisce a un modello generico di stack software e i suoi componenti sono in gran parte intercambiabili

**Metadirectory**
- è un servizio centralizzato di integrazione dei dati
- può gestire transazioni di dati tra più directory o tra directory e database, questi tipi di servizi includono varie funzionalità per filtrare i dati e/o valutare o monitorare i dati in transito

---

## 2021-09-20

![notebook scheme](res/img/20210920.png)

#### Glossary

- **Programmi**
    - desktop
    - web
    - app mobile

- **Processo**
    - attività che deve essere inserita in un catalogo
    - chi fa cosa
    - entità dinamica caricata su memoria RAM generata da un programma

- **IAM** <sup>[Identity Access Management]</sup>
    - riguarda la definizione e la gestione dei ruoli e dei privilegi di accesso delle singole entità di rete (utenti e dispositivi) a una varietà di applicazioni cloud e locali
    - obiettivo principale: avere un'identità digitale per individuo o elemento; essa deve essere mantenuta, modificata e monitorata durante tutto il ciclo di vita di accesso di ciascun utente o dispositivo

- **GDPR** <sup>[General Data Protection Regulation]</sup>
    - regolamento dell'UE in materia di trattamento dei dati personali e di privacy
    - obiettivo: rafforzare la protezione dei dati personali di cittadini e residenti nell'UE, sia all'interno che all'esterno dei confini dell'UE, restituendo ai cittadini il controllo dei propri dati personali, semplificando il contesto normativo che riguarda gli affari internazionali, unificando e rendendo omogenea la normativa privacy dentro l'UE

- **Commitment**
    - se manca la volontà di chi sta in alto per fare qualcosa per chi sta in basso, è un problema\
    ![hierarchy](res/img/commitment.png)

---

### PROGETTO: ORARIO

1) **Identificare gli stakeholders che si occupano della creazione**
2) **Risorse Tecniche:**
    - individuare il programma di supporto per la creazione (GPI UNTISI)
3) **Definizione dell'organico (input del programma):**
    - creato da qualcun'altro che deve comunicare ogni cambiamento
    - composto da:
        - docenti
        - classi
        - materie
        - aule
4) **Definire un protocollo di comunicazione tra responsabili orario e organico**
5) **Output** -> 4 file .txt

![schema progetto orario](res/img/progetto_orario.png)

---

## 2021-09-17

![wp2pcs](res/img/wp2pcs.png)

![microservices](res/img/microservices.png)

### VM: Configurazione di rete

- **NAT**\
    -> **DHCP**: virtualizzatore\
    -> tutte le macchine hanno lo stesso indirizzo IP di classe A (10.x.x.x)

- **NAT Network**\
    -> **DHCP**: virtualizzatore\
    -> le macchine hanno indirizzi IP diversi, poichè le VM fanno parte della stessa rete

- **Bridge**\
    -> **DHCP**: si delega, in base al contesto _(indirizzi IP statici/assegnati dal DHCP del router)_\
    -> non si fa differenza tra VM e macchine fisiche\
    -> **DISCRIMINANTE** -> classe degli indirizzi IP

#### Glossary

- **Microservizi**
    - è un tipo di struttura architetturale che permette la rapida, frequente e affidabile distribuzione di applicazioni grandi e complesse, inoltre permette all'organizzazione di evolversi nel suo stack
    - questo tipo di architettura definisce un'app come un insieme di servizi che sono:
        - altamente mantenibili e testabili
        - liberamente accoppiati
        - distribuibili indipendentemente
        - organizzati intorno alle funzionalità dell'azienda

- **Container**
    - VM specializzata che ospita un microservizio
    - unità standard di software che impacchetta il codice e tutte le dipendenze, per far funzionare velocemente e affidabilmente l'applicazione da un ambiente all'altro.
    - l'immagine di un container Docker è un pacchetto leggero, autonomo ed eseguibile del software che include tutto il necessario per eseguire un'applicazione: codice, runtime, system tools, system libraries e impostazioni.

- **Orchestratore**
    - strumenti per amministrare, scalare, e mantenere applicazioni containerizzate
    - es.: Kubernetes, Docker Swarm 

- **LDAP** <sup>[Lightweight Directory Acces Protocol]</sup>
     - protocollo standard per l'interrogazione e la modifica dei *servizi di directory* <sup>(un qualsiasi raggruppamento di informazioni che può essere espresso come record di dati e organizzato in modo gerarchico)</sup>

- **Protocollo**
    - insieme di regole convenzionali che disciplinano il funzionamento di un sistema di comunicazione
    - permette di accedere ai servizi

- **BC/DR** <sup>[Business Continuity/Disaster Recovery]</sup>
    - pratica che serve per prepararci a minimizzare gli effetti di eventi che vanno ad intaccare il servizio significativamente
    - suddiviso in due parti:
        - *Business Continuity* -> concentrato sulla parte di operazioni aziendali, coinvolge la progettazione e la creazione di policies e procedure, che assicurino il funzionamento delle procedure essenziali, durante e dopo il disastro
        - *Disaster Recovery* -> concentrato sulla parte tecnica, definisce come il dipartimento di IT di un'organizzazione recupererà da un disatro naturale/artificiale 

- **Appliance**
    - termine generico che racchiude molti aspetti dei sistemi integrati e delle soluzioni correlate che attraversano data center, PC e distribuzione di software
    - può avere molti significati e interpretazioni da parte del settore, dei fornitori con relative iniziative di mercato e derivati
    - sono più di semplici pacchetti IT con il marketing: offrono tecnologia congiunta, hardware, gestione software e servizi.

- **check update**
    - port 8530
    - cerca il servizio **WSUS**
    - porta WSUS in un servizio interno
    - si collega con il WSUS in cloud e scarica l'update su quello "locale"
    - le macchine fanno l'update appoggiandosi al WSUS sulla rete locale

---

## 2021-09-15

![application](res/img/app.png)

<sup>*P.A.* -> procedura aziendale</sup>

---

### IO <sup>[applicazione opensource]</sup>
<sup>**keywords:** identità, sicurezza, LDAP, GDPR</sup>

Offre servizi dello Stato/Provincia/Comune -> es.: Green Pass, Cashback, etc.

---

### workstation -> peer-to-peer -> client/server

**Server:**
- SW
    - DB
    - web
    - print
    - ***file*** -> tra i protocolli di comunicazione utilizza il protocollo SMB <sup>(Server Message Block)</sup>, che è causa di buchi nella sicurezza

![img](res/img/wmi.png)

---

### AD
<sup>Active Directory</sup>

- Sistema server centralizzato, cuore di Windows Server, che si fonda sui concetti di dominio (in particolare di un Dominio Windows Server) e di directory, ovvero un insieme di directory services (servizi di rete), gestiti da un domain controller e adottati dai sistemi operativi Microsoft a partire da Windows 2000 Server

- Definisce la modalità con cui vengono assegnate agli utenti tutte le risorse di rete, secondo l'assegnazione da parte dell'amministratore di sistema di Group Policy

-  LDAP viene usato come database in cui vengono memorizzate in forma centralizzata tutte le informazioni di un dominio di rete, relativamente ad autenticazioni ed accesso ai servizi, mantenendo tutte queste informazioni sincronizzate tra i vari server

### VDI
<sup>Virtual Desktop Infrastructure</sup>

Infrastruttura per la virtualizzazione dei client

 - hosting di un ambiente desktop su un server centralizzato
 - forma di virtualizzazione desktop, in quanto l'immagine specifica gira su VMs e viene inviata al client attraverso una rete

---

| OS        | Multitask                    | Multiuser                    |
|-----------|------------------------------|------------------------------|
| DOS       |   <ul><li>- [ ] </li></ul>   |   <ul><li>- [ ] </li></ul>   |
| Windows   |   <ul><li>- [x] </li></ul>   |   <ul><li>- [ ] </li></ul>   |
| GNU/Linux |   <ul><li>- [x] </li></ul>   |   <ul><li>- [x] </li></ul>   |

**Multitask** -> più processi in exec contemporaneamente
**Multiuser** -> più utenti collegati contemporaneamente

---

## 2021-09-13

**GPI** -> Gestione Progetto, Organizzazione di Impresa

**Progetto**
- ha un inizio e una fine
- vanno identificati gli *stakeholeder*
- ***R&D*** -> Research & Development <sup>(progetti che potrebbero non arrivare ad una conclusione)</sup>

---

### *Business Model Canvas*
![Business Model Canvas](/res/img/business_model_canvas.png)

***KPI*** -> Key Performance Indicators, determinano la qualità

---

### Principio di Pareto | 80% 20%
<sup>**keywords:** semplificare, razionalizzare, ridimensionare, focalizzare</sup>

Il *principio di Pareto* afferma che il 20% delle cause provoca l'80% degli effetti; è un punto di riferimento utile per pianificare, analizzare e risolvere i problemi e raggiungere gli obiettivi.

Si può applicare in qualsiasi ambito.
**Esempi:**
| 80%             | 20%          |
|-----------------|--------------|
| Progetto finito | Manutenzione |
| Pensare         | Programmare  |

---

### *Scan-Plan-Do-Check-Act Cycle*
<sup>[processo di miglioramento continuo]</sup>

![Scan-Plan-Do-Check-Act](/res/img/spdca.png)

***Scan*** -> Identify the problem\
***Plan*** -> Recognize an opportunity and plan a change\
***Do*** -> Test the change\
***Check*** -> Review the result, analize it and identify what you've learned\
***Act*** -> Take action based on what you've learned

---

### *ITIL*
<sup>Information Technology Infrastructure Library</sup>

Si basa sul **CMDB** <sup>(Content Management DataBase)</sup>, è un insieme di pratiche dettagliate, per attività di IT, che si concentrano sull'allineamento con i bisogni del business.
