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

* the generated identifier consists of 24 characters, 12 bytes, according to the rules is divided into 4 parts: the timestamp (4 bytes) | machine id (3 bytes) | process id (2 bytes) | random number (3 bytes) *

> detailed documentation please see: http://www.mongodb.org/display/DOCS/Object+IDs
