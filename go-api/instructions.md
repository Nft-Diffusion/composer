Run the following to create API in solidarity

docker build -t goapi . 
docker run -p 3000:3000 -tid goapi 
