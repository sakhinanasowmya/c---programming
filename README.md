QUESTION 1 : PRINT A HELLO WORLD 
#include <stdio.h>

int main() {
    // Write C code here
    printf("Hello world");

    return 0;
}


QUESTION 2 : SUM OF TWO NUMBERS 
#include <stdio.h>

int main() {
   int num1, num2, sum;

   printf("Enter the first number: ");
   scanf("%d", &num1);

   printf("Enter the second number: ");
   scanf("%d", &num2);

   sum = num1 + num2;

   printf("The sum of %d and %d is %d\n", num1, num2, sum);

   return 0;
}


QUESTION 3 : CALUCATE a+b*c
#include <stdio.h>

int main() {
   int a, b, c, result;

   printf("Enter the value of a: ");
   scanf("%d", &a);

   printf("Enter the value of b: ");
   scanf("%d", &b);

   printf("Enter the value of c: ");
   scanf("%d", &c);

   result = a + b*c;

   printf("The result of %d + %d*%d is %d\n", a, b, c, result);

   return 0;
}

QUESTION  4: AREA OF CIRCLE 
#include <stdio.h>

#define PI 3.14159

int main() {
    double radius, area;
    
    printf("Enter the radius of the circle: ");
    scanf("%lf", &radius);
    
    area = PI * radius * radius;
    
    printf("The area of the circle with radius %lf is %lf\n", radius, area);
    
    return 0;
}



QUESTION 5 : TEMPERATURE CONVERSION 
#include <stdio.h>

int main() {
    float celsius, fahrenheit;
    
    printf("Enter temperature in Celsius: ");
    scanf("%f", &celsius);
    
    fahrenheit = (celsius * 1.8) + 32;
    
    printf("%.2f Celsius = %.2f Fahrenheit\n", celsius, fahrenheit);
    
    return 0;
}


QUESTION 6: SIMPLE INTEREST CALCULATION
#include <stdio.h>

int main() {
    float principle, rate, time, interest;
    
    printf("Enter principle amount: ");
    scanf("%f", &principle);
    
    printf("Enter rate of interest: ");
    scanf("%f", &rate);
    
    printf("Enter time period: ");
    scanf("%f", &time);
    
    interest = (principle * rate * time) / 100;
    
    printf("Simple Interest = %.2f\n", interest);
    
    return 0;
}

QUESTION 7:SWAP TWO NUMBERS 
#include <stdio.h>

int main() {
    int a, b, temp;
    
    printf("Enter two numbers to swap: ");
    scanf("%d %d", &a, &b);
    
    printf("Before swapping: a = %d, b = %d\n", a, b);
    
    temp = a;
    a = b;
    b = temp;
    
    printf("After swapping: a = %d, b = %d\n", a, b);
    
    return 0;
}


QUESTION 8: REVERSE 3 DIGITS 
#include <stdio.h>

int main() {
    int num, rev = 0, rem;
    
    printf("Enter a three-digit number: ");
    scanf("%d", &num);
    
    while (num != 0) {
        rem = num % 10;
        rev = rev * 10 + rem;
        num /= 10;
    }
    
    printf("The reversed number is: %d\n", rev);
    
    return 0;
}


QUESTION 9: REVERSE 4 DIGIT NUMBER 
#include <stdio.h>

int main() {
    int num, rev = 0, rem;
    
    printf("Enter a four-digit number: ");
    scanf("%d", &num);
    
    while (num != 0) {
        rem = num % 10;
        rev = rev * 10 + rem;
        num /= 10;
    }
    
    printf("The reversed number is: %d\n", rev);
    
    return 0;
}


QUESTION 10: SUM OF ASCII VALUES
#include <stdio.h>

int main() {
    char str[100];
    int sum = 0;
    
    printf("Enter a string: ");
    fgets(str, 100, stdin); // read string with spaces using fgets
    
    for (int i = 0; str[i] != '\0'; i++) {
        sum += str[i];
    }
    
    printf("The sum of ASCII values is: %d\n", sum);
    
    return 0;
}


QUESTION 11:BIGGEST OF TWO NUMBER
#include <stdio.h>

int main() {
    int num1, num2;
    
    printf("Enter the first number: ");
    scanf("%d", &num1);
    
    printf("Enter the second number: ");
    scanf("%d", &num2);
    
    if (num1 > num2) {
        printf("%d is the biggest number.\n", num1);
    } else {
        printf("%d is the biggest number.\n", num2);
    }
    
    return 0;
}


QUESTION 12:BIGGEST TWO NUMBERS
#include <stdio.h>

int main() {
    int num1, num2;
    
    printf("Enter the first number: ");
    scanf("%d", &num1);
    
    printf("Enter the second number: ");
    scanf("%d", &num2);
    
    if (num1 > num2) {
        printf("%d is the biggest number.\n", num1);
    } else {
        printf("%d is the biggest number.\n", num2);
    }
    
    return 0;
}

QUESTION 13 :BIGGEST THREE NUMBERS
#include <stdio.h>

int main() {
    int num1, num2, num3;
    
    printf("Enter the first number: ");
    scanf("%d", &num1);
    
    printf("Enter the second number: ");
    scanf("%d", &num2);
    
    printf("Enter the third number: ");
    scanf("%d", &num3);
    
    if (num1 > num2 && num1 > num3) {
        printf("%d is the biggest number.\n", num1);
    } else if (num2 > num1 && num2 > num3) {
        printf("%d is the biggest number.\n", num2);
    } else {
        printf("%d is the biggest number.\n", num3);
    }
    
    return 0;
}


QUESTION 14: EVEN OR ODD
#include <stdio.h>

int main() {
    int num;
    
    printf("Enter a number: ");
    scanf("%d", &num);
    
    if (num % 2 == 0) {
        printf("%d is an even number.\n", num);
    } else {
        printf("%d is an odd number.\n", num);
    }
    
    return 0;
}

QUESTION 15:TYPES OF TRIANGLE
#include <stdio.h>

int main() {
    int side1, side2, side3;
    
    printf("Enter the lengths of three sides of a triangle: ");
    scanf("%d %d %d", &side1, &side2, &side3);
    
    if (side1 == side2 && side2 == side3) {
        printf("The triangle is an equilateral triangle.\n");
    } else if (side1 == side2 || side2 == side3 || side3 == side1) {
        printf("The triangle is an isosceles triangle.\n");
    } else {
        printf("The triangle is a scalene triangle.\n");
    }
    
    return 0;
}

QUESTION 16: LEAP YEAR OR NOT
#include <stdio.h>

int main() {
    int year;
    
    printf("Enter a year: ");
    scanf("%d", &year);
    
    if (year % 4 == 0) {
        if (year % 100 == 0) {
            if (year % 400 == 0) {
                printf("%d is a leap year.\n", year);
            } else {
                printf("%d is not a leap year.\n", year);
            }
        } else {
            printf("%d is a leap year.\n", year);
        }
    } else {
        printf("%d is not a leap year.\n", year);
    }
    
    return 0;
}


QUESTION 17:ARMSTRONG OR NOT
#include <stdio.h>
#include <math.h>

int main() {
    int num, originalNum, remainder, n = 0, result = 0, power;
    
    printf("Enter an integer: ");
    scanf("%d", &num);
    
    originalNum = num;
    
    // count the number of digits in the given number
    while (originalNum != 0) {
        originalNum /= 10;
        ++n;
    }
    
    originalNum = num;
    
    // calculate the sum of nth powers of its digits
    while (originalNum != 0) {
        remainder = originalNum % 10;
        
        // raise the remainder to the power of n and add to the result
        power = round(pow(remainder, n));
        result += power;
        
        originalNum /= 10;
    }
    
    // check if the sum is equal to the given number
    if (result == num) {
        printf("%d is an Armstrong number.\n", num);
    } else {
        printf("%d is not an Armstrong number.\n", num);
    }
    
    return 0;
}


QUESTION 18: ROOTS OF QUADRATIC EQUATIONS
#include <stdio.h>
#include <math.h>

int main() {
    double a, b, c, discriminant, root1, root2, realPart, imaginaryPart;
    
    printf("Enter coefficients a, b and c: ");
    scanf("%lf %lf %lf", &a, &b, &c);
    
    // calculate the discriminant
    discriminant = b * b - 4 * a * c;
    
    // check if discriminant is positive, negative, or zero
    if (discriminant > 0) {
        // calculate the two real roots
        root1 = (-b + sqrt(discriminant)) / (2 * a);
        root2 = (-b - sqrt(discriminant)) / (2 * a);
        
        printf("Roots are real and different.\n");
        printf("Root1 = %.2lf\n", root1);
        printf("Root2 = %.2lf\n", root2);
    } else if (discriminant == 0) {
        // calculate the real and equal roots
        root1 = root2 = -b / (2 * a);
        
        printf("Roots are real and same.\n");
        printf("Root1 = Root2 = %.2lf\n", root1);
    } else {
        // calculate the real and imaginary parts of the roots
        realPart = -b / (2 * a);
        imaginaryPart = sqrt(-discriminant) / (2 * a);
        
        printf("Roots are complex and different.\n");
        printf("Root1 = %.2lf + %.2lfi\n", realPart, imaginaryPart);
        printf("Root2 = %.2lf - %.2lfi\n", realPart, imaginaryPart);
    }
    
    return 0;
}


QUESTION 19:QUADRANT OF A POINT
#include <stdio.h>

int main() {
    float x, y;
    
    printf("Enter the coordinates of the point: ");
    scanf("%f %f", &x, &y);
    
    if (x > 0 && y > 0) {
        printf("The point (%.2f, %.2f) is in the First quadrant.\n", x, y);
    } else if (x < 0 && y > 0) {
        printf("The point (%.2f, %.2f) is in the Second quadrant.\n", x, y);
    } else if (x < 0 && y < 0) {
        printf("The point (%.2f, %.2f) is in the Third quadrant.\n", x, y);
    } else if (x > 0 && y < 0) {
        printf("The point (%.2f, %.2f) is in the Fourth quadrant.\n", x, y);
    } else if (x == 0 && y == 0) {
        printf("The point (%.2f, %.2f) is at the origin.\n", x, y);
    } else if (x == 0 && y != 0) {
        printf("The point (%.2f, %.2f) lies on the Y-axis.\n", x, y);
    } else if (x != 0 && y == 0) {
        printf("The point (%.2f, %.2f) lies on the X-axis.\n", x, y);
    }
    
    return 0;
}

QUESTION  20: DAYSOFWEEK
#include <stdio.h>

int main() {
    int day, month, year, dayOfWeek;
    int t[] = {0, 3, 2, 5, 0, 3, 5, 1, 4, 6, 2, 4};
    char* days[] = {"Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"};

    printf("Enter the date in format (DD/MM/YYYY): ");
    scanf("%d/%d/%d", &day, &month, &year);

    if (month < 3) {
        year -= 1;
    }

    dayOfWeek = (year + year/4 - year/100 + year/400 + t[month-1] + day) % 7;
    
    printf("The day of the week for %d/%d/%d is %s.\n", day, month, year, days[dayOfWeek]);
    
    return 0;
}

QUESTION 21: CHOICE BASED ARITHEMIC 
#include <stdio.h>

int main() {
    int a, b, choice, result;
    
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);
    
    printf("Choose the operation:\n");
    printf("1. Addition\n");
    printf("2. Subtraction\n");
    printf("3. Multiplication\n");
    printf("4. Division\n");
    
    scanf("%d", &choice);
    
    switch(choice) {
        case 1:
            result = a + b;
            printf("%d + %d = %d\n", a, b, result);
            break;
        case 2:
            result = a - b;
            printf("%d - %d = %d\n", a, b, result);
            break;
        case 3:
            result = a * b;
            printf("%d * %d = %d\n", a, b, result);
            break;
        case 4:
            if (b == 0) {
                printf("Error: division by zero.\n");
            } else {
                result = a / b;
                printf("%d / %d = %d\n", a, b, result);
            }
            break;
        default:
            printf("Error: invalid choice.\n");
    }
    
    return 0;
}


QUESTION 22: VOWELS OR CONSTANT 
#include <stdio.h>

int main() {
    char ch;

    printf("Enter a character: ");
    scanf("%c", &ch);

    if(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' || ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
        printf("%c is a vowel\n", ch);
    } else {
        printf("%c is a consonant\n", ch);
    }

    return 0;
}

QUESTION 23: INCOME TAX CALCULATION
#include <stdio.h>

int main() {
    float income, tax;

    printf("Enter your income: ");
    scanf("%f", &income);

    if(income <= 250000) {
        tax = 0;
    } else if(income <= 500000) {
        tax = (income - 250000) * 0.05;
    } else if(income <= 1000000) {
        tax = 12500 + ((income - 500000) * 0.2);
    } else {
        tax = 112500 + ((income - 1000000) * 0.3);
    }

    printf("Your income tax is %.2f\n", tax);

    return 0;
}


QUESTION 24: ENERGY BILL CALCULATION
#include <stdio.h>

int main() {
    float units, bill;

    printf("Enter the units consumed: ");
    scanf("%f", &units);

    if(units <= 50) {
        bill = units * 0.5;
    } else if(units <= 150) {
        bill = 25 + ((units - 50) * 0.75);
    } else if(units <= 250) {
        bill = 100 + ((units - 150) * 1.20);
    } else {
        bill = 220 + ((units - 250) * 1.50);
    }

    printf("Your energy bill is %.2f\n", bill);

    return 0;
}

                             SET -3
                             
QUESTION 25: SUM OF NUMBER RANGE 
#include <stdio.h>

int main() {
    int start, end, sum = 0;

    printf("Enter the start and end numbers: ");
    scanf("%d %d", &start, &end);

    for(int i = start; i <= end; i++) {
        sum += i;
    }

    printf("The sum of numbers between %d and %d is %d\n", start, end, sum);

    return 0;
}

QUESTION 26: SUM OF DIGITS IN A GIVEN NUMBER 
#include <stdio.h>

int main() {
    int num, sum = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    for(; num != 0; num /= 10) {
        int digit = num % 10;
        sum += digit;
    }

    printf("The sum of digits is: %d\n", sum);

    return 0;
}


QUESTION 27: REVERSE THE NUMBERS 
#include <stdio.h>

int main() {
    int num, reverse = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    while(num != 0) {
        int digit = num % 10;
        reverse = reverse * 10 + digit;
        num /= 10;
    }

    printf("The reversed number is: %d\n", reverse);

    return 0;
}


QUESTION 28 : GCD OF TWO NUMBERS 
#include <stdio.h>

int main() {
    int num1, num2, gcd;

    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);

    // GCD cannot be greater than the smaller number
    int smaller = (num1 < num2) ? num1 : num2;

    for(int i = 1; i <= smaller; i++) {
        if(num1 % i == 0 && num2 % i == 0) {
            gcd = i;
        }
    }

    printf("The GCD of %d and %d is %d\n", num1, num2, gcd);

    return 0;
}


QUESTION 29 : LCM OF TWO NUMBERS 
#include <stdio.h>

int main()
{
    int num1, num2, lcm, max;
    
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);

    max = (num1 > num2) ? num1 : num2;

    while(1)
    {
        if(max % num1 == 0 && max % num2 == 0)
        {
            lcm = max;
            break;
        }
        max++;
    }

    printf("LCM of %d and %d is %d.", num1, num2, lcm);

    return 0;
}

QUESTION 30: FACTORIAL 
#include <stdio.h>

int main()
{
    int num, i, fact = 1;
    
    printf("Enter a number: ");
    scanf("%d", &num);

    for(i = 1; i <= num; i++)
    {
        fact *= i;
    }

    printf("Factorial of %d is %d.", num, fact);

    return 0;
}


QUESTION 31: SUM OF FACTORS 
#include <stdio.h>

int main()
{
    int num, i, sum = 0;
    
    printf("Enter a number: ");
    scanf("%d", &num);

    for(i = 1; i <= num; i++)
    {
        if(num % i == 0)
        {
            sum += i;
        }
    }

    printf("Sum of factors of %d is %d.", num, sum);

    return 0;
}

QUESTION 32: PRIME NUMBERS OR NOT
#include <stdio.h>

int main()
{
    int num, i, isPrime = 1;
    
    printf("Enter a number: ");
    scanf("%d", &num);

    if(num == 1)
    {
        isPrime = 0;
    }
    else
    {
        for(i = 2; i <= num/2; i++)
        {
            if(num % i == 0)
            {
                isPrime = 0;
                break;
            }
        }
    }

    if(isPrime)
    {
        printf("%d is a prime number.", num);
    }
    else
    {
        printf("%d is not a prime number.", num);
    }

    return 0;
}


QUESTION 33: CUMMULATIVE INTEREST CALCULATION 
#include <stdio.h>

int main()
{
    float principal, rate, time, interest, cumulative_interest;
    int i, n;

    printf("Enter principal amount: ");
    scanf("%f", &principal);

    printf("Enter rate of interest: ");
    scanf("%f", &rate);

    printf("Enter time period in years: ");
    scanf("%f", &time);

    printf("Enter number of times interest is compounded per year: ");
    scanf("%d", &n);

    cumulative_interest = 0;
    for (i = 1; i <= n * time; i++)
    {
        interest = principal * rate / n / 100;
        principal += interest;
        cumulative_interest += interest;
    }

    printf("Cumulative interest = %.2f\n", cumulative_interest);
    printf("Total amount = %.2f\n", principal);

    return 0;
}



QUESTION  34: FIBONACCI SERIES 
#include <stdio.h>

int main() {
    int n, i, t1 = 0, t2 = 1, nextTerm;

    printf("Enter the number of terms: ");
    scanf("%d", &n);

    printf("Fibonacci Series: ");

    for (i = 1; i <= n; ++i) {
        printf("%d, ", t1);
       
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
    }


QUESTION 35: NCr calaculation  
#include <stdio.h>

int main() {
    int n, r, i, nCr = 1;

    printf("Enter the value of n and r: ");
    scanf("%d %d", &n, &r);

    for (i = 1; i <= r; ++i) {
 
        nCr *= n - i + 1;
        nCr /= i;
    }

    printf("nCr = %d", nCr);

    return 0;
}

QUESTION 36: LIST/COUNT OF PRIME NUMBERS 
#include <stdio.h>

int main() {
    int n, i, j, count = 0;

    printf("Enter the value of n: ");
    scanf("%d", &n);

    // Loop through numbers up to n
    for (i = 2; i <= n; ++i) {
        // Assume the number is prime
        int isPrime = 1;

        // Check if the number is divisible by any number up to i/2
        for (j = 2; j <= i/2; ++j) {
            if (i % j == 0) {
                isPrime = 0;
                break;
            }
        }

        // If the number is prime, print it and increment the count
        if (isPrime) {
            printf("%d ", i);
            ++count;
        }
    }

    printf("\nCount of prime numbers up to %d is: %d", n, count);

    return 0;
}

QUESTION 37: DIGITAL ROOT OF GIVEN NUMBER 
#include <stdio.h>

int main() {
    int num, sum = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    // Calculate the sum of the digits
    while (num > 0) {
        sum += num % 10;
        num /= 10;
    }

    // If the sum is a two-digit number, continue summing the digits
    while (sum > 9) {
        int temp = sum;
        sum = 0;
        while (temp > 0) {
            sum += temp % 10;
            temp /= 10;
        }
    }

    printf("Digital root of the number is: %d", sum);
    
    
    QUESTION 38: COUNT LEAP YEARS IN GIVEN RANGE 
#include <stdio.h>

int main() {
    int startYear, endYear, count = 0;

    printf("Enter the start year: ");
    scanf("%d", &startYear);

    printf("Enter the end year: ");
    scanf("%d", &endYear);

    // Loop through years from startYear to endYear
    for (int year = startYear; year <= endYear; ++year) {
        // Check if the year is a leap year
        if ((year % 4 == 0 && year % 100 != 0) || year % 400 == 0) {
            ++count;
        }
    }

    printf("Number of leap years between %d and %d is: %d", startYear, endYear, count);

    return 0;
}


    return 0;
}

QUESTION 39: SUM OF TRIANGULAR NUMBERS 
#include <stdio.h>

int main() {
    int n, sum = 0;

    printf("Enter the value of n: ");
    scanf("%d", &n);

    // Loop through the first n triangular numbers
    for (int i = 1; i <= n; ++i) {
        sum += (i * (i + 1)) / 2;
    }

    printf("The sum of the first %d triangular numbers is: %d", n, sum);

    return 0;
}


QUESTION 40: NUMBERS PATTERN 
#include <stdio.h>

int main() {
    int n;

    printf("Enter the number of rows: ");
    scanf("%d", &n);

    // Loop through rows
    for (int i = 1; i <= n; ++i) {
        // Loop through columns
        for (int j = 1; j <= i; ++j) {
            printf("%d ", j);
        }
        printf("\n");
    }

    return 0;
}


QUESTION 41: NUMBERS PATTERN
#include <stdio.h>

int main() {
    int n;

    printf("Enter the number of rows: ");
    scanf("%d", &n);

    // Loop through rows
    for (int i = 1; i <= n; ++i) {
        // Loop through columns
        for (int j = 1; j <= i; ++j) {
            printf("%d ", j);
        }
        printf("\n");
    }

    return 0;
}


QUESTION 42: PASCAL TRIANGLE 
#include <stdio.h>

int main() {
    int n, c, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &n);

    // Loop through rows
    for (i = 0; i < n; i++) {
        // Print spaces for right alignment
        for (c = 0; c <= n - i - 2; c++) {
            printf(" ");
        }
        // Loop through columns
        for (j = 0; j <= i; j++) {
            // Calculate the value using the binomial coefficient
            int coefficient = 1;
            for (c = 1; c <= j; c++) {
                coefficient = coefficient * (i - c + 1) / c;
            }
            printf("%4d", coefficient);
        }
        printf("\n");
    }

    return 0;
}

QUESTION 43: SUM AND AVERAGE OF 1D ARRAY
#include <stdio.h>

int main() {
    int arr[100], n, i;
    float sum = 0, avg;

    printf("Enter the size of array: ");
    scanf("%d", &n);

    printf("Enter %d elements in the array:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        sum += arr[i]; // Calculate sum of elements
    }

    avg = sum / n; // Calculate average of elements

    printf("Sum of elements in the array: %.2f\n", sum);
    printf("Average of 
    
    elements in the array: %.2f\n", avg);

    return 0;
}


QUESTION 45:  MIN AND MAX OF 1D ARRAY
#include <stdio.h>

int main() {
    int arr[100], n, i, min, max;

    printf("Enter the size of array: ");
    scanf("%d", &n);

    printf("Enter %d elements in the array:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Initialize min and max with the first element of the array
    min = max = arr[0];

    // Find the minimum and maximum values
    for(i = 1; i < n; i++) {
        if(arr[i] < min) {
            min = arr[i];
        }
        if(arr[i] > max) {
            max = arr[i];
        }
    }

    printf("Minimum value in the array: %d\n", min);
    printf("Maximum value in the array: %d\n", max);

    return 0;
}


QUESTION 46: REVERSE THE ARRAY 
#include <stdio.h>

int main() {
    int arr[100], n, i, temp;

    printf("Enter the size of array: ");
    scanf("%d", &n);

    printf("Enter %d elements in the array:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Reverse the elements of the array
    for(i = 0; i < n/2; i++) {
        temp = arr[i];
        arr[i] = arr[n-i-1];
        arr[n-i-1] = temp;
    }

    printf("Array elements after reversing:\n");
    for(i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}


QUESTION 47: DIFF EVEN AND ODD NUMBERS 
#include <stdio.h>

int main() {
    int arr[100], n, i, evenSum = 0, oddSum = 0, diff;

    printf("Enter the size of array: ");
    scanf("%d", &n);

    printf("Enter %d elements in the array:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Calculate the sum of even and odd numbers in the array
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0) {
            evenSum += arr[i];
        } else {
            oddSum += arr[i];
        }
    }

    // Calculate the difference between the sum of even and odd numbers
    diff = evenSum - oddSum;

    printf("Sum of even numbers: %d\n", evenSum);
    printf("Sum of odd numbers: %d\n", oddSum);
    printf("Difference between the sum of even and odd numbers: %d\n", diff);

    return 0;
}


QUESTION  48: DIFF BETWEEN EVEN AND ODD INDEXED NUMBERS 
#include <stdio.h>

int main() {
    int arr[100], n, i, evenSum = 0, oddSum = 0, diff;

    printf("Enter the size of array: ");
    scanf("%d", &n);

    printf("Enter %d elements in the array:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Calculate the sum of even-indexed and odd-indexed numbers in the array
    for(i = 0; i < n; i++) {
        if(i % 2 == 0) {
            evenSum += arr[i];
        } else {
            oddSum += arr[i];
        }
    }

    // Calculate the difference between the sum of even-indexed and odd-indexed numbers
    diff = evenSum - oddSum;

    printf("Sum of even-indexed numbers: %d\n", evenSum);
    printf("Sum of odd-indexed numbers: %d\n", oddSum);
    printf("Difference between the sum of even-indexed and odd-indexed numbers: %d\n", diff);

    return 0;
}


QUESTION 49: DECIMAL TO BIN/HEX/OCTAL CONVERSATION 
#include <stdio.h>

int main() {
    int decimal, quotient, remainder, binary = 0, i = 1, octal = 0, j = 1;

    printf("Enter a decimal number: ");
    scanf("%d", &decimal);

    quotient = decimal;

    // Convert decimal to binary
    while(quotient != 0) {
        remainder = quotient % 2;
        binary += remainder * i;
        i *= 10;
        quotient /= 2;
    }

    // Convert decimal to octal
    quotient = decimal;
    while(quotient != 0) {
        remainder = quotient % 8;
        octal += remainder * j;
        j *= 10;
        quotient /= 8;
    }

    printf("Decimal number = %d\n", decimal);
    printf("Binary number = %d\n", binary);
    printf("Octal number = %d\n", octal);

    return 0;
}


QUESTION 50: BIN/OCTAL/HEX CONVERSATION TO DECIMAL 
#include <stdio.h>
#include <math.h>

int main() {
    int decimal = 0, binary, octal, hexadecimal;

    // Convert binary to decimal
    printf("Enter a binary number: ");
    scanf("%d", &binary);
    int i = 0;
    while(binary != 0) {
        int remainder = binary % 10;
        decimal += remainder * pow(2, i);
        binary /= 10;
        i++;
    }
    printf("Decimal number = %d\n", decimal);

    // Convert octal to decimal
    decimal = 0;
    printf("Enter an octal number: ");
    scanf("%d", &octal);
    i = 0;
    while(octal != 0) {
        int remainder = octal % 10;
        decimal += remainder * pow(8, i);
        octal /= 10;
        i++;
    }
    printf("Decimal number = %d\n", decimal);

    // Convert hexadecimal to decimal
    decimal = 0;
    char hexadecimal_str[20];
    printf("Enter a hexadecimal number: ");
    scanf("%s", hexadecimal_str);
    int length = strlen(hexadecimal_str);
    for(int i = 0; i < length; i++) {
        int value;
        if(hexadecimal_str[i] >= '0' && hexadecimal_str[i] <= '9') {
            value = hexadecimal_str[i] - '0';
        } else if(hexadecimal_str[i] >= 'A' && hexadecimal_str[i] <= 'F') {
            value = hexadecimal_str[i] - 'A' + 10;
        } else if(hexadecimal_str[i] >= 'a' && hexadecimal_str[i] <= 'f') {
            value = hexadecimal_str[i] - 'a' + 10;
        }
        decimal += value * pow(16, length - i - 1);
    }
    printf("Decimal number = %d\n", decimal);

    return 0;
}


QUESTION 51: NO.OF DAYS ELAPSED 
#include <stdio.h>

// Function to check if a given year is a leap year
int isLeapYear(int year) {
    if((year % 4 == 0 && year % 100 != 0) || year % 400 == 0) {
        return 1;
    } else {
        return 0;
    }
}

// Function to calculate the number of days in a given month of a given year
int getDaysInMonth(int month, int year) {
    switch(month) {
        case 2:
            if(isLeapYear(year)) {
                return 29;
            } else {
                return 28;
            }
        case 4:
        case 6:
        case 9:
        case 11:
            return 30;
        default:
            return 31;
    }
}

int main() {
    int day1, month1, year1;
    int day2, month2, year2;

    printf("Enter the first date (dd/mm/yyyy): ");
    scanf("%d/%d/%d", &day1, &month1, &year1);

    printf("Enter the second date (dd/mm/yyyy): ");
    scanf("%d/%d/%d", &day2, &month2, &year2);

    // Calculate the number of days between the two dates
    int days = 0;
    // Count the number of days elapsed in year1
    for(int i = month1; i <= 12; i++) {
        days += getDaysInMonth(i, year1);
    }
    days -= day1;
    // Count the number of days elapsed in years between year1 and year2
    for(int i = year1 + 1; i < year2; i++) {
        if(isLeapYear(i)) {
            days += 366;
        } else {
            days += 365;
        }
    }
    // Count the number of days elapsed in year2
    for(int i = 1; i < month2; i++) {
        days += getDaysInMonth(i, year2);
    }
    days += day2;

    printf("Number of days elapsed between the two dates: %d\n", days);

    return 0;
}


QUESTION 52: ARRAY SORTING -BUUBLE SORT 

#include <stdio.h>

void bubbleSort(int arr[], int n) {
    int i, j, temp;
    for(i = 0; i < n - 1; i++) {
        for(j = 0; j < n - i - 1; j++) {
            if(arr[j] > arr[j + 1]) {
                // swap arr[j] and arr[j + 1]
                temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
}

int main() {
    int arr[] = {5, 3, 8, 4, 2};
    int n = sizeof(arr) / sizeof(arr[0]);
    int i;
    printf("Original array: ");
    for(i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
    bubbleSort(arr, n);
    printf("Sorted array: ");
    for(i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
    return 0;
}


QUESTION 53: LINEAR SEARCH 
#include <stdio.h>

int linearSearch(int arr[], int n, int target) {
    int i;
    for(i = 0; i < n; i++) {
        if(arr[i] == target) {
            return i; // return the index of the target value
        }
    }
    return -1; // target value not found
}

int main() {
    int arr[] = {5, 3, 8, 4, 2};
    int n = sizeof(arr) / sizeof(arr[0]);
    int target = 8;
    int index = linearSearch(arr, n, target);
    if(index == -1) {
        printf("Target value not found in the array\n");
    } else {
        printf("Target value found at index %d\n", index);
    }
    return 0;
}
 
QUESTION 54: TOGGLE CASE 

#include <stdio.h>
#include <string.h>

void toggleCase(char *str) {
    int i;
    int len = strlen(str);
    for(i = 0; i < len; i++) {
        if(str[i] >= 'A' && str[i] <= 'Z') {
            str[i] = str[i] + 32; // convert uppercase to lowercase
        } else if(str[i] >= 'a' && str[i] <= 'z') {
            str[i] = str[i] - 32; // convert lowercase to uppercase
        }
    }
}

int main() {
    char str[100];
    printf("Enter a string: ");
    fgets(str, 100, stdin);
    toggleCase(str);
    printf("Toggled case string: %s", str);
    return 0;
}


QUESTION 55: CONVERT STRING AS INTEGER 

#include <stdio.h>
#include <stdlib.h>

int main() {
    char str[100];
    int num;

    printf("Enter a string: ");
    fgets(str, 100, stdin);

    num = atoi(str);
    printf("The integer value of the string is: %d", num);

    return 0;
}


QUESTION 56: COMPUTE TOTAL SECONDS 
#include <stdio.h>

int main() {
    int hours, minutes, seconds;
    long totalSeconds;

    printf("Enter the hours: ");
    scanf("%d", &hours);
    printf("Enter the minutes: ");
    scanf("%d", &minutes);
    printf("Enter the seconds: ");
    scanf("%d", &seconds);

    totalSeconds = (hours * 3600) + (minutes * 60) + seconds;

    printf("Total seconds: %ld", totalSeconds);

    return 0;
}

QUESTION 57: COUNT NO.OF DAYS
#include <stdio.h>
#include <time.h>

int main() {
    struct tm start_date = {0};
    struct tm end_date = {0};
    time_t start_time, end_time, diff_time;
    double diff_days;

    printf("Enter start date (dd-mm-yyyy): ");
    scanf("%d-%d-%d", &start_date.tm_mday, &start_date.tm_mon, &start_date.tm_year);
    start_date.tm_year -= 1900; // adjust year
    start_date.tm_mon -= 1; // adjust month

    printf("Enter end date (dd-mm-yyyy): ");
    scanf("%d-%d-%d", &end_date.tm_mday, &end_date.tm_mon, &end_date.tm_year);
    end_date.tm_year -= 1900; // adjust year
    end_date.tm_mon -= 1; // adjust month

    start_time = mktime(&start_date);
    end_time = mktime(&end_date);

    diff_time = difftime(end_time, start_time);

    diff_days = (double) diff_time / (24 * 60 * 60);

    printf("Number of days between the two dates: %.0lf", diff_days);

    return 0;
}


QUESTION 58:ROTATE STRING
#include <stdio.h>
#include <string.h>
#include <stdlib.h>

void rotate_string(char *str, int n) {
    int len = strlen(str);
    char *new_str = (char*) malloc(len + 1);

    // Copy shifted characters to new string
    for (int i = 0; i < len; i++) {
        int j = (i + n) % len;
        new_str[j] = str[i];
    }

    // Append rotated characters to new string
    for (int i = 0; i < n; i++) {
        new_str[len + i] = str[i];
    }

    // Print rotated string
    printf("Rotated string: %s\n", new_str);

QUESTION 59: DATA VALIDATION
#include <stdio.h>
#include <string.h>
#include <ctype.h>

int main() {
   int age;
   char name[50], email[50];

   // validate age
   do {
      printf("Enter your age (between 18 and 60): ");
      scanf("%d", &age);
   } while (age < 18 || age > 60);

   // validate name
   do {
      printf("Enter your name (up to 50 characters): ");
      scanf("%s", name);
   } while (strlen(name) > 50);

   // validate email
   do {
      printf("Enter your email: ");
      scanf("%s", email);
   } while (strchr(email, '@') == NULL);

   // convert name to uppercase
   for (int i = 0; i < strlen(name); i++) {
      name[i] = toupper(name[i]);
   }

   printf("\nAge: %d\nName: %s\nEmail: %s\n", age, name, email);

   return 0;
}



















