랜덤값 범위 지정 : (최대값 - 최소값 + 1) + 최소값
```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    srand((unsigned)time(NULL));
    printf("rand() = %d \n", rand() % 10);      //  0 ~  9   ==> (9 - 0 + 1) + 0
    printf("rand() = %d \n", rand() % 10 + 1);  //  1 ~ 10   ==> (10 - 1 + 1) + 1
    printf("rand() = %d \n", rand() % 16 + 20); // 20 ~ 35   ==> (35 - 20 + 1) + 20

    return 0;
}

```

Q. 로또 생성기

```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int lotto[6] = {0};
    srand((unsigned)time(NULL));
    for (int i = 0; i < 6; i++)
    {
        lotto[i] = rand() % 45 + 1;
        printf("%d ", lotto[i]);
    }

    return 0;
}
```
