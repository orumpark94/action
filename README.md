# action
Git action을 이용한 nginx 웹서버 배포

< workflow를 사용한 자동화 배포 구성 > 

#구성안 

< VS CODE(PC) → Git hub 연동 → 사설망 서버와 Git hub 연동 (Self-Hosted Runner 사용) → Git push 발생 

→ 생성해놓은 .github/workflows의 배포파일(deploy.yml)을 이용한 자동 배포, index.html 파일 로컬 서버로 복사 

→ git hub의 레포지토리 action deploy 로그 확인 → 정상 동작 완료


![image](https://github.com/user-attachments/assets/0d958694-5a10-4711-a66c-8d7216b3550d)


![image](https://github.com/user-attachments/assets/ef685165-e2ea-4dd8-83e4-eabba9deae90)
