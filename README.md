# Итоговая проверочная работа
Схема Алгоритма (функции фильтра чисел)
![Итогова работа блок-схема](https://github.com/SergioRAIS/Itog/assets/130254963/b00c70d9-8412-4198-8039-a94e97962ee6)
Код функции фильтра чисел
[inovayarab.md](https://github.com/SergioRAIS/Itog/files/12553296/inovayarab.md)
Задача: Написать программу, которая из имеющегося массива строк формирует новый массив из строк.
using System;
string[] array =
{
    "a",
    "bb",
    "ccc",
    "dddd",
    "eeeee",
    "z"
};
 
var result = new string[array.Length];
var realSize = 0;
foreach (var value in array)
{
    if (value.Length <= 3)
    {
        result[realSize] = value;
        realSize++;
    }
}
 
Console.WriteLine(string.Join(Environment.NewLine, result, 0, realSize));
