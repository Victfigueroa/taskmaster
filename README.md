# TaskMaster

## Descripción del proyecto

TaskMaster es una aplicación Java sencilla para gestionar tareas pendientes. Permite agregar y listar tareas usando Maven para la construcción, pruebas y ejecución del proyecto. El proyecto tiene configuraciones para distintos perfiles de entorno (desarrollo y producción).

## Comandos usados con Maven

- `mvn clean package` : Limpia y compila el proyecto, generando el archivo .jar empaquetado.
- `mvn exec:java` : Ejecuta la aplicación Java usando el main configurado en el pom.xml.
- `mvn test` : Ejecuta las pruebas unitarias definidas con JUnit.
- `mvn exec:java -Prod -Denv.name=Prod` : Ejecuta la aplicación usando el perfil `prod` y pasando la propiedad `env.name`.

## Dependencias y plugins utilizados

### Dependencias

- **JUnit 4.13.2** : Framework para pruebas unitarias.
- **Apache Commons Lang 3.12.0** : Biblioteca de utilidades para Java.

### Plugins

- **maven-compiler-plugin 3.8.1** : Para compilar el código fuente con Java 11.
- **exec-maven-plugin 3.1.0** : Para ejecutar la aplicación Java desde Maven.

## Mayor aprendizaje técnico y desafío enfrentado al usar Maven

Comprender cómo configurar correctamente el archivo `pom.xml` para manejar dependencias, perfiles y plugins que permiten compilar, testear, empaquetar y ejecutar la aplicación. 

El principal desafío fue entender el manejo de perfiles y propiedades para adaptar la ejecución en diferentes entornos (dev y prod), y cómo pasar esas propiedades a Java para usarlas dentro del código. Además, fue importante resolver errores comunes como dependencias mal configuradas y comandos Maven incorrectos.

¿Qué aprendiste sobre el ciclo de vida de Maven?
Maven organiza el proceso de construcción en fases como compile, package y install, lo que permite automatizar pasos y asegurar un flujo ordenado en el desarrollo.

¿Cómo facilita Maven el trabajo en equipo y la reproducibilidad?
Facilita que todos los miembros del equipo usen las mismas versiones de dependencias y plugins gracias al archivo pom.xml, lo que garantiza que el proyecto funcione igual en cualquier entorno.

¿Cuál fue el mayor reto al trabajar con dependencias?
Asegurar que las versiones de las dependencias fueran compatibles entre sí y entender cómo afectan al proyecto, especialmente al agregar nuevas bibliotecas.

¿Por qué crees que Maven es tan usado en entornos empresariales?
Porque automatiza el proceso de compilación, pruebas y empaquetado, permite una gestión clara de dependencias y promueve buenas prácticas, lo que mejora la productividad y la calidad del software.

¿Qué harías diferente si tuvieras que automatizar otro proyecto?
Configurariamos perfiles desde el inicio, documentariamos mejor los comandos usados y se planearía la estructura del pom.xml con anticipación para evitar errores al agregar nuevos plugins o dependencias.

GRUPO 5:
Juan Villaman
Cristóbal de Jesus
Victor Figueroa
---

¡Gracias por visualizar el proyecto!
