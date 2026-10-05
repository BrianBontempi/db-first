Esercizio di oggi: DB First
nome repo: db-first
Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.
Per la consegna, potete inserire la vostra tabella in un file markdown come vi ho fatto vedere a lezione, oppure farla su Excel, Fogli Google ecc e fare uno screen.




## Tabella `cars`

COL | TYPE | ATTRIBUTE
--- | --- | ---
id | BIGINT UNSIGNED | PRIMARY KEY AUTO_INCREMENT
targa | VARCHAR(10) | NOT NULL UNIQUE
marca | VARCHAR(50) | NOT NULL
modello | VARCHAR(50) | NOT NULL
prezzo | DECIMAL(9,2) | NOT NULL
km | INT UNSIGNED | NOT NULL DEFAULT 0
cambio | CHAR(1) | NOT NULL DEFAULT 'm'
stato | VARCHAR(20) | NULL
anno_immatricolazione | SMALLINT UNSIGNED | NOT NULL
alimentazione | VARCHAR(20) | NOT NULL
cilindrata | SMALLINT UNSIGNED | NULL
colore | VARCHAR(30) | NOT NULL
porte | TINYINT UNSIGNED | NOT NULL DEFAULT 5
descrizione | TEXT | NULL
venduta | TINYINT(1) | NOT NULL DEFAULT 0

Note:
- `cambio`: 'm' = manuale, 'a' = automatico
- `stato`: condizioni dell'auto (es. ottimo, buono, da revisionare)
- `alimentazione`: benzina, diesel, gpl, metano, ibrida, elettrica
