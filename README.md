# java-calculator-precourse

# 구현해야할 기능 목록

## 기본 기능

- 숫자 추출 : 입력된 문자열에서 숫자를 추출한다. (기본 구분자 -> ":", "," )
    - ex. "" -> return 0
    - ex. "1,2" -> return 1,2
- 숫자 합산 : 추출한 숫자 배열들을 모두 더한다.

## 커스텀 구분자 기능

- 커스텀 구분자 지원 : 문자열 앞부분의 '//' 와 '\n' 사이에 위치한 문자를 커스텀 문자 사용
    - ex. "//;\n1;2;3" -> return 6

## 예외 처리

- 잘못된 예외 처리 : 사용자가 잘못된 값을 입력할 경우 `IllegalArgumentException`을 발생시키고, 애플리케이션을 종료한다.
    - ex. "1,2,abc" ->
    - ex. 커스텀 구분자를 추가하지 않았는데, 문자열에 들어가 있는 경우
    - ex."-1,2,3" -> 구분자와 양수로 구성된 문자열이므로, 구분자에 '-' 가 추가로 들어가있지않은 이상, 바로 예외처리
  