# Bari Student Cost of Living

Questo progetto analizza e simula il costo della vita di uno studente universitario a Bari
utilizzando Python e tecniche di analisi dei dati.

L’obiettivo è stimare la spesa mensile, comprenderne la composizione e valutare il rischio
di sforamento del budget in presenza un aumento dell’affitto.

# Contesto e motivazione

Il costo della vita rappresenta una delle principali voci di incertezza per uno studente
fuori sede. In particolare, variazioni improvvise dell’affitto possono avere un impatto
significativo sulla sostenibilità del budget mensile.

Il progetto utilizza dati sintetici ma realistici, costruiti su valori medi, per simulare
uno scenario di spesa annuale e valutare gli effetti di un aumento dell’affitto pari al 35%.

# Dataset

Il dataset è generato direttamente nel notebook e copre un periodo di 12 mesi.

Caratteristiche principali:
- frequenza giornaliera
- valori medi deterministici (nessuna casualità nei dati di base)
- categorie di spesa tipiche di uno studente universitario

Categorie considerate:
- rent
- groceries
- transport
- eating_out
- university
- bills
- leisure

Il file risultante è salvato in: expenses_12months_avg.csv

## Analisi e visualizzazioni

L’analisi comprende:
- calcolo della spesa totale mensile
- ripartizione della spesa per categoria
- visualizzazione dell’andamento temporale

I principali grafici prodotti sono salvati nella cartella `results/`.

## Simulazione Monte Carlo

La parte centrale del progetto è una simulazione Monte Carlo finalizzata a stimare
l’impatto di un aumento dell’affitto del 35%, da 320€ a 432€ mensili (incrementi al giorno d'oggi possibili).

Ipotesi principali:
- l’aumento dell’affitto avviene una sola volta ed è permanente
- le spese non legate all’affitto variano mese per mese
- il budget mensile di riferimento è fissato a 1200€

La simulazione consente di stimare:
- la distribuzione della spesa mensile prima e dopo l’aumento
- la probabilità di sforamento del budget
- l’incremento medio della spesa mensile dovuto allo shock

# Note finali

Il progetto è pensato come esercizio di analisi dei dati e simulazione applicata
a un problema reale di gestione del budget personale.

I dati possono essere facilmente sostituiti con spese reali (anche personali) mantenendo
la stessa struttura del dataset.
