# Kafka 기반 실시간 사용자 이벤트 분석 시스템

## 📚 프로젝트 개요

- **목표:** Kafka → Redis Streams → ClickHouse → Grafana → Slack 연동 구조로,  
  실시간 사용자 이벤트 수집, 저장, 시각화, 자동 알림까지 경험하는 DevOps 실습 프로젝트

## 🏗️ 아키텍처

[User Events] | v [Kafka Producer] → [Kafka Broker] → [Kafka Consumer] → [Redis Streams] | v [ClickHouse] → [Grafana Dashboard] | v [Slack 알림]


## 🛠️ 기술 스택

- Kafka, Redis Streams, ClickHouse, Grafana, Slack Webhook
- Python (Producer/Consumer, 데이터 파이프라인 구현)
- Docker, Docker Compose (전체 환경 컨테이너화)
- (선택) Node.js, Shell script 등 자유 확장 가능

## 🎯 실습 목표

- 실시간 대용량 데이터 파이프라인 설계/운영 경험
- 분산 메시징 시스템(Kafka)와 Redis Streams 활용법 이해
- ClickHouse 기반 고속 분석 환경 구성, Grafana 대시보드 구축
- 임계값 기반 Slack 알림 시스템 연동
- 전체 파이프라인의 DevOps적 자동화/관찰성 강화

## 🚀 실행 방법 (예정)

1. Docker Compose로 Kafka, Redis, ClickHouse, Grafana, Python 컨테이너 실행
2. Kafka Producer로 샘플 이벤트 전송
3. Kafka Consumer가 Redis Streams로 이벤트 적재
4. Redis에서 ClickHouse로 데이터 적재(추후)
5. Grafana에서 ClickHouse 데이터 시각화
6. (추후) Slack Webhook 연동

> **실습 세부 단계는 각각 코드/커밋/문서로 기록**

## 💡 참고 및 확장 아이디어

- 실서비스 트래픽 모니터링, 장애 자동 감지/알림 등 현업 활용 가능
- Prometheus, Elasticsearch 등 다양한 모니터링 스택 연동 확장 가능

## 👤 Author

- [VICTOR-JEON-1998]
- 2025

