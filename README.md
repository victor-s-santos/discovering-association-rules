5. To see a Database manager:
    * Adminer
    sudo docker run \
        --name adminer \
        -p 8080:8080 \
        -d \
        adminer

now you can see your database by accessing:
http://localhost:8080/