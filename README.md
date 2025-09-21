### Лабораторная работа 2
***
# Задача 1
* ввел три числа и сделал проверку по неравенству треугольника
```
#include <iostream>
using namespace std;

int main()
{
	int a, b, c;
	cin >> a >> b >> c;
	if (a + b > c && a + c > b && b + c > a)
	{
		cout << "YES" << endl;
	}
	else 
	{
		cout << "NO" << endl;
	}
}

```
***
# Задача 2
* ввел три числа и разобрал все варианты их растановки в ряду
```
#include <iostream>
using namespace std;
int main()
{
    int a,b,c;
    cin >> a >> b >> c;
    if ((a >= b && b >= c) || (c >= b && b >= a))
    {
        cout << b << endl;

    }
    else if ((b >= a && a >= c) || (c >= a && a >= b))
    {
        cout << a << endl;
    }
    else if ((a >= c && c >= b) || (b >= c && c >= c))
    {
        cout << c << endl;
    }
    return 0;
}
```
***
# Задача 3.1
* ввел три числа и проверил ряд на возрастание
```
#include <iostream>
using namespace std;
int main()
{
    int a, b, c;
    cin >> a >> b >> c;
    if (c > b && b > a)
    {
        cout << "YES" << endl;
    }
    else
    {
        cout << "NO" << endl;
    }
    return 0;
}

```
***
# Задача 3.2
* так же как и в 3.1 , но появляется случай равенства чисел в ряду
```
#include <iostream>
using namespace std;
int main()
{
    int a, b, c;
    cin >> a >> b >> c;
    if (c >= b && b >= a)
    {
        cout << "YES" << endl;
    }
    else
    {
        cout << "NO" << endl;
    }
    return 0;
}
```
