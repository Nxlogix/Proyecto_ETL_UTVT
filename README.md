# Proyecto ETL con SSIS – Comercializadora UTVT S.A. de C.V.

## Descripción

Este proyecto implementa un proceso ETL (Extract, Transform and Load) utilizando SQL Server Integration Services (SSIS) para integrar información proveniente de archivos CSV hacia un Data Warehouse denominado **DWUTVTVentas**.

El objetivo principal es mejorar la calidad de los datos mediante procesos de limpieza, validación, transformación y carga, permitiendo generar información confiable para el área de Business Intelligence.

## Objetivos

* Integrar datos de clientes, productos y ventas.
* Eliminar registros duplicados.
* Validar información antes de cargarla.
* Registrar errores durante la ejecución.
* Automatizar el movimiento y compresión de archivos.
* Mantener un historial de cambios mediante Git y GitHub.

## Tecnologías utilizadas

* SQL Server
* SQL Server Integration Services (SSIS)
* Visual Studio 2022
* Git
* GitHub
* PowerShell

## Estructura del proyecto

Proyecto_ETL_UTVT/

* data/
* database/
* docs/
* evidencias/
* ssis/
* README.md
* .gitignore
* Release_1.0.txt

## Base de datos

Nombre:

DWUTVTVentas

Tablas:

* DimCliente
* DimProducto
* FactVentas
* LogErrores
* LogProceso

## Flujo ETL

1. Lectura de archivos CSV.
2. Limpieza de datos.
3. Eliminación de duplicados.
4. Validación de reglas de negocio.
5. Carga de dimensiones.
6. Carga de tabla de hechos.
7. Registro de errores.
8. Registro de estadísticas.
9. Movimiento de archivos procesados.
10. Compresión de archivos.

## Variables utilizadas

* RutaEntrada
* RutaProcesados
* RutaErrores
* FechaProceso
* TotalLeidos
* TotalInsertados
* TotalErrores

## Control de versiones

El proyecto utiliza Git con las siguientes ramas:

* main
* feature/clientes
* feature/productos
* feature/ventas

Los commits siguen la convención Conventional Commits.

## Autor
Alan Ronlado Serrano Colin
Sofía Sánchez Durán

Universidad Tecnológica del Valle de Toluca.

