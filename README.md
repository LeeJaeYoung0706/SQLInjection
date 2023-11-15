# SQLInjection

### SQL Injection 공격에 대해서 정리해보도록합니다.

#### 보통 아이디 값에 ' -- 을 넣게 되면 주석처리가 됨으로 뒤에 AND 절로 Password를 검증하게 될 때 SQL Injection에 취약하게 됩니다.
#### 그렇기 때문에 ORM을 사용하거나 특수문자처리를 통해서 SQLInjection을 처리하거나 프로시져 함수를 사용하는 기법들이 있습니다.
#### OR 1 = 1 을 넣게 되면 인덱스 1에 검색된 값이 노출 됨으로 어드민 계정이 털릴 확률이 높아지기 때문에 반드시 막아야합니다.! 

#### 그렇기 때문에 Node.js로 구성한 홈페이지의 경우 시퀄라이져를 사용하게 되면 ORM , Salt 비교를 통해서 SQL Injection에 방어하기 쉬웠던 것입니다!.
