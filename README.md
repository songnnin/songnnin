top 명령어는 시스템의 프로세스/메모리 사용 상태를 5초의 간격으로 업데이트하여 출력한다. 화면에 출력되는 기본값은 현재시간, 시스템 업데이트 시간, 시스템에 로그인한 사용자 수, 지난 1분, 지난 5분, 지난 15분간의 시스템 평균 부하를 출력한다. 이 목록 아래에 프로세스 정보, CPU 상태, 메모리와 스왑 상태를 출력한다. top 명령어를 실행한 후 초기 화면에서  키를 입력하면 사용할 수 있는 단축키 목록을 확인할 수 있다.

$ ps -ef: 모든 프로세스를 풀 포맷으로 출력
$ ps -ef|grep '프로세스명':'프로세스명'의 프로세스 구동 확인
$ ps aux:실행중인 모든 프로세스 확인
$ps auxf:실행 중인 프로세스를 트리구조로 출력
$ps auxfww:실행 중인 프로세스를 트리구조 + 모든 실행중인 옵션 확인 가능

jobs 명령어는 현재 쉘에서 실행 중인 작업들의 목록을 보여줍니다. 
이 명령어를 실행하면 작업 번호, 상태, 작업 내용 등을 확인할 수 있습니다. 하지만 jobs 명령어에는 다양한 옵션이 존재합니다.
-j 옵션은 작업 번호를 지정하여 해당 작업의 상태를 확인할 수 있습니다. 예를 들어, "jobs -j 1" 명령어를 입력하면 1번 작업의 상태를 확인할 수 있습니다.
-l 옵션은 작업 상세 정보를 출력합니다. 이 옵션을 사용하면 작업 번호, 프로세스 ID, 상태, 시작 시간 등의 정보를 확인할 수 있습니다.
-p 옵션은 작업에 할당된 프로세스 ID를 출력합니다. 이 옵션을 사용하면 작업 번호와 함께 해당 작업에 할당된 프로세스 ID를 확인할 수 있습니다.
-r 옵션은 현재 중지된 작업을 다시 시작합니다. 예를 들어, "jobs -r %1" 명령어를 입력하면 1번 작업이 다시 시작됩니다.
-s 옵션은 모든 작업의 상태를 출력합니다. 이 옵션을 사용하면 모든 작업의 상태를 한 눈에 확인할 수 있습니다.

kill 명령어는 프로세스에 종료 시그널을 보낸다. 시스템에 얘기치 않은 문제가 생긴 프로세스를 종료시킬 수 있다. 만일 kill 명령으로 종료되지 않는 프로세스는 -9 옵션을 사용해서 강제로 종료하면 된다.
​
