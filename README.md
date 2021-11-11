# Jobs Searcher 
# Introduzione
Il programma permette all'utente di:

Visualizzare le proposte di lavoro in Pyhton. Richiede in ingresso la città dove ricercare il lavoro (Bosto, Chicago, Houston, Los Angeles, San Francisco), il tipo di contratto (Full Time, Part Time, Unknown), numero dei dipendenti dell'azienda (1-10, 11-50, 51-100 , 100+, Unknown) e se è possibile lo smartworking (True, False, Unknown).

Visualizzare le statistiche dei lavori trovati. Richiede in ingresso la città e il linguaggio di programmazione (Java, Python, SQL).

Visualizzare le statistiche dei lavori trovati. Richiede in ingresso la città dove effettuare le statistiche.

# Diagrammi UML

<b><i> Diagramma casi d'uso </i></b>
![Casi_d_uso](https://user-images.githubusercontent.com/75088702/141357338-0a809332-4f30-4667-b9a7-f1f3680e67e5.png)

Nel diagramma riportato qui sopra (casi d'uso) vengono mostrate le possibili azioni che l'utente puoò svolgere, in base alle sue scelte il programma si comporterà di conseguenza 

<b><i> Diagrammi delle sequenze </i></b>
![Sequenze_filtri](https://user-images.githubusercontent.com/75088702/141357700-9a6115d8-ac3d-46f8-b04c-112d05762b62.png)
![Sequenza_Statsg](https://user-images.githubusercontent.com/75088702/141358010-2745639c-6288-4da2-b647-435326acfc38.png)
![Sequenza_Stats](https://user-images.githubusercontent.com/75088702/141358121-2e2e3fcc-aa8c-4998-9037-1998ebc7b0c4.png)

Nei diagrammi riportati qui sopra (sequenze) vengono illustrati i processi dinamici di interazione fra le classi ogni qualvolta che l'utente eseguirà una richiesta 

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

<b><i>Esempio</i></b>

![Local_1](https://user-images.githubusercontent.com/75088702/141354799-4b2c7735-18fd-44e4-8d4e-8e5423e985ca.png)
![Console_1](https://user-images.githubusercontent.com/75088702/141354823-55d52734-a9fd-4b7b-933e-8b01ab5b31c2.png)
![Local_2](https://user-images.githubusercontent.com/75088702/141355091-296ddc71-957a-496c-a79c-9afe95a0b94f.png)
![console_2](https://user-images.githubusercontent.com/75088702/141355099-008ee8de-537d-4127-b91b-bb51b3e4854b.png)


# Test

Abbiamo implementato 3 unità di test:

1.<b>arrotondaTest</b>: Verifica che la funzione "arrotonda (double d)" ,presente in  Stats.java e StatsG.java, arrotondi a due cifre decimali.

2.<b>exceptionTesting</b>: Verifica che in caso di cità invalida venga segnalato l'errore con l'output corretto.

3.<b>aTesting</b>: Verifica che il metodo "public Vector<DownloadCity> filtra" presente in FiltersLavori.java dati tre parametri restituisce quello corretto.

# Autori
  Il programma è stato sviluppato in modo equo da:
  
  Tamburi Lorenzo (s1096088) e Taras Adrian Corneliu (s1096692)
