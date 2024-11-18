```csharp
public class Desenvolvedor
{
    public string Nome { get; set; }
    public string LinguagemFavorita { get; set; }
    public int AnosDeExperiencia { get; set; }

    public void Apresentar()
    {
        Console.WriteLine($"Olá, meu nome é {Nome}, minha linguagem favorita é {LinguagemFavorita} e tenho {AnosDeExperiencia} anos de experiência.");
    }
}