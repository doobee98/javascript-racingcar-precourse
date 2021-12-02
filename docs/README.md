## 구현할 기능 목록

# 기본 세팅

- [x] ESLint + Prettier 세팅
- [ ] 전체 디렉토리 기본 구조 잡기 (skeleton)

# 자동차 경주 게임 - 게임

- [ ] **모델 정의** 게임에서 사용할 데이터 모델 객체 정의
  - 자동차
  - 자동차 경주 라인 (자동차의 위치값, 전진 메소드)
- [ ] **입력값 검증** 게임 룰에 맞는 입력값인지 검증
  - 자동차 이름이 콤마로 잘 연결되어 있는지, 5자 이하인지, 읽을 수 없는 문자(공백 등)이 있는지 확인
  - 시도할 횟수가 숫자로 잘 입력되어 있는지 확인
  - [ ] 시도할 횟수에 자체적으로 제약을 걸지 말지 고민 중 (1 ~ 20 정도의 범위?)
- [ ] **게임 진행** progressGame 함수를 한번 호출할 때마다 모든 자동차가 한번씩 전진 시도, 이걸 '시도할 횟수' 만큼 반복
- [ ] **게임 결과** 우승자를 판단

# 자동차 경주 게임 - DOM 연결

- [ ] **DOM 객체 정의** HTML에서 id로 지정한 DOM elements를 로딩
- [ ] **결과 출력용 DOM 출력값 템플릿** index.html에서 'racing-winners' id를 지정할 마땅한 태그가 없으므로, 직접 해당 id를 가진 element를 주입하기 위한 템플릿 정의
- [ ] **입력 이벤트 핸들러 작성** 클라이언트가 제출 버튼을 누르는 onClick 이벤트 핸들러를 지정할 수 있도록 함
  - car-names-submit
  - racing-count-submit
- [ ] **출력 메소드 작성** 게임 서버에서 보여줄 결과 출력을 위한 메소드를 작성
  - 입력 오류 발생 시 alert
  - 자동차 경주 과정 및 결과 출력

# 자동차 경주 게임 - 클라이언트

- [x] **HTML 변경** 문제에서 요구하는 id 선택자 지정