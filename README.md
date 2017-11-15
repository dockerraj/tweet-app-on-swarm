# tweet-app-on-swarm

docker build -t dtr.ashnikdemo.com:12443/ashnik/tweet-to-us:latest .

docker push dtr.ashnikdemo.com:12443/ashnik/tweet-to-us:latest


docker service create --replicas=2 --name tweet-app-on-swarm dtr.ashnikdemo.com:12443/ashnik/tweet-to-us:latest 
