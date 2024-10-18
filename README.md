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
    "Das ist ein Docstring als Beschreibung der Klasse"
def __init__(self, argument):
    """Das ist ein Mehrzeilenkommentar
       als Beschreibung der __init__-Methode
    """
    self.attribut = argument    
def method_name(self):
    """Das ist noch ein Mehrzeilenkommentar
       für eine weiter Methode
    """
    pass
```
      
Ein Docstring sollte klar und prägnant den Zweck der Klasse oder Methode zusammenfassen, die sie beschreibt. Sie sollte alle Parameter erklären, deren Verwendung nicht sofort offensichtlich ist, und ist auch ein guter Ort, um kurze Beispiele zur Nutzung der API (Application Programming Interface) einzufügen.
