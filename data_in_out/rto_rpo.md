### RTO (Recovery Time Objective, 목표 복구 시간)
- 비상사태 또는 업무 중단 시점으로부터 복구되어 가동될 때까지의 소요 시간
- ex. 장애 발생 후 24시간 내 복구 가능

### RPO (Recovery Point Objective, 목표 복구 시점)
- 비상사태 또는 업무 중단 시점으로부터 데이터를 복구할 수 있는 기준점
- ex. 장애 발생 전인 지난 주 금요일에 백업시켜 둔 복원 시점으로 복구 가능

```
<정보처리기사 실기 2020년 2회 15번 문제>
다음은 IP 인프라 서비스 관리 실무와 관련된 <실무 사례>에 대한 설명이다. 가장 적합한 용어를 한글 또는 영문으로 쓰시오.

A는 ㈜한국아이티 보안관제실에서 정보시스템의 정보관리를 위해 모니터링을 담당하며 근무하고 있다. 시스
템 운영 중 자연재해나 시스템 장애 등의 이유로 대고객 서비스가 불가능한 경우가 종종 발생한다. 
A는 이런 장애 발생시 서비스를 정상적으로 수행하기 위해 구축 시스템을 관리하는 역할을 한다. 
이 용어는 이런 비상 상황이 발생 했을 때, "서비스 중단 시점과 서비스 복원 시점 간에 허용되는 최대 지연 시간"을 가리킨다.

서비스가 불가능한 경우
> 서비스 중단 시점과 서비스 복원 시점 간 최대 지연 시간
정답: RTO 또는 목표 복구 시간
```