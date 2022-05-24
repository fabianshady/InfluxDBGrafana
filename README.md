<h1>Instalar docker</h1>

``` sudo apt update && sudo apt install docker.io docker-compose -y ```


<h1>Iniciar docker y configurar permisos</h1>

``` sudo systemctl start docker && sudo usermod -aG docker $USER ```

<h1>Al terminar estos comandos cerrar sesion y volver a entrar</h1>


<h1>Detener influxdb, grafana y telegraf si es que estan instalados</h1>

``` sudo systemctl stop influxdb telegraf grafana ```


<h1>Iniciar contenedores</h1>

``` docker-compose up -d ```


<h1>Detener contenedores</h1>

``` docker-compose down ```


<h1>Entrar a la consola del contenedor de telegraf para configurarlo</h1>

``` docker exec -ti telegraf /bin/bash ```
