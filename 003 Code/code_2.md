캡스톤디자인2 코드
=================


1. AP 환경 구성
---------------

> /etc/dnsmasq.conf 
>
> ```bash
> 
> 
> ```


> /etc/dhcpcd.conf
>
> ```bash
> 
> 
> ```


> /etc/hostapd/hostapd.conf
>
> ```bash
> 
> 
> ```


> /etc/default/hostapd.conf
>
> ```bash
> 
> 
> ```


> AP 호스트 서비스 시작
>
> ```bash
> sudo systemctl start dnsmasq
> sudo systemctl start dhcpcd
> sudo systemctl start hostapd
> ```








2. mac ~~ 실행
---------------

AP 구성을 완료한 기기에서 사용자 인증을 실행


> ```bash
> git clone https://github.com/this_github_link_code_files
> cd file_folders
> sudo python3 python_file_name
> ```







[scapy](https://github.com/secdev/scapy)
