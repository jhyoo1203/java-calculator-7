# 문자열 덧셈 계산기

## 🔥 구현할 기능 목록

---

### 입력
- [x] 문자열 입력 기능
    ```
    덧셈할 문자열을 입력해 주세요.
    1,2:3
    ```

### 출력
- [x] 결과 출력 기능
  - 구분자를 기준으로 분리한 각 숫자의 합 반환
    ```
    결과 : 6
    ```

### 구분자
- [x] 쉼표(,) 또는 콜론(:) 구분자 기능
  - [x] 구분자를 저장하는 Separator 클래스 구현
  - [x] 초기 정규표현식 생성 ```,|:```

- [x] 커스텀 구분자 기능(쉼표, 콜론 외)
    - 예시: ```//;\n```
    - prefix: ```//```, suffix: ```\n```로 커스텀 구분자 등록
    - prefix + 구분자 + suffix
    - [x] 정규표현식에 ```|``` + ```구분자```를 더하여 구분자 업데이트
    - [x] 구분자로 ```|```, ```.``` 사용 시, 앞에 이스케이프 문자 ```\\``` 추가
  

---
### 🚫 예외 처리
- ```IllegalArgumentException```

##### 문자열 입력
- [ ] 음수 입력 시 예외 처리(커스텀 구분자로 - 기호 등록 제한)
- [ ] 구분자 다음에 특수기호 혹은 문자가 오면 예외처리
- [ ] 숫자 구분 모호성을 고려해 커스텀 구분자에 숫자 입력 예외 처리
- [ ] 커스텀 구분자 길이 5로 제한

---
### 라이브러리
```Java
// 예시
import camp.nextstep.edu.missionutils.Console;

String value = Console.readLine();
```