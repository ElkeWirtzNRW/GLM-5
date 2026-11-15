# Repositoryweite Agenten- und Arbeitsregeln

## Verbindliche systemweite Entwicklungs-, Versions- und QS-Regel (15.11.2026)

**Originalanweisung Elke Wirtz (unverändert):**

> Ich möchte Entwicklung statt immer von vorne anzufangen.
> Testdatenbanken nicht neu erstellen oder mit Versionen in Archiv Datenbank hinterlegen.
> Ich will mit dem System nachvollziehen können wie der Verlauf der Entwicklung gelaufen ist.
> Desweiteren müssen erfolgreiche Test in der MariaDB in GitHub synchronisiert werden oder abgelegt werden wenn noch nicht vollständig eingefügt.
> QS in allen Vorgängen durchführen.
> Fehlerquote 0%

**Geltung und Umsetzung:** Für alle Repositorys, Chats, Teams und Agenten gilt: Vorhandene Arbeit, Projektanweisungen, Checkpoints, Dateien, offene Issues/PRs, Datenbankverträge und Freigabegates vor Änderungen prüfen und den bestehenden Entwicklungsstrang fortführen; keine parallelen Neuaufbauten. Jede Änderung und jeder Test erhält nachvollziehbare Referenzen auf Auftrag, Modul, Commit, Issue/PR, Testlauf, Ergebnis, QS und Freigabestatus. Durchgängige QS vor, während und nach Änderungen einschließlich Integrations- und Regressionstests; Ziel ist eine Fehlerquote von 0 %, ohne ungeprüfte Fehlerfreiheit zu behaupten. Bestehende Inhalte nicht löschen oder überschreiben; Freigaben und Projektsperren respektieren.

**Für Repositorys mit MariaDB-/GitHub-Entwicklungsumgebung:** Bestehende persistente Entwicklungsdatenbanken wiederverwenden; keine Testdatenbank als Ersatz für den Entwicklungsbestand neu aufbauen. Erforderliche isolierte CI-Tests strikt trennen. Vorhandene Archivdatenbank und Versionierungsstrukturen vor Änderungen prüfen. Erfolgreiche Tests dem Entwicklungsstand in MariaDB zuordnen und synchronisieren; solange das technisch nicht implementiert ist, unveränderliche GitHub-Testreferenzen mit offener Synchronisierungskennzeichnung dokumentieren. Keine behauptete Datenbank-Synchronisierung ohne tatsächlichen Schreib- und Rücklesetest. GitHub-Codespace-/CI-MariaDB und produktive Webhosting-MariaDB bleiben getrennt.

**Querverweis:** https://github.com/ElkeWirtzNRW/tmmbusiness360-/issues/15#issuecomment-6897648585 . Diese Ergänzung erteilt keine Freigabe für produktive Änderungen, neue Datenbanken, Merge oder Veröffentlichung.
