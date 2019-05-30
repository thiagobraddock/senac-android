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
