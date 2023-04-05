#define _CRT_SECURE_NO_WARNINGS 
#include<stdio.h>


int main() {
    int A, B, C;
    
    scanf_s("%d\n %d\n %d", &A, &B, &C);

    int angle = A + B + C;

    if (A == 60 && A == B && B == C) {
    
        printf("Equilateral");
    }
    else if (angle == 180 && (A == B || B == C || C == A)) {
    
        printf("Isosceles");
    }
    else if (angle == 180 && (A != B && B != C && C != A)) {
    
        printf("Scalene");
    }
    else {
    
        printf("Error");
    }

    return 0;
}
