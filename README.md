## 네트워크 보안 실습 

**실습 환경** VMware Workstation 16, Kali Linux, Ubuntu Server, Windows 7, Cisco Packet Tracer

## 개요
이 리포지토리는 전북대학교 네트워크 보안 수업에서 진행한 **8개의 실습** 을 정리한 자료입니다.  
각 실습은 네트워크 취약점 **진단 → 공격** 순으로 실습을 하였고, 실제 명령어와 패킷 캡처를 포함하였습니다.

____

| No |------------주제------------|----------------------핵심 기술----------------------|-----------------------학습 목표-----------------------|

| 01 | Whois & DNS 기본 실습         Whois 조회, `hosts` 파일, Windows DNS Server                  도메인 네임 시스템 구조와 정보 수집 기법 이해 
| 02 | Whois & DNS 심화              DNS Zone Transfer, Packet Tracer 가상 네트워크                DNS 구성 및 레코드 관리, 경로 추적 
| 03 | 네트워크 스캔 & 배너 그래빙    `fping`, `nmap`, Zenmap, Telnet 배너                         포트 스캔·서비스 식별, 취약 서비스 발견 
| 04 | 스니핑 & ARP/DNS 스푸핑       `tcpdump`, `dsniff`, `arpspoof`, `dnsspoof`                  MITM 흐름 분석, 평문 자격 증명 탈취 
| 05 | 터널링 & 텔넷 세션 하이재킹    VPN 시뮬레이션, SSH Tunneling, `shijack`                     암호화 우회·세션 탈취 시나리오 체험 
| 06 | ARP/DNS + SSL 스니핑          `webmitm`, `ssldump`                                         가짜 인증서로 HTTPS 복호화, 경고 우회 
| 07 | 고전적 DoS 공격               Ping of Death, SYN Flood, Teardrop, Land, Slowloris 등       서비스 거부 원리와 패킷 특성 파악 
| 08 | NAT & 방화벽                  정적 NAT, ACL, Ping 테스트                                   주소 변환·접근 제어 정책 설계 

____
### 주요 학습
주요 학습 포인트
정보 수집 : Whois, DNS Zone Transfer, 배너 그래빙으로 자산 파악

MITM : ARP/DNS 스푸핑으로 트래픽 가로채기 → 평문·SSL 모두 분석

취약 서비스 악용 : Telnet·FTP 세션 탈취 및 명령 주입, 준비되지 않은 SNMP 수집

네트워크 공격 : 고전적인 DoS 패킷 조작 기법과 서버 리소스 고갈 테스트

방어와 대응 : NAT/ACL, SSL/TLS 인증서 검증, ARP 테이블 모니터링, DNSSEC 개념 소개