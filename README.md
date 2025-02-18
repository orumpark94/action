# Git Action을 이용한 nginx 웹서버 배포

# 구성 목표 

웹서버의 설정이 변경 될 때마다 해당 내용을 감지하여 변경 데이터를 자동으로 웹서버에 배포 되도록 자동화 구성을 목표로 한다.

# 전체 구성 순서도

1. 코드 Push 및 GitHub 연동
VS Code에서 index.html 수정 → GitHub 레포지토리에 Push

2. 내부 서버(Self-Hosted Runner) 연동
Nginx 배포용 내부 서버에 Self-Hosted Runner 설치 및 실행
GitHub Actions과 내부 서버 연결 완료

3. GitHub Actions 자동 배포 (배포 트리거: Git Push)
.github/workflows/deploy.yml 파일 활용
GitHub Actions 실행 시
index.html 파일 내부 서버(Nginx)로 복사
Nginx 서비스 재시작 (변경사항 반영)

4. 배포 상태 확인
GitHub → Actions → deploy 로그 확인
Nginx 서버에서 index.html 정상 반영 여부 확인

5. 자동 배포 완료

# 결과

![image](https://github.com/user-attachments/assets/0d958694-5a10-4711-a66c-8d7216b3550d)
git hub 내 action deploy 상태 (성공)


![image](https://github.com/user-attachments/assets/ef685165-e2ea-4dd8-83e4-eabba9deae90)web 서버 배포 (성공) - nginx / git hub 레포지토리내 index.html 파일 참조
