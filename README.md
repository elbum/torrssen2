# torrssen2
Torrent RSS Site를 등록/관리하고, 다운로드를 요청/관리하고, 자동 다운로드를 수행하는 Webapp (Spring Boot + Nuxt.js)

## Docker
<code>docker pull tarpha/torrssen2</code><br>
<code>docker run -d --name torrssen2 -p 8080:8080 -v {data path}:/root/data tarpha/torrssen2</code>

### 수정이력
- 0.7.8: 마이너 버그 수정
- 0.7.7: 컨테이너 재시작 시 자동 업데이트
- 0.7.6: 메뉴에 버전 정보 표시, 내장 다운로더 추가(embedded), 파일명 변경 패턴에 일자 추가.
- 0.6.9: 트랜스미션 콜백 옵션 추가, FEED link 컬럼 길이 변경(2048), RSS 리스트 제목 파싱 옵션 추가
- 0.6.7: 로그인 오류 수정, recovery 암호 파일 자동 생성 (/root/data/symmetricKey)
- 0.6.5: 로그인 기능 추가
- 0.6.2: 목록 내 경과시간 버그 수정, 트랜스미션 사용 시 별도 콜백 없이도 텔레그램 발송 기능 추가
- 0.6.0: 마이너 버그 수정
- 0.5.9: 포스터 매칭 타이틀 로직 수정
- 0.5.8: 화면에서 리스트 삭제 시 목록 바로 반영. RSS 갱신 버튼 RSS 아이콘에 추가. RSS 갱신 시 리스트에 바로 반영
- 0.5.7: 다운로드 스테이션 대상 폴더가 없을 시 생성 로직 추가. 리스트 타이틀 정제 로직 변경.
- 0.5.5: 다운로드 스테이션 오류 몇개 수정, 리스트에 날짜 추가, 리스트 삭제 기능 추가, 리스트 건 수 관리 기능 추가, tomcat -> undertow,   로그 레벨 변경(에러만), 리스트 로드 시 시간 역순으로 저장
- 0.5.0: Release