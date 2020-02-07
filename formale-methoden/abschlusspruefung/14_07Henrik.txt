Abschlussprüfung Henrik (2. am 2. Tag)
======================================

Alex hat gefragt.

Daten Typen und Induktion
-------------------------
* Spezifiziere mal Map (Key - Value Store)
* Was brauchen wir da?
    - Sorten (Key, Value, Map)
    - Konstruktoren (mkMap, insert)
    - nicht frei (-> Einfügereihenfolge egal)

* Was brauchen wir jetzt noch?
    - Extensionalitätsaxiom (-> hinschreiben)
    - $m_1 = m_2$ $\Leftrightarrow$ $\(\all k . k \in m_1 \Leftrightarrow k \in m_2  \) \wedge \( \all k . k \in m_1 \Rightarrow m_1[k] = m_2[k]\)$
    - $\in$ sollte gutem Definitionsprinzip folgen
    - $\in$ axiome hinschreiben
* Sind wir jetzt fertig?
    - Nein, zeigen, dass EQ Kongruenz ist
* Was haben wir Spezifizert?
    - Hierarchipersistent
    - Eindeutig modulo Unterspezifikation (in diesem Fall)
* Was für gute Def.-prinzipien gibt es?
    - Sturkturell Rec., Wohlfundiert Rec., Nicht Rec., Ex. und Eind. 

* Ja, was ist denn Wohlfundiert Rec.
    - Die Argumente nehmen nach einer noether'schen Ordnung ab
* Nöhter'sche Ordnung?
    - Keine Unendlich absteigenden Ketten
* Wir haben dann noch kurz über den Satz mit dem man zeigen kann das eine Allg. Rec. Funktion eine wohlfundierte ist (-> vgl. Folie 230) geredet (weil ich da smh drauf gekommen bin)

Programme
---------

* Wo brauchen wir noch noeth. rec. ?
    - Schleifen, Prozeduraufrufe
* Worüber machen wir da die Induktion?
    - Prozedur: Argumente und im worst case über das $n$
    - Schleife: Abnehmendes $t$ in im worst case über die anzahl der durchläufe
* Ok, für Programme haben wir ja die Dynamische Logik, was gibt es denn da für Konstrukte?
    - Box und Diamond
* Semantik von Box hinschreiben
* Du hast da Relationale Semantik verwendet, warum nehmen wir die her?
    - Nichtterminierung (expilziet das Bottom erwähnen macht Alex glücklich)
    - Lookahead: Indeterminismus
* Wie ist die Relationale Semantik definiert?
    - Strukturell Rekursiv
* Was ist da jetzt nicht so schön?
    - Schleifen und Prozeduraufrufe
* Also?
    - Natürliche Semantik
* Ein wenig darüber erzählen:
    - $\hat{R}_{ns}$ erklären
    - Regelbasiert
* Was haben wir uns damit eingekauft?
    - Fixpunkte
* Knaster-Tarski und Kleene erklären
    - Auch bezug zur Nat. Semantik herstellen

Indeterminismus  
---------------

* Was für ein Konstrukt hatten wir da?
    - Choose (und Or)
* Wann kann man Or implementieren?
    - Ja, z.B. mit Zufallszahl
* Und Choose?
    - Nein, unbeschränken indeterminismus kann man nicht implementieren.
* Was ist beschränkter bzw. unbeschränkter Indeterminismus und was geht kaputt?
    - Terminierung schwierig -> Neue Regeln
* Ich hab an diesem Punkt einfach mal ausgeholt und gleich noch dran gehängt, dass in diesen Regeln dann choose nicht mehr stetig ist, fanden beide gut.
* Was für ein Kalkül benutzen wir dann mit choose?
    - WP
* Semantik von Strong Diamond hinschreiben.

Abstrakte Datentypen und Kontrakte
----------------------------------

* Wie sehen Abstrake Datentypen aus?
    - $\(Z, Init, Op_i\)$
* Was sind die $Op_i$? 
    - Kontrakte
* Wie können die Aussehen?
    - Voredingung + Nachbedingung
    - Relational
    - Operational
* Wie sieht eine ganz allgemeine Operationale regel mit Vorbedingung $\phi$ und Nachbedingung $\psi$ aus?
    - $\phi \vdash \langle | p | \rangle \psi$
* Was kann man dann sehen, wenn man die benutzt?
    - Trace
* Was muss für Konkretisierungen gelten?
    - SEM(CDT) $\subseteq$ SEM(ADT)
    - Erklären was das bedeutet
* Wie beweist man das?
    - Abs und Beweisverpflichtungen
* Was schaut man sich da an?
    - In und Outputs
    - Abs "mapped" konkreten auf Abstrakten zustand

KIV
---

Gleich wie bei Jorge.

Viel Spaß und Viel Glück in der Prüfung! 
