# ObjectId
> ObjectId 来自于mongodb，是一种可排序的全局唯一标识符(GUID)。
## Use

https://www.nuget.org/packages/Junyu.ObjectId

```C#
using System;

namespace Demo
{
    class Program
    {
        static void Main(string[] args)
        {
            var id= ObjectId.GenerateNewId().ToString();

            Console.WriteLine(id);  //5a4c769ea719be0daca68075
        }
    }
}
```
