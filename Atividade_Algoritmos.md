Questão 04

\#include <iostream>



int main() {

&#x20;   int a,b,c,maior;



&#x20;   std::cout << "Digite o Primeiro numero: ";

&#x20;   std::cin >> a;



&#x20;   std::cout << "Digite o Segundo numero: ";

&#x20;   std::cin >> b;



&#x20;   std::cout << "Digite o Terceiro numero: ";

&#x20;   std::cin >> c;



&#x20;   if (a>b \&\& a>c) {

&#x20;       std::cout << "Maior numero: " << a;

&#x20;   }



&#x20;   else if (b>a \&\& b>c) {

&#x20;       std::cout << "Maior numero: " << b;

&#x20;   }



&#x20;   else if (c>a \&\& c>b){

&#x20;       std::cout << "Maior numero: " << c ;

&#x20;   }



&#x20;   else{

&#x20;       std::cout << "Os numeros são iguais!";

&#x20;   }



&#x20;    

&#x20;   return 0;

}



Questão 05



\#include <iostream>



int main() {

&#x20;   int a,b,media;



&#x20;   std::cout << "Digite a Primeira nota: ";

&#x20;   std::cin >> a;



&#x20;   std::cout << "Digite a Segunda nota: ";

&#x20;   std::cin >> b;



&#x20;   media == (a+b)/2;



&#x20;   std::cout << "Primeira nota: "<< a << "\\n";

&#x20;   std::cout << "Segunda nota: "<< b << "\\n";

&#x20;   std::cout << "Media: " << media << "\\n";

&#x20;   

&#x20;   if (media >= 7) {

&#x20;       std::cout << "Situação: APROVADO";

&#x20;   }



&#x20;   else if (media >= 4 \&\& media < 7) {

&#x20;       std::cout << "Situação RECUPERAÇÃO";

&#x20;   }



&#x20;   else{

&#x20;       std::cout << "Situação: REPROVADO";

&#x20;   }



&#x20;   

&#x20;   

&#x20;    

&#x20;   return 0;

}



Questão 06

\#include <iostream>

\#include <iomanip> 



using namespace std;



int main() {

&#x20;   float valorCompra;



&#x20;   cout << "Digite o valor da compra (R$): ";

&#x20;   cin >> valorCompra;



&#x20;   

&#x20;   if (valorCompra < 0) {

&#x20;       cout << "Erro: O valor da compra não pode ser negativo!" << endl;

&#x20;       return 1; 

&#x20;   }



&#x20;   float porcentagemDesconto = 0.0;



&#x20;   if (valorCompra >= 500) {

&#x20;       porcentagemDesconto = 0.15; 

&#x20;   } else if (valorCompra >= 300) {

&#x20;       porcentagemDesconto = 0.10; 

&#x20;   } else if (valorCompra >= 100) {

&#x20;       porcentagemDesconto = 0.05;  

&#x20;   } else {

&#x20;       porcentagemDesconto = 0.00;  

&#x20;   }



&#x20;   float valorDesconto = valorCompra \* porcentagemDesconto;

&#x20;   float valorFinal = valorCompra - valorDesconto;



&#x20;   cout << fixed << setprecision(2);



&#x20;   cout << "\\n--- RESUMO DA COMPRA ---" << "\\n";

&#x20;   cout << "Valor original: R$ " << valorCompra << "\\n";

&#x20;   cout << "Desconto (" << (porcentagemDesconto \* 100) << "%): R$ " << valorDesconto << "\\n";

&#x20;   cout << "Valor final a pagar: R$ " << valorFinal << "\\n";



&#x20;   return 0;

}



Questão 07



\#include <iostream>



using namespace std;



int main() {

&#x20;   int idade;



&#x20;   cout << "Digite a sua idade: ";

&#x20;   cin >> idade;



&#x20;   if (idade < 0) {

&#x20;       cout << "Erro: A idade nao pode ser negativa!" << endl;

&#x20;   } 

&#x20;   

&#x20;   else if (idade <= 11) {

&#x20;       cout << "Faixa etaria: Crianca" << endl;

&#x20;   } 

&#x20;   else if (idade <= 17) {

&#x20;       cout << "Faixa etaria: Adolescente" << endl;

&#x20;   } 

&#x20;   else if (idade <= 59) {

&#x20;       cout << "Faixa etaria: Adulto" << endl;

&#x20;   } 

&#x20;   else {

&#x20;       cout << "Faixa etaria: Idoso" << endl;

&#x20;   }



&#x20;   return 0;

}



Questão 08



\#include <iostream>

\#include <iomanip> 



using namespace std;



int main() {

&#x20;   double massa, altura;



&#x20;   cout << "Peso (kg): ";

&#x20;   cin >> massa;



&#x20;   cout << "Altura (m): ";

&#x20;   cin >> altura;





&#x20;   if (massa <= 0 || altura <= 0) {

&#x20;       cout << "Erro: Massa e altura devem ser valores maiores que zero!" << endl;

&#x20;       return 1;

&#x20;   }



&#x20;   double imc = massa / (altura \* altura);



&#x20;   

&#x20;   cout << fixed << setprecision(2);

&#x20;   cout << "IMC: " << imc << endl;



&#x20;   cout << "Classificacao: ";

&#x20;   if (imc < 18.5) {

&#x20;       cout << "Abaixo do peso." << endl;

&#x20;   } 

&#x20;   else if (imc < 25.0) {

&#x20;       cout << "Faixa usual." << endl;

&#x20;   } 

&#x20;   else if (imc < 30.0) {

&#x20;       cout << "Sobrepeso." << endl;

&#x20;   } 

&#x20;   else {

&#x20;       cout << "Obesidade." << endl;

&#x20;   }



&#x20;   

&#x20;   cout << "\\nNota: O IMC é um indicador de triagem, não um diagnostico individual." << endl;



&#x20;   return 0;

}



Questão 09



\#include <iostream>



using namespace std;



int main() {

&#x20;   int codigo;

&#x20;   int status;



&#x20;   

&#x20;   cout << "Codigo de acesso: ";

&#x20;   cin >> codigo;



&#x20;   

&#x20;   cout << "Usuario ativo (1-Sim / 0-Nao): ";

&#x20;   cin >> status;



&#x20;   if (codigo == 1234 \&\& status == 1) {

&#x20;       cout << "Acesso autorizado." << endl;

&#x20;   } else {

&#x20;       cout << "Acesso negado." << endl;

&#x20;   }



&#x20;   return 0;

}



questão 10

\#include <iostream>



using namespace std;



int main() {

&#x20;   double num1, num2;

&#x20;   char operacao;



&#x20;  

&#x20;   cout << "Primeiro numero: ";

&#x20;   cin >> num1;



&#x20;   cout << "Segundo numero: ";

&#x20;   cin >> num2;



&#x20;   cout << "Operacao (+, -, \*, /): ";

&#x20;   cin >> operacao;



&#x20;   

&#x20;   if (operacao == '+') {

&#x20;       cout << "Resultado: " << num1 + num2 << endl;

&#x20;   } 

&#x20;   else if (operacao == '-') {

&#x20;       cout << "Resultado: " << num1 - num2 << endl;

&#x20;   } 

&#x20;   else if (operacao == '\*') {

&#x20;       cout << "Resultado: " << num1 \* num2 << endl;

&#x20;   } 

&#x20;   else if (operacao == '/') {

&#x20;       

&#x20;       if (num2 == 0) {

&#x20;           cout << "Erro: Divisao por zero nao permitida!" << endl;

&#x20;       } else {

&#x20;           cout << "Resultado: " << num1 / num2 << endl;

&#x20;       }

&#x20;   } 

&#x20;   else {

&#x20;       

&#x20;       cout << "Erro: Operador invalido!" << endl;

&#x20;   }



&#x20;   return 0;

}





PARTE 2



Questão 11



\#include <iostream>



using namespace std;



int main() {

&#x20;   for (int i = 1; i <= 20; i++) {

&#x20;       cout << i << " ";

&#x20;   }

&#x20;   cout << endl;



&#x20;   return 0;

}



Questão 12



\#include <iostream>



using namespace std;



int main() {

&#x20;   int i = 10;



&#x20;   while (i >= 0) {

&#x20;       cout << i << " ";

&#x20;       i--;

&#x20;   }

&#x20;   

&#x20;   cout << endl << "Fim da contagem!" << endl;



&#x20;   return 0;

}



Questão 13



\#include <iostream>



using namespace std;



int main() {

&#x20;   int n;



&#x20;   cout << "Digite um numero: ";

&#x20;   cin >> n;



&#x20;   for (int i = 1; i <= 10; i++) {

&#x20;       cout << n << " x " << i << " = " << (n \* i) << endl;

&#x20;   }



&#x20;   return 0;

}



Questão 14



\#include <iostream>



using namespace std;



int main() {

&#x20;   int quantidadePares = 0;



&#x20;   for (int i = 1; i <= 100; i++) {

&#x20;       if (i % 2 == 0) {

&#x20;           cout << i << " ";

&#x20;           quantidadePares++;

&#x20;       }

&#x20;   }



&#x20;   cout << endl << "Quantidade de pares encontrados: " << quantidadePares << endl;



&#x20;   return 0;

}



Questão 15



\#include <iostream>



using namespace std;



int main() {

&#x20;   int n;



&#x20;   cout << "Digite N: ";

&#x20;   cin >> n;



&#x20;   

&#x20;   if (n <= 0) {

&#x20;       cout << "Erro: N deve ser um inteiro positivo!" << endl;

&#x20;       return 1;

&#x20;   }



&#x20;   int soma = 0;

&#x20;   int i = 1;



&#x20;   while (i <= n) {

&#x20;       soma += i; 

&#x20;       i++;

&#x20;   }



&#x20;   cout << "Soma: " << soma << endl;



&#x20;   return 0;

}



Questão 16



\#include <iostream>

\#include <iomanip>



using namespace std;



int main() {

&#x20;   double soma = 0.0;

&#x20;   double nota;



&#x20;   for (int i = 1; i <= 10; i++) {

&#x20;       cout << "Digite a nota " << i << " (0 a 10): ";

&#x20;       cin >> nota;



&#x20;      

&#x20;       while (nota < 0.0 || nota > 10.0) {

&#x20;           cout << "Nota invalida! Digite novamente a nota " << i << ": ";

&#x20;           cin >> nota;

&#x20;       }



&#x20;       soma += nota;

&#x20;   }



&#x20;   double media = soma / 10.0;



&#x20;   cout << fixed << setprecision(2);

&#x20;   cout << "Media das 10 notas: " << media << endl;



&#x20;   return 0;

}



Questão 17



\#include <iostream>



using namespace std;



int main() {

&#x20;   int numero;



&#x20;   do {

&#x20;       cout << "Digite um numero entre 1 e 10: ";

&#x20;       cin >> numero;



&#x20;       if (numero < 1 || numero > 10) {

&#x20;           cout << "Valor invalido." << endl;

&#x20;       }

&#x20;   } while (numero < 1 || numero > 10);



&#x20;   cout << "Valor aceito: " << numero << endl;



&#x20;   return 0;

}



Questão 18



\#include <iostream>



using namespace std;



int main() {

&#x20;   int n;



&#x20;   cout << "Digite um numero (0 a 20): ";

&#x20;   cin >> n;



&#x20;   if (n < 0 || n > 20) {

&#x20;       cout << "Erro: Digite um valor entre 0 e 20!" << endl;

&#x20;       return 1;

&#x20;   }



&#x20;   unsigned long long fatorial = 1;



&#x20;   for (int i = 1; i <= n; i++) {

&#x20;       fatorial \*= i;

&#x20;   }



&#x20;   cout << "Fatorial de " << n << ": " << fatorial << endl;



&#x20;   return 0;

}



Questão 19



\#include <iostream>



using namespace std;



int main() {

&#x20;   int n;



&#x20;   cout << "Digite um numero: ";

&#x20;   cin >> n;



&#x20;   if (n <= 1) {

&#x20;       cout << n << " nao e um numero primo." << endl;

&#x20;       return 0;

&#x20;   }



&#x20;   bool ehPrimo = true;



&#x20;   for (int i = 2; i \* i <= n; i++) {

&#x20;       if (n % i == 0) {

&#x20;           ehPrimo = false;

&#x20;           break;

&#x20;       }

&#x20;   }



&#x20;   if (ehPrimo) {

&#x20;       cout << n << " e um numero primo." << endl;

&#x20;   } else {

&#x20;       cout << n << " nao e um numero primo." << endl;

&#x20;   }



&#x20;   return 0;

}



Questão 20



\#include <iostream>



using namespace std;



int main() {

&#x20;   int inicio, fim;



&#x20;   cout << "Inicio do intervalo: ";

&#x20;   cin >> inicio;



&#x20;   cout << "Fim do intervalo: ";

&#x20;   cin >> fim;



&#x20;   if (inicio > fim) {

&#x20;       cout << "Erro: O inicio nao pode ser maior que o fim!" << endl;

&#x20;       return 1;

&#x20;   }



&#x20;   int qtdPrimos = 0;



&#x20;   cout << "Numeros primos: ";



&#x20;   for (int num = inicio; num <= fim; num++) {

&#x20;       if (num <= 1) {

&#x20;           continue;

&#x20;       }



&#x20;       bool ehPrimo = true;

&#x20;       for (int i = 2; i \* i <= num; i++) {

&#x20;           if (num % i == 0) {

&#x20;               ehPrimo = false;

&#x20;               break;

&#x20;           }

&#x20;       }



&#x20;       if (ehPrimo) {

&#x20;           cout << num << " ";

&#x20;           qtdPrimos++;

&#x20;       }

&#x20;   }



&#x20;   cout << endl << "Quantidade de primos: " << qtdPrimos << endl;



&#x20;   return 0;

}

