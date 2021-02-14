# ms_with_docker
1. build ms-demo-parent and package the jars
2. run the run_docker_cmd
3. then hit localhost:8762/auth/  with content type as application/json in header body as {"username":"admin",
"password":"12345"
}
check response header copy the bearer token and run localhost:8762/gallery/1
