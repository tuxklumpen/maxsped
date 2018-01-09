
Review Partial Edge Drawings
============================

Zusammenfassung/Inhalt
----------------------

% kurze Beschreibung des Inhalts der Ausarbeitung in eigenen Worten (nicht Abstract)
Die Arbeit befasst sich mit der Darstellung von Graphen, bei der einige Kanten nicht komplett durchgezeichnet werden, um Kreuzungen der Kanten zu vermeiden. Es gibt eine Reihe von Darstellungsarten, die angewandt werden können und jeweils unterschiedliche Regeln befolgen und Symmetrien hervorrufen (oder auch nicht). Nicht jede dieser Darstellungsarten kann für einen Graphen verwendet werden, da unter Umständen durch die Anzahl der Knoten und Kanten zu wenig Platz ist, um Kreuzungen komplett zu vermeiden. Die vorliegende Arbeit gibt einen Überblick über State-of-the-art in diesem Forschungsbereich, behandelt offene Probleme und befasst sich im Detail mit Bounds von vollständigen Graphen die einseitig convex gezeichnet sind, sowie zwei Algorithmen bezüglich Ink-Maximizierung bzw. Ink-Erasing von "eingebetteten" Graphen (= Graphen die die Position der Knoten+Kanten vorgegeben haben).


% Was ist die Problemstellung und das Ziel in der Ausarbeitung?
Das Ziel ist es, einen Einblick in das Forschungsgebiet der partial edge drawings zu bieten, und versucht durch detailliertere Erläuterungen eines Papers ein tieferes Verständnis in einen aktuell erforschten Teil dieses Forschungsgebiets zu bieten.

% Was sind die Ergebnisse?
Das Ergebnis ist eine kompakte Einführung in das Thema, welches einerseits einen Überblick über State-of-the-art und open questions bietet, andererseits auch detaillierte Ergebnisse eines aktuellen Papers erläutert. 




Einschätzung/Evaluation
-----------------------

% ... Stärken und Schwächen des Textes

% Was ist gut und anschaulich / unklar beschrieben, wo sind Fehler in Argumenten?

"Many proofs [...] start from $\delta=1/4$ are then generalized" ... Sehr hilfreich die Bedeutung von 1/4 im Context zu anderen Arbeiten dieses Gebiets darzulegen!

Durchwegs anschaulich und verständlich erklärt!


Bei Related Work - "A practical approach for 1/4-SHPEDs", was kann man sich unter einer "force" vorstellen? Heißt das soviel wie, die Knoten stoßen sich ab, je nachdem wo sich ihre Stubs schneiden würden?


Bei "Progress on Partial Edge Drawings", was genau bedeutet das “ \in YYY” in den Ungleichungen? Bezieht es sich in weiterer Folge auf die Variable auf der linken Seite der Ungleichung?

Was bedeutet bandwidth? Wo ist es definiert?

Bei "Partial Edge Drawing: Homogeneity is more important than Crossings and Ink" ist der Punkt $u$ in $S_{left}$ miteingerechnet. Könnte man auch extra nochmal erwähnen damit es auf Anhieb klar ist.


% Wie interessant und innovativ sind die Ergebnisse/verwendeten Techniken? (= Bewertung Original-Paper)


% Titel passend?
Im Sinne einer Seminararbeit ist der Titel passend, da die Ausarbeitung einen Überblick über das Thema geben soll. Für eine wissenschaftliche Arbeit die veröffentlicht wird, würde man wohl einen spezifischeren Namen geben.



% aussagekräftiger Abstract?
Das Abstract ist aussagekräftig und gibt kurz und bündig den Inhalt der Arbeit wieder.


% Motiviert Einleitung gut die Problemstellung?
Die Einleitung motiviert die Problemstellung indem es unter anderem anhand eines anschaulichen Beispiel den Nutzen dieser Drawings zeigt.


% ausreichende Quellenangaben für Aussagen, Behauptungen, ausgelassene Beweise?
Wenn es nicht um das im Detail untersuchte Original-Paper ging, wurde stets auf Quellenangaben geachtet.


% hilfreiche und kompakte Abbildungen für Aussagen?
Abbildungen sind in einem ausreichenden Maß vorhanden und sehr gut umgesetzt!

Abbildungen bestehend aus mehreren Unterabbildungen könnten beim Hauptlabel schon Informationen enthalten, was der Zusammenhang der einzelnen Unterabbildungen ist und nicht einfach "Example from YYY". Womöglich besser "Figure 4: Interactive visualization tool (Burch et al. [5])". Die Abbildung soll mMn auch alleine ohne den Context des Textes einen gewissen Sinn oder Orientierung geben, wohin man die Abbildung einordnen kann. Ein Abbildungsverzeichnis mit einigen Einträgen "Example from YYY", "Example from ZZZ" wäre ebenfalls begrenzt sinnvoll.



% Wird auf Schwächen der beschriebenen Algorithmen und Ergebnisse eingegangen?
Die Anwendbarkeit der vorgestellten Algorithmen wurde richtigerweise eingegrenzt und offene Fragen dargelegt.


% Text sinnvoll strukturiert?
Die Arbeit selbst ist sinnvoll im Sinne einer Seminararbeit, welche einen Überblick über ein Thema gibt, strukturiert. Aufeinander aufbauende Passagen sind in einem guten Textfluss eingebettet.

% Seitenumfang angemessen? (12-15 Seiten)
Der Seitenumfang ist angemessen.


% sprachliche Qualität?
Gute sprachliche Qualität! Verständlich geschrieben, auch für Nicht-Experten.


% Gesamteindruck der Ausarbeitung? z.B. "sehr gut, kaum Kritikpunkte", "gut, mehrere kleinere Korrekturen und wenige größere Korrekturen nötig", "noch viele größere Korrekturen erforderlich"
Ein paar Ungenauigkeit in der Argumentation/Wortwahl sind vorhanden, sowie ein paar Satzstellungen könnten verbessert werden um es noch flüssiger lesen zu können. Detailgrad der Erklärung und Abbildungen sind sehr gut. Somit wäre es gut, noch ein paar Korrekturen durchzuführen.



Liste größerer Kritikpunkte
---------------------------
% größere Schwächen im Text, z.B. Struktur, Ergebnisse/Beweise/Argumente unklar/falsch, Argumentationslücken, zusätzliche Details nötig, triviale Dinge zu ausführlich
% konstruktive Kritik: Probleme benennen und Ratschläge geben wie man sie beheben kann. Ggf. grafische (Gegen-)Beispiele

Hier eine Liste mit Kritikpunkten, die oft aus kleineren Ungenauigkeiten resultieren, aber deshalb nicht zwangsweise grobe Fehler sind.

Bei Abschnitt "3 Related Work" meinst du wohl, dadurch dass es für einen "complete graph K_n" gilt, gilt is in weiterer Folge auch für jeden Graphen mit $n$ Knoten. So wie es dort steht, könnte man fälschlicherweise verstehen, "complete graph"s sind die Menge aller Graphen mit $n$ Knoten.

Bei "Partial Edge Drawing: Homogeneity is more important than Crossings and Ink" schreibst du "large angles (< 90 deg)". Im Original wird von "angles of at least pi/3" gesprochen, was > 60 deg wären. Von < 90 deg finde ich auf Anhieb nichts.

Beim Beweis für Theorem "There is no set of 16 points [...]" steht auf Seite 6 unten "The point b can not lie above a or below the stub av otherwise the point set would not be in convex position". Es wurde zwar definiert, aber nicht was convex ist. Somit weiß man nur intuitiv, wodurch ein Punkt unterhalb des stubs av die Convexheit verletzen würde.

Bei diesem Beweis ist wenn ich das richtig verstehe die Position eines Punktes immer gewissermaßen eingeschränkt, da sonst die 'convex' Eigenschaft verletzt werden würde. Dies wurde richtigerweise am Beispiel "The point b can not lie above a or below the stub av otherwise the point set would not be in convex position" dargelegt. Die weitere Argumentation mit den 6 Punkten die in S_{left} eingefügt werden, brauchen jedoch ebenfalls diesen Constraint, sonst funktioniert die Argumentation nicht. Es würde wohl ein Satz genügen, der explizit besagt, dass der Constraint für jeden Punkt gilt.

Wo hört das Theorem auf? Q.E.D. fehlt
Es gibt mehrere Theoreme, es wäre gut wenn diese durchnummeriert wären, damit man sich darauf beziehen kann.

Bei 4.1 Upper Bounds for Complete Graphs - "Generalization", ist es unklar wie viele von welchen strips verwendet werden. Nimmt man die Aussage "the i-th strip has to be $\delta^2/(1-\delta)^i$ und schaut sich Abbildung 8 an, dann wird klar, dass die selben strips öfters verwendet werden. Es steht jedoch nicht geschrieben, welche Regeln hierbei befolgt werden. "From that, a bound of the total number of strips that fit in the bounding box with a given delta can be obtained [...]". Wird hierbei immer der 3. strip in der Mitte so oft gesetzt, bis kein Platz mehr ist? Muss schlussendlich die Summe aller Strips auf 1 kommen?
Somit kann man den Bound für die "total number of strips" nicht nachvollziehen.

Bei 5.1 "Maximizing Ink in 2-Planar Drawings" im Absatz "This ordering in the intersection graph is applied to the edges [...]" sollte man definieren dass $n$ die Länge so einer zusammenhängenden Komponente ist. Sonst ist nicht sofort klar, wie das ordering genau auf das drawing $\Gamma$ angewandt wird. Erst implizit durch "In the case C_i was a cycle [...]".

Auf Seite 9, 3. Absatz ("The number of choices we have [...]"), es wäre doch auch möglich den forwardstub zu zeichnen, sofern er kleiner gleich dem backwardsstub ist. Man weiß nur mit Sicherheit, dass die nächste Kante nicht komplett gezeichnet werden kann und maximal die länge des backwardstub.


Bei 5.2 "Erasing Ink in Arbitrary Graph Drawings" erster Absatz unter dem Theorem, $e_0, ..., e_{k+1}$ wären k+2, und nicht wie beschrieben k+1 pairs of edge segments. Außerdem kommt anschließend im Text $e_1, ..., e_{k+1}$ vor, sowie in der Abbildung 12 werden diese pairs $e_0, ..., e_k$ benannt.

Definitionen könnten mit einer "Definition" Überschrift versehen werden (ähnlich wie für "Theorem"), damit man Definitionen schneller wieder findet und nicht im Text suchen muss.



Liste kleinerer Fehler
----------------------

% Korrekturvorschläge für Rechenfehler, Rechtschreib-/Grammatikfehler, Layoutprobleme

siehe außerdem beigefügtes PDF mit Kommentaren


