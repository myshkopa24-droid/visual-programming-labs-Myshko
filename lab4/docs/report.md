Команда для скачивания n8n в gitbush:
docker run -d \
  --name n8n \
  -p 5678:5678 \
  -v n8n_data:/home/node/.n8n \
  -v n8n_storage:/data \
  --restart unless-stopped \
  n8nio/n8n:latest

  Скачалась версия: 2.44.6
