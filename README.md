---
layout: post
current: post
cover: assets/images/1400x800(bg_image).png
navigation: True
title: 유지원 첫째 주
date: 2021-02-21 21:00:00 +0900
tags: "Jiwon"
class: post-template
subclass: 'post'
author: "jiwon"
disqus: False
---

# 프로그래밍의 개념
1. 프로그래밍이란?
  - computer: 명령어들(instruction)의 리스트에 따라 데이터를 처리하는 기계
  - 계산기: computer와 달리 다양한 프로그램을 수행하지 않는다.
  - 프로그램(program): 특정한 작업을 수행하도록 설계된 명령어들의 리스트

  - computer 언어는 0/1의 이진수, 즉 기계어(machine language)이므로 자연어보다는 보다 기계어에 가까운 프로그래밍 언어를 컴파일 해 기계어로 변환한다.

1. 프로그래밍 언어
  - 기계어(machine language)
    - 이진수.
    - 하드웨어에 따라 다름(ex. CPU가 인텔/ARM)
  - 어셈블리어(assembly language)
    - CPU의 명령어들을 기호(symbolic name)으로 표기할 수 있음
    - 저급언어(low-level language)
      - 기호 이름과 CPU 명령어가 일대일 대응됨
      - CPU가 달라지면 실행할 수 없음
  - 고급 언어(high-level language)
    - computer 구조에 얽매이지 않음. 독립적
    - 프로그램 이해, 유지, 보수 쉬움
    - ex. c, c++, java, c#, objective-c, fotran, pascal, cobol
    - 아래로 갈수록 인간의 언어에 가까워 사용이 편리함

1. C언어 소개
  - 간결하다.
  - 효율적이다.(크기 L, 속도 H, 메모리 L)
  - 저수준부터 고수준까지 모두 만들 수 있다.
  - 이식성(portability)가 높다.
    - 다른 CPU 가지는 하드웨어로 쉽게 이식 가능하다.(많이 이용하니까)
  - C 배우면 C++에서도 지원된다.
  * 임베디드 시스템(embeded system)
    - 특수목적의 시스템. com이 장치에 내장되어 있음.
    - 하나/몇 개의 미리 결정된 작업만을 수행함.

1. 알고리즘이란?
  - com이 수행해야 할 단계적인 절차를 기술한 것.
  -  기술 방법
    - 자연어
    - 순서도(flowchart, 흐름도)
    - 의사코드(pseudo-code)
  - tip: 문제가 충분히 작아질 때(CPU가 바로 실행할 수 있을 정도)까지 계속해서 분해한다.

1. 프로그램 개발 과정
  1. 요구사항 분석
  1. 알고리즘 개발
  1. 소스 작성(코딩)
  1. 컴파일과 링크
    - 에디터(소스코드)->컴파일러(오브젝트 파일)->링커(실행 파일)->실행
    - 통합 개발 환경 사용하면 한 번에 가능
  1.  프로그램 실행과 디버깅
  1. 유지, 보수

# 프로그래밍 작성 과정
1. 통합개발환경(IDE)
  - 편집+컴파일+실행+디버깅
  - ex. visual studio, 이클립스, Dev-c++
  - 프로젝트(project): 하나의 실행파일 만드는 데 필요한 소스코드, 아이콘, 이미지, 데이터 들어있는 컨테이너
  - 솔루션(solution): 문제 해결에 필요한 여러 프로젝트 갖고 있는 컨테이너.

# 실전
1. 시작
```c
int main(void)
{
}
```
1. 주석
```c
/* */
//
```
1. 변수
  1. 정수형 변수
  1. 실수형 변수
1. 상수
```c
const int year = 2000;
// 상수 변수형
```
1. 특수문자(Escape Sequence)

  |특수문자|기능|
  |:---:|:---:|
  |\a|경고음|
  |\b|백스페이스|
  |\f|폼피드(Form Feed)|
  |\n|다음 줄(개행)|
  |\r|캐리지 리턴(Carriage Return, 커서 줄 맨 앞으로)|
  |\t|수평 탭|
  |\v|수직 탭|
  |\'|작은 따옴표 풀력|
  |\"|큰 따옴표 출력|
  |\?|물음표 출력|
  |\\|역슬래쉬 출력|

1. 서식문자 자료형

  |자료형|부호|유형|설명|바이트|
  |:---:|:---:|:---:|:---:|:---:|
  |정수형|O|short|short형 정수|2|
  |정수형|O|int|정수|4|
  |정수형|O|long|long형 정수|4|
  |정수형|X|unsigned short|.|2|
  |정수형|X|unsigned int|.|4|
  |정수형|X|unsigned long|.|4|
  |문자형|O|char|문자 및 정수|1|
  |문자형|X|unsigned char|문자 및 부호없는 정수|1|
  |부동소수점형|.|flaot|단일정밀도 부동소수점|4|
  |부동소수점형|.|double|두배정밀도 부동소수점|8|

1. printf()
  - %로 서식 지정
  - 파이썬과 달리 뒤의 인자들 %()로 묶을 필요 없다.

1. scanf()
  - 키보드 입력을 받아서 저장
  - &로 서식 지정
  - 파이썬과 달리 서식 지정이 가능하다.
