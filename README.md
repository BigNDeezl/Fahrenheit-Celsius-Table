# Fahrenheit-Celsius-Table

#include <stdio.h>

/* print Fahrenheit-Celsius table
  for fahr = 0, 20, ...300 */
  int main()
  {
      int fahr, celsius;
      int lower, upper, step;

      lower = 0;    /* Lower limit of temp table */
      upper = 300;  /* Upper limit of temp table */
      step = 20;    /* step size */

      fahr = lower;
      while (fahr <= upper) {
        celsius = 5 * (fahr - 32) / 9;
        printf("%d\t%d\n", fahr, celsius);
        fahr = fahr + step;
      }
  }
