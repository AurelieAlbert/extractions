# eNATL60-BLBT02 surface velocities

 - Configuration : [eNATL60](../simulations/enatl60.md)
 - Simulation : [eNATL60-BLBT02](../simulations/enatl60-blbt02.md)
 - Region : [North Atlantic](../regions/eNATL.md)
 - Period : 01/07/2009-30/06/2010
 - Frequency : 1h
 - Variables : somecrty, sozocrtx
 - Vertical levels : surface
 - Path : 
   - on [MEOM opendap](../platforms/opendap.md) : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/eNATL60/eNATL60-BLBT02/surf/catalog.html
   - on [cal1 server](../platforms/cal1.md) : 
       - sozocrtx : /mnt/meom/workdir/alberta/eNATL60/eNATL60-BLBT02-S/1h/SSU
       - somecrty : /mnt/meom/workdir/alberta/eNATL60/eNATL60-BLBT02-S/1h/SSV
   - on [CINES-occigen](../platforms/occigen.md) :
       - sozocrtx in netcdf format : /store/albert7a/eNATL60/eNATL60-BLBT02-S/1h/SSU.tar
       - somecrty in netcdf format : /store/albert7a/eNATL60/eNATL60-BLBT02-S/1h/SSV.tar
       - sozocrtx in zarr format : /store/albert7a/eNATL60/zarr/eNATL60-BLBT02-SSU-1h.tar
   - on [CNES-hal](../platforms/hal.md) :
       - sozocrtx in netcdf format : /work/ALT/odatis/eNATL60/BLBT02/gridU-2D
       - somecrty in netcdf format : /work/ALT/odatis/eNATL60/BLBT02/gridV-2D
       - sozocrtx in zarr format : /work/ALT/odatis/eNATL60/zarr/eNATL60-BLBT02-SSU-1h
       - somecrty in zarr format : /work/ALT/odatis/eNATL60/zarr/eNATL60-BLBT02-SSV-1h      
   - on [PANGEO cloud](../platforms/pangeo.md) :                 
       - sozocrtx in zarr format : 
       ```
           from intake import open_catalog
           cat = open_catalog("https://raw.githubusercontent.com/pangeo-data/pangeo-datastore/master/intake-catalogs/ocean/MEOM-NEMO.yaml")
           ds  = cat["eNATL60_BLBT02_SSU"].to_dask()
       ```
       - somecrty in zarr format : 
       ```
           from intake import open_catalog
           cat = open_catalog("https://raw.githubusercontent.com/pangeo-data/pangeo-datastore/master/intake-catalogs/ocean/MEOM-NEMO.yaml")
           ds  = cat["eNATL60_BLBT02_SSV"].to_dask()
       ```
