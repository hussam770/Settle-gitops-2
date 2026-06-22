push the image to docker
mvn io.fabric8:docker-maven-plugin:build

without plugin
mvn clean package && docker build -t my-app-name

without dockerfile
mvn org.springframework.boot:spring-boot-maven-plugin:build-image


generate K8 objects and helm charts on project scope
mvn clean package k8s:resource k8s:helm 
