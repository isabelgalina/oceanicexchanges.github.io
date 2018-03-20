---
layout: post
title: Digital National Newspaper Library of Mexico, Hemeroteca Nacional Digital de México
tags: [dh, DiD, data reports]
author: igalina, alerma
---

# Digital National Newspaper Library of Mexico
_Report also available in [Español](#espanol)_

## Collection’s History
México’s National Digital Newspaper Library (HNDM, in Spanish) was created between 2004 and 2008.  Like many libraries at that time, these new digital storage methods were used both to preserve the originals as well as to provide increased access. 
The project focused on digitalizing México’s National Newspaper Library’s microfilm collection, which was created in 1960. The documents were selected according to the following criterion: the newspaper’s degree of conservation, the demand as well as their historical, patrimonial, journalistic, and documentary importance. In this way the digitization project aimed to offer new forms of access and use of the historical newspapers, including search options by word, phrase, year and date range. 

## Collection’s composition
Today, the HNDM has almost 8 million digitized pages from 941 newspaper titles between 1722 and 2006. Out of these, 516 titles (1722-1889) are Open Access, and 425 (1890-2006) are restricted and can only be accessed from inside the Newspaper Library’s facilities.
The microfilmed and digital archives can be found in the National Newspaper Library’s Fondo Reservado (special collections) which includes: Mexican periodical publications between 1722 and 1917; foreign periodical publications from 1665 to 1920; the Garcia Valseca collection and the newspaper miscellanea and important newspapers microfilms collections (Hemeroteca Nacional Digital de México (c); n.d.).
For Oceanic Exchanges, the HNDM will participate with newspapers between 1800 and 1914, which is equivalent to 771 titles and 2,069,247 pages.

## Data and Metadata
The HNDM’s digitalization was obtained from 35mm microfilm rolls that the National Newspaper Library created. The publication’s stills have been reduced 21 times relative to their original size and contain between 140 and 180 line pairs per millimeter (pl/mm). This reduces the effects due to time on paper and ink tones from the original documents and produces a better contrast. 
To create the HNDM collection every page of every item from the newspaper was digitized in a bitonal TIFF image, and OCR was used to obtain text. This is stored in XML format that also includes descriptive metadata of the publications as well as metadata for the coordinates of each word on the page.
        	According to an analysis by the Dirección General de Cómputo y de Tecnologías de Información y Comunicación at UNAM (the National University’s Computing and Communication and Information Technologies General Office), the OCR average success rate, in the XML, is 54%. On the image’s readability, it was found that 72% have good readability, about 15% is regular, and 13% is bad. Their quality was 56% good, 34% regular, and less than 10% bad.
        	The dataset’s XML archive works with three metadata schemes (Dublin Core, custom OCR/XML Data, and Metadata Encoding & Transmission Standard) in a METS metadata scheme that includes, at the beginning of the file, a publication’s description in Dublin Core with: date, title, city, state, country, category, collection and language. It’s followed by an OCR structure that divides the page’s content in columns, regions, paragraphs, lines, and words with an associated coordinate. XML are in a MongoDB v.3.6 database, which works with the objects of: publication, item, page, collection, and publication’s description.

##References
Curiel, G., & Jimenez, R. J. (2015). Diez años de la Hemeroteca Nacional Digital de México. Breve reseña de una larga gestión de preservación y acceso, 2002-2012 en I Textos, pixeles y bits: Reflexiones sobre la publicación digital. Retrieved December 19, 2017, from http://www.hndm.unam.mx/files/acerca-de-hndm/diez-anios-de-la-hemeroteca-nacional-digital-de-mexico.pdf
Hemeroteca Nacional Digital de México (a). (n.d.). Antecedentes. Retrieved December 19, 2017, from http://www.hnm.unam.mx/index.php/quienes-somos/antecedentes
Hemeroteca Nacional Digital de México (b).  (n.d.).Acerca de HNDM, Retrieved December 19, 2017, from   http://www.hndm.unam.mx/index.php/es/acerca-de-hndm 
Hemeroteca Nacional Digital de México (c).  (n.d.).Fondos, Retrieved December 19, 2017, from http://www.hnm.unam.mx/index.php/hemeroteca-nacional-de-mexico/colecciones/fondo-reservado/hemeroteca-nacional-digital-mexico
