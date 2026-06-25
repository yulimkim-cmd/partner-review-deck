# Partner Review Deck — Claude Code Skill

파트너 대면 미팅용 실적 리뷰 장표를 자동 생성하는 [Claude Code](https://claude.ai/code) 스킬입니다.

## 기능

- python-pptx로 PPTX 자동 생성 (8슬라이드 구조)
- Action Title 원칙 적용 (제목 = 결론)
- 파트너 대상 언어로 자동 변환 (UV→유입, CVR→전환율)
- 내부 데이터(GMV, 마진, 순위) 자동 제외
- MRT 디자인 시스템 적용

## 설치

```bash
# Claude Code에서 스킬 폴더로 복사
cp -r partner-review-deck ~/.claude/skills/
```

또는 Claude Code에서:
```
이 폴더를 스킬로 추가해줘
```

## 사용법

Claude Code에서:
```
테라투어 상반기 리뷰 장표 만들어줘
```

## 장표 구조

| # | 슬라이드 | 내용 |
|---|---------|------|
| 1 | 커버 | 파트너명, 기간, 브랜드 디자인 |
| 2 | 상반기 전체 성과 | 성장/하락 분해 + 월별 YoY |
| 3 | 노선별 실적 | 송객순 + 하이라이트 + YoY |
| 4 | 비수기 프로모션 | 유입 하락 + 프로모션 효과 |
| 5 | 딥다이브 | 핵심 이슈 분석 |
| 6 | 우수파트너 효과 | 선정 전후 비교 |
| 7 | 하반기 협업 방향 | 파트너 공유용 |
| 8 | Thank You | |

## 디자인

- 컬러: MRT Blue `#00AFEC` 기반
- 폰트: Pretendard
- 헤더: Blue Dark 바 + Red 액센트
- Action Title: 모든 슬라이드 제목이 결론

## 작성 원칙

1. **제목 = 결론** (Action Title)
2. **1슬라이드 1메시지**
3. **파트너 대상 언어** (내부 용어 금지)
4. **내부 데이터 제외** (GMV, 마진, 순위)
5. **So What 해석** (데이터만 나열 금지)

## License

MIT
