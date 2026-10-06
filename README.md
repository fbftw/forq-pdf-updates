# FORQ PDF – Setup und Updates

Dieses Repository enthält **nur die veröffentlichten Dateien** von FORQ PDF, keinen Quellcode.

- **Erstinstallation:** `FORQ-PDF-Setup.exe` aus dem [neuesten Release](https://github.com/fbftw/forq-pdf-updates/releases/latest) herunterladen und ausführen. Es sind keine Administratorrechte nötig.
- **Updates:** FORQ PDF fragt hier beim Start selbst nach einer neueren Fassung und bietet sie an („Jetzt aktualisieren?“).

## Dateien je Release

| Datei | Zweck |
|---|---|
| `FORQ-PDF-Setup.exe` | Installation bzw. manuelles Update |
| `freigabe.json` | signierte Freigabe (Fassung, Prüfsumme des Pakets) |
| `FORQ-PDF-<Fassung>.forqcomponent` | Update-Paket für die automatische Aktualisierung |
| `*.sha256` | Prüfsummen |

FORQ PDF nimmt ein Update nur an, wenn `freigabe.json` mit dem Freigabeschlüssel der FORQ-Familie signiert ist und das Paket genau zur signierten Prüfsumme passt. Eine veränderte oder untergeschobene Datei wird abgelehnt.
