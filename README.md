# PCRM XTE WEN 3.0 

- 홈페이지 : [data-m.ci.kr](http://www.data-m.co.kr/).

## PCRM XTE WEB 3.0 API Infra
PCRM XTE WEB 3.0 API는 블록체인의 태생적 이슈와 문제점인 느린 네트워크, DAPP개발의 기능적 제한 등 인프라 구성의 접근성을 해결함과 기존 서비스 및 시스템 등이 블록체인에 용이하게 참여할 수 있도록 지원함을 목적으로 합니다. 

## PCRM XTE WEB 3.0 API Interface
API는 성능을 고려하여 Sync 타입과 Async 타입으로 분류됩니다. 제휴사는 각 API에 해당되는 기능을 적용하며 JSON, C/C++, JAVA등 다양한 개발언어를 지원합니다.

| API | 요청 | 처리 | 기능 | 비고 |
|----------------------------|--------|--------|------|------|
|Exchange Rate Inquiry|Partners|MW30P|Item/Point/etc to PlayToken 환율 조회<br>PlayToken to Item/Point/etc 환율 조회<br>(파트너사가 사용자에게 제공하는 각종 혜택 등)||
|Exchange |Partners|MW30P|Item/Point/etc to PlayToken 전환<br>PlayToken to Item/Point/etc 전환|Async|
|Passport|Partners|MW30P|주요 API 실행을 위한 인증 서비스||
|Withdrawal Address|Partners|MW30P|Partner사의 사용자가 보유한 외부에서 사용할 수 있는<br>블록체인 주소에 대한 검증 및 등록/변경 (인출주소) ||
|Withdrawal pre-trade|Partners|MW30P|인출 예비 거래||
|Withdrawal|Partners|MW30P|인출 가능 토큰(PlayToken 등)을 외부 주소로 인출|Async|
|Block Notify|MW30P|Partners|Exchange API, Withdrawal API의 블록체인 처리 결과 전송<br>(Confirm 완료 여부)|Async|
