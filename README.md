
#include <stdio.h>

int main()
{
    int phy, chem, bio, math, comp;
    float per;

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
    per = (phy + chem + bio + math + comp) / 5.0 *100;

    printf("Percentage = %.2f\n", per); */

    /* Find grade according to the percentage */
    if (per >= 90)
    {
        printf("You got Grade A");
    }
    else if (90 < per <= 70)
    {
        printf("You got Grade A");
    }
    else if (70 < per <= 50)
    {
        printf("You got Grade B");
    }
    else
    {
        printf("You got Grade F");
    }

    return 0;
}
