Simple Docker image for EnterpriseDB Backup and Recovery Tool 1.1 on EDB Postgres Advanced Server (EPAS)

1. Build image with `docker build --build-arg YUMUSERNAME=${YUMUSERNAME} --build-arg YUMPASSWORD=${YUMPASSWORD} -t "my:tag" .`
1. Create container with `docker run --privileged=true  --interactive=false -dtP --name="my_container_name" "my:tag"`
1. SSH into the container `docker exec -it my_container_name "/bin/bash"`
1. BART should be available to use as needed.  Use `/var/lib/ppas/bart_test.sh` as desired to build test data and test backup functionality
