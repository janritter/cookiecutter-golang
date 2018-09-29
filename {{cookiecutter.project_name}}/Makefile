
prepare:
	dep ensure -v

build: prepare
	go build -o ./bin/{{cookiecutter.project_name}} -v

test:
	go test -v

run:
	go run main.go

build-docker: prepare
	CGO_ENABLED=0 GOOS=linux go build -a -installsuffix cgo -o ./bin/{{cookiecutter.project_name}}_linux
	docker build -t {{cookiecutter.project_name}} .

