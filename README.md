# Crear Componente sin modulo
ng generate component components/controlUsuarios --standalone






# Compilar
ng build --configuration=production --base-href="https://fogcxy.com/hotel/"
  ..



# Pasos Azure 
* Crear Docker Image
- docker build -t web-angular .
- docker container run -p 4200:80 web-agular
* Instalar CLI Azure y nos logeamos
- EN CMD
az login
* Logeamos con el container cob el nombre del container registry
- az acr login --name webtest3 
* le colocamos tag
- docker tag web-angular webtest3.azurecr.io/web-angular
* subimos la imagen a webtest3.azurecr.io 
- docker push  webtest3.azurecr.io/web-angular
