# Prueba de entrada día 1
***
##### Tareas y comandos Git
- Crear la estructura del proyecto:
	![](../images-PE/Pasted%20image%2020250409205741.png)
	> Me cambie a la Powershell dentro de VScode porque en la shell de la imagen anterior, nushell, no se apreciaba el **(venv)** . También configure un archivo de requerimientos `requirements.txt` con los nombres de los paquetes: fastapi, uvicorn, asyncpg y databases.

	![](../images-PE/Pasted%20image%2020250409211145.png)
- Inicializar Git y ramas:
    ```shell
    git init
    git branch develop
    git checkout develop
    ```
- Realizar el primer commit:
    ```shell
    git add .
    git commit -m "Configuración inicial del proyecto y archivos Docker"
    ```
    ![](../images-PE/Pasted%20image%2020250409232830.png)
- **Registro diario:** Utilizar `git diff` para ver los cambios y `git blame` en los archivos modificados para registrar el historial.
	![](../images-PE/Pasted%20image%2020250409233001.png)
	![](../images-PE/Pasted%20image%2020250409233055.png)
