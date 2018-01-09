
Review Strict Confluent Graph Drawing
=====================================

Zusammenfassung/Inhalt
----------------------

% kurze Beschreibung des Inhalts der Ausarbeitung in eigenen Worten (nicht Abstract)
Die Arbeit ist über das Thema strict confluent drawings von Graphen. Anschaulich erklärt sind confluent drawings vergleichbar mit einem Schienennetz (Kanten), bei dem zwei Bahnhöfe (Knoten) A und B miteinander verbunden sind, wenn ein Zug von A startet und ohne umzukehren direkt (ohne Zwischenbahnhof) B erreichen kann. Durch Kanten die sich als Tangenten berühren, werden unübersichtliche crossings in nicht-planaren Graphen vermieden. Strict confluent drawings gehen noch weiter, indem ein Pfad von einem beliebigen Knoten A nach B eindeutig sein muss, sowie keine Kante denselben Knoten als Anfang und Ende hat. Diese Arbeit behandelt zunächst die Grundlagen des Themas, beleuchtet anschließend im Hauptteil die Komplexität des Problems (NP-vollständig), ob ein gegebener Graph ein strict confluent drawing besitzt. Außerdem behandelt die Arbeit einen Algorithmus, welcher erkennt ob ein Graph ein outer planar strict confluent drawing besitzt, bei dem alle Knoten entlang eines Kreises angeordnet sind und alle Kanten innerhalb des Kreises sind.


% Was ist die Problemstellung und das Ziel in der Ausarbeitung?
Das Ziel ist es, einen Einblick in das Forschungsgebiet der strict confluent drawings zu bieten und für ein aktuelles Paper anhand eigener anschaulicher Ausarbeitungen der dort vorhandenen Ergebnisse, ein tieferes und schnelleres Verständnis zu bieten.


% Was sind die Ergebnisse?
Das Ergebnis ist eine kompakte Einführung in das Thema, welches einerseits einen Überblick über State-of-the-art und open questions bietet, andererseits auch detaillierte Ergebnisse eines aktuellen Papers erläutert.



Einschätzung/Evaluation
-----------------------

% ... Stärken und Schwächen des Textes

% Was ist gut und anschaulich / unklar beschrieben, wo sind Fehler in Argumenten?

Die Einleitung ist verständlich und Bildhaft geschrieben. Gibt es zu der Behauptung eine kurze Begründung (grundsätzliche Idee warum das funktioniert) warum confluent drawings Vorteile gegenüber edge bundling bei false adjacencies, unambiguity und information faithfulness haben?
Related Work beinhaltet einige neue Konzepte, auf die nicht erklärend eingegangen wird, wäre aber vermutlich overkill alles zu erklären.

Guter Start in Punkt 5 bei der Erklärung, dass es der Beweis im Originalpaper erklärt und mit einer anderen Herangehensweise erklärt wird, damit man das Original besser versteht. Auch die Begründung, dass solche Beweise öfters im Bereich Algorithmik Geometry vorkommen, weckt im Leser vermutlich Interesse, diese Arbeit (speziell diesen Teil) als für ihn relevant einzustufen.

Es scheint alles gut argumentiert zu sein, wenn auch durch die Komplexität des Themas es sehr schwierig ist zu verstehen.

Bei Lemma 3.2 kann ich das Argument nicht nachvollziehen, dass alle 4 vertices des K_{2,2} Subgraphen einen Grad von mindestens 3 haben müssen, "as we have transformed all edges incident to degree-2 vertices into direct edges that do not pass through any junctions". Die Fallunterscheidung bei Lemma 3.1 Abbildung 4 (first case) zeigt bei der Transformation, dass die unteren beiden Knoten zwei neue Kanten wegführen. Ist der Grad eines Knoten im Beispiel Abbildung 4 im transformed drawing größer als im original drawing? Wie ist der Grad eines Knoten in so einem Drawing definiert? 

Ist ein grid graph eine connected component (z.B. für x_1) oder die ganze Zeichnung (also x_1 + x_2 + x_3  usw)? Laut Text verstehe ich dass jede connected component ein grid graph ist, die Bezeichnung der Abbildung 7 sagt, alles zusammen ist ein einziger grid graph

Ist ein "subdivision vertex" jener Knoten in der Mitte der 3 Knoten einer grünen bzw. roten Kante?

Bei Lemma 4.1, warum gibt es bei der zweiten Fallunterscheidung nur die Möglichkeit, dass ein Circle eine einzige Junction hat, und nicht mehrere?

Wo wird definiert was ein "face" ist?

Bei 5.1 NP-Hardness, haben alle "resulting graphs" ein planares embedding? Gilt diese Aussage wirklich allgemein? 
-> Was ist wenn in diesem Beispiel noch eine clause "-x_3 v -x_4 v x_5" dabei wäre, also in Folge dessen zwei clauses mit denselben Variablen aber unterschiedlichen Vorzeichen?


Seite 10: "at least one variable in a positive literal is true" ... meinst du clause statt literal? Literal bestehen ohnehin nur aus einer Variable


Bei "7 Algorithm" im 1. Punkt des algorithm overview, was genau ist mit "neighbor" gemeint? Immer der im Kreis im Uhrzeigersinn/Gegenuhrzeigersinn anzutreffende Nachbar eines Knoten? Der nächste Knoten den man bekommt wenn man einen Pfad im Uhrzeigersinn/Gegenuhrzeigersinn folgt? 
-> Wozu braucht man "let x be the next neighbor of y that is (counter)clockwise of z" und nicht einfach "let x bet the next (counter)clockwise neighbor of y"?

Die Grafiken sind alle passend und übersichtlich!


% Wie interessant und innovativ sind die Ergebnisse/verwendeten Techniken? (= Bewertung Original-Paper)


% Titel passend?
Im Sinne einer Seminararbeit ist der Titel passend, da die Ausarbeitung einen Überblick über das Thema geben soll. Für eine wissenschaftliche Arbeit die veröffentlicht wird, würde man wohl einen spezifischeren Namen geben.


% aussagekräftiger Abstract?
Womöglich wäre auch die grundlegende Idee im Abstract sinnvoll, was der Vorteil von (strict) confluent drawings gegenüber anderen Techniken sind.

% Motiviert Einleitung gut die Problemstellung?
Gute und verständliche Einleitung! Womöglich wäre noch ein Bild von einem größeren Graphen sinnvoll, bei dem confluent drawings die visuelle Komplexität deutlich verbessern (z.B. Hasse Diagramm aus den Folien (?)).

% ausreichende Quellenangaben für Aussagen, Behauptungen, ausgelassene Beweise?
Quellenangaben scheinen durchgängig vorhanden wo es um Aussagen geht, die nicht vom Original-Paper kommen... Gut!


% hilfreiche und kompakte Abbildungen für Aussagen?
Die Abbildungen sind sehr gut! Ab und an noch eine zusätzliche Grafik wäre sicherlich förderlich, um Leser mit wenig Erfahrung im Gebiet Graphenzeichnen schneller verstehen zu lassen.


% Wird auf Schwächen der beschriebenen Algorithmen und Ergebnisse eingegangen?
Ich kann mich erinnern, in der Präsentation hast du gesagt, das Originalpaper hat nur wenige Grafiken verwendet und dadurch war es mühsam alles zu verstehen. Das könnte man durchaus noch stärker hervorheben, dass diese Seminararbeit das besser/leichter für den Leser machen möchte.


% Text sinnvoll strukturiert?
Wenn ich das richtig verstehe sind es zwei verschiedene Probleme/Algorithmen (strict confluent drawing und outer planar strict confluent drawing Erkennung) die in der Ausarbeitung behandelt werden. Ich finde die Struktur könnte konkreter auf diese Algorithmen abgestimmt sein, und nicht z.B. "Canonical diagrams" und "Algorithm" als top level Überschriften. Wenn man die Arbeit schnell mal drüberblättert, kann genau das den Unterschied ausmachen, ob dieser Teil (oder überhaupt die ganze Arbeit) gelesen wird oder nicht. "Algorithm" ist z.B. sehr allgemein und ohne den übergeordneten Kontext nicht aussagekräftig. Wenn man "Canonical diagrams" nicht kennt und man nicht weiß dass es dabei auch um outer planar strict confluent drawings geht, blättert man womöglich drüber.


% Seitenumfang angemessen? (12-15 Seiten)
Seitenumfang passt!


% sprachliche Qualität?
Sprachlich ist der Text sehr gut verfasst. Ich denke die Komplexität beim Lesen kommt vor allem durch das Thema selbst. Die geschriebenen Sätze sind im Normalfall nicht zu lang und auch nicht zu verschachtelt.


% Gesamteindruck der Ausarbeitung? z.B. "sehr gut, kaum Kritikpunkte", "gut, mehrere kleinere Korrekturen und wenige größere Korrekturen nötig", "noch viele größere Korrekturen erforderlich"
Gesamt gesehen wirkt die Ausarbeitung auf mich gut durchdacht und vollständig. Ein paar kleinere Korrekturen könnte man vornehmen, womöglich auch je nachdem welche Zielgruppe man mit dieser Ausarbeitung bedienen will (je nachdem, für Anfänger in diesem Bereich ggf. noch etwas mehr mit Grafiken arbeiten?... Liegt aber womöglich auch an mir.)



Liste größerer Kritikpunkte
---------------------------
% größere Schwächen im Text, z.B. Struktur, Ergebnisse/Beweise/Argumente unklar/falsch, Argumentationslücken, zusätzliche Details nötig, triviale Dinge zu ausführlich
% konstruktive Kritik: Probleme benennen und Ratschläge geben wie man sie beheben kann. Ggf. grafische (Gegen-)Beispiele

Wie bereits in "Einschätzung/Evaluation" beschrieben, könnte man bei der Struktur etwas ändern.

Ich hatte beim Verständnis des Textes ein paar Unklarheiten (siehe ebenfalls in Einschätzung/Evaluation) dabei, heißt aber nicht zwangsweise dass es falsch oder ungut beschrieben ist.


Liste kleinerer Fehler
----------------------

% Korrekturvorschläge für Rechenfehler, Rechtschreib-/Grammatikfehler, Layoutprobleme

siehe beigefügtes PDF mit Kommentaren


