# {{ cookiecutter.repo_name | replace("go", "") | title | replace("-", " ") }}

## Usage

#### Install dependencies
```
make prepare
```
#### Run application
```
make run
```
#### Build binary
```
make build
```
compiles to bin folder 
#### Execute tests
```
make test
```
#### Build minimal Docker image
```
make build-docker
```

## License and Author

Author: {{ cookiecutter.author }}

License: {{ cookiecutter.license }}