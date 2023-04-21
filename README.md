# Practice-vending-machine-programming-C
Beverage vending machine C language console programming
![image](https://user-images.githubusercontent.com/115389450/233519726-3cf0545d-63a7-4635-bdbd-14d1e606f4ba.png)
```
#include <stdio.h>


int main(void)
{
    int cola=1200;
    int universe_cola=1900;
    int zero_cola=1200;
    int sprite=1100;
    int hwnta=900;
    int docter_peper=1100;
    int monster=1800;
    int poweraid=1900;
    int nestea=1600;
    int glasovitaminwater=2100;
    int minitaid=1700;
    int jojia_coffee=900;
    int ambasa=900;
    int matecha=1700;
    int total=0;
    int money=0;
    int choose=0;


    printf("음료를 구매하실려면 돈을 넣어 주세요 : ");
    scanf("%d", &money);

    while(money>total)
    {
        printf("음료수 종류는 아래와 같습니다.\n");
        printf("1번 콜라(1200원), 2번 우주맛 콜라(1900원), 3번 제로콜라(1200원)\n");
        printf("4번 스프라이트(1100원),5번 환타(900원), 6번 닥터페퍼(1100원)\n");
        printf("7번 몬스터(1800원), 8번 파워에이드(1900원),9번 네스티(1600원)\n");
        printf("10번 글라소 비타민 워터(2100원), 11번 미니메이드(1700원)\n");
        printf("12번 조지아커피(900원),13번 암바사(900원), 14번 마테차(1700원)\n");
        printf("15번 계산하기\n");
        printf("원하는 음료의 숫자를 입력해 주세요, 계산하려면 15번을 눌러주세요.: ");
        scanf("%d", &choose);

            switch(choose)
            {
                case 1 :
                if(money>total)
                {
                    printf("+++++++++++콜라선택, 콜라는 1200원입니다+++++++++++\n"); 
                    total += cola;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 2 :
                if(money>total) 
                {
                    printf("+++++++++++우주맛 콜라 선택, 우주맛 콜라는 1900원입니다+++++++++++\n");
                    total += universe_cola; 
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 3 :
                if(money>total) 
                {
                    printf("+++++++++++제로콜라 선택, 제로콜라는 1200원입니다.+++++++++++\n");
                    total += zero_cola; 
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 4 :
                if(money>total) 
                {
                    printf("+++++++++++스프라이트 선택, 스프라이트는 1100원입니다.+++++++++++\n");
                    total += sprite;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 5 :
                if(money>total) 
                {
                    printf("+++++++++++환타 선택, 환타는 900원입니다.+++++++++++\n");
                    total += hwnta;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 6 :
                if(money>total) 
                {
                    printf("+++++++++++닥터페퍼 선택, 닥터페퍼는 1100원입니다.+++++++++++\n");
                    total += docter_peper;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 7 :
                if(money>total) 
                {
                    printf("+++++++++++몬스터 선택, 몬스터는 1800원입니다.+++++++++++\n");
                    total += monster;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 8 :
                if(money>total) 
                {
                    printf("+++++++++++파워에이드 선택, 파워에이드는 1900원입니다.+++++++++++\n");
                    total += poweraid;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }   
                case 9 :
                if(money>total) 
                {
                    printf("+++++++++++네스티 선택, 네스티는 1600원입니다.+++++++++++\n");
                    total += nestea;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 10 :
                if(money>total) 
                {
                    printf("+++++++++++글라소 비타민 워터 선택, 글라소 비타민 워터는 2100원입니다.+++++++++++\n");
                    total += glasovitaminwater;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 11 :
                if(money>total) 
                {
                    printf("+++++++++++미닛메이드 선택, 미닛메이드는 1700원입니다.+++++++++++\n");
                    total += minitaid; 
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 12 :
                if(money>total) 
                {
                    printf("+++++++++++조지아 커피 선택, 조지아 커피는 900원입니다.+++++++++++\n"); 
                    total += jojia_coffee;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                    }
                case 13 :
                if(money>total) 
                {
                    printf("+++++++++++암바사 선택, 암바사는 900원입니다.+++++++++++\n"); 
                    total += ambasa;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 14 :
                if(money>total) 
                {
                    printf("+++++++++++마테차 선택, 마테차는 1700원입니다.+++++++++++\n"); 
                    total += matecha;
                    printf("남은 돈은 %d원입니다.\n", money-total); break;
                }
                case 15 : 
                printf("선택한 음료를 계산합니다.\n"); // 계산하기 누르기 전까지는 선택한 음료 저장,
                {
                    printf("**********************\n");
                    int change=0;
                    change = money-total;
                    printf("+++++++++++계산하고 남은 돈 : %d+++++++++++\n", change);
                    break;
                }                                            // 총 금액의 합산을 변수에 저장하여
                                                        // 입력한 돈과 비교하여 계산
                                                        // 입력한 돈이 주문의 합보다 적으면
                                                        // 돈이 부족하다고 하며 종료
            }
            if(money<total)
            {
                printf("돈이 부족합니다.\n");
            }   
    }
    return 0; 
} 
```
- - -
﻿
이제까지 살아오면서 한번도 진지하게

c언어를 생각했던 적도, 공부했던 적도 없었고,

조금 잘하시는 분들은

이미 이단계를 넘어선 분들이다.

현재 내상황을 객관적으로 보고 인정하고,

그렇다고 위축될 필요도 없고,

이제까지 안했는데, 지금 한다고 뭐가 달라질까? 라는 생각을 가지게 되면

사실 공부뿐아니라 운동도 못하고 아무것도 못하는 것 같다.

아무것도 안하면 아무것도 달라지지 않는다.

﻿
- - -
- - -
﻿12. 홀수, 짝수 판별하기
- - -
```
#include <stdio.h>

int main(void)
{
   int a; 
   
   printf("정수 입력 : "); 
   scanf("%d", &a);

   if((a!=0)&&(a%2==0)) // a가 0이아니고, a를 2로나누었을 때 나머지가 0일경우 - 짝수
   {
      printf("a는 짝수입니다.\n");
   }
  else if(a%2==1) // a를 2로 나누었을 때 나머지가 1일 경우 - 홀수
  {
      printf("a는 홀수입니다.\n");
  }
  else
  {
     printf("a는 홀수도 짝수도 아닙니다.(0일경우)\n");
  }
  return 0;
}
```
- - -
3의 배수 판별하기
- - -
```
#include <stdio.h>

int main(void)
{
    int a;

    printf("정수 입력 : ");
    scanf("%d", &a);

    if((a!=0)&&a%3==0)
    {
        printf("a는 3의 배수입니다.\n");
    }
    else
    {
        printf("a는 3의 배수가 아닙니다.\n");
    }

    return 0;
}
```
- - -
1, -2, 3, -4, .. 99, -100의 합 구하기
- - -
```
#include <stdio.h>

int main(void)
{
    int sum=0;
    for(int i=1; i<=100; i++) // 100번 반복한다.
    {
        if(i%2==0) // 나머지가 0이면 짝수 표현
        {
            sum=sum-i; // -를 붙여서 음수 표현
            printf("%d\n", sum);
        }
        else // 위에가 아닐경우 홀수 
        {
            sum=sum+i; // +를 붙여서 양수 표현
            printf("%d\n", sum);
        }
    }
    printf("결과는? : %d\n", sum);
    return 0;
}
```
- - -
계승 구하기. 계승은 ? 팩토리얼 !
팩토리얼은?
n! = (n-1)*(n-2)*(n-3)*...*1
- - -
```
#include <stdio.h>
// 계승? 계승은 팩토리얼
// n!= (n-1)*(n-2)*(n-3)*... *1 ;
// n!= 1*2*3*...*n;


int main(void)
{
    int n;
    int i;
    int factorial=1;

    printf("정수 입력 : ");
    scanf("%d", &n);

    for(i=n; i>=1; i--)
    {
        factorial*=i;
    }

    printf("%d!=%d\n", n, factorial);

    return 0;
}
```
```
#include <stdio.h>
// 계승? 계승은 팩토리얼
// n!= (n-1)*(n-2)*(n-3)*... *1 ;
// n!= 1*2*3*...*n;


int main(void)
{
    int n;
    int i;
    int factorial=1;

    printf("정수 입력 : ");
    scanf("%d", &n);

    for(i=1; i<=n; i++)
    {
        factorial*=i;
    }

    printf("%d!=%d\n", n, factorial);

    return 0;
}
```
- - -
약수 구하기
약수란? 어떤 자연수를 나누어 떨어지게 하는 수
ex) 10의 약수는 1,2,5,10
- - -
```
#include <stdio.h>

int main(void)
{
    int n;
    int i;

    printf("약수를 구하려는 수를 입력 : ");
    scanf("%d", &n);

    printf("%d의 약수 : ", n);

    for(i=1; i<=n; i++) // i가 n값하고 같아질 때까지 반복한다.
    {
        if(n%i==0) // 나머지가 0이면 아래 값을 출력한다. 즉 약수
        {
            printf("%d ", i);
        }
    }
    return 0;
}
```
- - -
﻿
++소수 구하기 플러스 문제

소수란? 1과 자기 자신만으로 나누어지는 수 = 즉 약수의 개수는 2개

소수가 아니면? 약수는 3개이상이다.

흠.. 약수에서 소수로 넘어갈 수 있군요??

﻿
- - -
```
#include <stdio.h>
// 소수란? 1과 자기자신만으로 나누어지는 수
// 소수 구하기
// ex. 1,2,3,5,7,11,13,17,19,23,29,31
// 소수가 아닌수?
// 4,
// if 소수면 1
// else 아니면 0dsa
int main(void)
{
    int n;
    int count = 0; // 약수 숫자세기위한 count 함수

    printf("숫자 입력 : ");
    scanf("%d", &n);

    for(int i=1; i<=n; i++) // n값보다 작거나 같을 때까지 반복, 이유는? n을 15입력했을때 약수는 15를 넘을 수 없으므로 
        {
            if(n%i==0) // 약수 구하기 위한 조건
            {
                count = count + 1; // 1을 더해준 이유는 //약수 개수 세기 위해서. 약수1개 발견 > +1
            }
        }
    printf("약수의 개수 %d개\n", count);
    printf("약수의 개수가 2보다 작거나 같으면 소수, \n3개이상이면 소수가 아닙니다.\n");
    if(count<=2)
    {
        printf("소수입니다.(1)\n");
    }
    else
    {
        printf("소수가아닙니다(0)\n");
    }
    return 0;
}
```
- - -
﻿
공약수 구하기

공약수란? 주어진 두 정수를 나누어 떨어지게 하는 수

ex) 10과 12의 공약수? = 1,2

﻿
- - -
```
#include <stdio.h>

int main()
{
    int n1, n2;

    printf("공약수를 구하려는 두 정수 입력: ");
    scanf("%d %d", &n1, &n2);

    for(int i=1; i<=n1&&i<=n2; i++)
    {
        if((n1%i==0)&&(n2%i==0))
        {
            printf("%d ", i);
        }
    }
    return 0;
}
```
- - -
최대 공약수 구하기
- - -
```
#include <stdio.h>

int main(void)
{
    int n1,n2;
    int great; // 최대공약수를 담을 변수

    printf("최대공약수를 구하려는 두 정수 입력 : ");
    scanf("%d %d", &n1, &n2);

    for(int i=1; i<=n1&&i<=n2; i++)
    {
        if(n1%i==0&&n2%i==0)
        {
            great=i; // 최대 공약수 담았다!
        }
    }
    printf("최대공약수는 %d입니다.", great);

    return 0;
}
```
- - -
소수 구하기
- - -
```
#include <stdio.h>

int main(void)
{
    int n;
    int i;
    printf("소수판별하기 숫자 입력: ");
    scanf("%d", &n);

    for(i=2; i<n-1; i++) // ex. n에 5를 입력하면 1,2,3,4로 수가 나온다.
    {
        if(n%i==0) // 만약에 6을 입력하면 1부터 5까지의 수가 나오는데 그 수 중에서 나누었을 때 나머지가 0이면 반복문 탈출
            break; // 
    }
    if(n-1>i) // n-1이 i보다 클 경우, 예를 들어 4를 입력하면 1,2,4로 i가 2일때 4를 2로나누었을 때 나머지가 0이다.소수가아님.
        printf("소수가 아닙니다.\n");

    else // n-1<i보다 작은 경우? 그러니까 i값이 n-1직전까지 판별한다. 즉 5인데 4까지 수를 판별했을 때 나머지가 0이 아니다.
        printf("소수입니다.\n"); // 소수이다.

    return 0;
}
```
- - -
피보나치 수열 구하기
- - -
```
#include <stdio.h>

//피보나치 수열 구하기
// 0,1,1,2,3,5,8,13,21...
// c=a+b

int main(void)
{
    int a=0;
    int b=1;
    int c;
    int n;

    printf("몇번째까지 피보나치수열을 구할까요? : ");
    scanf("%d", &n);

    for(int i=0; i<n; i++)
    {
        printf("%d ", a);
        c=a+b;
        a=b;
        b=c;
    }
    return 0;
}
```
- - -
최댓값 구하기
- - -
```
#include <stdio.h>
// 무작위 숫자 a개를 입력받고
// 그 수중 최대값 구하기

int main(void)
{
    int a;
    int max=0;

    scanf("%d", &a);
    max=a;

    for(;;)
    {
    if(a!=0)
    {
        if(a>max)
        {
            max=a;
        }
        scanf("%d", &a);
        
    }
    else
    {
        printf("%d", max);
        break;
    }
    }

    return 0;
}
```
- - -
1부터 10까지 정수의 약수 구하기
- - -
```
#include <stdio.h>

int main(void)
{
    for(int i=1; i<=10; i++)
    {
        printf("\n%d:", i); // 1부터 10
        for(int j=1; j<=i; j++)
        {
            if(i%j==0)
            {
                printf("%d ",j); // 1의 약수, 2의 약수, ... 10의 약수
            }
        }
    }
    return 0;
}
```
- - -
2부터 100까지의 소수 구하기
- - -
```
#include <stdio.h>

int main(void)
{
    for(int i=2; i<=100; i++) // 2부터 100까지의 수
    {
        int chk=1; // 1이면 소수표현
        for(int j=2; j<=i-1; j++) // 2부터 100까지의 수에서 1을 뺀 수, 
                                      // 즉 3이 소수냐?판단할때 그 전까지의 수를 나눴을때 나머지가 0이 나와서 딱 떨어지면 소수가 아님.
        {
            if(i%j==0) // 소수가 아닐 때
            {
                chk=0; // 0 표시
            }
        }
        if(chk==1)
        printf("%d는 소수입니다(%d)\n", i, chk);
        else
        printf("%d는 소수가 아닙니다(%d)\n", i, chk);
    }
    return 0;
}
```
- - -
﻿1, (1+2), (1+2+3)...(1+2+3+...10)의 합을 구하기
- - -
```
#include <stdio.h>

int main(void)
{
    int n=0;
    int sum=0;

    for(int i=1; i<=10; i++) // 1부터 10까지의 수
    {
        n=n+i; // n은 n에서 1을 더한 수
        sum=sum+n; // 합은 합에서 n을 더한 수
        printf("수의 합 : %d\n", sum); // 즉 1, 1+2, 4, 1+2+3, 10, 이런 식으로...
    }
    printf("수의 합 : %d\n", sum);

    return 0;
}
```
- - -
구구단 (가로출력)
- - -
```
#include <stdio.h>

int main(void)
{
    for(int a=1;a<10;a++)
        {
            for(int b=2;b<10;b++)
            {
                printf(" %dx%d=%2d |", b, a, a*b); // 터미널에 출력되는 값.
            }
            printf("\n");
        }
    return 0;
}
```
![image](https://user-images.githubusercontent.com/115389450/233520905-d213b34b-cfda-430f-bc5b-dc49a351a081.png)
- - -
구구단 (세로출력)
- - -
```
#include <stdio.h>

int main(void)
{
    for(int a=2; a<10; a++)
    {
        for(int b=1; b<10; b++)
        {
            printf(" %d x %d = %d", a, b, a*b);
            printf("\n");
        }
    }
    return 0;
}
```
![image](https://user-images.githubusercontent.com/115389450/233521003-b6f826c2-0cd0-48a2-af18-e8002bddfd92.png)
```
#include <stdio.h>
#include <stdlib.h>

void calculate(int num); // main 함수에서 음료수를 선택할 때 불러오기 위한 함수
void list(int call); // main 함수에서 음료수 리스트를 불러오기 위한 함수 . 
                     // c언어는 순서(논리)지향적이고, main 함수가 종료되면 끝이 난다.
                    // 그러므로 main 함수 이전에 불러오기 위한 함수를 선언 해 준다.
int main(void)
{
    int drink[14] = {1200, 1900, 1200, 1100, 900, 1100, 1800, 1900, 1600, 2100, 1700, 900, 900, 1700}; 
// 배열, 메모리 14칸에 각각 음료수 값을 넣어준다
    int money; // 지불한 금액
    int total=0; // 음료수를 선택한만큼의 금액
    int num; // 음료수 번호
    char buy; // 문자열, r(음료선택) s(음료계산) x(종료)를 받기 위해서 char형 함수 
    int call=0; // 음료수 리스트를 불러오기 위해서

    printf("음료수를 사려면 돈을 넣어주세요\n : ");
    scanf("%d", &money);

    for(;;) // 무한루프 반복
    {
        printf("\n현재 금액 : %d원 . 계산할 금액: %d원\n",money, total); 
        printf("\n(r)음료선택, (s)계산, (x)종료 : \n"); // 여기서 궁금한게 터미널에 2번 출력된다..; 
        scanf("%c", &buy); // r, s x중 입력

        switch(buy)
        {
            case 114:  // 문자열 r(음료선택)은 숫자 114를 의미한다.(아스키 코드)
            list(call); // 음료수 리스트를 불러온다.
            printf("\n 음료수 번호를 선택하세요 : ");
            scanf("%d", &num);
            calculate(drink[num]); // calculate를 불러오고, 배열값 중 선택한 음료수 번호의 가격이 입력.  
            total += drink[num]; // 총 금액은 계속 선택한 음료수 값 저장
            break; // 탈출
            case 115: // 문자열 s(계산)은 숫자 115를 의미한다(아스키코드)
            if(money<total) // 돈이 선택한 음료수 총 금액의 합보다 적을 경우
            {
                printf("금액이 부족하여 음료수 못사!\n"); // 
                return 0;
            }
            else
            {
                printf("%d원 계산합니다\n", total);
                money -= total;
                printf("잔액 %d원을 반환합니다.\n", money);
                return 0;
            }
            case 120: // 문자열 x(종료)는 숫자 120을 의미한다(아스키 코드)
                printf("종료합니다\n");
                return 0;
            default: 
                break; 
        }
    }
}

void list(int call)
{
    printf("(1.콜라.1200원)(2.우주맛콜라.1900원)(3.제로콜라.1200원)\n(4.스프라이트.1100원)(5.환타.900원)(6.닥터페퍼.1100원)\n(7.몬스터.1800원)(8.파워에이드.1900원)(9.네스티.1600원)\n(10.글라소비타민워터.2100원)(11.미닛메이드.1700원)\n(12.조지아커피900원)(13.암바사900원)(14.마테차.1700원)\n");
}

void calculate(int num)
{
        printf("\n음료 추가되었습니다. (%d원) \n", num);
}
```
![image](https://user-images.githubusercontent.com/115389450/233521105-4ef06f1e-b1fc-4a50-8cce-22c2e62bd131.png)
- - -
문제 해결을 위한 아스키코드 참고 표 
- - -
![image](https://user-images.githubusercontent.com/115389450/233521168-2de8ef8a-724b-42d8-9ec4-93530a4641e4.png)
![image](https://user-images.githubusercontent.com/115389450/233521201-38ec9038-343d-4c81-8630-fcd11222d3b4.png)



