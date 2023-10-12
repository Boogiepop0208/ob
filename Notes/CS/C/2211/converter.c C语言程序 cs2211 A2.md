[cs2211]的A2 [[C语言]]

#asn 

`#include <stdio.h>

  

void fahrenheitToCelsius();

void celsiusToFahrenheit();

void centimeterToInch();

void inchToCentimeter();

void kilometerToMile();

void mileToKilometer();

void usgallonToLiter();

void literToUsgallon();

  
  
  

int main()

{

    int n;

    char ltr;


    do

    {

        printf("Welcome to the converter!\n\n"

       "Please enter the corresponding integer to select the corresponding operation.\n"

       "1 for conversion between Celsius and Fahrenheit\n"

       "2 for conversion between Centimetre and Inch\n"

       "3 for conversion between Kilometer and Mile\n"

       "4 for conversion between Gallon and Liter\n"

       "0 for quit\n\n");

  

        printf("Enter a number: ");

        scanf(" %d", &n);

        if (n == 1){

            do

            {

                printf("C for convert from Celsius to Fahrenheit.\n"

                "F for convert from Fahrenheit to Celsius.\n"

                "Enter C or F: ");

                scanf(" %c", &ltr);

                if (ltr == 'C'){

                    celsiusToFahrenheit();

                }

                else if (ltr == 'F'){  

                    fahrenheitToCelsius();

                }

  

            }while (ltr != 'C' && ltr != 'F');

        }

        else if (n == 2)

        {

            do

            {

                printf("C for convert from Centimeter to Inch.\n"

                "I for convert from Inch to Centimeter.\n"

                "Enter C or I: ");

                scanf(" %c", &ltr);

                if (ltr == 'C'){

                    centimeterToInch();

                }

                else if (ltr == 'I'){  

                    inchToCentimeter();

                }

            } while(ltr != 'C' && ltr != 'I');

        }

        else if (n == 3)

        {

            do

            {

                printf("K for convert from Kilometer to Mile.\n"

                "M for convert from Mile to Kilometer.\n"

                "Enter K or M: ");

                scanf(" %c", &ltr);

                if (ltr == 'K'){

                    kilometerToMile();

                }

                else if (ltr == 'M'){  

                    mileToKilometer();

                }

            } while(ltr != 'K' && ltr != 'M');

        }

        else if (n == 4)

        {

            do

            {

                printf("G for convert from USGallon to Liter.\n"

                "L for convert from Liter to USGallon.\n"

                "Enter G or L: ");

                scanf(" %c", &ltr);

                if (ltr == 'G'){

                    usgallonToLiter();

                }

                else if (ltr == 'L'){  

                    literToUsgallon();

                }

            } while(ltr != 'G' && ltr != 'L');

        }

        else if (n == 0)

        {

            return -1;

        }

    } while (n != 0);

    return 0;

}

  
  

void celsiusToFahrenheit() {

    float oriNum, conVal;

    printf("Enter a number to calculate: ");

    scanf(" %f", &oriNum);

    conVal = oriNum * 9.0/5.0 + 32;

    printf("%f Celsius is equal to %f Fahrenheit.\n", oriNum, conVal);

    printf("\n");

}

  

void fahrenheitToCelsius() {

    float oriNum, conVal;

    printf("Enter a number to calculate: ");

    scanf(" %f", &oriNum);

    conVal = (oriNum - 32) * 5/9;

    printf("%f Fahrenheit is equal to %f Celsius.\n", oriNum, conVal);

    printf("\n");

}

  

void centimeterToInch() {

    float oriNum, conVal;

    printf("Enter a number to calculate: ");

    scanf(" %f", &oriNum);

    conVal = oriNum * 0.393701;

    printf("%f Centimeter is equal to %f Inch.\n", oriNum, conVal);

    printf("\n");

}

  

void inchToCentimeter() {

    float oriNum, conVal;

    printf("Enter a number to calculate: ");

    scanf(" %f", &oriNum);

    conVal = oriNum * 2.54;

    printf("%f Inch is equal to %f Centimeter.\n", oriNum, conVal);

    printf("\n");

}

  

void kilometerToMile() {

    float oriNum, conVal;

    printf("Enter a number to calculate: ");

    scanf(" %f", &oriNum);

    conVal = oriNum * 0.621371;

    printf("%f kilometer is equal to %f Mile.\n", oriNum, conVal);

    printf("\n");

}

  

void mileToKilometer() {

    float oriNum, conVal;

    printf("Enter a number to calculate: ");

    scanf(" %f", &oriNum);

    conVal = oriNum * 1.60934;

    printf("%f Mile is equal to %f kilometer.\n", oriNum, conVal);

    printf("\n");

}

  

void usgallonToLiter() {

    float oriNum, conVal;

    printf("Enter a number to calculate: ");

    scanf(" %f", &oriNum);

    conVal = oriNum * 3.78541;

    printf("%f USGallon is equal to %f Liter.\n", oriNum, conVal);

    printf("\n");

}

  

void literToUsgallon() {

    float oriNum, conVal;

    printf("Enter a number to calculate: ");

    scanf(" %f", &oriNum);

    conVal = oriNum * 0.264172;

    printf("%f Liter is equal to %f USGallon.\n", oriNum, conVal);

    printf("\n");

}`