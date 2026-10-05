# Quiz Game în C++

Un joc de tip quiz în consolă, scris în C++. Programul pune 20 de întrebări de cultură generală, fiecare cu 4 variante de răspuns (A, B, C, D), iar la final afișează scorul și procentul.

## Cum arată

```
1. Cate continente exista?
A. 5
B. 6
C. 7
D. 8
Raspuns: C

...

Scor: 17/20
Procent: 85%
```

## Cerințe

- Un compilator C++ (de exemplu `g++`)

## Compilare și rulare

```
g++ quiz_basic.cpp -o quiz
./quiz
```

Pe Windows, rularea se face cu `quiz.exe`.

## Cum se joacă

1. Rulezi programul.
2. Pentru fiecare întrebare scrii litera răspunsului (A, B, C sau D) și apeși Enter. Merg și literele mici.
3. La final vezi scorul și procentul.

## Cum adaugi o întrebare

Copiezi un bloc existent din `quiz_basic.cpp` și schimbi textul și litera corectă:

```cpp
cout << "Intrebarea ta?\nA. ..\nB. ..\nC. ..\nD. ..\nRaspuns: ";
cin >> r;
if (r == 'B' || r == 'b') scor++;
```

Dacă schimbi numărul de întrebări, actualizează și afișarea scorului. Procentul se calculează cu `scor * 100 / N`, unde `N` este numărul total de întrebări.

## Posibile îmbunătățiri

- Întrebări în ordine aleatorie
- Categorii și nivel de dificultate
- Salvarea celui mai mare scor într-un fișier
