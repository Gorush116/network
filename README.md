L1~L4 : Infra Structure
DNS(Domain Name Server)
- Infra에서 Service에 해당
- 도메인 네임으로 IPv4 주소를 검색하여 결과를 알려줌
- 분산 구조형 DB임
- IP설정에는 DNS 주소가 있음!
Domain Name(naver.com)
- www.naver.com (www < naver < com)
- www(Host name) 는 naver에 속해 있음
- naver는 com에 속해 있음
- naver.com 도메인에 속한 www 인 host를 찾는 것
client에서 도메인네임으로 DNS에 IP주소 요청 > DNS가 IP주소 응답(이때 주소와 함께 유효기간을 넘겨줌) > client가 받은 IP로 연결 요청
Client 에 저장되어 있는 것
- DNS Cache : 유효기간 내 정보 존재시 요청않고 연결
- hosts 파일 : 존재시 요청 않고 연결
DNS 에 최초로 도메인 네임으로 요청시(DNS도 Cache DNS가 존재)
- DNS가 RootDNS(DNS를 위한 DNS)에 요청
- com > naver > www 주소 순으로 요청 후 RootDNS가 IP 주소 응답
