# Ecommerce - Esame finale

Un importante committente ha richiesto la realizzazione di un’app che permetta di visualizzare il catalogo dei propri prodotti

Sarà necessario sviluppare una pagina per mostrare la lista di tutti i prodotti, ed una pagina per mostrare il dettaglio di ogni prodotto.

Il committente ha fornito due API, una per ottenere la lista dei prodotti:

```
GET https://raw.githubusercontent.com/andrea689/db/main/exams/ecommerce/products
```

Ed un'altra API per ottenere il dettaglio del singolo prodotto avente id `<PRODUCT_ID>`:

```
GET https://raw.githubusercontent.com/andrea689/db/main/exams/ecommerce/product_details/<PRODUCT_ID>
```

## Pagina 1 - Lista prodotti

La pagina "Lista prodotti" deve mostrare per ogni prodotto:

- foto principale (`main_photo`)
- nome del prodotto (`name`)
- descrizione (`short_description`)
- prezzo (`price`)

Inoltre è richiesto di aggiungere un tasto per ordinare la lista dei prodotti in base al prezzo (crescente o decrescente)

Al click del singolo prodotto bisognerà aprire la pagina "Dettaglio prodotto"

## Pagina 2 - Dettaglio prodotto

La pagina "Dettaglio prodotto" deve mostrare:

- foto principale (`main_photo`)
- categoria (`category`)
- marca (`brand`)
- nome del prodotto (`name`)
- descrizione (`description`)
- valutazione media (`vote_average`)
- quantità disponibile (`stock_quantity`)
- prezzo (`price`)

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
