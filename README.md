# LaTeX-Package für WHS-Abschlussarbeiten

Dieses LaTeX-Package erstellt die Titelseite sowie die eidesstattliche Erklärung für WHS-Abschlussarbeiten.

# Einbinden

Die Dateien `whsthesis.sty` und `background.png` in das LaTeX-Projekt kopieren. Anschließend in der LaTeX-Main-Datei das Package wie folgt einbinden:

```latex
\usepackage{whsthesis}
```

# Einrichten

Vor der Verwendung müssen unterschiedliche Variablen mit den Paramteren der Abschlussarbeit gesetzt werden. Folgende Variablen müssen zwangsweise gesetzt werden:

- `\whsThesisTitle`
- `\whsThesisType`
- `\whsDegree`
- `\whsFirst`
- `\whsLast`
- `\whsPlaceOfBirth`
- `\whsCourseOfStudy`
- `\whsDepartment`
- `\whsFirstExaminer`
- `\whsSecondExaminer`

Andere Variablen können optional gesetzt werden: 

- `\whsPlace` (default: Bocholt)
- `\whsDateOfSubmission` (default: \today)
- `\whsBackgroundImage{<customPath>/background}` (Pfad zum Speicherort der background.png-Datei, default: img/background)

# Befehle

## Hintergrund

```latex
\whsBackground
```

legt für die aktuelle Seite das WHS-Hintergrundbild an

## Titelseite

```latex
\whsTitlePage
```

erstellt die Titelseite entsprechend der Vorgaben aus dem Moodle

## Eidesstattliche Erklärung

```latex
\whsStatutoryDeclaration
```

erstellt die eidesstattliche Erklärung entsprechend der Vorgaben aus dem Moodle

# Beispiel

Eine Beispieldatei ist im Verzeichnis `example` angefügt.
