Consegna:
- Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.

# Entity name: Car

# Table name: cars

- id | BIGINT - PRIMARY_KEY, UNIQUE, AUTO_INCREMENT, NOT NULL
- brand | VARCHAR(30) - NOT NULL
- model | VARCHAR(50) - NOT NULL
- vehicle_class | VARCHAR(30) - NULL
- engine (carburante) | VARCHAR(20) - NULL
- engine_capacity (cilindrata) | VARCHAR(10) - NULL
- color | VARCHAR(20) - NULL
- year | YEAR - NULL
- mileage (chilometraggio) | MEDIUMINT - NULL
- transmission (cambio) | VARCHAR(20) - NULL
- car_door (portiere) | TINYINT - NULL
- seats (sedili) | TINYINT - NULL
- emission_class (classe di emissione) | CHAR(6) - NULL
- co2_emission (emissioni di co2) | VARCHAR(20) - NULL
- consumption (consumi) | VARCHAR(20) - NULL
- previous_owners (proprietari precedenti) | TINYINT - NULL
- country_of_origin (paese di origine) |  VARCHAR(20) - NULL
- ?service_history? (storico tagliandi) | //
- last_maintenance (ultima manutenzione) | DATE - NULL
- car_crashed_and_repaired | TINYINT (true or false) - DEFAULT(0)
- license_plate (targa) | CHAR(7) - UNIQUE, NOT NULL
- price | DECIMAL(9, 2) - NOT NULL
- availability (disponibilità) | TINYINT - NULL