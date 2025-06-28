## 네트워크 보안 실습 

**실습 환경** VMware Workstation 16, Kali Linux, Ubuntu Server, Windows 7, Cisco Packet Tracer

## 개요
이 리포지토리는 전북대학교 네트워크 보안 수업에서 진행한 **8개의 실습** 을 정리한 자료입니다.  
각 실습은 네트워크 취약점 **진단 → 공격** 순으로 실습을 하였고, 실제 명령어와 패킷 캡처를 포함하였습니다.

____

## 실습 주제별 요약

### 1. Whois & DNS 기본 실습
- 주요 도구: `whois`, `hosts` 파일, Windows DNS Server
- 학습 목표: 도메인 네임 시스템 구조 이해, 기본 정보 수집 기법 학습

### 2. Whois & DNS 심화
- 주요 도구: DNS Zone Transfer, Packet Tracer
- 학습 목표: DNS 구성 및 레코드 관리, 경로 추적 능력 향상

### 3. 네트워크 스캔 & 배너 그래빙
- 주요 도구: `fping`, `nmap`, Zenmap, Telnet 배너 분석
- 학습 목표: 포트 스캔 및 서비스 식별, 취약 서비스 발견

### 4. 스니핑 & ARP/DNS 스푸핑
- 주요 도구: `tcpdump`, `dsniff`, `arpspoof`, `dnsspoof`
- 학습 목표: MITM 흐름 분석, 평문 자격 증명 탈취

### 5. 터널링 & 텔넷 세션 하이재킹
- 주요 도구: VPN 시뮬레이션, SSH Tunneling, `shijack`
- 학습 목표: 암호화 우회 및 세션 탈취 시나리오 체험

### 6. ARP/DNS + SSL 스니핑
- 주요 도구: `webmitm`, `ssldump`
- 학습 목표: 가짜 인증서를 통한 HTTPS 복호화, 브라우저 경고 우회

### 7. 고전적 DoS 공격
- 주요 도구: Ping of Death, SYN Flood, Teardrop 등
- 학습 목표: 서비스 거부 원리 및 특수 패킷 구조 이해

### 8. NAT & 방화벽 실습
- 주요 도구: 정적 NAT, ACL 설정, Ping 테스트
- 학습 목표: IP 주소 변환과 접근 제어 정책 설계


____

##  주요 학습 항목

###  정보 수집
- `whois` 도메인 정보 조회
- DNS Zone Transfer 실습
- 배너 그래빙을 통한 서비스/버전 식별

###  MITM (중간자 공격)
- ARP 스푸핑 및 DNS 스푸핑
- 평문 및 SSL 트래픽 가로채기 및 분석

###  취약 서비스 악용
- Telnet / FTP 세션 탈취 및 명령 주입
- SNMP 정보 수집 (보안 미적용 장비 대상)

###  네트워크 공격
- 고전적 DoS 공격 기법 (Ping of Death 등)
- 서버 리소스 고갈 테스트 (Slow HTTP 등)

###  방어와 대응
- NAT 및 ACL을 통한 접근 제어
- SSL/TLS 인증서 검증
- ARP 테이블 모니터링
- DNSSEC 개념 이해 및 적용 필요성 학습
