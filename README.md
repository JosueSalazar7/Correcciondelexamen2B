# Correcciondelexamen2B

CODIGO DE LA BASE DE DATOS UTILIZADA



CREATE database VEHICULOS
USE VEHICULOS

/*Creación de la tabla principal de datos*/
CREATE TABLE DATOS(
CI_DUENIO NUMERIC(10) PRIMARY KEY NOT NULL,
NOM_DUENIO VARCHAR(25) NOT NULL,
APE_DUENIO VARCHAR(25) NOT NULL,
EDAD NUMERIC (2) NOT NULL,
MARCA VARCHAR(15) NOT NULL,
COLOR VARCHAR (15) NOT NULL
)

/*Insertamos datos en la tabla de datos*/
INSERT INTO DATOS VALUES(1723359327,"JOSUE","SALAZAR",20)
select * from DATOS

/*Creamos la primera tabla que va a llenar el primer combo box que es el de selccionar una marca*/

CREATE TABLE MARCAS(
NOM_MARCA VARCHAR(15) NOT NULL
)
/*Ingresamos las marcas que van a estar disponibles*/

INSERT INTO MARCAS VALUES("RENAULT"),("CHEVROLET"),("MAZDA"),("HYUNDAI"),("VOLKSWAGEN"),("BMW"),("FORD"),("PEUGOT")

/*Creamos la senguna tabla que va a llenar el segundo combo box */

CREATE TABLE COLORES(
NOM_COLOR VARCHAR(15) PRIMARY KEY NOT NULL
)
/*Ingresamos los datos en la tabla*/

INSERT INTO COLORES VALUES("AMARILLO"),("ROJO"),("VERDE"),("NEGRO"),("AZUL"),("BLANCO")
