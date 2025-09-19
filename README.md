 ESTRUCTURA DE DATOS
Maestra: Blanca Aracely Aranda Machorro
Equipo: 5 Nombre: TechSolutions S.A. de C.V.
Monterrey Nuevo León a 29 de agosto de 2025
 
Índice del Proyecto Empresarial
1.	Introducción
2.	Alcance
a.	2.1 Funcionalidades Principales
b.	2.2 Limitaciones
3.	Análisis
a.	3.1 Análisis de Requisitos
b.	3.2 Análisis de Viabilidad
4.	Justificación
a.	4.1 Beneficios Esperados
5.	Diseño
a.	5.1 Clases Principales
b.	5.2 Diagrama del Sistema
c.	5.3 Foto de Interfaz
6.	Desarrollo
a.	6.1 Organización de Paquetes
b.	6.2 Uso de Estructuras de Datos
c.	6.3 Validaciones Implementadas
7.	Implementación
a.	7.1 Requisitos de Ejecución
b.	7.2 Pasos de Compilación y Ejecución
8.	Pruebas
a.	8.1 Casos de Prueba
b.	8.2 Resultados de las Pruebas
9.	Glosario de Términos
10.	Evidencia de Código 
11.	Autores
12.	Conclusión
13.	Bibliografía





1.Introduccion
El sistema de gestión empresarial desarrollado para TechSolutions S.A. de C.V. es una aplicación de consola en Java que combina la gestión de tareas departamentales utilizando estructuras de datos (pilas, colas y listas) con funcionalidades empresariales avanzadas como gestión de clientes, inventario, ventas, reportes y usuarios con roles.
Funcionalidades Principales:
•	Gestión de Tareas Departamentales: Utiliza pilas para emergencias, colas para desarrollo regular y listas para proyectos por departamento.
•	Gestión de Clientes: Registro de clientes con distinción VIP.
•	Control de Inventario: Administración de productos con alertas de stock bajo.
•	Sistema de Ventas: Procesamiento de ventas con cálculo de IVA y descuentos para clientes VIP.
•	Reportes: Generación de reportes de ventas, inventario y clientes.
•	Gestión de Usuarios: Sistema de login con roles (admin, empleado).
Limitaciones:
•	Interfaz de consola únicamente.
•	Persistencia de datos en archivos de texto.
•	No incluye interfaz gráfica ni base de datos.

Análisis 
Análisis de Requisitos:
El sistema debe permitir a TechSolutions gestionar eficientemente sus operaciones diarias, desde la asignación de tareas hasta el control de ventas y clientes. Se requiere un sistema que integre la gestión de tareas con las operaciones comerciales.
Análisis de Viabilidad:
•	Técnica: Java es adecuado para este tipo de aplicación, con estructuras de datos eficientes.
•	Económica: Desarrollo interno reduce costos.
•	Operacional: Fácil de usar para empleados con conocimientos básicos de computación.
Justificación

TechSolutions requiere un sistema integrado que mejore la eficiencia en la gestión de tareas y operaciones comerciales. La combinación de estructuras de datos permite una gestión óptima de prioridades, mientras que las funcionalidades empresariales facilitan el control de ventas y clientes.

Beneficios Esperados:
- Mejora en la organización de tareas por urgencia y departamento.
- Control preciso del inventario y ventas.
- Generación rápida de reportes para toma de decisiones.
- Seguridad mediante roles de usuario.

Diseño
Clases principales
•	Avance_TechSolutions_Final: Clase principal con menus
•	Cliente: guarda datos del cliente y si es VIP o no.
•	Producto: información de stock, precio y nombre.
•	Venta: maneja facturación, IVA y descuentos.
•	Inventario: controla la cantidad de productos y genera alertas.
•	Reporte: produce estadísticas de ventas e inventario.
•	Usuario: define roles y accesos al sistema.
•	Tarea, PilaTareas, ColaTareas, ListaTareas: Para gestion de tareas




Diagrama
 
Caso de uso
 






Flujo de tareas
 


Flujo de ventas
 
Foto de interfaz
 

Submenús Tareas urgentes, Desarrollo Regular y Gestión por Departamento:     
 
 Menu del Sistema Empresarial 
  
Salir del Sistema: 
  







Desarrolló
El sistema se programó en Java usando Programación orientada a objetos
Entorno de Desarrollo: Visual Studio Code 
Persistencia: Archivos de texto (.txt) 
Estructuras de Datos: Implementaciones propias de pila, cola y lista 
Se organizaron paquetes:
Clientes—gestion de clientes
Ventas---facturacion y reportes
Inventario---control de productos
Ui---interfaz de consola
Se usaron estructuras dinámicas (ArrayList, HashMap) para guardar clientes, productos y ventas.
También se añadieron validaciones para evitar errores, como ventas sin stock disponible
Implementación
Para la ejecución
•	Compatible con Windows, Linux y MacOS.
•	Requiere JDK 17 o superior.
Pasos de compilación y ejecución
Primera forma de Compilar:
javac main/SistemaApp.java
Ejecutar: 
o	Ejecutar la clase principal 
o	Java Avance_TechSolutions_Final 
o	Seguir los menús para navegar por las funcionalidades 
Segunda Forma de compilar
o	Abrir al archivo run_techsolutions.bat el cual iniciara el sistema y enseñara la interfaz en una ventana de comando 
o	Seguir los menús para navegar por las funcionalidades 

Pruebas
Casos de prueba
•	Registrar un cliente normal: aparece en la lista de clientes. 
   
•	Registrar un cliente VIP: aparece en la lista con beneficios especiales. 
a.	True = VIP / False = NO 
•	Realizar una venta: se descuenta del inventario y genera factura con IVA. 
  
•	Venta sin stock: el sistema alerta que no hay suficiente producto. 
  
•	Generar reporte de venta: muestra ventas realizadas en cierto periodo. 
  
•	Login como admin: acceso a todas las funciones. 
a.	 usuario: admin contraseña: admin123 
   
•	Login como empleado: acceso limitado. 
a.	Usuario: empleado contraseña: emp123 
   
 
 
•	Foto de los usuarios por el momento 
  





Resultados de pruebas
El sistema distingue entre clientes normales y VIP. 
El inventario se actualiza correctamente con cada venta. 
El sistema de ventas calcula correctamente IVA y descuentos 
La persistencia de datos funciona sin perdida de informacion 
Los reportes muestran datos consistentes. 
El login respeta los roles de usuario. 

GLOSARIO DE TÉRMINOS
•	Cliente VIP: cliente con beneficios.
•	Inventario: registro de productos disponibles en la empresa.
•	Reporte: resumen con información útil para la toma de decisiones.
•	POO (Programación Orientada a Objetos): programación que organiza el código en clases y objetos.
•	ArrayList / HashMap: estructuras de datos de Java usadas para manejar colecciones de información.






Fotos de Código: 
Archivo principal Avance_TechSolutions_Final.java y función Main()
  
  
 
PilaTareas.java	                          ListaTareas.java                                    Cola Tareas.java  Usuarios.java                                  Venta.java                                       Cliente.java 
  
Tarea.java                                         Producto.java                             Reporte.java run_techsolutions.bat (Abre la interfaz de usuario en una ventana de comando) 
  





Autores
Jesus David Marroquin Peña   AL07101520
 
Mauricio sanchez Figueroa AL07098275
 
Juan Porfirio Torres Rojas AL07099471
 
Ian Carlos Martinez Diaz AL03003400
 

Conclusión
El desarrollo de un sistema empresarial integral para TechSolutions S.A. de C.V. representa una solución efectiva a las problemáticas actuales de gestión de clientes, ventas, inventario y seguridad. Con la implementación de este sistema, la empresa logrará centralizar y automatizar procesos clave, lo que permitirá reducir errores administrativos, optimizar recursos y ofrecer un servicio diferenciado a sus clientes VIP, quienes son fundamentales para la rentabilidad del negocio.
Asimismo, la incorporación de módulos de reportes y notificaciones proporcionará información oportuna y confiable para la toma de decisiones estratégicas, fortaleciendo la capacidad competitiva de la organización. De esta manera, el sistema no solo responde a las necesidades presentes, sino que también sienta las bases para un crecimiento sostenible y una mejora continua en la relación con los clientes y en la eficiencia operativa de la empresa.






Bibliografías:
Kotler, P., & Keller, K. L. (2016). Dirección de marketing (15a ed.). Pearson.
Laudon, K. C., & Laudon, J. P. (2020). Sistemas de información gerencial (16a ed.). Pearson.
O’Brien, J. A., & Marakas, G. M. (2018). Sistemas de información en los negocios. McGraw-Hill.
Pressman, R. S. (2010). Ingeniería de software: Un enfoque práctico (7a ed.). McGraw-Hill.
Stair, R., & Reynolds, G. (2019). Principios de sistemas de información (13a ed.). Cengage.
