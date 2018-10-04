# DOM
Das Document Object Model (DOM, engl. für Dokumenten-Objekt-Modell) ist eine Spezifikation einer Programmierschnittstelle, 
welche HTML- oder XML-Dokumente als eine Baumstruktur darstellt, in der jeder Knoten ein Objekt ist, 
welches einen Teil des Dokumentes repräsentiert, z. B. einen Absatz, eine Überschrift, ein Video oder etwa eine Tabellenzelle. 
Die Schnittstelle ist plattform- und programmiersprachenunabhängig und erlaubt damit standardisiert, die Struktur und das 
Layout eines Dokumentes zu verändern. Im Webbrowser bildet dies einen wichtigen Baustein für dynamische Webseiten.
DOM wird vom World Wide Web Consortium definiert. Eine Implementierung, die der DOM-Spezifikation genügt, 
besteht im Sinne der objektorientierten Programmierung aus einem Satz von Klassen zusammen mit deren Methoden und Attributen. 

# Virtual DOM
Das virtuelle DOM ist eine Art abstrakte Kopie des tatsächlichen DOMs, die deutlich kleiner ist und auf das Nötigste an Informationen beschränkt. Dadurch kann sie weit schneller verändert werden und ist daher der Ort, wo Änderungen vorgenommen werden. Wann immer an diesem virtuellen DOM ein Update passiert, werden beide Varianten des DOMs durch einen Algorithmus verglichen 
und die Unterschiede dann gebündelt und in einem Schritt im tatsächlichen DOM angepasst.


