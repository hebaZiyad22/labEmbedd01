# labEmbedd01
#define GPIOODIR (*((volatile unsigned long *)0x50008000))
#define GPIO0DATA (*((volatile unsigned long *)0x50003ffc))
#define GPIO2DIR (*((volatile unsigned long *)0x50028000))
#define GPIO2DATA (*((volatile unsigned long *)0x50023ffc))
#define GPIO1DIR (*((volatile unsigned long *)0x50018000))
#define GPIO1DATA (*((volatile unsigned long *)0x50013ffc))
int main (void){
int seven_seg_encoder [] = {
0xC0, 0xF9,0xA4, 0x80,0x99,0x92,0x82,0xF8,0x00, 0x90
};
int i = 0
int num=555; GPIO2DIR 1 = 0 * 7F GPIOODIR |= 0b11110; GPIO1DIRI=0b1;
while (num>=0){
GPIO0DATA=0b10000;
GPIO2DATA = seven_seg_encoder[(num)%10]; for ( ( i = 0 ; i < 5000 i++);
GPIO0DATA=0b01000;
GPIO2DATA = seven_seg_encoder[(num/10) % 10]: for ( i = 0 ; i < 5000 i++); GPIO0DATA=0b00100;
GPIO2DATA = seven_seg_encoder[(num/100) %10]; for (i = 0) i < 5000 i++);
GPIO0DATA=0b00010; GPIO2DATA = seven_seg_encoder[num / 1000]; for ( i = 0 ; i < 5000 i++);
if (num == 0){ GPIO1DATA = 0b1; GPIO1DATA = 0b0;
}else {
}
return 0;}
