# Introduction-to-Artificial-Intelligence
Introduction to Artificial Intelligence, 인공지능기초

# OpenAI API 기반 문제 해결 프로젝트

1. 프로젝트 개요
- 제목: 구조화된 JSON 추출 시스템
- 선택한 문제 유형: 예시 과제 7번 - 복잡한 자연어 텍스트에서 명시된 정보들을 구조적으로 정리 (구인 공고, 행사 안내문 등)
- 목표: 이 프로젝트는 OpenAI API를 활용하여 자연어 텍스트에서 필요한 정보를 구조화된 JSON 형태로 추출하는 시스템을 구현하는 것입니다. 예를 들어, 행사 안내문에서 기업명, 행사명, 날짜, 장소, 기조 연설자 등의 정보를 추출하는 기능을 목표로 합니다.

2. 시스템 구성
- 사용한 모델: gpt-4o-mini
- 사용한 주요 파라미터:
  - temperature: 0.0
  - max_tokens: 1000
- 라이브러리 및 환경:
  - Python 3.x
  - openai
  - dotenv

3. 실행 방법

1. .env 파일에 OpenAI API 키 저장:
   `.env` 파일을 프로젝트 루트에 생성하고, OpenAI API 키를 저장합니다.
OPENAI_API_KEY=your-api-key-here

2. 필요한 라이브러리 설치:
프로젝트에 다음 명령어를 실행하여 필요한 라이브러리를 설치합니다.
pip install openai python-dotenv

3. 메인 실행 파일 실행: main.py 파일을 실행하여 프로그램을 실행합니다.
python main.py

4. 예시 입력 및 출력
- 입력 예시:
A 기업은 2025년 6월 1일 서울 강남에서 열리는 AI 콘퍼런스에 참가할 예정이며, 특별 강연은 김태훈 박사가 맡습니다.

-출력 예시:
"organization": "A 기업",
    "event": "AI 콘퍼런스",
    "date": "2025-06-01",
    "location": "서울 강남",
    "keynote_speaker": "김태훈 박사"

5. 파일 구성
  | 파일명 | 설명 |
|--------|------|
| main.py | 프로젝트 메인 실행 파일 |
| 202321855_AnYeongmin_DescriptiveAssignment.docx | 서술형 과제 보고서 |
| 202321855_AnYeongmin_AnalysisReport.docx | 실습 과제 보고서 |
| .env | API Key가 저장. |
| README.md | 실행 안내서 (본 문서) |

6. 참고자료
심플러스. (2024). 파이썬 OpenAI API key 숨기기: env파일, 환경변수 설정. 심플러스. https://simpleuse.tistory.com/entry/howtousekey
gliver. (2023). 환경 변수 (PATH)란?. 알고리듬. https://gliver.tistory.com/43
강의 자료 Chapter 6~8 (프롬프트 설계)

8. 기타
- 코드에는 적절한 주석(comment)을 포함하였습니다.
