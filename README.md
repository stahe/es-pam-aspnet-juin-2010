# [Creación de una aplicación web de tres capas con ASP.NET 2.0, C#, Spring.Net y NHibernate (2010)](https://stahe.github.io/es-pam-aspnet-juin-2010/)

Este documento presenta el desarrollo paso a paso de **SimuPaie**, una aplicación .NET diseñada para simular el cálculo de la remuneración de los cuidadores infantiles. El enfoque es doble: **establecer una arquitectura de software clara** e **implementar la solución utilizando las tecnologías .NET disponibles en ese momento**. En concreto, el documento describe una **arquitectura de tres capas** compuesta por una capa de acceso a datos (DAO), una capa de negocio y una capa de presentación, todas ellas integradas mediante **Spring IoC**.

## Objetivos del curso

El objetivo de este caso práctico es demostrar cómo diseñar una aplicación web fácil de mantener mediante una separación clara de responsabilidades:

- **Capa 1 - DAO**: acceso a los datos almacenados en la base de datos.
- **Capa 2 - Negocio**: cálculos de nóminas y reglas de negocio.
- **Capa 3 - IU**: interacción con el usuario y visualización de resultados.
- **Integración** de las capas mediante **interfaces .NET** e **inyección de dependencias con Spring IoC**.

El documento también describe el ciclo de procesamiento de las solicitudes de los usuarios: la aplicación recibe la solicitud, la reenvía si es necesario a la capa de negocio y luego a la capa de acceso a datos, antes de enviar una respuesta adecuada al cliente.

## Versiones sucesivas de la aplicación

La documentación no se limita a una única implementación. Ofrece varias variantes de SimuPaie para ilustrar diferentes enfoques arquitectónicos y de interfaz:

1. una versión **ASP.NET de un solo formulario** con una arquitectura de un solo nivel;
2. una versión equivalente mejorada con **Ajax**;
3. una versión **ASP.NET de tres niveles** con **NHibernate** para el acceso a datos;
4. una versión **de una sola página con múltiples vistas**;
5. una versión orientada a **servicios web** del lado del servidor;
6. una versión de cliente ASP.NET que consume este servicio;
7. una versión **multivista y multipágina**;
8. una versión de cliente del servicio web;
9. una variante de tres capas que se basa en mayor medida en clases de Spring para facilitar el uso de NHibernate;
10. una versión cliente **FLEX**.

## Requisitos previos

Este documento está dirigido a un nivel **intermedio**. Se da por supuesto un conocimiento básico de:
- **ASP.NET**
- **C# 2008**: clases, interfaces, herencia, polimorfismo
- **Spring IoC / inyección de dependencias**
- **arquitectura web de tres capas** y el modelo **MVC**.

## Herramientas y tecnologías tratadas

El caso práctico se basa en un conjunto coherente de herramientas y marcos de trabajo:

- **Visual C# 2008**
- **Visual Web Developer Express 2008**
- **SQL Server Express 2005**
- **Spring.Net / Spring IoC**
- **NHibernate**
- **NUnit** para pruebas unitarias.

## Qué ofrece este repositorio

Este recurso resultará de especial interés para los lectores que deseen:

- comprender la implementación de una **arquitectura de n capas** en un entorno .NET;
- ver cómo **desacoplar** las capas de presentación, lógica de negocio y acceso a datos;
- descubrir cómo utilizar **Spring.Net** para el ensamblaje de componentes;
- estudiar la integración de **NHibernate** en una aplicación web ASP.NET;
- seguir una ruta de aprendizaje paso a paso que avanza desde una versión sencilla hasta versiones más preparadas para la producción.

## Contenido del curso

El documento describe la arquitectura general de la aplicación y, a partir de la primera página, utiliza un diagrama para ilustrar las funciones del usuario, la aplicación, las tres capas y Spring IoC en la coordinación de todo el sistema. Por lo tanto, sirve tanto como **curso de arquitectura**, **guía de diseño** y **base de trabajo para la implementación práctica**.

Serge Tahé, junio de 2010