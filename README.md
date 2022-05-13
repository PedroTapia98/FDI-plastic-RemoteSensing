# FDI-plastic-RemoteSensing
# Identificación de Plásticos y microplásticos en el océano por medio de Percepción Remota

En la presente investigación se planteó la detección de plástico flotante (marino residuos) en océanos y mares utilizando Percepción Remota por medio del 
Sistema de satélite de imágenes gratis de Sentinel 2 (Copernicus.).Con el propósito de aplicar realces espectrales para detectar residuos plásticos en conjunto con la aplicación de Debris Tracker que proporciona datos de recolección de residuos plásticos.El propósito es ver la efectividad de la aplicación Debris Tracker en la imágenes de satélite y viceversa.Con el motivo de llegar a un mayor alcance con las imágenes de satélite.

## Aplicación de realces espectrales
## Indices

### NDVI, NDWI and FDI

Este enfoque se basa en el trabajo de Biermanns et al.Presentan la función FDI, que utilizan junto con NDVI como funciones para un clasificador bayesano ingenuo. Nuestro enfoque utiliza estos dos valores y agrega NDWI para tener imágenes con tres bandas.
El Índice de Vegetación de Diferencia Normalizada (NDVI) es un buen indicador para diferenciar la vegetación de otros materiales. Se basa en que las plantas, durante el proceso de fotosíntesis, absorben la luz en el bandas rojas (alrededor de 665 nm) y reflejan la luz para longitudes de onda superiores a 700 nm. Por lo tanto, tener un índice normalizado diferencia con estos valores esto logra un buen indicador en cuanto a la vegetación. La ecuación siguiente muestra la implementación del NDVI.
