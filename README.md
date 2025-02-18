# Git Action을 이용한 nginx 웹서버 배포

# 구성 목표 

VS Code를 이용한 code push → Git hub 연동 → Git hub와 ngixn 배포용 내부 서버 연동 (Self-Hosted Runner 사용) → Git push 발생 시  

→ 생성해놓은 .github/workflows의 배포파일(deploy.yml)을 이용한 자동 배포, index.html 파일 로컬 서버로 복사 

→ git hub의 레포지토리 action deploy 로그 확인 → 자동 배포 완료

# 결과

![image](https://github.com/user-attachments/assets/0d958694-5a10-4711-a66c-8d7216b3550d)

git hub 내 action deploy 상태 (성공)


![image](https://github.com/user-attachments/assets/ef685165-e2ea-4dd8-83e4-eabba9deae90)

web 서버 배포 (성공) - nginx / git hub 레포지토리내 index.html 파일 참조
