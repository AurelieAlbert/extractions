# eNATL60-BLB002 sea surface height

 - Simulation : [eNATL60-BLB002](https://github.com/AurelieAlbert/extractions/blob/main/simulations/enatl60-blb002.md)
 - Region : [North Atlantic](https://github.com/AurelieAlbert/extractions/blob/main/regions/NATL.md)
 - Period : 01/07/2009-30/06/2010
 - Variables : sossheig
 - Vertical levels : surface
 - Path : 
   - on [MEOM opendap](https://github.com/AurelieAlbert/extractions/tree/main/platforms) : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/eNATL60/eNATL60-BLB002/surf/catalog.html
   - on [cal1 server](https://github.com/AurelieAlbert/extractions/blob/main/platforms/cal1.md) : /mnt/meom/workdir/alberta/eNATL60/eNATL60-BLBT02-S/1h/SSH
   - on [CINES-occigen](https://github.com/AurelieAlbert/extractions/blob/main/platforms/occigen.md) :
       - sossheig in netcdf format : /store/albert7a/eNATL60/eNATL60-BLBT02-S/1h/SSH.tar
       - sossheig in zarr format : /store/albert7a/eNATL60/zarr/eNATL60-BLBT02-SSH-1h (chunks = 240,240,480)
   - on [CNES-hal](https://github.com/AurelieAlbert/extractions/blob/main/platforms/hal.md) :
       - sossheig in netcdf format : /work/ALT/odatis/eNATL60/BLB002/gridT-2D
       - sossheig in zarr format : /work/ALT/odatis/eNATL60/zarr/eNATL60-BLB002-SSH-1h 
       ```
       
