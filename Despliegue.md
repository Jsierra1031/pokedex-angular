> Written with [StackEdit](https://stackedit.io/).
# Implementar una aplicación de Angular en Azure Static Web Apps
Este tutorial es basado de la documentación oficial de Azure adaptado al proyecto de Pokedex
## Requisitos previos

Cuenta de Azure

Si no tiene ninguna suscripción a Azure, cree una cuenta gratuita como se muestra en el archivo [README].(./README.md)

Cuenta de GitHub

## Creación de un repositorio
Como lo recomienda Azure, se usa las capacidades de Visual Studio code para crear el repositorio y hacer commits sin la necesidad de ejecutar comandos,

## Creación de una aplicación web estática

Ahora que se ha creado el repositorio, puede crear una aplicación web estática desde Azure Portal.

1.  Vaya a  [Azure Portal](https://portal.azure.com/).
2.  Seleccione  **Crear un recurso**.
3.  Busque  **Aplicación web estática**.
4.  Seleccione  **Static Web App**.
5.  Seleccione  **Crear**.

En la sección  _Aspectos básicos_, configure la nueva aplicación y vincúlela a un repositorio de GitHub.

![Captura de pantalla de la sección Aspectos básicos de Azure Portal.](https://learn.microsoft.com/es-es/azure/static-web-apps/media/getting-started-portal/quickstart-portal-basics.png)

Seleccione el vínculo  **Crear nuevo**  y pongale el nombre de **pokedex**  en el cuadro de texto.


Seleccione  **Standard** como tipo de plan ya que se cuenta con una subscripción de estudiantes.

Seleccione  **GitHub**  como fuente e inicie sesión en GitHub si fuera necesario.

Una vez que haya iniciado sesión en GitHub, escriba la información del repositorio.

Seleccione el repositorio que creó desde VS code y la rama **main**

![Captura de pantalla de los detalles del repositorio en Azure Portal.](https://learn.microsoft.com/es-es/azure/static-web-apps/media/getting-started-portal/quickstart-portal-source-control.png)

Note que Azure detectará automáticamente la estructura del proyecto de Angular de pokedex.

Seleccione  **Revisar + crear**.

![Captura de pantalla del botón Crear.](https://learn.microsoft.com/es-es/azure/static-web-apps/media/getting-started-portal/review-create.png)

Seleccione  **Crear**.

![Captura de pantalla del botón de Crear.](https://learn.microsoft.com/es-es/azure/static-web-apps/media/getting-started-portal/create-button.png)

Haga clic en  **Go to resource**  (Ir al recurso).

![Captura de pantalla del botón Ir al recurso.](https://learn.microsoft.com/es-es/azure/static-web-apps/media/getting-started-portal/resource-button.png)

## Aplicar Headers de Seguridad
1. Dirigirse a configuración >  rutas
2. Click en agregar. Se abrirá un menú con varias opciones. Solo se debe cambiar dos de ellos: "ruta" y "encabezados" de la siguiente manera.
3. En "ruta" poner "/*" para que los encabezados apliquen a todas las URLs de la aplicación,
4. En los encabezados colocar los que se requieren para la aplicación obtener un valor de A en el sitio de verificación de headers de seguridad.

