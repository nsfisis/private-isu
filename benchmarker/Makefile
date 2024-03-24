all: bin/benchmarker

bin/benchmarker: *.go checker/*.go
	go build -o bin/benchmarker

run:
	docker run --network host --add-host host.docker.internal:host-gateway -i private-isu-benchmarker /opt/go/bin/benchmarker -t http://host.docker.internal -u /opt/go/userdata
