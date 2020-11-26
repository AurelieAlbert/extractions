# eNATL60-BLB002 surface velocities

 - Simulation : [eNATL60-BLB002](https://github.com/AurelieAlbert/extractions/blob/main/simulations/enatl60-blb002.md)
 - Region : [North Atlantic](https://github.com/AurelieAlbert/extractions/blob/main/regions/NATL.md)
 - Period : 01/07/2009-30/06/2010
 - Variables : somecrty, sozocrtx
 - Vertical levels : surface
 - Path : 
   - on [MEOM opendap](https://github.com/AurelieAlbert/extractions/tree/main/platforms) : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/eNATL60/eNATL60-BLB002/surf/catalog.html
   - on [cal1 server](https://github.com/AurelieAlbert/extractions/blob/main/platforms/cal1.md) : 
       - sozocrtx : /mnt/meom/workdir/alberta/eNATL60/eNATL60-BLB002-S/1h/SSU
       - somecrty : /mnt/meom/workdir/alberta/eNATL60/eNATL60-BLB002-S/1h/SSV
   - on [CINES-occigen](https://github.com/AurelieAlbert/extractions/blob/main/platforms/occigen.md) :
       - sozocrtx in netcdf format : /store/albert7a/eNATL60/eNATL60-BLB002-S/1h/SSU.tar
       - somecrty in netcdf format : /store/albert7a/eNATL60/eNATL60-BLB002-S/1h/SSV.tar
       - sozocrtx in zarr format : /store/albert7a/eNATL60/zarr/eNATL60-BLB002-SSU-1h.tar
   - on [CNES-hal](https://github.com/AurelieAlbert/extractions/blob/main/platforms/hal.md) :
       - sozocrtx in netcdf format : /work/ALT/odatis/eNATL60/BLB002/gridU-2D
       - somecrty in netcdf format : /work/ALT/odatis/eNATL60/BLB002/gridV-2D
       - sozocrtx in zarr format : /work/ALT/odatis/eNATL60/zarr/eNATL60-BLB002-SSU-1h
       - somecrty in zarr format : /work/ALT/odatis/eNATL60/zarr/eNATL60-BLB002-SSV-1h      
   - on [PANGEO cloud](https://github.com/AurelieAlbert/extractions/blob/main/platforms/pangeo.md) :                 
       - sozocrtx in zarr format : 
       ```
           from intake import open_catalog
           cat = open_catalog("https://raw.githubusercontent.com/pangeo-data/pangeo-datastore/master/intake-catalogs/ocean/MEOM-NEMO.yaml")
           ds  = cat["eNATL60_BLB002_SSU"].to_dask()
       ```
       - somecrty in zarr format : 
       ```
           from intake import open_catalog
           cat = open_catalog("https://raw.githubusercontent.com/pangeo-data/pangeo-datastore/master/intake-catalogs/ocean/MEOM-NEMO.yaml")
           ds  = cat["eNATL60_BLB002_SSV"].to_dask()
       ```
