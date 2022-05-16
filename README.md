# FDI-plastic-RemoteSensing
# Identificación de Plásticos y microplásticos en el océano por medio de Percepción Remota

Desarrollo de un sript para la detección de plástico flotante (marino residuos) en océanos y mares utilizando Percepción Remota por medio del 
Sistema de satélite de imágenes gratis de Sentinel 2 (Copernicus.).Con el propósito de aplicar realces espectrales para detectar residuos plásticos.

## Aplicación de realces espectrales
## Indices

### NDVI, NDWI and FDI

Este enfoque se basa en el trabajo de Biermanns et al.Presentan la función FDI, que utilizan junto con NDVI como funciones para un clasificador bayesano ingenuo. Nuestro enfoque utiliza estos dos valores y agrega NDWI para tener imágenes con tres bandas.
El Índice de Vegetación de Diferencia Normalizada (NDVI) es un buen indicador para diferenciar la vegetación de otros materiales. Se basa en que las plantas, durante el proceso de fotosíntesis, absorben la luz en el bandas rojas (alrededor de 665 nm) y reflejan la luz para longitudes de onda superiores a 700 nm. Por lo tanto, tener un índice normalizado diferencia con estos valores esto logra un buen indicador en cuanto a la vegetación. La ecuación siguiente muestra la implementación del NDVI.

![formula NDVI](https://github.com/PedroTapia98/FDI-plastic-RemoteSensing/blob/main/IMAGE-README.png)

El índice de diferencia de agua normalizado (NDWI) es un buen indicador para diferenciar el agua de otros materiales. Se basa en que el agua tiene alta reflectancia en la banda verde y alta absorción en el NIR banda, por lo que tener una diferencia normalizada con estos valores es una forma sencilla de estimar la presencia de agua.La siguiente ecuación muestra la implementación del NDWI.

![formula NDWI](https://github.com/PedroTapia98/FDI-plastic-RemoteSensing/blob/main/IMAGE-README2.png)

Finalmente, el Índice de Desechos Flotantes (FDI) fue introducido por Biermanns et al. [8]. Su trabajo lo demuestra logrando buenos resultados para la detección subpíxel de plásticos y otros tipos de desechos en el mar.

![formula FDI](https://github.com/PedroTapia98/FDI-plastic-RemoteSensing/blob/main/IMAGE-README3.png)
