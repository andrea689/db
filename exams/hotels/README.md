# Hotels - Esame finale

Un importante committente ha richiesto la realizzazione di un’app che permetta la prenotazione delle camere dei propri hotels

Sarà necessario sviluppare una pagina per mostrare la lista di tutti gli hotels, ed una pagina per mostrare le camere disponibili per ogni singolo hotel.

Il committente ha fornito due API, una per ottenere la lista degli hotel:

```
GET https://raw.githubusercontent.com/andrea689/flutter_course/main/exams/hotels/hotels
```

Ed un'altra API per ottenere le camere del singolo hotel avente id `<HOTEL_ID>`:

```
GET https://raw.githubusercontent.com/andrea689/flutter_course/main/exams/hotels/hotel_details/<HOTEL_ID>
```

## Pagina 1 - Lista hotels

La pagina "Lista hotels" deve mostrare per ogni hotel:

- foto principale (`main_photo`)
- nome (`name`)
- descrizione (`description`)
- valutazione media (`vote_average`)

Inoltre è richiesto di aggiungere un tasto per ordinare la lista degli hotel in base al voto medio (crescente o decrescente)

Al click del singolo hotel bisognerà aprire la pagina "Camere hotel"

## Pagina 2 - Camere hotel

La pagina "Camere hotel" deve mostrare:

- il nome dell'hotel (`name`)
- l'indirizzo dell'hotel (`address`)
- la lista delle camere (`rooms`) visualizzando per ogni camera:
  - tipologia di camera (`type`)
  - foto (`image`)
  - numero massimo di adulti consentito (`adults`)
  - dimensione della camera in mq (`mq`)
  - prezzo per notte in euro (`price_for_night`)

## Valutazione

Per il superamento dell'esame sono richiesti:

- una buona struttura e la corretta nomenclatura dei file e dei nomi delle classi
- codice ben indentato e suddiviso in file appropriati
- un buon utilizzo dei `Widget` per la realizzazione di una piacevole UI
- l'utilizzo di `flutter_bloc` e dei `Cubit` per la gestione dello stato

Inoltre è considerato un plus:

- l'utilizzo delle API per ottenere lista e dettaglio degli hotels

## Consegna

Concluso l'esame eseguire il comando

```
flutter clean
```

E creare uno zip della cartella del progetto, nominandolo `cognome_nome_flutter_exam.zip`
