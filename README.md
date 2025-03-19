# Arduino Keyboard Layout für Schweizer Tastaturen (CH-DE)

Dieses Projekt ermöglicht die Nutzung eines Schweizer Tastaturlayouts (DE-CH) mit der Arduino Keyboard Library.

## Installation

1. **Navigiere zum Arduino Keyboard Library Verzeichnis**  
   Öffne das Arduino Library-Verzeichnis auf deinem Rechner. Standardmäßig befindet es sich unter:
   - `[Arduino-Sketch-Ordner]/libraries/Keyboard/src`


2. **Datei herunterladen und einfügen**  
Lade die Datei `KeyboardLayout_de_CH` herunter und kopiere sie in das obige Verzeichnis.

3. **Keyboard Layout in der Library registrieren**  
Öffne die Datei `Keyboard.h` und füge unter `// Supported keyboard layouts` die folgende Zeile hinzu:
```cpp
extern const uint8_t KeyboardLayout_de_CH[];
```
## Verwendung im Sketch
Nachdem das Layout installiert wurde, kannst du es in deinem Arduino-Sketch wie folgt einbinden:
```cpp
#include <Keyboard.h>

void setup() {
    // Setze das Schweizer Layout
    Keyboard.begin(KeyboardLayout_de_CH); 
}

void loop() {
    // Dein Code...
}
```


## Hinweise
Dieses Layout ersetzt nicht das Standard-Layout, sondern erweitert die Arduino Keyboard Library um eine Unterstützung für CH-DE.
Falls die Library nicht richtig funktioniert, überprüfe, ob die Datei KeyboardLayout_de_CH korrekt im Verzeichnis liegt und die Zeile in Keyboard.h eingefügt wurde.
Viel Erfolg! 🚀

bash
Kopieren
Bearbeiten
