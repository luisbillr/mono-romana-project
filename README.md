# mono-romana-project

## Proyecto monográfico.

Aqui añadiremos los patrones a seguir para mantener la consistencia del proyecto.

#### Database

Tablas de la Base de Datos a utilizar

- Categoria
- Presentacion
- Articulo
- Trabajador
- Cliente
- Ingreso
- Proveedor
- Venta

#### Tareas

- **Estarlin Rivera** (Modulo de Categoria)
- **Jose Roman** (Modulo Presentacion)
- **Omar Yei** (Modulo Proveedor, Modulo Cliente)
- **Michael Williams** (Modulo Trabajador, Modulo Articulo)
- **Luis Bill** (Modulo Venta, Modulo Ingreso)

Cada Tabla es un modulo, hay que trabajarla en cada Capa..
Osea al que le toque un Modulo tendra que desarrollar la logica en cada capa.

#### Funcion de Las Capas

_**BusinessLogic**_: Capa de Logica, tendran los metodos que se conectaran con la Capa Data,
las clases creadas aqui terminaran con la letra BL(En Mayuscula) Ejemplo: CategoriaBL,
Cada Metodo que se declare sera static Ejemplo: public static Registrar(){}

_**Data**_: Capa Datos, tendran los crud(Crear, Leer, Actualizar y Borrar) del modulo encargado,
las clases creadas aqui terminaran con la palabra DAL(en Mayuscula) Ejemplo: CategoriaDAL.
los query seran con Store Procedure (Ya estan Creados en la Base de datos, solo tienen que buscar
los que le tocan y chequear el nombre que tienen).

_**Entity**_: Capa de Identidad, Tendran las clases(con sus Propiedades) que seran utilizadas
en las diferentes capas (Data,BusinnesLogic,PosSystem), es la unica que se puede
usar en todas las Capas.

_**PosSystem**_: Capa de Presentacion, tendran los formularios necesarios que lleva los modulos
asignados, se conecta con Entity y BusinessLogic.

---

> Nota: Para los Formularios Usar Blanco y Este tipo de Azul #46b3fe RGB(70, 179, 254),
> osea todo blanco y las decoraciones Azul (Botones, Bordes,etc).

Solo Usar Rojo Para los Botones de Advertencias (como Salir, Cancelar,Eliminar,etc..)
