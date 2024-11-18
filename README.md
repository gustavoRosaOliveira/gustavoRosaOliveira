```csharp
namespace DevProject.Models
{
    public class Developer
    {
        public string Name { get; set; }
    }
}

using DevProject.Models;

class Program
{
    static void Main(string[] args)
    {
        var mew = new Developer
        {
            Name = "Gustavo da Rosa Oliveira"
        };

        Console.WriteLine($"Developer criado: {mew.Name}");
    }
}