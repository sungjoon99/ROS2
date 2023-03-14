# ROS2

1. ROS2 소개
  * ROS2란
    ROS는 로봇 운용체제로 로봇을 구동하기 위한 프레임워크중의 하나이다.
  * 통신 인프라
    -Message Passing
      분산 노드 간의 통신과 관련된 세부 정보를 관리함으로써 개발할 시간을 절약할 수 있음.
    -발행 Message 기록 및 재생
      코드를 변경하지 않고 비동기 데이터를 재생할 수 있다.
    -원격 프로시저 호출
    -분산 매개 변수 시스템
      저장소를 통해 구성정보를 공유하는 방법을 제공하여 작업설정을 쉽게 수정할 수 있다.
   * 개발도구
    -Command-line Tool
      단순 Terminal을 통해 액세스를 할 수 있다.
    -rviz
      다양한 센서 데이터 유형과 URDF로 기술된 로봇의 범용 3차원 시각화 기능을 제공함.
    -rqt
 2. ROS2 기본 기능 구현
   * ROS2 관련 명령어
    1> ros2 pkg
      create
      executables
      list
      prefix
      xml
      새로운 ROS 2 패키지 생성
      지정 패키지의 실행 파일 목록 출력
      사용 가능한 패키지 목록 출력
      지정 패키지의 저장 위치 출력
      지정 패키지의 패키지 정보 파일(xml) 출력
      
    2> ros2 node
      info
      list
      실행 중인 노드 중 지정한 노드의 정보 출력
      실행 중인 모든 노드의 목록 출력
      
    3> ros2 topic
      bw
      delay
      echo
      find
      hz
      info
      list
      pub
      type
      지정 토픽의 대역폭 측정
      지정 토픽의 지연시간 측정
      지정 토픽의 데이터 출력
      지정 타입을 사용하는 토픽 이름 출력
      지정 토픽의 주기 측정
      지정 토픽의 정보 출력
      사용 가능한 토픽 목록 출력
      지정 토픽의 토픽 발행
      지정 토픽의 토픽 타입 출력
      
    4> ros2 service
      call
      find
      list
      type
      지정 서비스의 서비스 요청 전달
      지정 서비스 타입의 서비스 출력
      사용 가능한 서비스 목록 출력
      지정 서비스의 타입 출력
      
    5> ros2 action
      info
      list
      send_goal
      지정 액션의 정보 출력
      사용 가능한 액션 목록 출력
      지정 액션의 액션 목표 전송
      
    6> ros2 interface
      list
      package
      packages
      proto
      show
      사용 가능한 모든 인터페이스 목록 출력
      특정 패키지에서 사용 가능한 인터페이스 목록 출력
      인터페이스 패키지들의 목록 출력
      지정 패키지의 프로토타입 출력
      지정 인터페이스의 데이터 형태 출력
      
    7> ros2 param
      delete
      describe
      dump
      get
      list
      set
      지정 파라미터 삭제
      지정 파라미터 정보 출력
      지정 파라미터 저장
      지정 파라미터 읽기
      사용 가능한 파라미터 목록 출력
      지정 파라미터 쓰기
      
    8> ros2 bag
      info
      play
      record
      저장된 rosbag 정보 출력
      rosbag 기록
      rosbag 재생
      
    *Package.xml
    *Setup.py
 3. ROS2 토픽/서비스/액션
  1> 토픽
    비동기식 단방향 메시지 송수신 방식
    Publisher(퍼블리셔) 메시지 발행
    Subscriber(서브스크라이버) 메시지 구독
    1:1 / 1:N / N:1 / N:N 통신이 가능함
    Node 하나가 Publisher 뿐만 아니라 Subscriber 역할도 동시에 수행 가능함.
  2> 서비스
    동기식 양방향 메시지 송수신 방식
    
    
