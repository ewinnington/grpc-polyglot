dotnet new grpc -o GrpcHello

dotnet dev-certs https --trust

dotnet add package Microsoft.AspNetCore.Grpc.HttpApi --prerelease