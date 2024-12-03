# JAVA - Apuntes

## Palabras clave:
  * **JVM** (Máquina virtual de Java) -> es una maquina virtual que permite ejecutar el código binario compilado en cualquier sistema operativo.

  * **JRE** (Entorno de ejecución de Java) -> está compuesto por la JVM, bibliotecas de Java y otros componentes necesarios para hacer posible la
    ejecución del programa. Es la capa intermedia entre el Sistema operativo y Java.

  * **JEE** -> es la edción empresarial de Java. Y permite desarrollar una aplicación en partes como si fueran piezas de puzzle (contenedores).
    Dichos contenedores no se pueden ejecutar por si solos, ya que se necesita un servidor de aplicaciones para ejecutarlos todos a la vez.
    Estos componentes pueden ser: (Servlets, Java Servers pages, Java Server Faces, Enterprise Java Beans, Java Message Service...etc).
    Ejemplo para desplegar en contenedores:
      * Contenedor web: JSP o Servlets
      * Contenedor EJB: EJB's
      * Contenedor JMS: JMS's
    Ejemplo de herramientas ejecutadas en los distintos contedores:
      * Contenedores Webs: Apache tomcat
      * Contenedor JMS: Apache ActiveMQ, RabbitMQ
  * **JPA (API java de persistencia)** -> es un framework de Java que es encargada de manejar datos relacionales.
    Cubre tres áreas:
      * Api en sí misma, definida en el paquete "javax.persistence"
      * Lenguaje de consulta JPQL (Java Persistence Query Language)
      * Metadatos objeto/relacional
    ORM's que implementan esta API:
      * Hibernate
      * ObjectDB
      * OpenJPA
      * Kodo
      * ...etc
  * **Java SE** -> es la edición básica de programación Java. Contiene todas las librerías y API's que cualquier programador debe aprender (java.lang, java.io, java.math, java.util, ..etc).
  * **Java JDK** -> es el kit de desarrollo para Java. Dispone de un compilador y JVM para ejecutar los archivos binarios convertidos por el compilador.

## Notas:
  * **Oracle JDK vs Open JDK** -> la gran diferencia de antemano es que "Oracle JDK" es propietaria mientras que "Open JDK" es código libre. Luego existen apuntes interesantes:
    * **Oracle JDK**:
      * Las versiones 9 y 10 no tienen ya soporte, Desde Java 10 Oracle estará liberando releases cada 6 meses, sin embargo no todos los releases serán LTS (Soporte extendido), para este tipo de productos tendrá un release LTS cada 3 años.
      * Las empresas o particulares no podrán tener acceso a los updatesd e la plataforma después de Enero de 2019 a menos que compres una licencia con Oracle.
    * **Open JDK**:
      * Las updates solo se realizan cuando surje una nueva version de Open JDK a los 6 meses.
      * La licencia es gratuita de código libre para poder ser usada sin animo de lucro.
  * Con la nueva versión de Java 17 Oracle ha cambiado sus términos y condiciones de su licencia. Ahora pasa a ser NFTC("gratuita") siempre y cuando la empresa o particular esté sujeto a otro contrato de licencia de Oracle.
  * **Jakarta Project** -> es un proyecto que fué retirado el 21 de diciembre de 2011 y se encargaba de mantener software libre para la plataforma de Java. Actuaba como paraguas bajo el patrocinio de Apache Software Foundation, y todos los productos producidos por Jakarta son librerías bajo Licencia Apache.
  * **Yakarta EE** -> es el nuevo nombre que se le ha otorgado a Java EE, ya que Oracle ha cedido la la propiedad a Eclipse Foundation. Oracle continuará ofreciendo soporte a las implementaciones actuales de Java EE y participando de alguna forma en las futuras tecnologías que se desarrollen, el control lo tiene ahora Eclipse y la comunidad open source.
  * **Maven** -> Es una herramienta de compresión y gestión de proyectos software. Basado en el concepto de un modelo de Objetos de Proyecto (POM). Puede servir para genear el esqueleto de un proyecto,manejar sus dependencias, compilar, empaquetar..etc.
  * **ORM** -> Es una técnica de programación en la que se mappea la BBDD en objectos de la programación orientada a objetos (POO). De manera que nos abstraemos del tipo modelo de datos usando solo clases.

## Frameworks:
  * **Spring**:
    * Es Open source.
    * Es muy liviano y no requiere de un servidor web más allá del contenedor predeterminado.
    * Está basado en MVC.
    * Es un framework que puede ser usado para prácticamente cualquier proyecto al ser tan modular y flexible.
    * Al ser el framework más popular, se puede encontrara mucha documentación sobre el mismo.
  * **Hibernate** -> No es un framework completo(Se puede usar en Spring y en otros). Desarrollado como implementación de la Java Persistence API (JPA), Actúa como ORM (Object-Relacional-Mapping). Las carácteristicas mas importantes son las siguientes:
    * Es Open source.
    * Las consultas de SQL realizadas por Hibernate se llaman HQL (Hibernate Query Language).
    * Crea una capa de abstración para que el código no esté acoplado directamente a la base de datos, lo que permite que los desarrolladores no necesiten implementar código orientado a una base de datos en concreto.
  * **Struts** -> es un robusto framework creado por Apache pensado para desarrolladores web, sobre todo para personas que estén comenzando su carrera como desarrollador web.
  * **JSF(JavaServer Faces)** -> Es un framework con patrón MVC desarrollado por Oracle, y forma parte de Java Enterprise Edition 7, y se fundamenta en ayudar a los desarrolladores de backend para crear la parte frontend de aplicaciones complejas.
