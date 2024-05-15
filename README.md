#  smalloc.c 프로그램
C 프로그래밍 언어에서 동적 메모리 할당 기능을 제공하는 프로그램이다. 

## 🖥프로젝트 소개
- 메모리 블록의 할당, 재할당 및 해제 기능의 함수들을 포함한다. 
- 내부적으로 메모리 블록의 연결 리스트를 생성하고 유지하여 메모리를 관리한다.
- 사용중인 또는 사용하지 않는 메모리 블록에 대한 정보를 표시한다.


## 개발 기간 ##
* 2024.04.30 ~2024.05.15


## ✏개발 환경
- **OS** : UNIX 또는 Linux
- **Language** : C language
- **Compiler** : GCC 

## 사용 방법
- make 입력
- ./<test_case> 입력하여 실행


## 💡주요 기능 ##
- smalloc(size_t s) 메모리 할당: 지정된 크기의 메모리 블록을 할당합니다.
- sfree(void *p) 메모리 해제: 이전에 할당된 메모리 블록을 해제합니다.
- srealloc(void *p, size_t s) 메모리 재할당: 이전에 할당된 메모리 블록의 크기를 조정합니다.
- smcoalesce() 메모리 병합: 같은 페이지의 연속된 빈공간을 병합합니다
- smalloc_mode(size_t s, smmode m) 메모리 할당 방식 지정: 메모리 할당 방식을 지정하고 빈공간에 메모리를 할당합니다
- sdump() 결과 출력: used memory slots 및 unused memory slots에 대한 정보를 [메모리블록출력순서:메모리블록주소:메모리블록크기] 형식으로 표시합니다.