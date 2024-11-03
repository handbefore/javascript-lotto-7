# javascript-lotto-precourse
# <기능 목록>
## **1. 구입 금액 입력**
- [x] 구입 금액 입력 받기
- [x] 구입 금액은 1,000원 단위로 입력 받음

```
구입금액을 입력해 주세요.
```

### **예외 처리**
- [ ] 1,000원으로 나누어 떨어지지 않는 경우
- [ ] 숫자만 가능 (문자 x)
- [ ] 빈칸 불가능

## **2. 로또 번호 생성**
- [ ] 구입 금액에 해당하는 만큼 로또를 발행해야 함, 로또 1장의 가격은 1,000원
- [ ] 발행한 로또 수량 및 번호를 출력
- [ ] 로또 번호는 오름차순으로 정렬하여 보여줌 

```
8개를 구매했습니다.
```

## **3. 당첨 번호 입력**
- [ ] 당첨 번호 입력 받기
- [ ] 입력 받은 번호는 쉼표(,)를 기준으로 구분

```
당첨 번호를 입력해 주세요.
```   
- [ ] 보너스 번호를 입력 받기

```
보너스 번호를 입력해 주세요.
```

## **예외 처리**
```
[ERROR] 로또 번호는 1부터 45 사이의 숫자여야 합니다.
```
- [ ] 숫자만 가능 (문자 x)
- [ ] 빈칸 불가능
- [ ] 숫자는 한자리만 입력 가능

## 4. **당첨 통계**
- [ ] 사용자가 구매한 로또 번호와 당첨 번호를 비교

## 5. **결과 출력**
- [ ] 당첨 내역 출력
- [ ] 당첨 통계 출력
```
---
3개 일치 (5,000원) - 1개
4개 일치 (50,000원) - 0개
5개 일치 (1,500,000원) - 0개
5개 일치, 보너스 볼 일치 (30,000,000원) - 0개
6개 일치 (2,000,000,000원) - 0개
수익률을 출력
수익률은 소수점 둘째 자리에서 반올림한다. (ex. 100.0%, 51.5%, 1,000,000.0%)
총 수익률은 62.5%입니다.
로또 게임을 종료
```

<br/>

----
# **프로그래밍 요구 사항 1**
Node.js 20.17.0 버전에서 실행 가능해야 한다.
프로그램 실행의 시작점은 App.js의 run()이다.

package.json 파일은 변경할 수 없으며, 제공된 라이브러리와 스타일 라이브러리 이외의 외부 라이브러리는 사용하지 않는다.

프로그램 종료 시 process.exit()를 호출하지 않는다.

프로그래밍 요구 사항에서 달리 명시하지 않는 한 파일, 패키지 등의 이름을 바꾸거나 이동하지 않는다.

자바스크립트 코드 컨벤션을 지키면서 프로그래밍한다.
기본적으로 JavaScript Style Guide를 원칙으로 한다.

---
# **프로그래밍 요구 사항 2**
indent(인덴트, 들여쓰기) depth를 3이 넘지 않도록 구현한다. 2까지만 허용한다.   
힌트: indent(인덴트, 들여쓰기) depth를 줄이는 좋은 방법은 함수(또는 메서드)를 분리하면 된다.
3항 연산자를 쓰지 않는다.

함수(또는 메서드)가 한 가지 일만 하도록 최대한 작게 만들어라.

Jest를 이용하여 정리한 기능 목록이 정상적으로 작동하는지 테스트 코드로 확인한다.

---
# **프로그래밍 요구 사항 3**
함수(또는 메서드)의 길이가 15라인을 넘어가지 않도록 구현한다.

함수(또는 메서드)가 한 가지 일만 잘 하도록 구현한다.
else를 지양한다.

때로는 if/else, when문을 사용하는 것이 더 깔끔해 보일 수 있다. 어느 경우에 쓰는 것이 적절할지 스스로 고민해 본다.   
힌트: if 조건절에서 값을 return하는 방식으로 구현하면 else를 사용하지 않아도 된다.

구현한 기능에 대한 단위 테스트를 작성한다. 단, UI(System.out, System.in, Scanner) 로직은 제외한다.

