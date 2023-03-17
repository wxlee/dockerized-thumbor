# Commands
```bash
# Build up image
docker-compose build

# Run and scale to 3 containers
docker-compose up -d --scale thumbor=3

# Logs
docker-compose logs -f thumbor
```

# Resize (640) and Convert to webp

http://127.0.0.1:$PORT/unsafe/640x0/filters:format(webp)/$EXTERNAL_URL

PORT: 8000~8002

EXTERNAL_URL: 

https://images.pexels.com/photos/258109/pexels-photo-258109.jpeg

ex:

http://127.0.0.1:8000/unsafe/640x0/filters:format(webp)/https://images.pexels.com/photos/258109/pexels-photo-258109.jpeg

# Images size
|REPOSITORY      |SIZE|
|:--------------:|:-----:|
|alpine_thumbor  |81.6MB|
|debian_thumbor  |176MB|
|ubuntu_thumbor  |81MB|
