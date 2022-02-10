---
  session-id: 'session-38'
  title: 'Datenbanktests in 1 Zeile mit JUnit Jupiter Extensions'
  abstract: |
    Tests müssen einfach und kurz geschrieben werden, sonst macht's keiner. Gleichzeitig soll eine Testsuite schnell durchlaufen, selbst wenn ein komplexes Setup wie eine Datenbankinitialisierung nötig ist.

    Bei JUnit 4 fallen einem Setup und Teardown Methoden ein, als querschnittliche Lösung vielleicht noch Rules und Runners. Aber wie funktioniert das bei JUnit 5 (Jupiter) im Detail? Und kann das soweit optimiert werden, dass nicht jeder einzelne Test eine eigene Datenbank komplett initialisieren muss? Was passiert, wenn die Tests dann noch parallel ausgeführt werden und um die Datenbank konkurrieren?

    In diesem Vortrag zeige ich, wie eine Datenbankverbindung mithilfe von JUnit 5 Extensions mit minimalem Aufwand an Tests angebunden werden kann. Der Fokus liegt dabei auf Testperformance und Parallelität.
  meetupId: cyberland-ng-2
  speaker-id: 'philipp-hannemann'
  layout: session
---
