# Cyberland

Dieses Repository beinhaltet die auf Jekyll basierte Webseite des Cyberland.

## Aktueller Aufbau (Cyberland März 2020)

Aktuell werden auf der `index.html` die Infos zum Cyberland im März 2020 dargestellt. Für weitere Events kann jeweils eine markdown Datei unter `pages/events` angelegt werden. Damit dieses Event in der Navigation angezeigt werden kann muss die Property `title` im Metadaten-Header der Datei gesetzt werden (vergleiche andere Events). Der Inhalt einer Event-Seite kann frei gestaltet werden. Es gibt unter `_includes_/elements` ein paar Komponenten (z.B. ein Session-Grid) welche wiederverwendet werden können. 

## Styling der Webseite

Als Basis CSS für die Seite wird Bulma.io genutzt. Zusätzlich wirde FontAwesome hinzugefügt.
Spezifische CSS Regeln müssen in `_sass_/main.scss` hinzugefügt werden. Variablen von Bulma.io können in `_sass_/variables.scss` überschrieben werden. Der globale Eintrittspunkt ist die Datei `assets/css/styles.scss`. Diese sollte allerdings nicht angepasst werden.

## Events / Vorträge hinzufügen oder anpassen

TODO

### Einen neuen Speaker anlegen

Ein neuer Speaker kann in der YAML Datei `data/speakers.yml` angelegt werden. Bereits vorhandene Einträge in der Datei können als Vorlage dienen.

Zusätzlich muss unter `assets/speaker/` ein Avatar-Bild (PNG) des Speakers hinterlegt werden. Hierbei muss folgendes beachtet werden:

* Das Bild muss die Dimension 000x000 (TODO) haben.
* Das Bild muss ein PNG sein.
* Der Dateiname des Bildes muss der `id` des Speakers entsprechen. Beispiel: Für einen Speaker mit der `id` `max-mustermann` muss das PNG `max-mustermann.png` heißen.

### Einen neuen Vortrag anlegen

Für jeden Vortrag muss eine neue markdown Datei unter `_sessions/` angelegt werden. Da für jeden Vortrag eine individualle Seite generiert werden soll, können nicht einfach alle Vorträge in einer YAML Datei unter `data/` erfasst werden. Bereits vorhandene Dateien können als Vorlage dienen.

### Generierung der Vortragsseite

Zu jedem Vortrag wird automatisch eine Seite generiert. Hierfür wird die Datei `_layouts/session.html` als Template genutzt.