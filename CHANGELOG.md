# Changelog

Tutte le modifiche rilevanti a questo modulo sono documentate in questo file.

Il formato è basato su [Keep a Changelog](https://keepachangelog.com/it/1.1.0/)
e questo progetto aderisce al [Semantic Versioning](https://semver.org/lang/it/).

## 1.0.5

- Fix: aggiunto `etc/acl.xml` (la risorsa della sezione di configurazione non era dichiarata, quindi non assegnabile ai ruoli); corretta la descrizione del comando `Disable`.

## [1.0.4] - 2026-07-08

### Fixed
- Compatibilità PHP 8.4: parametro `$name` del costruttore reso nullable esplicito (`?string`) e tipo di ritorno `int` sul metodo `execute()` dei comandi console `Enable` e `Disable`. Assorbe le patch composer PHP 8.4 che il progetto store applicava su questo modulo.

## [1.0.3] - 2026-06-19

### Fixed
- `events.xml`: corretto il nome dell'evento, ora allineato all'id della sezione (`admin_system_config_changed_section_threecommerce_maintenance`), così l'observer `ConfigSaveObserver` viene effettivamente eseguito al salvataggio della configurazione.
- `system.xml`: corretto `showInDefault` del campo `ipList` da `6` (valore non valido) a `1`.

## [1.0.2] - 2026-06-01

## [1.0.1] - 2025-05-08

## [1.0.0] - 2025-04-29

- Prima release del modulo Magento 2 per la modalità di manutenzione.