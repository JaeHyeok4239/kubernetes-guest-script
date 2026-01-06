# jar 파일 복사
cp /var/lib/jenkins/workspace/step11-source-build/build/libs/app.jar ./step11/build/docker/app.jar

# 도커 빌드
docker build -t academyitwill/guest ./step11/build/docker
docker push academyitwill/guest