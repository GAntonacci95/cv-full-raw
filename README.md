# cv-full-raw

# cv-detail-crif

## EN 🇬🇧 (jul 2022 - jul 2025)

### CreMA for LegalTech

The batch project aimed at building a state machine to produce a final json
including enrichment data coming from external providers (business information, financial statement,
people diligence and investigation, real estate information, GenAI language model APIs), and model forecasts related to risk over credit portfolios.

The solution strategy involved:
- File transfer interfaces: customer files were exchanged either via s3 staging area or asynchronously via SFTP;
- Data and artifact stack: data was stored into s3 datalakes as partitioned parquets including timestamps to create a history, the data loaded from the database followed an ETL pipeline and exploited schemas and a data lineage strategy;
- Infrastructure stack: the application run through flow automated and orchestrated lambda functions;
- Software stack: the lambdas dynamically loaded wheels, packages, and layers designed for independence and modularity to grant quality, usability and maintainability;
- Output interfaces and monitoring: beyond output files, including the final json, logs and e-mails were introduced to monitor executions and metrics. Indeed, such logs were queried via cloudwatch, and an almost dynamic processes states visualization was provided through quicksight.

The solution expected results include: reduced enrichment time, reduced human error, enhanced operators productivity, and support for legal action decisions. However, we designed no quantitative kpi to highlight the process improvements.

Hard skill: athena, sql, git, zeep, xmltojson, pyyaml, networkx, jsonpointer, cython, fernet, setuptools, simple email service, cloudwatch;

Soft skill: creativity, detail and goal orientation, determination, focus, speed, independence, reflection, team-work beginner, information management beginner.

### CreMA Scoring

The batch project aimed at building a produzionalization AWS architecture for the scoring and visualization of batch portfolios using machine learning models.

The architecture was customized based on markets and customers dimensions.
What is more, the challenge involved the development of a
custom framework to lead the autonomy of data scientists towards a more structured coding approach.

The solution strategy involved:
- File transfer interfaces: customer files were exchanged either via s3 staging area or asynchronously via SFTP;
- Data and artifact stack: data was stored into s3 datalakes as partitioned parquets including timestamps to create a history;
- Infrastructure stack: the application run in a docker image tagged into ECR and loaded by a step-function. The step-function delt with the flow and dynamically loaded an always up-to-date code-commit repository;
- Software stack: the pipelines were built upon abstraction to meet client and market dimensions, so to have a custom execution depending on incoming data;
- Output interfaces and monitoring: beyond output files, customer specific views were introduced for sake of business-oriented presentations.
    
The solution expected results include: reduced deployment time thanks to pipelines abstraction, and easiness of usage by the team working on model updates via sagemaker.

Hard skill: python, aws, triggers, events, schedules, quicksight, pandas, code-commit, sagemaker, wsl.

### Single-deal APIs for credit insurance and business customers

Two more project streams involved the development of single-deal API in order to provide risk scores of credit portfolio entries with the guarantee of the ACID property.

To do so, models were dynamically loaded in case of need and an input, intermediate, output and enrichment history was hold for sake of traceability.
The intermediate and output results were analysed in the UAT stage to validate model performances.

Hard skill: pymee, pydantic, pickle, logger, log stream, postman, probabilistic finite state machine architecture;

Soft skill: market separation, brewer and nash model in communications, log monitoring, distributed stochastic processes and networks.

### Other less significant projects

- Usage of azure databricks, pyspark notebooks, power bi, dax;
- Porting of local notebooks on azure infrastructure, intuition of hr processes and people analytics;


## IT 🇮🇹 (lug 2022 - lug 2025)

### CreMA per LegalTech

Progetto batch che mirava alla costruzione di una macchina a stati per produrre un json contenente dati di arricchimento provenienti da diversi provider esterni (informazioni business ed intelligence, dati di bilancio, diligence e rintracci, informazioni mobiliari ed immobiliari, GenAI, API verso LLM) e previsioni di modelli relativi al rischio su portafogli di credito.

La strategia risolutiva incorporava:
- Interfacce di trasferimento file: i file clienti erano scambiati tramite area di stageing s3 od in modo asincrono via SFTP;
- Stack dati ed artefatti: i dati erano salvati in datalake s3 come parquet partizionati ed includevano timestamp per creare uno storico. Il caricamento dati da database seguiva una pipeline ETL, sfruttava schemi ed utilizzava una strategia di lineage;
- Stack infrastrutturale: l'applicazione eseguiva tramite un flusso di lambda function automatizzato tramite un orchestratore;
- Stack applicativo: le lambda caricavano dinamicamente wheels, pacchetti e layer progettati per indipendenza e modularità al fine di garantire qualità, usabilità e manutenibilità;
- Interfacce d'uscita e monitoraggio: oltre ai file di uscita, che includevano il json finale, sono stati introdotti logs ed e-mails per il monitoraggio di esecuzione e metriche. Tali log venivano interrogati via cloudwatch e permettevano una visualizzazione quicksight quasi dinamica degli stati dei processi.

I risultati attesi dalla soluzione includono: tempi di arricchimento ed errore umano ridotti, migliore produttività degli operatori e supporto per decisioni in merito ad azionabilità legale. Tuttavia non sono stati definiti kpi quantitativi per valutare i miglioramenti dello stream progettuale.

Skill verticali: athena, sql, git, zeep, xmltojson, pyyaml, networkx, jsonpointer, cython, fernet, setuptools, simple email service, cloudwatch;

Skill orizzontali: creatività, orientamento a dettaglio e gol, determinazione, concentrazione, velocità, indipendenza, riflessività, principio di lavoro di squadra e gestione informativa.

### CreMA Scoring

Progetto batch che mirava alla costruzione di un'architettura AWS per emulare la messa in produzione di modelli di machine learning per lo scoring e la visualizzazione di portafogli di credito.

L'architettura era personalizzata dipendentemente dalle dimensioni mercato e cliente.
Inoltre, la sfida prevedeva lo sviluppo di un framework custom per guidare l'autonomia dei data scientists verso un approccio di sviluppo più strutturato.

La strategia risolutiva prevedeva:
- Interfacce di trasferimento file: i file clienti erano scambiati tramite area di stageing s3 od in modo asincrono via SFTP;
- Stack dati ed artefatti: i dati erano salvati in datalake s3 come parquet partizionati per creare uno storico;
- Stack infrastrutturale: l'applicazione eseguiva in una docker image taggata in ECR. Questa era caricata da una step function che si occupava della gestione del flusso d'esecuzione e del caricamento dinamico di codice da una repository code-commit sempre aggiornata;
- Stack applicativo: le pipeline per mercato e cliente erano costruite implementando astrazioni in modo da garantire un'esecuzione personalizzata dipendenemente dai dati in arrivo;
- Interfacce d'uscita e monitoraggio: oltre ai file di uscita, sono state introdotte visualizzazioni specifiche per cliente al fine di facilitare le presentazioni orientate al business.

I risultati attesi della soluzione includono: riduzione del tempo di deployment e semplicità di utilizzo da parte del team che lavora su aggiornamenti di modello tramite sagemaker.

Hard skill: python, aws, triggers, events, schedules, quicksight, pandas, code-commit, sagemaker, wsl.

### API single-deal per clienti assicurazione credito e business

Un paio di ulteriori stream progettuali riguardavano lo sviluppo di API single-deal per fornire score di rischio credito relativo a portafogli garantendo la proprietà ACID.

Per farlo, i modelli erano caricati dinamicamente al bisogno e si teneva storico di informazioni d'ingresso, intermedie, d'arricchimento e d'uscita a fini di tracciabilità.
I risultati intermedi e d'uscita sono stati analizzati in fase di UAT per validare le performance di modello.

Skill verticali: pymee, pydantic, pickle, logger, log stream, postman, architettura macchina probabilistica a stati finiti;

Skill orizzontali: separazione di mercati, modello di comunicazione brewer and nash, monitoraggio log, processi stocastici e reti distribuite.

### Altri progetti meno significativi

- Uso di azure databricks, pyspark notebooks, power bi, dax;

- Porting di notebook locali su infrastruttura azure, intuizione del funzionamento di processi hr e di analisi personale;

# cv-detail-polimi

## EN 🇬🇧 (sep 2018 - oct 2021)

### M.Sc. Research Thesis

The project aimed at providing a sketchy
audio forensics integrity checking tool.

The solution involved an automated flow for the generation and versioning of synthetic data during the
experiments, extraction of feature-sets and usage of deep CNNs while comparing different model performances.

The resulting manuscript is available [here](https://www.politesi.polimi.it/bitstream/10589/179887/3/gabriele_antonacci_master_thesis.pdf),
and the code and details are available
[here](https://github.com/polimi-ispl/room_geometry_estimation) or [here](https://github.com/GAntonacci95/room_shape_classification).

Hard skill: python, wandb, experiments tracking
and reproducibility, pyroomacoustics,
librosa, numpy, scipy, tensorflow-gpu,
keras, nn architectural
tuning via evolutionary algorithms,
attention networks, explainability.

Soft skill: investigative creativity.

supervisor: Fabio Antonacci, opponent: Paolo Bestagini

### JuicyWhammy

A C++ VST-3 plug-in performing pitch
shifting on audio signals. The solution
encompasses JUCE audio framework, the
soundtouch C++ audio processing library,
and the soundflower audio driver.

The resulting code is available [here](https://github.com/GAntonacci95/juicy-whammy) and
the demo [here](https://www.dropbox.com/scl/fi/ze4tzlxr2xgtp5b3ym6vq/WhammyPlugDemo6.mp4?rlkey=4tdicgr6uuywco2ubl0kpvybf&e=3&dl=0).

Hard skill: c++, juce, soundtouch, soundflower, quicktime player;

Soft skill: compressor, dynamics, phase discontinuities.

### WebularSynth

A web-service emulating a modular synthesizer with a fully automated audio processing chain based on angular, modularity, webAudio and webMIDI apis.
The resulting code and demo are available [here](https://github.com/GAntonacci95/webular_synth).

Hard skill: angular, typescript, javascript, html, and css;

Soft skill: audio chain.

### EmoMusic

A Spotify extension based on facial emotion recognition which plays songs from your playlists depending on your current mood.
The resulting code is available [here](https://github.com/toboko/emomusic) or [here](https://github.com/GAntonacci95/emomusic)

### Polifonia Music Association - volunteering

Directed the Events Team for the concerts organizational aspects concerning authorizations, promotion and resources allocation.

Managed the IT Team while creating the association website which included custom internal functionalities.

Association website available [here](https://www.polifoniapolimi.it)

### Other less significant projects

- Basic tin-can telephone acoustical analysis. Soft skill: chinese whispers game, belief propagation and sum-product algorithm, gnutella, spf, dependencies, proxy, vpn.

### Studies certification

The digitally signed studies certification is available [here](https://github.com/GAntonacci95/cv-detail-polimi/blob/main/autocertificazione-lm-polimi_signedGA.pdf)

## IT 🇮🇹 (set 2018 - ott 2021)

### Tesi di Laurea Magistrale

Bozza progettuale volta a creare un tool per la verifica d'integrità di file audio.

La soluzione era composta da un flusso automatizzato per la generazione ed il versioning di dati sintetici sperimentali, estrazione di features ed il training di differenti deep CNNs di cui si sono valutate le performance.

Il manoscritto risultante è disponibile [qui](https://www.politesi.polimi.it/bitstream/10589/179887/3/gabriele_antonacci_master_thesis.pdf),
il codice ed i dettagli invece [qui](https://github.com/polimi-ispl/room_geometry_estimation) o [qui](https://github.com/GAntonacci95/room_shape_classification).

Skill verticali: python, wandb, tracciamento sperimentale per riproducibilità, pyroomacoustics,
librosa, numpy, scipy, tensorflow-gpu,
keras, tuning di architettura nn tramite algoritmi genetici, reti di attenzione, spiegabilità.

Skill orizzontali: creatività investigativa.

relatore: Fabio Antonacci, avversario: Paolo Bestagini

### JuicyWhammy

Un plugin VST-3 in C++ per effettuare il pitch shifting di segnali audio. La soluzione utilizzava il framework audio JUCE, la libreria soundtouch per il processing audio ed il driver audio soundflower.

Il codice risultante è disponibile [qui](https://github.com/GAntonacci95/juicy-whammy) e la demo [qui](https://www.dropbox.com/scl/fi/ze4tzlxr2xgtp5b3ym6vq/WhammyPlugDemo6.mp4?rlkey=4tdicgr6uuywco2ubl0kpvybf&e=3&dl=0).

Skill verticali: c++, juce, soundtouch, soundflower, quicktime player;

Skill orizzontali: compressore, dinamiche, discontinuità di fase.

### WebularSynth

Un web-service che emula un sintetizzatore modulare con una catena audio automatizzata e basata su angular, modulare ed utilizzante webAudio and webMIDI apis.
Il codice e le demo risultanti sono disponibili [qui](https://github.com/GAntonacci95/webular_synth).

Skill verticali: angular, typescript, javascript, html, and css;

Skill orizzontali: catena audio.

### EmoMusic

Un'estensione spotify basata su riconoscimento facciale che esegue canzoni della tua playlist in base al tuo stato d'animo.
Il codice risultante è disponibile [qui](https://github.com/toboko/emomusic) o [qui](https://github.com/GAntonacci95/emomusic)

### Associazione Musicale Polifonia - volontariato

Diretto il Team Eventi per aspetti concernenti autorizzazioni, promozione ed allocazione risorse.

Gestito il Team IT durante la creazione del sito associativo con funzionalità interne personalizzate.

Association website available [here](https://www.polifoniapolimi.it)

### Altri progetti meno significativi

- Analisi basilare del fonobarattolo. Soft skill: telefono senza fili, propagazione di credenze ed algoritmo somma-prodotto, gnutella, spf, dipendenze, intermediari, vpn.

### Certificazione studi

La certificazione degli studi firmata digitalmente è disponibile [qui](https://github.com/GAntonacci95/cv-detail-polimi/blob/main/autocertificazione-lm-polimi_signedGA.pdf)

# cv-detail-unibo

## EN 🇬🇧 (sep 2014 - dec 2017)

### B.Sc. Thesis

The stream aimed at creating a service for 3D point clouds stretching and alignment considering different acquisition sensors.

Hard skill: java, icp algorithm

Soft skill: perspective, vision

supervisor: Stefano Mattoccia, opponent: Federico Chesani

### GoodBikes

The project aimed at building a custom ERP application for bike rental.

The code is available [here](https://github.com/GAntonacci95/good_bikes).

Hard skill: c#, mvc, mvp, observer, adapter, facade;

Soft skill: orthogonality, single access point, positive and negative feedback loops, masks, appearance, facebook.

### Other relevant courses

- Computer networks, protocols and ISO/OSI communications model;
- Operating systems, semaphores and race conditions;
- Telecommunications, electronics (DAC, ADC), electrics, automation and automatic controls;

### Studies certification

The digitally signed studies certification is available [here](https://github.com/GAntonacci95/cv-detail-unibo/blob/main/autocertificazione-lt-unibo_signedGA.pdf)

## IT 🇮🇹 (set 2014 - dic 2017)

### Tesi di Laurea Triennale

Il filone puntava a creare un servizio per lo stretching e l'allineamento di nuvole di punti acquisite da differenti sensori.

Hard skill: java, icp algorithm

Soft skill: perspective, vision

relatore: Stefano Mattoccia, avversario: Federico Chesani

### GoodBikes

Il progetto mirava a costruire un'applicazione ERP personalizzata per gestire il noleggio di biciclette.

Il codice è disponibile [qui](https://github.com/GAntonacci95/good_bikes).

Hard skill: c#, mvc, mvp, osservatore, adattatore, facciata;

Soft skill: ortogonalità, singolo punto d'accesso, cicli feedback positivi e negativi, larsen, maschere, apparenza, copertina.

### Altri corsi rilevanti

- Reti di calcolatori, protocolli e modello di comunicazione ISO/OSI;
- Sistemi operativi, semafori, concorrenza e corse critiche;
- Telecomunicazioni, elettronica (DAC, ADC), elettrotecnica, automazione, controlli automatici;

### Certificazione studi

La certificazione degli studi firmata digitalmente è disponibile [qui](https://github.com/GAntonacci95/cv-detail-unibo/blob/main/autocertificazione-lt-unibo_signedGA.pdf)
