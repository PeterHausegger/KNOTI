<p align="center">
  <img src="knoti-logo.svg" width="140" alt="KNOTI Logo">
</p>

<h1 align="center">KNOTI</h1>

<p align="center">
  <b>Parametric nodes for building geometric structures from rods</b><br>
  <b>Parametrische Knoten für Strebenkonstruktionen und geometrische Körper</b>
</p>

<p align="center">
  <a href="https://peterhausegger.github.io/KNOTI/"><b>Open the tool / Werkzeug öffnen</b></a> ·
  <a href="https://peterhausegger.github.io/KNOTI/galerie.html">Gallery / Galerie</a> ·
  <a href="https://creativecommons.org/licenses/by-sa/4.0/">CC BY-SA 4.0</a>
</p>

<p align="center">
  <a href="#english">English</a> · <a href="#deutsch">Deutsch</a> · <a href="#contact">Contact / Kontakt</a>
</p>

---

<a id="english"></a>

## English

KNOTI is a free browser tool for designing nodes that join rods into geometric structures: from a single star node to a complete kit for a geodesic dome. You set a few values, KNOTI draws the parts and exports files for the laser cutter, the cutting plotter or the 3D printer.

KNOTI is made for teaching technology and design (Maker Education). Learners can go from a spatial idea to a buildable model and see directly how angles, edge lengths and materials depend on each other.

### Try it

Open **https://peterhausegger.github.io/KNOTI/** in a current browser (Chrome, Edge, Firefox, Safari), also on tablets. Nothing to install, no account, no data is uploaded. The whole tool is one HTML file and also works offline: download `index.html` and open it locally.

### Building in five steps

The sidebar follows the order in which you build:

1. **What to build?** Single node or a whole body.
2. **Which node type?** Star, cone or 3D node.
3. **Node shape:** number of arms, arm length and width, angles, corner radius.
4. **Rods:** width and length of the rods.
5. **Connection:** holes, tabs, hooks, cone seam or slot fold, each with its own settings.

### Three node types

| Type | Production | Description |
|---|---|---|
| **Star** | laser cutter, plotter, scissors | Flat star, the arms are folded at the blue fold lines. Simple and light, good for cardboard, thin wood or plastic sheets. |
| **Cone** | laser cutter, plotter | Flat sector that is rolled into a cone. Stiffer and true to the spatial angles; not buildable at saddle points. |
| **3D node** | 3D printer | Printed body with collars. The rods go into holes, or tubes slide over pegs. Round or square profile, optional flat side with a small embossed label for printing without supports. |

### Two modes

**Single node:** one part with freely chosen number of arms, angles and arm lengths.

**Body:** a complete kit for a whole body, with one node per corner, all rods and a build plan. Available bodies: tetrahedron, cube, octahedron, icosahedron, dodecahedron, geodesic sphere and dome (adjustable frequency), pyramid and frustum, box with angle, prism, antiprism, bipyramid, space grid, or your own model via **file import (STL or OBJ)**. With OBJ, every edge of the model becomes a rod exactly as modelled; wire models made of lines work too.

### Features

- **Construction with or without rods.** Without rods the arms of neighbouring nodes form the edges themselves (butting or overlapping).
- **Connection methods:** holes, tabs with optional barbs, hooks, cone seam, slot fold. Several can be combined. With tabs and hooks together you choose between two separate rod sets or tab rods that also carry hooks.
- **Centre hole and centre slot:** a hole in the middle of the star, or one slot per arm in the middle that forms a small star to plug something into.
- **Exact arm angles (star, body mode):** every rod is projected onto the centre plate of the node, every arm gets its own fold angle, printed on the part. Folded, each arm points exactly along its rod.
- **Every corner gets its own name** (A1, B7, ...), every arm names its neighbour, every rod names both ends. Identical letters mean identical parts.
- **Lego / Duplo presets:** hole grid 8 mm or 16 mm; for the star with a centre hole, all holes sit on the grid.
- **Laser details:** double layer (inner and outer shell), kerf compensation, corner radius, sheet layout on A4, A3 or your own laser bed.
- **3D printing details:** print tolerance for holes and pegs, export quality standard or fine.
- **3D view** of the body and the 3D nodes, rendered by the graphics card, rotatable and zoomable.
- **German and English** user interface.

### Exports

| Button | File | Content |
|---|---|---|
| Nodes (SVG) | `.svg` | all nodes, in colour layers for laser and plotter |
| Rods (SVG) | `.svg` | rods with holes, tabs, hooks, length and labels |
| Cut list (TXT) | `.txt` | rod lengths, number of parts per type, fold angles, assembly list |
| Build plan (PDF) | print view | A4 pages with 3D views, measurements and assembly order |
| STL | `.stl` / `.zip` | 3D node, or star and cone nodes for 3D printing; one file per node type in body mode |

The file names contain the most important measurements, so a part can be rebuilt from its name alone. Under *Output* you can switch individual colour layers off and add a **QR code** to the build plan that links back to exactly this setting.

### Colour code in the SVG files

| Colour | Meaning |
|---|---|
| red | cut (outline) |
| blue | rod end / fold line |
| magenta | crease / scoring line |
| black | holes and slots (cut) |
| purple | node labels |
| turquoise | additional information (lengths, fold angles, QR code); can be switched off for export |

### Saving and sharing

- **Undo / redo** with Ctrl+Z and Ctrl+Shift+Z.
- **Remember:** name and keep settings in your browser; the current state is kept automatically as "last state".
- **Save / Load:** a small `.knoti.json` file that can be loaded into any later version.
- **Share as link:** the complete setting is compressed into the web address. Whoever opens the link sees exactly your design.

### Quick start

1. Choose **Single node** or **Body**.
2. Choose the node type: **Star**, **Cone** or **3D node**.
3. Set the measurements: edge length, arm width, material thickness, connection.
4. Export, cut or print, assemble.

The **?** buttons next to the controls explain each setting.

### Background

KNOTI is developed by Peter Hausegger in the context of a doctoral project on Maker Education in Austrian technology and design teaching, following a design-based research approach. Feedback from classrooms, workshops and teacher education flows directly into new versions. Photos of projects built with KNOTI are welcome in the [gallery](https://peterhausegger.github.io/KNOTI/galerie.html).

### License

© 2026 Peter Hausegger. KNOTI is licensed under **[Creative Commons Attribution-ShareAlike 4.0 (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/)**, see [`LICENSE`](LICENSE). You may use, share and adapt it, also commercially, as long as you credit the author and share adaptations under the same license.

Parts produced with KNOTI (SVG, STL, build plans) are yours to use freely.

Third-party code included in `index.html`: [polygon-clipping](https://github.com/mfogel/polygon-clipping) (MIT, with splaytree, MIT), [earcut](https://github.com/mapbox/earcut) (ISC) and [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) by Kazuhiko Arase (MIT). LEGO and DUPLO are trademarks of the LEGO Group, which does not sponsor or endorse this project.

---

<a id="deutsch"></a>

## Deutsch

KNOTI ist ein freies Browser-Werkzeug zum Entwerfen von Knoten, mit denen sich Streben zu geometrischen Körpern zusammenbauen lassen: vom einzelnen Sternknoten bis zum kompletten Bausatz für eine geodätische Kuppel. Du stellst einige Werte ein, KNOTI zeichnet die Teile und erzeugt Dateien für Lasercutter, Schneideplotter oder 3D-Drucker.

KNOTI ist für den Unterricht in Technik und Design (Maker Education) gemacht. Lernende kommen von einer räumlichen Idee zum baubaren Modell und sehen dabei direkt, wie Winkel, Kantenlängen und Material zusammenhängen.

### Ausprobieren

**https://peterhausegger.github.io/KNOTI/** in einem aktuellen Browser öffnen (Chrome, Edge, Firefox, Safari), auch auf dem Tablet. Keine Installation, kein Konto, es werden keine Daten hochgeladen. Das ganze Werkzeug ist eine einzige HTML-Datei und funktioniert auch offline: `index.html` herunterladen und lokal öffnen.

### In fünf Schritten bauen

Die Seitenleiste folgt der Reihenfolge beim Bauen:

1. **Was bauen?** Einzelknoten oder ganzer Körper.
2. **Welcher Knotentyp?** Stern, Kegel oder 3D-Knoten.
3. **Knotenform:** Armzahl, Armlänge und -breite, Winkel, Eckenabrundung.
4. **Streben:** Breite und Länge der Streben.
5. **Verbindung:** Löcher, Zapfen, Haken, Kegelnaht oder Steckfalz, jeweils mit eigenen Einstellungen.

### Drei Knotentypen

| Typ | Fertigung | Beschreibung |
|---|---|---|
| **Stern** | Lasercutter, Plotter, Schere | Flacher Stern, die Arme werden an den blauen Knicklinien gefaltet. Einfach und leicht, gut für Karton, dünnes Holz oder Kunststoffplatten. |
| **Kegel** | Lasercutter, Plotter | Flacher Sektor, der zum Kegel gerollt wird. Formstabiler und winkeltreu; an Sattelpunkten nicht baubar. |
| **3D-Knoten** | 3D-Drucker | Gedruckter Körper mit Kragen. Die Streben stecken in Bohrungen, oder Rohre werden über Zapfen geschoben. Runder oder eckiger Querschnitt, optional mit flacher Seite und kleiner eingeprägter Beschriftung für den Druck ohne Stützen. |

### Zwei Modi

**Einzelknoten:** ein Teil mit frei wählbarer Armzahl, eigenen Winkeln und Armlängen.

**Körper:** ein kompletter Bausatz für einen ganzen Körper, mit einem Knoten pro Ecke, allen Streben und einem Bauplan. Verfügbare Körper: Tetraeder, Würfel, Oktaeder, Ikosaeder, Dodekaeder, geodätische Kugel und Kuppel (Frequenz einstellbar), Pyramide und Pyramidenstumpf, 8-Ecken-Körper mit Neigung, Prisma, Antiprisma, Doppelpyramide, Raumgitter oder ein eigenes Modell per **Datei-Import (STL oder OBJ)**. Bei OBJ wird jede Kante des Modells genau so zur Strebe, wie sie modelliert wurde; auch Drahtmodelle aus Linien funktionieren.

### Funktionen

- **Mit oder ohne Streben bauen.** Ohne Streben bilden die Arme benachbarter Knoten selbst die Kanten (mittig stoßend oder überlappend).
- **Verbindungsarten:** Löcher, Zapfen mit wahlweisem Widerhaken, Haken, Kegelnaht, Steckfalz. Mehrere lassen sich kombinieren. Bei Zapfen und Haken zusammen wählst du zwischen zwei getrennten Strebensätzen oder Zapfenstreben, die zusätzlich Haken tragen.
- **Mittelloch und Mittelschlitz:** ein Loch in der Mitte des Sterns, oder je Arm ein Schlitz in der Mitte, die zusammen einen kleinen Stern zum Einstecken bilden.
- **Exakte Armwinkel (Stern, Körpermodus):** Jede Strebe wird auf die Mittelplatte des Knotens projiziert, jeder Arm bekommt seinen eigenen Faltwinkel, der auf dem Teil steht. Gefaltet zeigt jeder Arm genau in Strebenrichtung.
- **Jede Ecke hat einen eigenen Namen** (A1, B7, ...), jeder Arm nennt seinen Nachbarn, jede Strebe beide Enden. Gleicher Buchstabe heißt gleiches Teil.
- **Lego-/Duplo-Vorlagen:** Lochraster 8 mm bzw. 16 mm; beim Stern mit Mittelloch, alle Löcher liegen im Raster.
- **Laser-Details:** Doppellage (Innen- und Außenschale), Schnittfugen-Korrektur, Eckenabrundung, Blattaufteilung auf A4, A3 oder den eigenen Laserbereich.
- **3D-Druck-Details:** Drucktoleranz für Bohrungen und Zapfen, Export-Qualität Standard oder Fein.
- **3D-Ansicht** des Körpers und der 3D-Knoten, von der Grafikkarte gezeichnet, dreh- und zoombar.
- Bedienoberfläche auf **Deutsch und Englisch**.

### Exporte

| Knopf | Datei | Inhalt |
|---|---|---|
| Knoten (SVG) | `.svg` | alle Knoten, in Farbebenen für Laser und Plotter |
| Streben (SVG) | `.svg` | Streben mit Löchern, Zapfen, Haken, Länge und Beschriftung |
| Schnittliste (TXT) | `.txt` | Strebenlängen, Stückzahl je Typ, Faltwinkel, Zusammenbau-Liste |
| Bauplan (PDF) | Druckansicht | A4-Seiten mit 3D-Ansichten, Maßen und Bauanleitung |
| STL | `.stl` / `.zip` | 3D-Knoten oder Stern- und Kegelknoten für den 3D-Druck; im Körpermodus eine Datei je Knotentyp |

Die Dateinamen enthalten die wichtigsten Maße, ein Teil lässt sich also allein aus dem Namen nachbauen. Unter *Ausgabe* lassen sich einzelne Farbebenen abschalten und ein **QR-Code** auf den Bauplan setzen, der zurück zu genau dieser Einstellung führt.

### Farbcode in den SVG-Dateien

| Farbe | Bedeutung |
|---|---|
| rot | schneiden (Umriss) |
| blau | Strebenende / Knicklinie |
| magenta | Faltlinie / Falz (ritzen) |
| schwarz | Bohrungen und Schlitze (schneiden) |
| lila | Knoten-Beschriftung |
| türkis | Zusatzinfo (Längen, Faltwinkel, QR-Code); beim Export abschaltbar |

### Speichern und Teilen

- **Zurück / Vor** mit Strg+Z und Strg+Umschalt+Z.
- **Merken:** Einstellungen unter einem Namen im Browser ablegen; der aktuelle Stand wird automatisch als "letzter Stand" gemerkt.
- **Speichern / Laden:** eine kleine `.knoti.json`-Datei, die sich in jede spätere Version laden lässt.
- **Als Link teilen:** die komplette Einstellung steckt komprimiert in der Adresse. Wer den Link öffnet, sieht genau deinen Entwurf.

### Schnellstart

1. **Einzelknoten** oder **Körper** wählen.
2. Knotentyp wählen: **Stern**, **Kegel** oder **3D-Knoten**.
3. Maße einstellen: Kantenlänge, Armbreite, Materialstärke, Verbindung.
4. Exportieren, schneiden oder drucken, zusammenbauen.

Die **?**-Knöpfe neben den Reglern erklären jede Einstellung.

### Hintergrund

KNOTI wird von Peter Hausegger im Rahmen eines Dissertationsprojekts zu Maker Education im österreichischen Technik-und-Design-Unterricht entwickelt (Design-Based Research). Rückmeldungen aus Unterricht, Workshops und Lehrer:innenbildung fließen direkt in neue Versionen ein. Fotos von Projekten, die mit KNOTI entstanden sind, sind in der [Galerie](https://peterhausegger.github.io/KNOTI/galerie.html) willkommen.

### Lizenz

© 2026 Peter Hausegger. KNOTI steht unter der Lizenz **[Creative Commons Namensnennung - Weitergabe unter gleichen Bedingungen 4.0 (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/deed.de)**, siehe [`LICENSE`](LICENSE). Du darfst das Werkzeug nutzen, weitergeben und verändern, auch kommerziell, solange du den Urheber nennst und Bearbeitungen unter derselben Lizenz weitergibst.

Mit KNOTI erzeugte Teile (SVG, STL, Baupläne) darfst du frei verwenden.

In `index.html` enthaltener Fremdcode: [polygon-clipping](https://github.com/mfogel/polygon-clipping) (MIT, mit splaytree, MIT), [earcut](https://github.com/mapbox/earcut) (ISC) und [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) von Kazuhiko Arase (MIT). LEGO und DUPLO sind Marken der LEGO Gruppe, die dieses Projekt weder unterstützt noch empfiehlt.

---

<a id="contact"></a>

## Contact / Kontakt

**Peter Hausegger**
Kirchliche Pädagogische Hochschule Edith Stein, Innsbruck / Stams

E-Mail: peter.hausegger [at] kph-es.at

Questions, ideas, bug reports and photos of your projects are very welcome, in German or English. For bugs, a shared link (*Share as link*) helps a lot, because it contains the exact setting.

Fragen, Ideen, Fehlermeldungen und Fotos eurer Projekte sind sehr willkommen, auf Deutsch oder Englisch. Bei Fehlern hilft ein geteilter Link (*Als Link teilen*) sehr, weil darin die genaue Einstellung steckt.

Bug reports are also possible via [GitHub Issues](https://github.com/PeterHausegger/KNOTI/issues). / Fehlermeldungen gehen auch über [GitHub Issues](https://github.com/PeterHausegger/KNOTI/issues).
