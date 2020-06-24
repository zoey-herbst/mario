#include <cs50.h>
#include <stdio.h>

int get_positive_int(void);//new string
int main(void)


   {
      int i = get_positive_int(); //positive number string

      printf("%i\n",i);

   }


   int get_positive_int(void)

{
    int n;

    do
    {
        n = get_int("%s", "Height: ");
    }


    while (n < 1 || n > 8); // number between 1-8



    for (int i = 0; i < n; i++) //height

    {

        for (int j = 0; j < n; j++) //width
       {
           if (i + j < n -1) //if the height + width is less than N -1

           printf(" ");

           else

           printf("#");
       }

        printf("\n");

    }
    return n;
}
