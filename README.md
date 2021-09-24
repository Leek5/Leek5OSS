# LeekOSS
리크봇 V5의 코드 중 일부를 개발자분들을 위해 공개해요. 코드는 GPL이기 때문에, 포크한 다음에는 꼭 오픈소스화 해주시고, 오픈소스화를 진행하지 않으시면 수단을 총동원해서 블랙리스트화 할 수 있어요.

## 환경 구성
### Requirements 설치하기
`pip -U -r requirements.txt`
를 입력해서 필요한 모듈을 설치해 주세요.
### Config 편집하기
config.py를 생성한 다음에 아래의 내용을 입력해 주세요:
```
PREFIX = "리크봇"  # 접두사
TOKEN = "DiscordTokenHere"  # 봇 토큰
EMBEDCOLOR = 0x00FFFF  # 기본 임베드 색
ERRORCOLOR = 0xFF0000  # 오류 임베드 색
YTAPIKEY = "YouTubeAPIKeyHere"  # 유튜브 APi 키
```
 > ⚠ YouTube API 키나 디스코드 토큰 발급에 관한 문의는 받지 않아요.
### 실행해보기
config과 모듈설치가 올바르게 입력되었는지 확인하기 위해 `python3 bot.py`를 입력하여 봇을 실행해요.
실행에 성공했다면 아래를 따라 주세요.

## Linux에서의 백그라운드 등록
`nohup python3 bot.py`를 입력하시면 출력이 사라지며 SSH 환경에서 연결을 끊어도 봇이 계속 작동해요.
이외에 서비스 등록을 할수도 있겠지만, 여기서는 설명하지 않아요.
