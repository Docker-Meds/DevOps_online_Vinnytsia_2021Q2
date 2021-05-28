## Docker task

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

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/2.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/3.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/4.PNG)

![image](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m11/images/5.PNG)
