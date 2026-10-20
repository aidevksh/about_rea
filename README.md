# about_rea

[REA (Reverse Engineer Anything)](https://github.com/morluto/rea)와 LLM 에이전트가 함께 리버스 엔지니어링을 수행하는 과정을 소스 코드 기준으로 분석하고, 관련 주제로 게임 매시업 모드의 구현 방식을 조사한 문서 모음입니다.

## 문서

| 파일 | 내용 |
| --- | --- |
| [docs/rea-llm-reverse-engineering.html](docs/rea-llm-reverse-engineering.html) | REA × LLM 리버스 엔지니어링 프로세스 흐름도. 설치부터 결과 전달까지 16단계, 도구 호출 한 번의 시퀀스, Evidence 구조, 실제 사례(DX-Ball·TH04·Notion), 안전장치와 한계 |
| [docs/game-mashup-mods.html](docs/game-mashup-mods.html) | 게임 섞기 모드(엘든링 × 오버워치, 사이버펑크 × 마인크래프트 등)가 에셋 이식, 패스스루(두 게임 동시 실행), AI 생성 영상 중 무엇인지와 각 방식의 구현 구조 |

HTML 파일은 내려받아 브라우저로 열면 됩니다. 도식은 인라인 SVG이고 라이트·다크 모드를 모두 지원합니다.

## 분석 기준

- 대상: [morluto/rea](https://github.com/morluto/rea) main 브랜치 커밋 `d72d856f5` (2026-10-16), 패키지 rea-agents 6.5.0
- `rea/`는 위 커밋에 고정한 git 서브모듈입니다. 함께 받으려면 `git clone --recurse-submodules`를 쓰세요.
- 방법: 저장소 문서와 소스를 읽어 분석했고, 빌드·테스트·스크립트는 실행하지 않았습니다. 문서 안의 `파일:라인` 근거는 이 커밋 기준입니다.
- 게임 매시업 조사일: 2026-10-16. 웹 문서와 저장소는 바뀌거나 사라질 수 있습니다.

## 라이선스

이 저장소의 문서는 [Apache License 2.0](LICENSE)을 따릅니다. 서브모듈 `rea/`는 원저작자(morluto)의 저장소이며 자체 라이선스(MIT)를 따릅니다. 문서에 인용한 제3자 자료의 권리는 각 원저작자에게 있습니다.
