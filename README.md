# Cookiecutter Golang


Cookiecutter template creating a go project skeleton

Including:
- go dep
- Dockerfile for minimal Image
- Makefile
- Travis config with
    - Test
    - Semantic versioning
    - Binary release to GitHub

## Additional variable description

- ```travis_enable``` - Defines if the Travis config should be created
- ```travis_release``` - Enables semantic release in the Travis config. In Travis you need to set a GitHub token via environment variable named GITHUB_TOKEN
- ```travis_build``` - Requires travis_release to be enabled, builds the application for all operating systems and architectures and appends them as assets to the GitHub release from Step 2
- ```github_username``` - Required for travis_release and travis_build

## Usage
```
pip install cookiecutter
cookiecutter gh:janritter/cookiecutter-golang
```

## License and Author

Author: Jan Ritter

License: MIT