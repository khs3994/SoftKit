<p align="center">
  <img src="assets/banner.png" alt="SoftKit" width="480">
</p>

# SoftKit

소프트웨어 개발의 소프트한 부분(커뮤니케이션, 기획, 문서)을 돕는 Claude Code 플러그인입니다. 코드 리뷰·PR 큐처럼 코드를 직접 다루는 쪽은 [HardKit](https://github.com/khs3994/HardKit)이 맡습니다.

## 설치

```
/plugin marketplace add https://github.com/khs3994/SoftKit
/plugin install softkit@softkit
```

## 구성

| 이름 | 종류 | 하는 일 | 예시 |
|---|---|---|---|
| `/surface` | 스킬 | 현재 세션에서 팀에 공유할 내용과 확인이 필요한 질문을 뽑아 대상별 메시지 초안을 만든다 | `/surface` |
| `/debrief` | 스킬 | 받은 슬랙·PR 코멘트·기획서를 두고 화자가 말하는 것, 불확실한 부분, 되물을 질문과 질문 문장을 정리한다 | "이 리뷰 코멘트 뭘 하라는 거야?" + 원문 |
| `communicator` | 에이전트 | 보낼 메시지를 대상과 채널에 맞게 쓰거나 다듬는다. `surface`와 `debrief`가 문장을 쓸 때도 이 에이전트를 쓴다 | "이거 슬랙에 보낼 건데 다듬어줘" + 초안 |

모든 스킬과 에이전트는 초안만 만들고 직접 전송하지 않습니다.

## 로컬 개발

```
git clone https://github.com/khs3994/SoftKit
/plugin marketplace add ./SoftKit
/plugin install softkit@softkit
```

파일을 수정한 뒤에는 `/plugin marketplace update softkit`으로 새로고침합니다.

## 라이선스

MIT
