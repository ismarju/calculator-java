# calculator-java project

- metrika
- pregled
- statička analiza

## Calculator.java

LOC = `134`
Broj linija koda = `188`

### Ciklomatska složenost

Pronađena je sljedeća ciklometrijska složenost (Codelyze):

- Calculator::evaluateExpression - ciklometrijska složenost = `12`
- Calculator::Calculate - ciklometrijska složenost = `12`
- Calculator::Run - ciklometrijska složenost = `1`

### Kognitivna složenost

Pronađena kognitivna složenost (Tubnine) je `12`

### Statička analiza

Pronađeni su sljedeći code smell (Tubnine):

1. Move this file to a named package. [Ln 1, Col 1]
   This code smell indicates that the file is not in a package, which can make it difficult to organize and maintain the code.
2. Add a private constructor to hide the implicit public one. [Ln 4, Col 14]
   This code smell indicates that there is an implicit public constructor, which can make it easier for unauthorized users to access the class.
3. Rename method "ToString" to prevent any misunderstanding/clash with method "toString" defined in superclass "java.lang.Object". [Ln 18, Col 30]
   This code smell indicates that the method name "ToString" is similar to the built-in method "toString", which can cause confusion.
4. Rename this method name to match the regular expression '^[a-z][a-zA-Z0-9]\*$'. [Ln 18, Col 30]
   This code smell indicates that the method name does not follow the recommended naming conventions, which can make it difficult to understand and maintain the code.
5. Rename this method name to match the regular expression '^[a-z][a-zA-Z0-9]\*$'. [Ln 24, Col 26]
   This code smell indicates that the method name does not follow the recommended naming conventions, which can make it difficult to understand and maintain the code.
6. Immediately return this expression instead of assigning it to the temporary variable "textResult". [Ln 70, Col 29]
   This code smell indicates that the code is assigning a value to a temporary variable and then immediately returning the same value, which can be confusing and inefficient.
7. Rename this method name to match the regular expression '^[a-z][a-zA-Z0-9]\*$'. [Ln 74, Col 25]
   This code smell indicates that the method name does not follow the recommended naming conventions, which can make it difficult to understand and maintain the code.
8. Remove this redundant jump. [Ln 183, Col 13]
   This code smell indicates that there is a redundant jump, which can make the code harder to understand and maintain

## Start.java

LOC = `19`
Broj linija koda = `26`

### Ciklomatska složenost

Pronađena je sljedeća ciklometrijska složenost (Codelyze):

- Calculator::evaluateExpression - ciklometrijska složenost = `3`

### Kognitivna složenost

Pronađena kognitivna složenost (Tubnine) je `3`

### Statička analiza

Pronađeni su sljedeći code smell (Tubnine):

1. Move this file to a named package. [Ln 1, Col 1]
   This code smell indicates that the file is not in a package, which can make it difficult to organize and maintain the code.
2. Rename this local variable to match the regular expression '^[a-z][a-zA-Z0-9]\*$'. [Ln 6, Col 10]
   This code smell indicates that the variable name does not follow the recommended naming conventions, which can make it difficult to understand and maintain the code.
3. Replace this use of System.out or System.err by a logger. [Ln 8, Col 3]
   This code smell indicates that the code is using the System.out or System.err classes, which can make it difficult to control the output and can lead to security issues.
4. Replace this use of System.out or System.err by a logger. [Ln 19, Col 5]
   This code smell indicates that the code is using the System.out or System.err classes, which can make it difficult to control the output and can lead to security issues.
