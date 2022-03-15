# ATM system based on fingerprint via android/ios application
1. ATM desktop application or Web App?:
   1. desktop application is more similar to the "ATM enviorament"
   2. If i use a web app i can make a server that hosts it and the fingerprint system can be used on mobile or with the faceId with iphone.

If I use a web app I can make generic functions which the user interacts with a touch monitor. but how can the atm recognize who is using the ATM?
I go to the atm and with the app scan a qr code that identifies the atm. From that the smartphone sends a request to a central server that route the request to the appropriate ATM.<br>The ATM gets a LOCKED attribute and the user can do his stuff.<br>When is time to get money, the atm sends a request to the web app for authotization, that can be either fingerprint or faceId. The phone sends the authorization signal to the atm, and if is correct grants the money, if not you have three tryes.

## Base ATM functions
1. Getting money
2. Making a deposit (Deposito contanti o assegni -> Gli assegni devono poi essere controllati)
3. Cash advances
4. Pagamento di bollettini postali

Partire da prelievo.

## Necessarie:
1. Server centrale
   1. Possibile uso di wsl2 per avere un server linux in locale
   2. Linguaggio: js / nodejs
2. Applicazione smartphone
   1. Flutter: Problema con flutter, dovrei usare due sistemi differenti per creare il lato server ed il lato client, aumentando il, già abbastanza grande, carico di lavoro
   2. Appena si apre l'applicazione schermata di caricamento animata durante la connessione al server. Poi fake home page dove l'unico tasto funzionante è la scansione del codice qr ed un "profilo" base del cliente
   3. MIT app inventor => Ricerca
3. applicazione desktop/webapp su atm:
   1. flutter

