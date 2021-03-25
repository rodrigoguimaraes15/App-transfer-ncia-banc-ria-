using System;



namespace DIO.Bank

{

  public class Usuario

  {

​    int senha;

​    public Usuario(int senha)

​    {

​      this.senha = senha;

​    }



​    public String validaSenha() {

​      Console.Write("Digite a senha novamente para validação ");

​      int validaSenha = int.Parse(Console.ReadLine());



​      if(validaSenha == senha)

​      {

​        Console.WriteLine("Senha validada com sucesso!!");

​      } 

​      else 

​      {

​        throw new ArgumentOutOfRangeException();         

​      }

​      

​      return "Senha Validada com sucesso!";

​    }

  }

}