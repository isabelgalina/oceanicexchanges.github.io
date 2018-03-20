---
layout: post
title: Digital National Newspaper Library of Mexico, Hemeroteca Nacional Digital de México
tags: [dh, DiD, data reports]
author: igalina, alerma
---

# Digital National Newspaper Library of Mexico
_Report also available in [Español](#espanol)_

## Data quantity
The Hemeroteca Nacional Digital de México is the Digital National Newspaper Library of Mexico.  The HNDM consists of 7 million Mexican newspaper pages from 1722 to 2006 from all Mexican states. 

* Total number of titles: 941 
* Number of open-access titles: 516
* Number of restricted access titles: 425

* Total number of digitized pages: 7,947,608
* Open access pages: 4,103,332
* Restricted access pages: 3,844,276

## Data quality 
Newspapers for the HNDM were scanned from microfilm. The microfilm was in 35mm format. 

Bi-tonal TIFF images at 300 dpi. OCR is contained in XML files.  The OCR quality of the collection derived from a sample study is 54%.  Image legibility is 72.16% good, 14.77% regular and 13.07% bad. Image quality is: 56.14% good, 34.01% regular and 9.85% bad.

## Metadata/Metadatos

The collection includes three levels of metadata. Dublin Core is shown below: 

|_Element_ |            |      _Description_     |
|----------|------------|:----------------------:|
| Date     |            |    Publication date    |
| Title    |            |     Newspaper title    |
| Coverage | City       |   City of publication  |
|          | State      |  State of publication  |
|          | Country    | Country of Publication |
|          | Category   | Publication frequency  |
| Language |            | Language               |
| Source   | Collection | Collection             |

The second type of metadata is "Custom OCR XML Data" which was defined by the company who did the digitization. Uses a similar description to ALTO (Technical Metadata for Optical Character Recognition) and describes the distribution of the content by page. 

The last type of metadata is METS (Metadata Encoding & Transmission Standard).

The files are currently handled by a database in MongoDB version 3.6 which uses the following main entities for data data description. 

| Entity / Class                | Fields / Attributed                                                                                                                                                                                                                                                                                                            |
|-------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Publication                   | ID, Titulo, Subtitulo, TotalItems, TipoAcceso, Estatus, Idioma, País, Estado, Ciudad, Frecuencia, TipoPublicacion, fechaInicio, fechaFinalizo, fechaDeRegistro, fechaDeModificacion, colecciones_id, totalImagenesActual, PrimerPaginaDePublicacion_id, Fecha, totalArchivosXML                                                                    |
| Item                          |id, publicacion_id, anio, mes, dia, colecciones_id, totalPaginas, estatusProceso, estatus, fechaDeRegistro, fechaDeModificacion, tipoAcceso                                                                                                                                                                                              |
| Página                        |id, titulo, subtitulo, item_id, publicacion_id, colecciones_id, tipoAcceso, estatus, idioma, país, estado, ciudad, frecuencia, tipoPublicacion, fecha, fechaDeRegistro, fechaDeModificacion, pagina, paginaAnterior_id, paginaSiguiente_id, imagen, rutaImagen, tipoDeArchivo, espacioDeColor, tamanioArchivo, resolucion, rutaXML, totalPalabrasOCR, ocr |
| Colección                     |id, nombre, descripción, nombreCorto, tipoAsignacion, tipoElemento, criterios, estatus, pagina, Representativa_id, fechaInicioApertura, fechaInicioCierre, elementosAsignados, elementoAsignado.tipo, elementoAsignado.Id                                                                                                                   |
| Descripción de la publicación |id, publicacion_id, publicacionTitulo, tipoAcceso, Estatus, texto, textoOriginal, primerPaginaDePublicacion_id, coleccion_id, versionTextoOriginal, carpetaAnterior                                                                                                                                                                     |

## Data Availability & Legal Restrictions Concerning the Data
Newspaper titles from 1722 to 1889 are in open access. 
1890 to 2006 can only be consulted within the National Library controlled by IP address. 

## Collection History

The National Newspaper Library of Mexico (Hemeroteca Nacional de México - HN) was created in 1944 to curate the newspaper collections of the National Library of Mexico (Biblioteca Nacional de México – BM) which was founded in 1867. In 1929, by federal mandate the custody of the National Library of Mexico was transferred from the Ministry of Public Education (Secretaría de Educación Pública) to the National University of Mexico (Universidad Nacional Autónoma de México – UNAM). In 1936 a legal deposit decree established that publishers in the country should deposit two copies of every book, newspaper, and magazine in the National Library. (Hemerotéca Nacional de México; 2017)

During the 1960s the HN began microfilming its collection and started a program to "select and microfilm the most relevant old collections from the archive" (Curiel & Jiménez; 2015: p.2). The micrographic archive consists of prints on silver gel and currently contains more than 28 million microfilmed pages. Curiel y Jiménez (Curiel & Jiménez; 2015: p.2) describe that the criterion taken into account for microfilming was the "historical, patrimonial, journalistic and documentary importance, as well as the state of conservation, user demand as well as issues related to copyright."
 
It was considered that microfilm was an ideal way of conserving the collection as well as providing an alternative form of access to the materials. During the 1990’s the silver gel prints were copied to diazonium salt microfilm and access to users was provided in rooms with microfilm readers and printers (Curiel & Jiménez; 2015: p.3). 

Digitization was first explored towards the end of the 1990s.  In 2000, the National Digital Newspaper Library of Mexico (Hemeroteca Nacional Digital de México - HNDM) project began although it wasn’t until 2002 that funding was secured and digitalization began. The decision was made to digitize the microfilm rather than the physical newspapers for two mains reasons. First, the microfilms had already been through a selection process. Secondly, it would allow the digitization process to be done without impacting the originals or creating any disruption to users of the collection. 

In total, 947 Mexican and foreign publication titles between 1722 to 2010 were digitized. These titles amount to almost nine million digitalized pages, of which 516 are open access and can be viewed freely online, whilst 425 are restricted and can only be viewed inside the HNDM consultation room within the main library building. The sum of the microfilmed and digitized newspapers are grouped under the collection Fondo Reservado which is described as: “Mexican periodical publication from 1722 to 1917; foreign periodical publication between 1665 to 1920; García Valseca collection; miscellaneous newspapers and microfilms of important periodicals”.(REF)

## References
1. Hemeroteca Nacional de México. (n.d.). Antecedentes. Recuperado diciembre 19, 2017, de [http://www.hnm.unam.mx/index.php/quienes-somos/antecedentes](http://www.hnm.unam.mx/index.php/quienes-somos/antecedentes)
2. Curiel, G., & Jimenez, R. J. (2015). Diez años de la Hemeroteca Nacional Digital de México. Breve reseña de una larga gestión de preservación y acceso, 2002-2012. En _I Textos, pixeles y bits: Reflexiones sobre la publicación digital_. Recuperado diciembre 19, 2017, de  http://www.hndm.unam.mx/files/acerca-de-hndm/diez-anios-de-[http://www.hndm.unam.mx/files/acerca-de-hndm/diez-anios-de-la-hemeroteca-nacional-digital-de-mexico.pdf](la-hemeroteca-nacional-digital-de-mexico.pdf)
3. Información obtenida del Documento “Revisión del Sistema de Consulta y Gestión de la Hemeroteca Nacional Digital de México”. Generado en 2012 por la Dirección General de Cómputo y de Tecnologías de Información y Comunicación de la UNAM.
4. Diccionario de Datos del Diagrama Entidad Relación de la HNDM.

# <a name="espanol"></a>Hemeroteca Nacional Digital de México

## Cantidad de datos
La colección de la Hemeroteca Nacional incluye 7 millones de páginas de periódicos mexicanos de 1722 a 2006 de todos los estados de la república mexicana. 

* Total de títulos: 941 
* Total de títulos acceso abierto: 516
* Total de títulos de acceso restringido: 425

* Total de páginas digitalizadas: 7,947,608
* Páginas de acceso abierto: 4,103,332
* Páginas de acceso restringido: 3,844,276

## Calidad de los datos

La digitalización de la HNDM fue obtenida a partir de rollos de microfilm que la Hemeroteca Nacional genera en formato de 35mm los cuales contienen fotogramas de las publicaciones con una reducción de 21 veces respecto al tamaño original y entre 140  y 180 pares de  líneas  por  milímetro  (pl/mm) con una gama cromática en escala de grises de   hasta   20   medios pasos con un contraste medianamente alto.Esto ha permitido obtener fotogramas con una reducción considerable de los efectos del paso del tiempo ocasionados en los tonos del papel y las tintas del original, que permite por otro lado resaltar el  contraste  real  de  los  documentos.

Esto permitió generar imágenes bitonales de formato TIFF a 300 dpi.  El OCR está contenido en archivos XML. Un estudio realizado por la Dirección General de Cómputo y de Tecnologías de Información y Comunicación de la UNAM indicó que después de realizar un análisis sobre una muestra representativa, indicó lo siguiente:

El promedio del nivel de acierto del OCR es del 54%.
Con respecto a la legibilidad de las imágenes el 72.16 % fue buena, el 14.77 % regular y sólo el 13.07 % fue mala.
Con respecto a la calidad de las imágenes el 56.14 % fue buena, el 34.01 % regular y sólo el 9.85 % fue mala.

## Metadatos

A partir del análisis realizado a los archivos XML de la muestra, se encontró que se manejan tres esquemas de metadatos.

Un primer grupo  de archivos XML del sistema de la HNDM, son validados por los 15 elementos básicos del Dublin Core, de los cuales sólo se hace uso de los siguientes:



|_Elemento_|            |      _Descripción_         |
|----------|------------|:--------------------------:|
| Date     |            |  Fecha de publicación      |
| Title    |            |  Título del periódico      |
| Coverage | City       | Ciudad de publicación      |
|          | State      | Estado de publicación      |
|          | Country    |    País publicación        |
|          | Category   | Periodicidad del periódico |
| Language |            |         Lenguaje           |
| Source   | Collection |         Colección          |


El segundo grupo de metadatos ocupa un esquema “Custom OCR XML Data”, el cual fue definido por el proveedor DIGIX. Este realiza una tarea similar a la del esquema ALTO (Technical Metadata for Optical Character Recognition) , que describe la distribución del contenido que se encuentra en la página, indicando las coordenadas donde se encuentran las columnas las cuales dividen en regiones y líneas, dentro de las cuales se encuentran contenidas párrafos y palabras; las regiones y párrafos se encuentran delimitadas dentro de una área establecida como atributos de estas etiquetas, así como también se encuentran indizadas las coordenadas de las palabras identificadas por el OCR de DIGIX (DgxIOCr 1.5.2460.31821). 

El último grupo de utiliza  el estándar METS (Metadata Encoding & Transmission Standard)

Estos archivos actualmente se encuentran cargados en una Base de Datos en MongoDB versión 3.6, la cual maneja a las siguientes entidades principales con la siguiente descripción de datos:

| Entity / Class                | Fields / Attributed                                                                                                                                                                                                                                                                                                            |
|-------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Publication                   | ID, Titulo, Subtitulo, TotalItems, TipoAcceso, Estatus, Idioma, País, Estado, Ciudad, Frecuencia, TipoPublicacion, fechaInicio, fechaFinalizo, fechaDeRegistro, fechaDeModificacion, colecciones_id, totalImagenesActual, PrimerPaginaDePublicacion_id, Fecha, totalArchivosXML                                                                    |
| Item                          |id, publicacion_id, anio, mes, dia, colecciones_id, totalPaginas, estatusProceso, estatus, fechaDeRegistro, fechaDeModificacion, tipoAcceso                                                                                                                                                                                              |
| Página                        |id, titulo, subtitulo, item_id, publicacion_id, colecciones_id, tipoAcceso, estatus, idioma, país, estado, ciudad, frecuencia, tipoPublicacion, fecha, fechaDeRegistro, fechaDeModificacion, pagina, paginaAnterior_id, paginaSiguiente_id, imagen, rutaImagen, tipoDeArchivo, espacioDeColor, tamanioArchivo, resolucion, rutaXML, totalPalabrasOCR, ocr |
| Colección                     |id, nombre, descripción, nombreCorto, tipoAsignacion, tipoElemento, criterios, estatus, pagina, Representativa_id, fechaInicioApertura, fechaInicioCierre, elementosAsignados, elementoAsignado.tipo, elementoAsignado.Id                                                                                                                   |
| Descripción de la publicación |id, publicacion_id, publicacionTitulo, tipoAcceso, Estatus, texto, textoOriginal, primerPaginaDePublicacion_id, coleccion_id, versionTextoOriginal, carpetaAnterior                                                                                                                                                                     |

## Disponibilidad y restricciones legales

Las publicaciones periódicas de 1722 a diciembre de 1889 se encuentran disponibles para su consulta de acceso abierto y de enero de 1890 a 2006 sólo pueden ser consultadas al interior del edificio de la Hemeroteca.

## Historia de la colección

La Hemeroteca Nacional de México fue creada en 1944 para resguardar el acervo hemerográfico de la Biblioteca Nacional de México que fue fundada en 1867.  Por mandato del gobierno federal, en 1929 la Biblioteca Nacional dejó de depender de la Secretaría de Educación Pública y se integró a la Universidad Nacional Autónoma de México. En 1936 fue emitido el decreto de Depósito Legal, que obliga a los editores de todos los estados de la República al envío de dos ejemplares de libros, periódicos y revistas a la Biblioteca Nacional. (Hemerotéca Nacional de México; 2017)

En la década de los 1960 la HN adoptó la microfilmación y se comenzó con un programa para  “la selección y microfilmación de las colecciones antiguas más relevantes de su acervo” (Curiel & Jiménez; 2015: p.2).  El acervo micrográfico son películas en plata sobre gelatina y actualmente asciende a 28 millones de páginas microfilmadas. Curiel y Jiménez  mencionan que los criterios para microfilmar son la “importancia histórica, patrimonial, periodística y documental, el estado de conservación y el grado de demanda de los usuarios, así como los asuntos inherentes a los derechos de autor.”  (Curiel & Jiménez; 2015: p.2)

La microfilmación se consideró adecuada no solo para conservar sino también con una forma alternativa para dar servicio de consulta.  En la década de los 90’s se duplicaron los microfilmes en haluros de plata a micropelículas de sales de diazonio y se dio servicio a través de sala en donde se colocaron máquina lectoras e impresoras (Curiel & Jiménez; 2015: p.3)

Hacia finales de los años noventa se empezó a explorar las posibilidades de la digitalización.   En 2000 se inició el proyecto de la Hemeroteca Nacional Digital de México, aunque no fue sino hasta 2002 que se procuró el financiamiento y se comenzó con la digitalización.  Se tomó la decisión de digitalizar lo microfilmado, ya que este había sido seleccionado y permitía realizar la digitalización sin retirar los ejemplares o quitar el servicio de consulta.  Se digitalizaron 947 títulos de publicaciones mexicanas y extranjeras, correspondientes a los años de 1722 a 2010. En un mayor detalle, estos títulos se traducen en casi nueve millones de páginas digitalizadas, de las cuales se cuentan 516 títulos de libre acceso y 425 con acceso restringido, es decir, que sólo se pueden consultar dentro de las instalaciones de la HNDM de acuerdo a los señalamientos dictados por los derechos de autor o patrimoniales. El total de publicaciones microfilmadas y digitalizadas se ubican dentro de la estructura de las colecciones de la Hemeroteca Nacional bajo el título de Fondo Reservado, cuyo contenido es: “publicaciones periódicas mexicanas de 1722 a 1917; publicaciones periódicas extranjeras de 1665 a 1920; fondo García Valseca; Misceláneas hemerográficas y microfilmes de importantes periódicos”.(REF)

## Referencias
1. Hemeroteca Nacional de México. (n.d.). Antecedentes. Recuperado diciembre 19, 2017, de [http://www.hnm.unam.mx/index.php/quienes-somos/antecedentes](http://www.hnm.unam.mx/index.php/quienes-somos/antecedentes)
2. Curiel, G., & Jimenez, R. J. (2015). Diez años de la Hemeroteca Nacional Digital de México. Breve reseña de una larga gestión de preservación y acceso, 2002-2012. En _I Textos, pixeles y bits: Reflexiones sobre la publicación digital_. Recuperado diciembre 19, 2017, de  http://www.hndm.unam.mx/files/acerca-de-hndm/diez-anios-de-[http://www.hndm.unam.mx/files/acerca-de-hndm/diez-anios-de-la-hemeroteca-nacional-digital-de-mexico.pdf](la-hemeroteca-nacional-digital-de-mexico.pdf)
3. Información obtenida del Documento “Revisión del Sistema de Consulta y Gestión de la Hemeroteca Nacional Digital de México”. Generado en 2012 por la Dirección General de Cómputo y de Tecnologías de Información y Comunicación de la UNAM.
4. Diccionario de Datos del Diagrama Entidad Relación de la HNDM.
