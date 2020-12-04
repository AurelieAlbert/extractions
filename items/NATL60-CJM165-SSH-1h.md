# NATL60-CJM165 sea surface height

 - Configuration : [NATL60](../simulations/natl60.md)
 - Simulation : [NATL60-CJM165](../simulations/natl60-cjm165.md)
 - Region : [North Atlantic](../regions/NATL.md)
 - Period : 01/10/2012-30/09/2013
 - Frequency : 1h
 - Variables : sossheig
 - Vertical levels : surface
 - Path : 
   - on [MEOM opendap](../platforms/opendap.md) : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/NATL60-CJM165/1h/SSH/catalog.html
   - on [cal1 server](../platforms/cal1.md) : /mnt/meom/MODEL_SET/NATL60/NATL60-CJM165-S/1h/SSH/
   - on [CINES-occigen](../platforms/occigen.md) :
       - sossheig in netcdf format : /store/albert7a/NATL60/NATL60-CJM165-S/1h/SSH
    - on [PANGEO cloud](../platforms/pangeo.md) : https://catalog.pangeo.io/browse/master/ocean/MEOM_NEMO/NATL60_SSH/                
       - sossheig in zarr format : 
       ```
           from intake import open_catalog
           cat = open_catalog("https://raw.githubusercontent.com/pangeo-data/pangeo-datastore/master/intake-catalogs/ocean/MEOM-NEMO.yaml")
           ds  = cat["NATL60_SSH"].to_dask()
       ```
