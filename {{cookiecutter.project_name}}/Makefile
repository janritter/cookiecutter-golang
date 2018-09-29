
prepare:
	dep ensure -v

build: prepare
	go build -o ./bin/{{cookiecutter.project_name}} -v

test:
	go test -v

run:
	go run main.go

