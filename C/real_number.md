기초 입출력 - 실수형 입출력

```C
#include <stdio.h>

int main(){
    float x;
    scanf("%f",&x);
    printf("%f",x);
    return 0;
}
```
```
입력 예시 : 1.414213

출력 예시 : 1.414213
```
Q. 소수점 셋째 자리에서 반올림하여
소수점 이하 둘째 자리까지 출력하려면?

```C
#include <stdio.h>

int main(){
    float f = 0;
    scanf("%f", &f);
    printf("%.2f", f);
    return 0;
}
```
```
입력 예시 : 1.59254

출력 예시 : 1.59
```
* %.2f와 같은 형식으로 지정하면,
소수점 이하 셋째 자리에서 반올림하여 소수점 이하 둘째 자리까지 출력하라는 의미이다. 
