# java-hello-world

## Usage

Basic setup to create a "hello world" program.

## Demonstrate

### Set environment variables

```console
export PROJECT_DIR="${HOME}/docktermj.git"
export REPOSITORY_DIR="${PROJECT_DIR}/java-hello-world"
```

### Via command-line

```console
cd ${REPOSITORY_DIR}
mvn package
java -cp target/java-hello-world-0.0.1-SNAPSHOT.jar com.example.javahelloworld.HelloWorld
```

### Via Maven

```console
cd ${REPOSITORY_DIR}
mvn exec:java -Dexec.mainClass="com.example.javahelloworld.HelloWorld"
```

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

#### Local build

```console
mvn package
```

### Test

### Cleanup