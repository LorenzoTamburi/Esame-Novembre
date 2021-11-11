# Jobs Searcher 
# Introduzione
Il programma permette all'utente di:

Visualizzare le proposte di lavoro in Pyhton. Richiede in ingresso la città dove ricercare il lavoro (Bosto, Chicago, Houston, Los Angeles, San Francisco), il tipo di contratto (Full Time, Part Time, Unknown), numero dei dipendenti dell'azienda (1-10, 11-50, 51-100 , 100+, Unknown) e se è possibile lo smartworking (True, False, Unknown).

Visualizzare le statistiche dei lavori trovati. Richiede in ingresso la città e il linguaggio di programmazione (Java, Python, SQL).

Visualizzare le statistiche dei lavori trovati. Richiede in ingresso la città dove effettuare le statistiche.

# Rotte
Le richieste che l'utente può effettuare tramite Postman devono essere effettuate all'indirizzo
localhost:8080.

![Tab_Rotte](https://user-images.githubusercontent.com/75088702/141351259-258e4f83-4d00-4eaf-b7fe-eaf126a1b5ea.png)

Per ottenere i vettori è possibile usare anche l'interfaccia grafica: 

<b><i>Esempio</i></b>

<b><i>Esecuzione</i></b>
![Esempio_Inerf1](https://user-images.githubusercontent.com/75088702/141351790-96028780-fe87-4d76-a7b5-308c0a43834b.png)

<b><i>Risultato</i></b>
![Esempio_Interf2](https://user-images.githubusercontent.com/75088702/141351951-2943f3ea-4fe2-44ae-8421-0c04aa481a8b.png)

# Gestione Eccezioni

Per gestire le eccezioni abbiamo creato 3 classi: ApiRequestExceptions, ExceptionsGeneraln e ExceptionsHandler

Per quanto riguarda la rotta /stats abbiamo:

"Citta' non valida" quando l'utente inserisce un città che non corrispoinde alle 5 sopra citate

"Tipo linguaggio non valido" quando l'utente inserisce un linguaggio di programmazione che non corrispoinde ai 3 sopra citati


Per quanto riguarda la rotta /jobs abbiamo:

"Citta' non valida" quando l'utente inserisce un città che non corrispoinde alle 5 sopra citate

"Parametro per remoto non valido" quando l'utente inserisce un un parametro che non corrisponde a quelli che indicano se il lavoro si può  svolgere in remoto o meno

"Tipo contratto non valido" quando l'utente inserisce un un parametro che non corrisponde a quelli che indicano se il lavoro è full-time o part-time


Per quanto riguarda la rotta /alljobs abbiamo:

"Citta' non valida" quando l'utente inserisce un città che non corrispoinde alle 5 sopra citate

