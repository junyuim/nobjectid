# nobjectid
> objectid from mongodb is a sort of global unique identifier(guid)
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

*the generated identifier consists of 24 characters, 12 bytes, according to the rules is divided into 4 parts:  
the timestamp (4 bytes) | machine id (3 bytes) | process id (2 bytes) | increment number (3 bytes)*

> documentation please see: http://www.mongodb.org/display/DOCS/Object+IDs
