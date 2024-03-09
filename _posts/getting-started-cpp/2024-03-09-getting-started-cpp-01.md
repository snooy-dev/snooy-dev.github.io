---
title: 1. 첫 번째 프로그램 | C++ 시작하기
date: 2024-03-09 15:07:00 +0900
last_modified_at: 2024-03-09 15:07:00 +0900
categories: [C++, C++ 시작하기]
tags: [c++, tutorial]
pin: true
---

# 첫 번째 프로그램

"Hello, World!"를 화면에 출력하는 프로그램을 작성합니다.

## 코드 작성

다음은 "Hello, World!"를 화면에 출력하는 코드입니다.

```c++
#include <iostream>

using namespace std;

int main()
{
    cout << "Hello, World!" << '\n';    // "Hello, World!" 출력
    return 0;
}
```

이 프로그램을 실행하면 다음과 같이 "Hello, World!"가 출력됩니다.

```terminal
Hello, World!
```

## 코드 분석

위의 코드는 컴퓨터가 해야할 일을 나타내는 설명서라고 할 수 있습니다. 코드의 각 부분이 무엇을 의미하는지 살펴보겠습니다.

### 출력

먼저 5행에서는 실제로 출력을 실행합니다.

```c++
cout << "Hello, World!" << '\n';
```

"Hello, World!"라는 문자열을 출력하고, 개행 문자<sup style="color:gray;">newline character</sup>를 출력합니다.

`cout`은 표준 출력 스트림<sup style="color:gray;">standard output stream</sup>을 가리키고, `<<`는 "`cout`에 출력하라"를 의미합니다. `"Hello, World!"`는 문자열 리터럴<sup style="color:gray;">literal</sup>로 `"`로 구분합니다. `\n`는 개행 문자를 가리키는 특수 문자입니다.

> `cout`은 '씨-아웃'으로 발음하며, 'character output stream'의 줄임말입니다.
{: .prompt-info }

### 주석

5행 끝에 있는 이 부분은 주석<sup style="color:gray;">standard output stream</sup>입니다.

```c++
// "Hello, World!" 출력
```

한 행에서 `//`뒤에 오는 모든 내용은 주석입니다. 주석은 코드를 읽는 사람을 위해 작성하는 내용으로, 컴파일러는 주석을 무시합니다.

### 지시어

1행은 지시어<sup style="color:gray;">directive</sup>로, 그 중 다른 파일의 기능을 가져와 사용할 수 있게 지시하는 'include 지시어'입니다.

```c++
#include <iostream>
```

`iostream`은 표준 입출력을 위한 파일로, 이 파일에 `cout`이 있습니다.

### main 함수

다음과 같이 작성된 부분은 main 함수입니다.

```c++
int main()
{
    
    return 0;
}
```

main 함수는 프로그램의 시작점입니다. 모든 프로그램은 main 함수를 갖고 있습니다.

함수는 명령어의 집합입니다. 함수는 다음과 같은 4개의 요소로 이뤄집니다.

- **반환 타입**: 반환 타입은 함수가 실행된 후 함수를 실행시킨 주체에게 돌려주는 값의 타입을 의미합니다.

- **이름**: 함수의 이름입니다.

- **매개변수 목록**: `()`로 함수의 매개변수 목록을 나타냅니다.

- **몸체**: `{}`로 둘러사인 부분으로, 함수가 실행할 구문이 있습니다.

> main 함수의 반환 값은 사용하지 않습니다. 그러나 유닉스나 리눅스와 같은 시스템에서는 반환 값을 이용해서 프로그램이 성공적으로 종료했는지 판단합니다. 프로그램이 성공적으로 종료한 경우 main 함수는 `0`을 반환합니다.
{: .prompt-info }

> 다음은 가장 작은 C++ 프로그램입니다.
> ```c++
> int main() {}
> ```
{: .prompt-info }
