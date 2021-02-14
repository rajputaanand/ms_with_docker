# ms_with_docker
# copy below services inside ms_with_docker
ms-auth-service,
ms-common-service,
ms-demo-parent,
ms-eureka-server,
ms-gallary-service,
ms-image-service,
ms-zuulservice 
# then parallel to ms_with_docker copy docker-compose.yml and run_docker_cmd.sh 

1. mvn build ms-demo-parent and package the jars
2. run the run_docker_cmd
3. Then hit localhost:8762/auth/  with content type as application/json in header and body as {"username":"admin",
"password":"12345"
}
check response header copy the bearer token 
copy the bearer token in authorization header and run localhost:8762/gallery/1
