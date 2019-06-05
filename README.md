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

## Condição Lógica IF

O IF serve para determinar se um bloco de instruções **deve** ou **não** ser executado, pode-se dizer que sempre que for necessário **testar** algum valor usaremos o *if*.

### Operadores Lógicos

- == *Igualdade*
- != *Diferente*
- \>= *Maior ou igual* 
- <= *Menor ou igual*
- \>  *Maior*
- <  *Menor*

### Sintaxe

```dart
if(teste_logico)
{
    //faz isso se o teste for verdadeiro
}
else
{
    //faz isso se o teste for falso
}
```

### Exemplo if :floppy_disk:
```dart
string curso = "programador android";

if(curso == "programador android")
{
    print("Parabéns, você faz ótimas escolhas.");
}
else
{
    print("Vacilão, aposto que você faz ADM.");
}
```
### Exemplo if 2

```dart
void main() {
	double nota1, nota2, media;
  nota1 = 5;
  nota2 = 2;
  media = (nota1 + nota2) / 2;
  if(media >= 5)
  {
  		print("Aprovado com média $media");
  }
  else
  {
    	print("Reprovado com média $media");
  }
}
```

## Aula 3 - Lógica com DART

Foi importada a *biblioteca* **dart:math** para podermos usar funções matemáticas como potência e raiz quadrada, no exemplo abaixo foi usada a função **math.sqrt()** para calcular a raiz de delta.

- Após a importação foi dado um "apelido" para chamar a função através da sintaxe **as** (dart:math as **math**)
- Foram usados 2 if, o 1º para dar acesso através da palavra mágica *shazam* e o 2º para fazer a equação.
- Cada **if** tem seu próprio **else** , daí a importância de *identar* , organizar o código com **TABS**

### Exemplos usando math

```dart
print(math.sqrt(9)); //exibe a raiz de 9
print(math.pi); //exibe o valor de pi
print(math.pow(2,7)); //exibe o resultado de 2 elevado a 7.
```

### Exemplo Usando If dentro de If (Login e Equação de 2º grau)

```dart
import 'dart:math' as math; 

void main() { 

  String palavra_magica;
  palavra_magica = "shazam";
  if(palavra_magica == "shazam")
  {
    print("Exercício 1 - Bhaskara");
    double delta, a, b, c;
    a = 1;
    b = -10;
    c = 25;
    delta = (b * b) - 4 * a * c;
    print("O DELTA = $delta");  
    if(delta < 0)
    {
      print("Nenhuma raiz real pq o delta menor q zero."); 
    }
    else
    {
      double raiz_q, x1, x2;
      //Raiz Quadrada
      raiz_q = math.sqrt(delta);
      print("A RAIZ DE DELTA = $raiz_q");
      x1 = (-b + raiz_q) / (2 * a);
      x2 = (-b - raiz_q) / (2 * a);
      print("X1 = $x1");
      print("X2 = $x2");
    }
  }
  else
  {
    print("Acesso negado, você não é Digno.");  
  }
}
```




