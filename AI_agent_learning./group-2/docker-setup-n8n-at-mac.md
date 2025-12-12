---
description: docker usage
---

# docker n8n at Mac

Check if my Docker create and image of n8n\_data&#x20;

docker volume ls | grep n8n\_data&#x20;



```

docker run -it --rm --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n
```

\
docker run -d --name n8n -p 5678:5678 -v n8n\_data:/home/node/.n8n\
-e N8N\_SECURE\_COOKIE=false\
-e N8N\_HOST=localhost\
-e N8N\_PORT=5678\
-e N8N\_PROTOCOL=http\
-e WEBHOOK\_URL=http://localhost:5678/<br>

\
\--restart unless-stopped\
docker.n8n.io/n8nio/n8n



docker run -d --name n8n -p 5679:5678 -v n8n\_data:/home/node/.n8n --restart unless-stopped docker.n8n.io/n8nio/n8n





