```csharp
using DevProject.Models.Enums;

namespace DevProject.Models
{
    public class Person
    {
        public string Name { get; set; }

        public GenderEnum Gender { get; set; }

        public Person(string name, GenderEnum gender)
        {
            Name = name;
            Gender = gender;
        }
    }
}

using DevProject.Models.Enums;

namespace DevProject.Models
{
    public class Developer : Person
    {
        public Developer(string name, GenderEnum gender) : base(name, gender)
        {
        }
    }
}

namespace DevProject.Models.Enums
{
    public enum GenderEnum
    {
        Male = 1,
        Female = 2,
        Others = 3
    }
}

using DevProject.Models;
using DevProject.Models.Enums;

class Program
{
    static void Main(string[] args)
    {
        var mew = new Developer(
                "Gustavo da Rosa Oliveira",
                GenderEnum.Male
            );

        Console.WriteLine($"Developer criado: {mew.Name}");
    }
}