# 2026-07-01 학습 정리

## 학습 주제
- Kotlin 배열(Array, IntArray)과 반복문(for, indices, withIndex)
- 컬렉션(List, Set, Map)의 특징과 순회 방법
- 클래스와 객체지향 프로그래밍 기초
- 생성자(주 생성자, 보조 생성자), 상속, 오버라이딩
- data class와 companion object

## 핵심 정리
### 1. 배열과 반복문
- `Array(size) { ... }` 형태로 배열을 초기화할 수 있고, 람다를 사용해 초기값을 계산할 수 있다.
- `IntArray`는 기본형 배열이고, `Array<Int>`와는 다른 타입이다.
- 배열 순회는 `for (item in array)`, `for (i in array.indices)`, `for ((i, v) in array.withIndex())` 방식으로 할 수 있다.
- 값을 직접 수정할 때는 인덱스를 사용하는 방식이 적합하다.

### 2. 컬렉션
- `List`는 순서가 있고 중복을 허용한다.
- `Set`은 중복을 허용하지 않는다.
- `Map`은 `Key`와 `Value` 쌍으로 데이터를 저장하며, `keys`, `values`, `entries`로 순회할 수 있다.

### 3. 클래스와 생성자
- 클래스는 `init` 블록을 통해 초기화할 수 있다.
- 생성자 매개변수에 `val` 또는 `var`를 붙이면 클래스 프로퍼티로 바로 선언된다.
- 보조 생성자를 사용하면 다양한 방식으로 객체를 생성할 수 있다.

### 4. 상속과 오버라이딩
- Kotlin에서 상속하려면 부모 클래스에 `open` 키워드가 필요하다.
- 프로퍼티와 함수도 재정의하려면 `open`으로 선언하고, 자식 클래스에서 `override`를 사용해야 한다.

### 5. data class와 companion object
- `data class`는 데이터를 다루기 위한 클래스이며, 주 생성자 프로퍼티 기준으로 `equals()` 같은 기능이 동작한다.
- `companion object`를 사용하면 클래스 이름으로 바로 접근 가능한 정적 멤버처럼 사용할 수 있다.

## 한 줄 요약
오늘은 Kotlin의 배열, 반복문, 컬렉션, 클래스, 생성자, 상속, data class, companion object까지 객체지향 기초 문법을 실습 중심으로 학습했다.
