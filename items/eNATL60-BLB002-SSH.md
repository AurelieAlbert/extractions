# eNATL60-BLB002 sea surface height

 - Configuration : [eNATL60](../simulations/enatl60.md)
 - Simulation : [eNATL60-BLB002](../simulations/enatl60-blb002.md)
 - Region : [North Atlantic](../regions/eNATL.md)
 - Period : 01/07/2009-30/06/2010
 - Frequency : 1h
 - Variables : sossheig
 - Vertical levels : surface
 - Path : 
   - on [MEOM opendap](../platforms/opendap.md) : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/eNATL60/eNATL60-BLB002/surf/catalog.html
   - on [cal1 server](../platforms/cal1.md) : /mnt/meom/workdir/alberta/eNATL60/eNATL60-BLBT02-S/1h/SSH
   - on [CINES-occigen](../platforms/occigen.md) :
       - sossheig in netcdf format : /store/albert7a/eNATL60/eNATL60-BLBT02-S/1h/SSH.tar
       - sossheig in zarr format : /store/albert7a/eNATL60/zarr/eNATL60-BLBT02-SSH-1h (chunks = 240,240,480)
   - on [CNES-hal](../platforms/hal.md) :
       - sossheig in netcdf format : /work/ALT/odatis/eNATL60/BLB002/gridT-2D
       - sossheig in zarr format : /work/ALT/odatis/eNATL60/zarr/eNATL60-BLB002-SSH-1h 
      
