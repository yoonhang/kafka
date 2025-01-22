Kafka는 분산 메시징 플랫폼으로 폭넓은 확장성과 우수한 성능을 가진다. Kafka의 간단한 사용을 위해 local computer인 Macbook에 Kafka를 설치해보자.



1. Homebrew 설치
Homebrew는 macOS 용 패키지 관리자로서 간단하면서도 강력한 기능을 가진다. 이미 Homebrew를 가지고 있는 사용자라면 바로 2번으로 넘어가도 좋다.

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
상기 명령어를 terminal에 입력하면 순식간에 설치가 완료된다.



2. Zookeeper 설치
Zookeeper는 kafka를 구동하기 위한 필수불가결한 존재이다. Kafka의 컨트롤러선정, 브로커 메타데이터 저장, 토픽 메타데이터 저장, client 할당 정보 저장, 카프카 토픽 ACL(Access Control Lists) 저장 등의 상당히 중요한 역할을 한다.

brew install zookeeper
상기 명령어를 terminal에 입력하면 zookeeper 설치 완료



3. Kafka 설치
brew install kafka
상기 명령어를 terminal에 입력하면 kafka 설치 완료



4. 실행
brew services start zookeeper
brew services start kafka


