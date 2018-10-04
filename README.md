# Vue.js

Vue.js ist ein Framework, dass Entwicklern beim Erstellen von Webinterfaces oder einfachen Applikationen hilft.
Als modernes Framework nutzt Vue.js das von react.js bekannte virtual DOM. Dabei steht die Performance im Vordergrund.
Zunächst ist Vue.js nur eine einzelne Bibliothek ohne weitere Abhängigkeiten zu anderen Bibliotheken. Sie kümmert sich um die Anzeige von Daten auf einer HTML-Seite (View-Binding), Übernahme von Werten aus Formularen (Input-Binding) und Behandlung von Nutzer-Interaktionen (Event-Binding). Dabei bietet Vue.js Unterstützung für Templates, Mixins, Strukturierung der Anwendung in Komponenten, berechnete und gecachte Werte und Übergänge (Transitions).

# Stage 1: Kleine Hello World App mit Vue.js

1. Index.html
```ruby
<html>
<head>
    <!--implements production version, optimized for size and speed-->
    <script src="https://cdn.jsdelivr.net/npm/vue"></script>
</head>
<body>  
    
    <!--declaration of component-->
    <div id="app">
      {{ message }}
    </div>
    
    <!--load source code-->
    <script src="app.js"></script>

</body>
</html>
```
2. app.js
```ruby
var app = new Vue({
    el: '#app',
    data: {
      message: 'Hello World!'
    }
  })
```
Beim Öffnen der index.html im Browser erscheint ein "Hello World!"

Zu jeder Vue.js-Anwendung gehören drei Teile:
- Definieren des Teils der Website, für die Vue.js zuständig sein soll. In diesem Fall ist das DOM-Element eindeutig mit app benannt. Darin ist auch das Template enthalten, das Vue.js für die Anzeige benutzen soll.
- Laden der JavaScript-Bibliothek für Vue.js. Für Entwicklungszwecke ist eine nicht minifizierte Version, die zusätzliche Fehler- und Warnmeldungen enthält, vorhanden.
- Schließlich startet Vue.js innerhalb der Website. In diesem Fall wird die Referenz app auf die Seite mitgegeben, an die sich Vue.js binden soll. Mit data erhält Vue.js eine Struktur, die zum Beispiel Daten für die Anzeige enthält.

The v-bind attribute you are seeing is called a directive. Directives are prefixed with v- to indicate that they are special attributes provided by Vue, and as you may have guessed, they apply special reactive behavior to the rendered DOM. 

```ruby
    <div id="app-2">
        <span v-bind:title="message">
          What time is it?
        </span>
      </div>
```

```ruby
  var app2 = new Vue ({
    el: "#app-2",
    data: {
        message: 'It is ' + new Date().toLocaleString()
    }
  })
```
Zeit und Datumsanzeige erscheinen beim Hovern.

# Stage 2: Erstellen einer Navigation

Zusätzliche Bibliotheken des Vue.js-Projekts können weitere Funktionen aktivieren. Dazu gehören unter anderem Routing für die Navigation zwischen verschiedenen Komponenten der Anwendung, Vuex für State-Handling in der Anwendung und Server-Side Rendering.

# Quellen:
https://vuejs.org/v2/guide/
https://www.heise.de/developer/artikel/Vue-js-Zeitgemaesse-und-wartbare-JavaScript-Client-Anwendungen-4041158.html?seite=all

