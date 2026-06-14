# SNS Mommy

RisuAI 플러그인 — **sns_nai**(SNS/메신저 롤플레이 시뮬레이터 + NAI 이미지)와 **Asset Mommy**(NovelAI 에셋 생성·관리 + 외견 추출)를 **하나로 통합**한 단일 플러그인. iOS(아이폰) 최적화.

## 설치 (RisuAI)

1. RisuAI → 설정 → 플러그인 → 플러그인 가져오기
2. URL: `https://raw.githubusercontent.com/aredsea/sns-mommy/main/sns-mommy.js`
3. import 후 새로고침
4. **기존 sns_nai / Asset Mommy 플러그인은 삭제**하세요(중복 방지). 설정·API 키는 전역 저장소라 통합본이 그대로 승계합니다.

## 버전 규칙

`MAJOR.MINOR.PATCH` — 매 릴리스마다 PATCH를 올리고, PATCH가 10이 되면 MINOR로 올림(PATCH는 0). 예) `1.0.9 → 1.1.0`.
플러그인 목록 이름(`SNS Mommy x.y.z`)으로 로드된 버전을 확인할 수 있습니다.

## 통합 로드맵 (단계별)

- **1단계 (현재): 패키징 머지** — 두 플러그인을 한 파일/한 헤더로 결합. 각 코드는 자기 클로저에서 그대로 동작(기능 변경 없음). 업데이트는 네이티브 `//@update-url` 단일 채널.
- 2단계: NAI/LLM 설정 단일화(키·URL·모델 1벌).
- 3단계: NAI 이미지 엔진(요청·전송·ZIP) 공유 코어.
- 4단계: 생성 이미지 단일 저장소 + 카테고리 분류 + 통합 갤러리.
- 5단계: 통합 레퍼런스 시스템 + "이 캐릭터 자동 설정(원클릭)" — 캐릭터 추가 에셋 분석 → 의상별 레퍼런스 자동 구성 → 채팅/SNS 변형 생성.
- 6단계: 모바일 앱 템플릿 기반 UI 전면 리디자인(간결 표면 + 고급 설정 숨김/노출).

## 사용 개요

- **SNS**: 채팅창 햄버거 메뉴 → SNS NAI 진입. 채팅 내용을 반영해 SNS 게시물·이미지 생성.
- **Asset Mommy**: 캐릭터 외견 추출(lb-xnai.lb.extra), NovelAI 에셋 생성·교체, 캐릭터/의상별 레퍼런스.
- **연동**: 캐릭터 레퍼런스를 채팅 이미지 변환과 SNS 이미지 생성이 공통으로 사용.

## 출처

기존 두 플러그인([sns-nai](https://github.com/aredsea/sns-nai), [asset-mommy](https://github.com/aredsea/asset-mommy))을 통합한 것입니다. 향후 업데이트는 이 레포에서 진행됩니다.
