(# C-programs-
For c language 
/* Question: */
/* Write a program to input marks of 5 subjects and calculate percentage and print grade according to
percentage >= 90 = Grade A+
90 < percentage <= 70 = Grade A
70 < percentage <= 50 = Grade B
percentage < 50 = Grade F */

#include <stdio.h>

int main()
{
    int phy, chem, bio, math, comp;
    float per;

    /* We can take input seprate subject as well as combine*/

    /* Method 1 */

    /* Input marks of five subjects from user */
    /* printf("Enter five subjects marks: ");
    scanf("%d%d%d%d%d", &phy, &chem, &bio, &math, &comp); */

    /* Method 2 */

    printf("Enter your Physics marks : ");
    scanf("%d", &phy);
    printf("Enter your Chemistry marks : ");
    scanf("%d", &chem);
    printf("Enter your Biology marks : ");
    scanf("%d", &bio);
    printf("Enter your Mathematics marks : ");
    scanf("%d", &math);
    printf("Enter your Computer marks : ");
    scanf("%d", &comp);

    /* Calculate percentage by percentage formula */
    per = (phy + chem + bio + math + comp) / 5.0;

    /* %.2f is used to print fractional values up to two decimal places, we can also use %f
    printf("Percentage = %.2f\n", per); */

    /* Find grade according to the percentage */
    if (per >= 90)
    {
        printf("You got Grade A+ . Excellent!");
    }
    else if (90 < per <= 70)
    {
        printf("You got Grade A . Very Good!");
    }
    else if (70 < per <= 50)
    {
        printf("You got Grade B . Keep it up!");
    }
    else
    {
        printf("You got Grade F . You need to stop playing PUBG");
    }

    return 0;
}
