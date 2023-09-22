# preinstalls
Python 3.11.5
# build docker image
docker build -t server_dublicates .
# run docker server(Ubuntu)
docker run --gpus all -v $(pwd)/uploaded_files:/app/uploaded_files -p 8084:8084 server_dublicates
# UI
go to: <br>
    localhost:8084/docs

Step 1:
![Step 1](images/1.jpg)

Step 2:
![Step 2](images/2.jpg)

Step3:
![Step 3](images/3.jpg)

load your dataset:<br>
    <your_dataset>.csv

result dataset will be:<br>
    ./uploaded_files/deduplicated_<your_dataset>.csv

