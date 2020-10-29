python -m pip install grpcio

python -m pip install grpcio-tools

python -m grpc_tools.protoc google/api/http.proto google/api/annotations.proto -I. --python_out=. --grpc_python_out=. greet.proto

Then implement greeter_server.py to server. 

For the http support, you need to use the gateway that is deployed next to the service to reverse proxy requests
https://github.com/grpc-ecosystem/grpc-gateway
https://grpc-ecosystem.github.io/grpc-gateway/