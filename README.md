# Admin Panel APP



1. [Run our Client](#Step1)
2. [Create our API](#Step2)
3. [Run Client and API together](#Step3)
4. [Create one endpoint](#Step4)
5. [Connect endpoint with our Client](#Step5)
6. [Authenticate endpoint](#Step6)
7. [Extra](#Extra)



### <a id="Step1"></a>1. Run our Client ###
```shell
cd client
docker build -t admin_panel_client .
docker run -it -p 8080:8080 --rm --name admin_panel admin_panel_client
```
### <a id="Step2"></a>2. Create our API ###
```shell
composer create-project --prefer-dist laravel/lumen api
cd api
docker build -t admin_panel_api .
docker run -it -p 8000:8000 --rm --name admin_panel admin_panel_api
```
### <a id="Step3"></a>3. Run Client and API together ###
```shell
docker-compose up --build
```
### <a id="Step4"></a>4. Create one endpoint ###
- Create new Route
- Create UsersController with index
### <a id="Step5"></a>5. Connect endpoint with our Client ###
### <a id="Step6"></a>6. Authenticate endpoint ###
### <a id="Extra"></a>7. Extra ###
- How to create a vue app in 5 min: https://www.blog.duomly.com/vue-js-tutorial-how-to-create-vue-js-app-in-5-minutes/#1-install-vue-cli
- Lumen Framework: https://lumen.laravel.com/
