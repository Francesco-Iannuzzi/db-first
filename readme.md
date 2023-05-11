Consegna:
- Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.

Attributes:

- PRIMARY_KEY / INDEX / UNIQUE / AUTO_INCREMENT / NULL / NOTNULL / DEFAULT(value)


Numbers:

- TINYINT / SMALLINT / MEDIUMINT / INT / BIGINT / FLOAT(I, D) / DOBLUE (I, D) / DECIMAL(I, D)

Strings:

- CHAR() / VARCHAR() / TEXT / MEDIUMTEXT / LONGTEXT

Dates:

- DATETIME (YYYY-MM-GG HH:II:SS) / DATE (YYYY-MM-GG) / TIME (HH:II:SS) / YEAR (YYYY) / TIMESTAP 


# Table name: cars

## Entity name: Car

## Table columns:

- id                                            | BIGINT - PRIMARY_KEY, UNIQUE, AUTO_INCREMENT, NOTNULL, INDEX
- brand                                         | VARCHAR(30) - NOTNULL, INDEX
- model                                         | VARCHAR(50) - NOTNULL, INDEX
- vehicle_class                                 | VARCHAR(30) - NULL, INDEX
- engine (carburante)                           | VARCHAR(20) - NOTNULL, INDEX
- engine_capacity (cilindrata)                  | VARCHAR(10) - NULL
- color                                         | VARCHAR(20) - NULL
- year                                          | YEAR - NULL, INDEX
- km (chilometraggio)                           | MEDIUMINT - NOTNULL, INDEX
- transmission (cambio)                         | VARCHAR(20) - NULL
- car_door (portiere)                           | TINYINT - NULL
- seats (sedili)                                | TINYINT - NULL
- emission_class (classe di emissione)          | CHAR(5) - NULL
- co2_emission (emissioni di co2)               | VARCHAR(20) - NULL
- consumption (consumi)                         | VARCHAR(20) - NULL
- previous_owners (proprietari precedenti)      | TINYINT - NULL
- country_of_origin (paese di origine)          | VARCHAR(20) - NULL
- ?service_history? (storico tagliandi)         | //
- last_maintenance (ultima manutenzione)        | DATE - NULL
- car_crashed_and_repaired                      | TINYINT (true or false) - DEFAULT(0)
- license_plate (targa)                         | CHAR(7) - UNIQUE, NOTNULL
- vin (telaio)                                  | CHAR(17) - NOTNULL, UNIQUE, INDEX
- price                                         | DECIMAL(9, 2) - NOTNULL, INDEX
- availability (disponibilità)                  | TINYINT - NULL, INDEX
- note                                          | TEXT - NULL