# Senac
## Curso Desenvolvimento De Aplicativos Móveis

### Usando DART e FLUTTER

**Aula 1 - Variáveis**

**Variaveis**

Um valor armazenado na memoria ram do computador,
que perde seu valor sempre que o PC é desligado.
Seu valor pode ser modificado a qualquer momento.
Resumindo, a variavel é como uma caixa, onde eu guardo
um determinado valor, este valor podendo ser um numero,
um texto,um valor lógico (sim/nao), etc.

**Tipos de Variáveis**

- String - textos 
- int - números inteiros 
- double - números decimais

### Exemplo 1 - Tipos de Variáveis

```dart
void (){
  String nome = "Joao";
  int idade = 16;
  double altura = 1.68
  }
 ```
 
### Exemplo 2 - Cálculo Simples

```dart
void main() {

double altura, peso , imc;

altura = 1.68;

peso = 83.0;

imc = peso / (altura * altura);

print ("SEU IMC É -> $imc");

}
```


## Aula 2

**${renda_pessoa.toStringAsFixed(2)}**

O método toStringAsFixed() foi usado para formatar as casas (2) decimais da variável(renda_pessoa) double.

```dart
void main() {
  String nome, sobrenome, email, senha, cpf, endereco, sexo, celular, curso, nome_social;
  int ano_nasc, idade, qtd_moradores;
  double renda_familiar, renda_pessoa;
 

  nome = "Thiago Antonio" ;
  sobrenome = "dos Santos Oliveira";
  nome_social = "";
  email = "braddock@hotmail.com";
  senha = "123changeja" ;
  cpf = "111.222.333-66";
  endereco = "Rua dos Alfeneiros 9.3/4";
  sexo = "masculino";
  celular = "(19)99666-0000";
  curso = "Programador de Disp. Móveis";
  ano_nasc = 1989;
  idade = 2019 - ano_nasc;
  qtd_moradores = 2;
  renda_familiar = 5355.22;
  renda_pessoa = renda_familiar / qtd_moradores;

  print("**************************");
  print("Confirmação de Cadastro");
  print("**************************");
  print("\nNome: $nome $sobrenome");

  if (nome_social != "")
  {
    print("Nome Social: $nome_social");
  }

  print("E-mail: $email");
  print("Sexo: $sexo");
  print("Celular: $celular");
  print("Ano de Nascimento: $ano_nasc");
  print("Idade: $idade");
  print("CPF: $cpf");
  print("\n**************************");
  print("Informações SENAC");
  print("**************************");
  print("\nCurso: $curso");
  print("Endereço: $endereco");
  print("Moradores na mesma residência: $qtd_moradores");
  print("Renda Familiar: R\$ $renda_familiar");
  print("Renda por pessoa: R\$ ${renda_pessoa.toStringAsFixed(2)}");
 
}

```
