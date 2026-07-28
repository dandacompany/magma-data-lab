# magma-data-lab

MAGMA(3040 남성 패션 브랜드)의 데이터 분석 사업부 작업 저장소입니다.
인프런 「Hermes × Codex 가상 오피스」 섹션 7(데이터 분석)이 이 저장소 위에서 진행됩니다.

회사소개 사이트(magma-content-site)가 회사를 보여주는 곳이라면,
이 저장소는 데이터가 모이고 다듬어지는 일터입니다.
실적 보고서를 사이트에 올리는 마지막 단계만 content-site에서 진행합니다.

## 구조 한눈에

```
supabase/        데이터베이스 스키마 변경 기록 (실습 중 생성됩니다)
data/collect/    수집한 시장 데이터 CSV
data/mart/       판매·프로모션 실습용 데이터
dashboard/       BI 대시보드 앱 (실습 중 생성됩니다)
```

## 유닛별로 채워지는 자리

| 실습 | 채울 자리 | 만들어지는 것 |
| --- | --- | --- |
| 데이터베이스 준비 | `supabase/` | 스키마 설계와 마이그레이션 파일 |
| 웹 데이터 수집·적재 | `data/collect/` | 무신사·네이버·쿠팡 수집 CSV |
| 데이터 정제·분석 | `data/mart/` | 판매 데이터 마트와 정제 기록 |
| BI 대시보드 | `dashboard/` | 대시보드 앱과 배포 |

## 준비물

- Supabase 계정 (무료 요금제)
- supabase CLI (첫 실습에서 함께 설치합니다)
- Hermes 에이전트 (Ada 프로필)

## 처음 5분 체크리스트

1. GitHub에서 이 저장소를 Fork 하거나 Use this template으로 내 저장소를 만듭니다.
2. 내 컴퓨터의 정해진 위치로 clone 합니다.
   ```bash
   git clone (내 저장소 주소) ~/.hermes/workspace/magma-data-lab
   cd ~/.hermes/workspace/magma-data-lab && pwd
   ```
3. 이후의 모든 데이터 작업은 이 폴더 안에서 진행합니다.
   터미널을 새로 열 때마다 `pwd`로 위치를 확인하는 습관을 권합니다.

## 주의

- 이 저장소에는 공개 데이터와 실습용 모의 데이터만 저장합니다.
- 접속 토큰이나 데이터베이스 비밀번호는 절대 커밋하지 않습니다. `.gitignore`가 `.env` 계열을 막아두었지만, 커밋 전에 한 번 더 확인하세요.
