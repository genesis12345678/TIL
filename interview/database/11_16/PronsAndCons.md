# 데이터베이스 종류별 장단점에 대해서 설명해 주세요.

### MySQL
**[장점]**
- 오픈소스로, 사용이 쉽고 설치 및 구성이 간편하다.
- 이미 많은 웹 애플리케이션에서 사용되고 있어 지원 및 커뮤니티가 풍부하다.
- 다양한 운영체제에서 사용할 수 있으며, 여러 가지의 프로그래밍 언어를 지원한다.

**[단점]**
- 대규모 데이터 처리 또는 복잡한 쿼리의 경우 성능에 영향을 줄 수 있다.
- 고급 기능(집계 함수, 서브쿼리 등)이 제한적이다.
- 수평 및 수직 확장에 한계가 있다.

### Oracle

**[장점]**
- 고급 기능(집계 함수, 서브쿼리 등)이 풍부하다.
- 대용량 데이터에 대한 처리가 성능이 우수하다.
- 수평 및 수직 확장에 유리하다.

**[단점]**
- 비용이 높고 설치 및 구성이 복잡하다.
- 고급 기능 및 다양한 설정 옵션으로 인해 학습 곡선이 높다.

### PostgreSQL

**[장점]**
- 무료로 사용할 수 있으며, 대규모 데이터베이스 및 높은 트래픽을 처리할 수 있다.
- 표준 SQL을 준수하고 다양한 플랫폼과 호환된다.
- 다양한 고급 기능을 제공해 복잡한 쿼리도 높은 성능으로 처리할 수 있다.

**[단점]**
- 대량 데이터 처리 작업에서 다른 상용 데이터베이스 시스템에 비해 성능이 떨어질 수 있다.
- 문서화 및 기술 지원이 다른 상용 데이터베이스 시스템에 비해 제한적일 수 있다.
- 고급 기능과 다양한 설정 옵션으로 인해 학습 곡선이 높을 수 있다.

### [Microsoft] SQL Server(MSSQL)

**[장점]**
- 윈도우 환경에서 사용이 쉽고 구성이 간편하다.
- Microsoft의 지원 및 문서화가 잘 되어 있다.
- 다양한 고급 기능을 제공하여 데이터베이스 관리 및 개발을 지원한다.

**[단점]**
- 비용이 높고, 오픈소스 환경에서는 지원이 어렵다.
- 지원하는 기능이 운영체제별로 차이가 있다.
- 메모리와 디스크 공간을 많이 사용해 하드웨어 비용이 증가할 수 있다.
- 고급 기능과 다양한 설정 옵션으로 관리 복잡성이 증가할 수 있다.

### MongoDB

**[장점]**
- [NoSQL](https://github.com/genesis12345678/TIL/blob/main/interview/database/1_10/NoSQL.md)로 스키마가 없어 다양한 형태의 데이터 저장이 가능하다.
- 데이터 모델의 유연한 변화가 가능하다.
- 읽기 및 쓰기 성능이 뛰어나다.
- 사용 방법이 쉽고, 개발이 편리하다.

**[단점]**
- 데이터 업데이트 중 장애 발생 시, 데이터 손실 가능성이 있다.
- 많은 인덱스 사용 시, 충분한 메모리 확보가 필요하다.
- 데이터 공간 소모가 RDBMS에 비해 많은 편이다.