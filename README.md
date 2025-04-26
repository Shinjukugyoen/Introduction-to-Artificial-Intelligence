# Introduction-to-Artificial-Intelligence
Introduction to Artificial Intelligence, 인공지능기초

# OpenAI API 기반 문제 해결 프로젝트

## 프로젝트 개요
- **제목**: 구조화된 JSON 추출 시스템
- **선택한 문제 유형**: 예시 과제 7번 - 복잡한 자연어 텍스트에서 명시된 정보들을 구조적으로 정리 (구인 공고, 행사 안내문 등)
- **목표**: 이 프로젝트는 OpenAI API를 활용하여 자연어 텍스트에서 필요한 정보를 구조화된 JSON 형태로 추출하는 시스템을 구현하는 것입니다. 예를 들어, 행사 안내문에서 기업명, 행사명, 날짜, 장소, 기조 연설자 등의 정보를 추출하는 기능을 목표로 합니다.

## 시스템 구성
- **사용한 모델**: gpt-4o-mini
- **사용한 주요 파라미터**:
  - `temperature`: 0.0 (출력의 일관성을 위해 낮은 값 사용)
  - `max_tokens`: 1000 (출력 길이에 제한을 둡니다)
- **라이브러리 및 환경**:
  - Python 3.x
  - openai
  - dotenv

## 실행 방법

1. **.env 파일에 OpenAI API 키 저장**:
   `.env` 파일을 프로젝트 루트에 생성하고, OpenAI API 키를 다음과 같이 저장합니다.
