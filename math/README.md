## 컴퓨터와 수학

### 대수학의 수체계

```ts

             복소수(Complex number)
                        |
        ------------------------------
        |                             |
허수(imaginary number)         실수 (real number)
                                      |
                      -------------------------------
                      |                              |
                무리수(irrational number)  유리수(rational number)
                                                      |
                                    --------------------------------------
                                    |                                     |
                              정수가 아닌 유리수                      정수(integer)
                                    |                                     |
                              -------------              --------------------------------
                              |            |             |                |             |
                          유한소수      순환소수       음(negative)의 정수  0     양(positive)의 정수
                                                                             자연수(natural number)
```

- 자연수 : 1,2,3,4, ...
- 음의 정수 : -1,-2,-3, ...
- 유한소수 : 1/4, 3/10, ...
- 순환소수 : 2/3, 3/7, ...
- 무리수 : √2, √3, π(파이), ...
- 허수 : i
- 복소수 : a + bi
- 대수학 기본 정리 = 복소수를 계수로 갖는 1차 이상의 다항식은, 반드시 복소수 근을 갖는다.
- => 복소수 이상의 수의 확장은 없다.

### 컴퓨터의 수체계

- int 는 정수형을 처리하기 위한 변수.
- 과거 컴퓨터는 cpu는 16bit(2byte)씩 연산
- 현재 cpu는 34bit(4byte), 64bit(8byte) 를 이용
- cpu의 연산을 최적화하기 위한 data크기를 설정한것이 변수단위

- 32bit cpu의 처리 비트수.
- char: 8비트 정수형
- short: 16비트 정수형
- int: 32비트 정수형
- long long: 64비트 정수형
