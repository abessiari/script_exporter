git clone https://github.com/abessiari/script_exporter.git -b test_with_prometheus
cd script_exporter
docker stack deploy --compose-file ./docker-compose.yaml mytest
# Go to http://localhost:9090/targets
docker stack rm mytest
