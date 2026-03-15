# 8051-led-blink
#include <reg51.h>

void delay()
{
    int i,j;
    for(i=0;i<200;i++)
    {
        for(j=0;j<200;j++);
    }
}

void main()
{
    while(1)
    {
        P1 = 0xFF;   // LED ON
        delay();

        P1 = 0x00;   // LED OFF
        delay();
    }
}
