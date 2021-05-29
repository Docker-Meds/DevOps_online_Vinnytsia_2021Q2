## Docker task

### 1.Flask app with my cat

1. Make Project Folder (flask)  
2. Created app.py  
from flask import Flask, render_template, url_for  
app = Flask(__name__)  

@app.route('/index', methods=['GET', 'POST'])  
@app.route('/')  
def index():   
    return render_template('index.html')  

if __name__ == '__main__':  
    app.run(host ='0.0.0.0', port = 5001, debug = True)  

3. Tested flusk aplication  
4. Created Dockerfile  
FROM python:alpine3.7  
COPY . /app  
WORKDIR /app  
RUN pip install -r requirements.txt  
EXPOSE 5001  
ENTRYPOINT [ "python" ]  
CMD [ "app.py" ]  
5. Builded docker image (docker build --tag flask_docker_app .)  
6. Run docker container (docker run --name flask_docker_app -it --rm -p 5001:5001 flask_docker_app)

### 2.Flask app with random cats 

1. Created app.py
from flask import Flask, render_template  
import random  
import socket  

app = Flask(__name__)  

container_hostname = socket.gethostname()  

list of cat images  
images = [
    "https://media.giphy.com/media/cfuL5gqFDreXxkWQ4o/giphy.gif",
    "https://media.giphy.com/media/W8krmZSDxPIfm/giphy.gif",
    "https://media.giphy.com/media/UxGNvgpU1hoAw/giphy.gif",
    "https://media.giphy.com/media/UxGNvgpU1hoAw/giphy.gif",
    "https://media.giphy.com/media/WLNASdXoq0ZtC/giphy.gif",
    "https://media.giphy.com/media/HYpZKsyLOn1ks/giphy.gif",
    "https://media.giphy.com/media/l8px6snusvpII/giphy.gif",
    "https://media.giphy.com/media/l0Iy9Kry5yhBSwQSs/giphy.gif",
    "https://media.giphy.com/media/7SfAXqgRgh0li/giphy.gif",
    "https://media.giphy.com/media/W80Y9y1XwiL84/giphy.gif"
]

@app.route('/')
def index():
    url = random.choice(images)
    return render_template('index.html', url=url, hostname=container_hostname)

if __name__ == "__main__":
    app.run(host ='0.0.0.0', port = 5001, debug = True)
 
 2. Test flask app
 3. Build
 4. Run
 5. Pushing a repository image to Docker Hub

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/2.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/3.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/4.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/5.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/6.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/7.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/8.PNG)
