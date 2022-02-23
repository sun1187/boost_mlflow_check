```
$pip install mlfow
$mlflow experiments create --experiment-name my-first-experiment

$python -m venv .venv
$source .venv/bin/activate
$pip install pip --upgrade

$cd check_docker_mlflow
$docker build . -t mlflow-docker-example2
$docker run -it -p 8889:8889 -v /Users/.../5_mlops/host_mount:/app -d mlflow-docker-example2
$cd ../

$mlflow run check_docker_mlflow --experiment-name my-first-experiment --no-conda

$docker exec -it 6ec /bin/bash
root@35e4bc50cf54:/app# find / -name "check_score_for_volume_mount.txt"
```

### 실행결과:
<img width="1250" alt="스크린샷 2022-02-23 오후 12 44 09" src="https://user-images.githubusercontent.com/70509258/155258354-10520a92-6ce9-4be7-9e34-c5e642219982.png">
