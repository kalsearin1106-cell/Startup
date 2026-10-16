# 기업분석 PDF 리포트 skill

사용자가 제공한 사진, 문서, 웹페이지 URL만 근거로 기업분석 보고서를 만들고, 추출 사실과 PDF 초안에서 각각 검토를 받는 Codex skill입니다.

## 설치

Codex 개인 skill 폴더에 이 저장소를 `company-report-pdf` 이름으로 clone합니다.

```powershell
git clone <private-repository-url> "$env:USERPROFILE\.agents\skills\company-report-pdf"
```

그 다음 Codex에서 `$company-report-pdf`를 호출하거나 기업분석 보고서/PDF 작성을 요청합니다. 업데이트하려면 이 폴더에서 `git pull`을 실행합니다.

## 사용 흐름

1. 회사, 보고서 목적·독자, 프로젝트별 저장 폴더와 자료를 전달합니다.
2. 출처 인벤토리와 추출한 사실을 검토하고 수정합니다.
3. 보고서 원고와 PDF 초안을 검토합니다.
4. 확정한 산출물을 프로젝트별 폴더에 보관합니다.

회사별 원본 자료와 리포트는 이 skill 저장소에 넣지 않습니다. 이 저장소에는 재사용 가능한 지침과 범용 자료만 관리합니다.

