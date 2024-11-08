# Python basics and concepts (link collection)

### Funktionen in Python

* [Eintrag zu Funktionen in der offiziellen Dokumentation zu Python 3.12 auf python.org](https://docs.python.org/3.12/tutorial/controlflow.html#defining-functions)
* [Funktionen in Python auf w3schools.com](https://www.w3schools.com/python/python_functions.asp)

### Python Tutorial on W3-Schools
[Python Tutorial](https://www.w3schools.com/python/default.asp)

### Python inheritance (Vererbung) on W3-Schools
[Python Inheritance](https://www.w3schools.com/python/python_inheritance.asp)

### Python Polymorphism on W3-Schools
[Python Polymorphism](https://www.w3schools.com/python/python_polymorphism.asp)

### Python docstrings in classes
Klassen sollten gur dokumentiert werden (gilt im Übrigen für jeden Code). Python unterstützt dies durch die Verwendung von Docstrings. Jede Klasse, Funktion oder Methodenkopfzeile kann eine standardmäßige Python-Zeichenkette als erste Zeile nach der Definition (die Zeile, die mit einem Doppelpunkt endet) haben. Diese Zeile sollte genauso eingerückt sein wie der nachfolgende Code.
Bsp.:
```python
class Classname():
    "Das ist ein einzeliger Docstring als Beschreibung der Klasse"

    def __init__(self, argument):
        """Das ist ein Mehrzeilenkommentar
           als Beschreibung der __init__-Methode
        """
        self.attribut = argument    

    def method_name(self):
        """Das ist noch ein Mehrzeilenkommentar
           für eine weitere Methode
        """
        pass
```
      
Ein Docstring sollte klar und prägnant den Zweck der Klasse oder Methode zusammenfassen, die sie beschreibt. Sie sollte alle Parameter erklären, deren Verwendung nicht sofort offensichtlich ist, und ist auch ein guter Ort, um kurze Beispiele zur Nutzung der API (Application Programming Interface) einzufügen.

### `__name__` (dunder name variable)
`__name__` ist eine spezielle Variable in Python. Das Besondere daran ist, dass Python ihr einen anderen Wert zuweist, je nachdem, wie das enthaltende Skript ausgeführt wird.

Wenn du ein Modul importierst, führt Python die Datei aus, die dem Modul zugeordnet ist.

Häufig möchtest du ein Skript schreiben, das direkt ausgeführt oder als Modul importiert werden kann. Die Variable ermöglicht es dir, dies zu tun.

Wenn du das Skript direkt ausführst, legt Python die Variable auf `__name__ = "__main__"` fest.

Wenn du jedoch eine Datei als Modul importierst, legt Python den Modulnamen auf die Variable fest. Das ist meist der Name der Datei ohne die .py Endung. Es ist daher `__name__ = Modulname`

Der Ausdruck
```python
if __name__ == "__main__":
    ...
```
kann daher verwendet werden, um den if-Block nur dann auszuführen, wenn das Programm als Skript ausgeführt wird.
