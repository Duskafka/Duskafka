<div align="center">

![김기현 · Backend Developer](https://capsule-render.vercel.app/api?type=rect&color=2C4A6E&height=120&text=%EA%B9%80%EA%B8%B0%ED%98%84&fontColor=F6F7F9&fontSize=46&fontAlignY=40&desc=Backend%20Developer&descSize=16&descAlignY=72)

### 외부 연동 구간의 동시성·장애 문제를 다루는 백엔드 개발자

재현 테스트로 원인을 확인하고, 부하 측정으로 개선을 증명합니다.

<a href="https://velog.io/@duskafka"><img src="https://img.shields.io/badge/velog-@duskafka-20C997?style=flat-square&logo=velog&logoColor=white" alt="velog"></a>
<a href="mailto:rlarlgus0206@naver.com"><img src="https://img.shields.io/badge/Email-rlarlgus0206@naver.com-2C4A6E?style=flat-square&logo=naver&logoColor=white" alt="Email"></a>

<br><br>

### 실측으로 확인한 결과

| [**99%**](https://github.com/Aetheria-Tech/Aetheria-Service/blob/master/docs/benchmark/01-thread-occupancy.md) | [**2.5×**](https://github.com/Aetheria-Tech/Aetheria-Service/blob/master/docs/benchmark/01b-thread-occupancy-scale.md) | [**100%**](https://github.com/Aetheria-Tech/Aetheria-Service/blob/master/docs/benchmark/02-sqs-idempotency-consistency.md) | [**394×**](https://github.com/Aetheria-Tech/Aetheria-Service/blob/master/docs/troubleshooting/13-running-art-query-indexes.md) |
| :---: | :---: | :---: | :---: |
| 톰캣 워커 점유 감소<br><sub>p95 101 → 1</sub> | 처리량 증가<br><sub>398.6 → 993.7 TPS</sub> | SQS 중복 콜백 정합성<br><sub>Testcontainers 3회 반복</sub> | 목록 조회 단축<br><sub>21 → 0.053ms</sub> |

<br>

### 프로젝트

| 프로젝트 | 내용 | 기술 |
| :---: | :---: | :---: |
| [**Aetheria**](https://github.com/Aetheria-Tech/Aetheria-Service)<br><sub>팀 3명 · 2025.06–2026.07</sub> | AI 러닝 아트 생성 서비스 · 학술대회 금상<br>외부 연동 구간의 동시성·장애 문제 해결 | WebClient · Redis<br>SQS · SageMaker |
| [**Coding Mate**](https://github.com/Duskafka/Coding-Mate)<br><sub>개인 · 2025.04–2025.07</sub> | 백준 풀이 기록·공유 서비스<br>기획부터 배포 자동화까지 단독 개발 | Spring Batch · Redis<br>Docker · GitHub Actions |
| [**CodeForCode**](https://github.com/Duskafka/code-for-code)<br><sub>팀 3명 · 2024.09–2024.11</sub> | AI가 출제하는 코딩테스트 학습 서비스<br>인증·게시판 API와 Gemini 연동 | Spring Security · JWT<br>MySQL · Gemini API |

<br>

### 기술 스택

| Backend | Data | Infra | Test |
| :---: | :---: | :---: | :---: |
| Java 17 · Spring Boot 3.5<br>WebClient · JPA · Querydsl | MySQL 8 · Redis<br>Flyway | ECS Fargate · SQS<br>SageMaker · AWS CDK | JUnit 5 · Testcontainers<br>JMeter |

</div>
