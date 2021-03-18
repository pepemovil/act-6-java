1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
#ifdef __MSDOS__
    #include <iostream.h>
    #include <stdlib.h>
#else
    #include <iostream>
    #include <cstdlib>
    using namespace std;
#endif

int main (void)
{
    int i, nota_1, nota_2, nota_3, nota_4;
    int nota_5, promedio;
    for (i=1; i<=5; i++)
    {
        cout << "PROCESO " << i << endl;
        cout << "Ingresa el valor de nota 1: ";
        cin >> nota_1;
        cin.get();
        cout << "Ingresa el valor de nota 2: ";
        cin >> nota_2;
        cin.get();
        cout << "Ingresa el valor de nota 3: ";
        cin >> nota_3;
        cin.get();
        cout << "Ingresa el valor de nota 4: ";
        cin >> nota_4;
        cin.get();
        cout << "Ingresa el valor de nota 5: ";
        cin >> nota_5;
        cin.get();
        promedio=(nota_1+nota_2+nota_3+nota_4+nota_5)/5;
        if(promedio<71)
            cout << "reprobado" << endl;
        cout << "Valor de promedio: " << promedio << endl;
        cout << endl;
    }
    return EXIT_SUCCESS;
}
