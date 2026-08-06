<p align="center">
  <img src="assets/banner.png" alt="SoftKit" width="480">
</p>

# SoftKit

소프트웨어 개발의 '소프트한 부분' — 기획 검토, 문서화, 커뮤니케이션 — 을 자동화하는 툴킷입니다.

코드를 짜는 것은 일의 일부일 뿐입니다. SoftKit은 그 주변의 모든 것을 돕는 Claude 플러그인입니다. 작업 전 스펙을 검토하고, 공수 산정을 점검하고, 스프린트를 계획하고, 흩어진 맥락을 남이 읽을 수 있는 문서로 바꿔 줍니다.

코드 자체는 짝꿍인 [HardKit](https://github.com/khs3994/HardKit)이 담당합니다.

## 구성

**커뮤니케이션**

- **`surface` 스킬** — 현재 세션에서 팀에 공유할 내용과, 아직 누군가의 답이 필요한 모호한 지점을 끄집어낸 뒤, 대상별 전달용 메시지 초안을 만들어 줍니다. 초안만 만들며 직접 전송하지는 않습니다.
- **`communicator` 에이전트** — 개발 맥락을 특정 대상에게 맞는 명확하고 적절한 톤의 메시지로 바꿔 주는 범용 소통 전문가입니다. 단독으로도 쓰이고, `surface`가 초안을 작성할 때 문장 작성 엔진 역할도 합니다.

기획·공수·플래닝·문서 관련 킷이 이어서 추가될 예정입니다.

## 설치

Claude Code에서 아래 두 명령으로 설치합니다.

```
/plugin marketplace add https://github.com/khs3994/SoftKit
/plugin install softkit@softkit
```

설치가 끝나면 `surface` 스킬과 `communicator` 에이전트가 활성화됩니다.

### 로컬(개발용) 설치

repo를 클론한 뒤 로컬 경로로 마켓플레이스를 추가해도 됩니다.

```
git clone https://github.com/khs3994/SoftKit
```

```
/plugin marketplace add ./SoftKit
/plugin install softkit@softkit
```

플러그인 파일을 수정한 뒤에는 `/plugin marketplace update softkit` 로 새로고침하거나 세션을 다시 시작하면 반영됩니다.

## 사용법

- **`/surface`** — 대화를 어느 정도 진행한 뒤 "이 내용 팀에 공유하고 확인받을 것 정리해줘" 같은 상황에서 실행합니다. 진행/결정/확인필요/블로커를 뽑아 대상별 초안을 만들어 줍니다.
- **`communicator`** — "이 메시지 상대방이 이해하기 쉽게 다듬어줘"처럼 문장을 다듬거나 톤을 조정할 때 사용합니다.

## 라이선스

MIT
