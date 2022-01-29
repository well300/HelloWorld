# HelloWorld.c

//C learning

#include <stdio.h> 
#include <ctype.h>
#include <stdbool.h> //For Bool
#include <string.h>
#include <math.h>

int main(){
//comments & escape sequences 💬

   //This is a comment blah
   /*
   This 
   is 
   a 
   multiline
   comment
   */
  /* escape sequence = character combination consisting of a backslash \
                      follow by letter or combination of digits.
                      They specify action within a liner or string of text.
                      \n = newline
                      \t = tab
                      */
   /*   
   printf("I\nlike\npizza!\n");
   printf("1\t2\t3\n4\t5\t6\n7\t8\t9\n\n");
   printf("\"Its really good\" - But now im bored of pizza\n\n");
   */

//variables 💰

   // variable = Allocate space in memory to store a value
   //            We refer to a variable's name to acces the store value.
   //            That variable now behaves as if it was the value it contains.
   //            But we need to declair what type of data we are storing.
/*
   int x; //declaration
   x = 123; //initialization
   int y = 321; //declaration + initialization

   int age = 18; //integer [%d]
   float gpa = 7.5; //floating point number [%f]
   char grade = 'B'; //snigle character [%c]
   char name[] = "Bro"; //array of characters [%s]

   printf("Hello %s\n", name);
   printf("You are %d year old\n", age);
   printf("Your grade is %c\n", grade);
   printf("Your gpa is %f\n\n", gpa);
*/
//data types 📊
/*
char a = 'C';                //single character    %c
char b[] = "Bro";            //array of characters %s

float c = 3.141592653589793;           //4 bytes (32 bita of precision) 6 - 7 digits %f
double d = 3.141592653589793; //8 bytes (64 nits of precision) 15 - 16 digits %lf

bool e = false;             //1 byte (true or false) %d

char f = 120;              //1 byte (-128 to +127) %d or %c
unsigned char g = 255;     //1 byte (0 to +255) %d or %c

short h = 32767;          //2 bytes (-32,768 to +32, 767) %d
unsigned short i = 65535; //2 bytes (0 to +65, 535) %d

int j = 2147483647;              //4 bytes (-2,147,483,648 to +2, 147,483,647) %d
unsigned int k = 4294967295l;  //4 bytes (0 to +4, 294, 967, 295) %u

long long int l = 9223372036854775807;             //8 bytes (-9 quintillion to +9 quintillion) %lld
unsigned long long int m = 18446744073709551615U;  //8 bytes (0 to +18 quintillion) %llu

//printf("%c\n", a);   // char
//printf("%s\n", b);   // character array
//printf("%0.15f\n", c);   //float
//printf("%0.15lf\n", d);  //double
//printf("%d\n", e);   //bool
//printf("%c\n", f);   //char as numeric value
//printf("%d\n", g);   //unsigned char as numeric value
//printf("%d\n", h);   // short
//printf("%d\n", i);   // unsigned short
//printf("%d\n", j);   // int
//printf("%u\n", k);   // unsigned int
//printf("%lld\n", l); // long long int
//printf("%llu\n", m); // unsigned long long int
*/

//format specifiers 🔧

// Formate specifier % = defines and formate a type of data to be displayed

// %c = character
// %s = string (array of characters)
// %f = float
// %lf = double
// %d = integer

// %.1 = decimal precision
// %1 = minimum field width
// %- = left align

/*
float item1 = 5.75;
float item2 = 10.00;
float item3 = 100.99;

printf("Item 1: ₹%8.2f\n", item1);
printf("Item 2: ₹%8.2f\n", item2);
printf("Item 3: ₹%8.2f\n\n", item3);
*/

//constants 🚫

/*constent = fixed value that cannot by the program during its exexution

float PI = 3.14169;

printf("%f\n\n", PI);*/

//arithmetic operators ➗

// + (addition)
// - (subtraction)
// * (multiplication)
// / (division)
// % (modilis)
// ++ increment
// -- decrement 

//int n = 4;
//int o = 2; 

//int p = n + o;
//int p = n - o;
//int p = n * o;
//float p = n / (float) o;
//int p = n % o;

//n++;
//o--;

//printf("%d", n);

//augmented assignment operators 🧮

//augmented assignment operators = used to replace a statement where an operator
//                                 takes a variable as one of its arguments
//                                 and then assigns the result back to the same variable
//                                 x = x + 1 
//                                 x+=1

//int q = 10;

// q = q + 2;
// q+=2;

// q = q - 3;
// q-=3;

// q = q * 4;
//q*=4;

//q = q / 5;
//q/=5;

//q = q % 2;
//q%=2;

//printf("%d", q);

//user input ⌨️

/*

char name[25]; //bytes
int age;

printf("\nWhat is your name");
//scanf("%s", &name);
fgets(name, 25, stdin);
name[strlen(name)-1] = '\0';

printf("\nHow old are you?");
scanf("%d", &age);

printf("\nHello %s, how are you?", name);
printf("\nYou are %d year old", age);

*/

//math functions 📚

/*    
    double A = sqrt(9);
    double B = pow(2, 4);
    int C = round(3.14);
    int D = ceil(3.14);
    int E = floor(3.99);
    double F  = fabs(-100);
    double G = log(3);
    double H = sin(45);
    double I = cos(45);
    double J = tan(45);

    printf("\n%lf", J);

*/

//circle circumference program ⚪
/*
    const double PI = 3.14159;
    double radius;
    double circumference;
    double area;

    printf("\nEnter the radius of a circle: ");
    scanf("%lf", &radius);

    circumference = 2 * PI * radius;
    area = PI * radius * radius;

    printf("\ncircumference: %lf", circumference);
    printf("\narea: %lf", area);
*/

//hypotenuse calculator program 📐

/*
      double A;
      double B;
      double C;

      printf("Enter side A: ");
      scanf("%lf", &A);

      printf("Enter side B: ");
      scanf("%lf", &B);

      C = sqrt(A*A + B*B);

      printf("Side C: %lf", C);
*/

//if statements ✔️
/*
        int age;

        printf("\nEnter your age: ");
        scanf("%d", &age);

        if(age >= 18){
           printf("You are now signed up!");
        }
        else if(age ==0){
           printf("You can't sign up! You were just born!");
        }
        else if( age < 0){
           printf("You haven't been yet!");
        }
        else{
           printf("you are too yound to sign up!");
        }
*/

//switch statements 🔽

// switch = A more efficient alternative to using many "else if" statement
//          allows a value to be tested for equality  against many cases
/*
char grade;

printf("\nEnter a latter grade: ");
scanf("%c", &grade);

if(grade == 'A'){
   printf("perfect!\n");
}
else if(grade == 'B'){
   printf("You did good!\n");
}
else if(grade == 'C'){
   printf("You did okay!\n");
}
else if(grade == 'D'){
   printf("At least it's not an F!\n");
}
else if(grade == 'F'){
   printf("YOU FAILED!\n");
}
else{
   printf("That's not a valid grade");
}


switch(grade){
   case 'A':
      printf("Perfect!\n");
      break;
   case 'B':
      printf("You did good!\n");
      break;
   case 'C':
      printf("You did okay!\n");
      break;
   case 'D':
      printf("At least it's not an F!\n");
      break;
   case 'F':
      printf("YOU FAILED!\n");
      break;
   default:
      printf("That's not a valid grade");        
         
}
*/

//temperature conversion program 🌡️

/*
     char unit;
     float temp;

     printf("\nIs the temperature in (F) or (C): ");
     scanf("%c", &unit);

     unit = toupper(unit);

     if(unit == 'C'){
        printf("\nEnter the temp in Celsius: ");
        scanf("%f", &temp);
        temp = (temp * 9/5) + 32;
        printf("\nThe temp in Farenheit is: %.1f", temp);
     }
     else if(unit == 'F'){
        printf("\nEnter the temp in Farenheit: ");
        scanf("%f", &temp);
        temp = ((temp- 32) * 5) / 9;
        printf("\nThe temp in Celsius is: %.1f", temp);        
     }
     else{
        printf("\n %c is not a valid unit of measurement", unit);
     }
*/

//calculator program 🖩

/*
         char operator;
         double num1;
         double num2;
         double result;

         printf("\nEnter an operator (+ - * /): ");
         scanf("%c", &operator);

         printf("Enter number 1: ");
         scanf("%lf", &num1);

         printf("Enter number 2: ");
         scanf("%lf", &num2);

         switch(operator){
            case '+':
               result = num1 + num2;
               printf("\nresult: %lf", result);
               break;
            case '-':
               result = num1 - num2;
               printf("\nresult: %lf", result);
               break; 
            case '*':
               result = num1 * num2;
               printf("\nresult: %lf", result);
               break;
            case '/':
               result = num1 / num2;
               printf("\nresult: %lf", result);
               break;                                
            default:
                 printf("%c is not valid", operator);
         }      
*/

// AND logical operator &&

/*
  // logical operators = && (AND) checls if two conditions are true

   float temp = 25;
   bool sunny = true;

   if(temp >= 0 && temp <= 30 && sunny){
      printf("The weather is good!");

   }
   else{
      printf("\nThe weather is bad!");
   }
*/

