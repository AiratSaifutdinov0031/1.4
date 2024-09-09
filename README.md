На экране отображаются изображения, по 3 в каждом ряду. У пользователя в альбоме всего 52 изображения. Требуется определить, сколько полных рядов можно сформировать и сколько изображений останется.
В решении должны быть объявлены переменные, которые содержат необходимые значения. Используя эти переменные, выполните простые математические операции для получения результатов.

ОТВЕТ: При решении данной задачи получаем, что фотографии поместятся в 17 рядах, а одна фотография не помещеаеттся

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Task_3._1._1
{
    class Program
    {
        static void Main(string[] args)
        {
            int photosCount = 52;
            int countPerColumn = 3;

            int fullRowsCount = photosCount / countPerColumn; 
            int overflowCount = photosCount % countPerColumn;

            Console.WriteLine("Заполнится рядов - " + fullRowsCount);
            Console.WriteLine("Не влезит фотографий - " + overflowCount);


            Console.ReadLine();
        }
    }
}
