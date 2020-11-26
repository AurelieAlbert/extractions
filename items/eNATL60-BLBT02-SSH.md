# eNATL60-BLBT02 sea surface height

 - Simulation : [eNATL60-BLBT02](https://github.com/AurelieAlbert/extractions/blob/main/simulations/enatl60-blbt02.md)
 - Region : [North Atlantic](https://github.com/AurelieAlbert/extractions/blob/main/regions/NATL.md)
 - Period : 01/07/2009-01/10/2010
 - Variables : sossheig
 - Vertical levels : surface
 - Path : 
   - on [MEOM opendap](https://github.com/AurelieAlbert/extractions/tree/main/platforms) : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/eNATL60/eNATL60-BLB002/surf/catalog.html
   - on [cal1 server](https://github.com/AurelieAlbert/extractions/blob/main/platforms/cal1.md) : /mnt/meom/workdir/alberta/eNATL60/eNATL60-BLBT02-S/1h/SSH
   - on [CINES-occigen](https://github.com/AurelieAlbert/extractions/blob/main/platforms/occigen.md) :
       - sossheig in netcdf format : /store/albert7a/eNATL60/eNATL60-BLBT02-S/1h/SSH.tar
       - sossheig in zarr format : /store/albert7a/eNATL60/zarr/eNATL60-BLBT02-SSH-1h (chunks = 240,240,480)
   - on [CNES-hal](https://github.com/AurelieAlbert/extractions/blob/main/platforms/hal.md) :
       - sossheig in netcdf format : /work/ALT/odatis/eNATL60/BLBT02/gridT-2D
       - sossheig in zarr format : /work/ALT/odatis/eNATL60/zarr/eNATL60-BLBT02-SSH-1h (chunks = 240,240,480)
       - sossheig in zarr format : /work/ALT/odatis/eNATL60/zarr/eNATL60-BLBT02-SSH-1h-mballaro (chunks = 1,4729,8354)
   - on [PANGEO cloud](https://github.com/AurelieAlbert/extractions/blob/main/platforms/pangeo.md) :                 
       - sossheig in zarr format : 
       ```
           from intake import open_catalog
           cat = open_catalog("https://raw.githubusercontent.com/pangeo-data/pangeo-datastore/master/intake-catalogs/ocean/MEOM-NEMO.yaml")
           ds  = cat["eNATL60_BLBT02_SSH"].to_dask()
       ```
   - on [Jean-Zay-IDRIS](https://github.com/AurelieAlbert/extractions/blob/main/platforms/jean-zay.md) :                 
       - sossheig in zarr format : /gpfswork/rech/yrf/rote001/eNATL60/zarr/eNATL60-BLBT02-SSH-1h.tar
   - on [DAHU-GRICAD](https://github.com/AurelieAlbert/extractions/blob/main/platforms/gricad.md) :                 
       - sossheig in zarr format : /bettik/alberta/eNATL60/zarr/eNATL60-BLBT02-SSH-1h (chunks = 240,240,480)      
