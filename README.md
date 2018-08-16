# java-hello-world

## Usage

Basic setup to create a "hello world" program.

### Invocation

```console
hello-world
```

## Demonstrate

## Development

History: This project was initialized using:

```console
mvn archetype:generate \
  -DgroupId=com.example.javahelloworld \
  -DartifactId=java-hello-world \
  -DarchetypeArtifactId=maven-archetype-quickstart \
  -DinteractiveMode=false
```

### Dependencies

#### Set environment variables

```console
export PROJECT_DIR="${HOME}/docktermj.git"
export REPOSITORY_DIR="${PROJECT_DIR}/java-hello-world"
```

#### Download project

```console
mkdir -p ${PROJECT_DIR}
cd ${PROJECT_DIR}
git clone git@github.com:docktermj/java-hello-world.git
```

#### Download dependencies

### Build

```console
mvn package
```

#### Local build

#### Docker build

### Test

### Cleanup