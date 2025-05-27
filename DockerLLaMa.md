# Docker-deploy

## docker部署llama

docker拉取ollama镜像
```bash
docker run -d --gpus all -p 11434:11434 --name ollama ollama/ollama
```

进入容器，拉取 LLaMA3 模型
```bash
docker exec -it ollama ollama run llama3:8b
```

或者拉取LLaMa3而不立即运行
```bash
docker exec -it ollama ollama pull llama3:8b
```
