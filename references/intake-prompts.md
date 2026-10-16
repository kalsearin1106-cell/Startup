# Intake form and reusable request prompt

Use these Korean templates as the default for Korean-language requests. Translate them for the user's language. Present the form and prompt when the skill is first invoked unless the user has already provided the relevant details or asks to proceed directly. Fill known fields from the conversation; leave only genuinely unresolved fields for the user.

## Short intake form

```text
기업명:
분석 목적:
독자:
기준일:
중점 분석 항목: (예: 사업모델, 투자 이력, 재무, 시장·경쟁, 임상·규제, 지식재산)
자료 조사 범위: 제공 자료만 / 공개 자료도 검색·검증
분량·형식·언어:
프로젝트 폴더:
검토 방식: 자료 목록 확인 후 초안 / 바로 초안 / 기타
첨부 파일·링크:
```

If the user says “자료조사도 해줘” or equivalent, interpret that as permission to research relevant public sources for the requested analysis. Do not infer permission to use private, paid, or account-gated sources. Ask about access only if it is necessary and cannot be avoided.

## Copyable prompt

```text
첨부 자료와 아래 조건을 바탕으로 [기업명] 기업분석 리포트를 작성해줘.

- 분석 목적: [목적]
- 독자: [독자]
- 기준일: [YYYY-MM-DD]
- 중점 항목: [분석 항목]
- 자료 조사 범위: [제공 자료만 / 공개 자료 검색·검증 허용]
- 분량·형식·언어: [조건]
- 프로젝트 폴더: [경로]
- 검토 방식: [단계별 검토 / 바로 초안]

작성 원칙:
1. 사실, 회사 주장, 공공·제3자 자료, 분석 의견을 구분해 표시해줘.
2. 제공 자료만 사용하도록 지정한 경우 외부 검색을 하지 마. 공개 자료 조사를 허용한 경우에는 공시·정부·규제기관·임상등록부·특허 데이터베이스 등 원출처를 우선해 실제 내용을 확인해줘.
3. 중요한 사실과 숫자마다 파일명·페이지·표·화면 또는 URL과 확인 위치를 기록해줘.
4. 자료 간 차이는 각 값과 출처를 나란히 보여주고 임의로 합치지 마. 재무자료의 표시·추출·산식 오류와 회사 원문 오류를 구분해 검증해줘.
5. 투자 내역은 확인 가능한 개별 항목과 출처 범위를 보존해줘. 합산 시 포함 항목과 산식을 밝히고, 원출처가 보장하지 않는 누적 투자유치액이나 실제 납입액으로 표현하지 마.
6. 근거 없는 원인·수치·전망·상태를 만들지 마. 검증되지 않은 내용은 제외하거나 검증 질문으로 제시해줘.
7. 계산은 산식과 사용값을 함께 적고, 표·차트·본문·출처 목록의 값이 일치하는지 확인해줘.
8. 사용자 검토를 요청하기 전에 오타, 중복, 불필요한 주석과 작업 과정 문구, 출처 누락, 페이지 가독성을 자체 점검해줘.
9. 결론이 조건부라면 어떤 임상·재무·계약 정보가 확인될 때 판단이 어떻게 달라질 수 있는지 근거와 연결해줘. 근거 없는 수치 기준은 만들지 마.
10. 밸류에이션, 지분 희석, 최신 현금흐름, 개발비 계획이 확인되지 않으면 투자 매력도나 자금 여력을 단정하지 말고 평가 한계를 결론에 반영해줘.

단계별 검토를 선택한 경우:
- 먼저 자료 목록, 확인 사실과 위치, 불명확한 점, 부족한 자료를 정리해서 보여주고 내 확인을 기다려줘.
- 확인을 받은 다음 Markdown 보고서와 PDF 초안을 만들어 내부 검수 후 다시 검토를 요청해줘.
- 최종 확인 전에는 완료본으로 확정하지 마.

기존 결과물을 덮어쓰지 말고, 새 버전을 만들 때 최신 검토본이 무엇인지 명확히 알려줘.
```

## Applying the form without creating friction

- Do not make the user fill every field when their message already answers it.
- If the user has not specified an output path, use the current project/workspace or an explicitly named folder and state the choice; ask only if multiple plausible destinations exist.
- If the user asks for fast execution and the missing item is a style preference, use a plain default and proceed.
- If source-scope permission, report purpose, or a material conclusion depends on an unresolved choice, ask one concise question before dependent work.
- Treat the supplied prompt as a reusable scaffold, not as permission to insert placeholder content. Resolve or omit every placeholder before drafting.
