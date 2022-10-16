#include <stdio.h>
#include <math.h>

void menu();

//perhitungan

float hitungBrsAritmatika(float x, float y, float z){
    return (x + (y-1) * z);
    
}

float jumlahBrsAritmatika(float a, float b, float c){
    return ((b * 0.5) * (2 * a + (b-1) * c));
           }

//menu

void aritmatika1(){
    float bil1, bil2, b;
    int x;
    printf("||===============================||");
    printf("||        BARIS ARITMATIKA       ||");
    printf("||===============================||");
    printf("|| BIlangan Pertama : \n");
    scanf("%f", &bil1);
    printf("|| BIlangan Kedua : \n");
    scanf("%f", &bil2);
    printf("|| Masukan nilai bilangan atau suku :");
    scanf("%d", &x);
    b=bil2-bil1;
    printf("NIlai suku ke-%d adalah %.f", x, hitungBrsAritmatika(bil1, b, x));
    printf("||===============================|| \n");
    printf("\n");
    
    
}

void aritmatika2(){
    float bil1, bil2, b;
    int x;
    printf("||===============================||");
    printf("||        BARIS ARITMATIKA       ||");
    printf("||===============================||");
    printf("|| BIlangan Pertama : \n");
    scanf("%f", &bil1);
    printf("|| BIlangan Kedua : \n");
    scanf("%f", &bil2);
    printf("|| Masukan nilai bilangan atau suku :");
    scanf("%d", &x);
    b=bil2-bil1;
    printf("Jumlah suku ke-%d adalah %.f", x, jumlahBrsAritmatika(bil1, b, x));
    printf("||===============================|| \n");
    printf("\n");
}

void menu(){
    int pilih;
    
    printf("1. Baris Aritmatika \n");
    printf("2. Deret Aritmatika \n");
    printf("Pilih salah satu : \n");
    scanf("%d", &pilih);
    
    switch(pilih){
        case 1:
            printf("\n");
            aritmatika1();
            break;
        case 2:
            printf("\n");
            aritmatika2();
            break;
            
            
    }
    
    
    
    
    
}
