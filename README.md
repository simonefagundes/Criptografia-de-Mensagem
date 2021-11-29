string mensagemOriginal = "Dados com necessidade de proteção";
string mensagemDecodificada = "";

Pessoa alice = new Pessoa ("Alice);
Pessoa bob = new Pessoa ("bob");

string ChavePublicaDoBod = bob.ChavePublica;
var bytesCodificados = alice.CodificarMensagem(mensagemOriginal, ChavePublicaDoBod);

Console.WriteLine("String decifrada: {0}", mensagemDecodificada);
Console.ReadLine();








public class Pessoa
{
    private readonly string nome;
    private readonly string chavePrivada;

    public string ChavePublica {get;}

    public Pessoa (string nome)
    {
        this.nome = nome;
    }
}

