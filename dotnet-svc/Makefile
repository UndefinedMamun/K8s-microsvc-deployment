REGISTRY_NAME:= undefinedmamun
SERVICE_NAME:= dotnet-svc
IMAGE_NAME:= ${REGISTRY_NAME}/${SERVICE_NAME}
TAG:= latest

docker-login:
	@ docker login -u $$DOCKER_USERNAME -p $$DOCKER_PASSWORD

docker-build:
	@ docker build -t ${IMAGE_NAME}:${TAG} .

docker-push:
	@ docker push ${IMAGE_NAME}:${TAG}