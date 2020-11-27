# eNATL60 grid files

 - Configuration : [eNATL60](https://github.com/AurelieAlbert/extractions/blob/main/simulations/enatl60.md)
 - Region : [North Atlantic](https://github.com/AurelieAlbert/extractions/blob/main/regions/NATL.md)
 - Variables : grid variables
 - Path : 
   - on [MEOM opendap](https://github.com/AurelieAlbert/extractions/tree/main/platforms) : 
      - coordinate file : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/eNATL60/eNATL60-I/catalog.html?dataset=meomscanpublic/eNATL60/eNATL60-I/coordinates_eNATL60.nc
      - mesh mask : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/eNATL60/eNATL60-I/catalog.html?dataset=meomscanpublic/eNATL60/eNATL60-I/mesh_mask_eNATL60.nc
      - bathymetry : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/eNATL60/eNATL60-I/catalog.html?dataset=meomscanpublic/eNATL60/eNATL60-I/bathymetry_eNATL60.nc
   - on [cal1 server](https://github.com/AurelieAlbert/extractions/blob/main/platforms/cal1.md) : 
      - coordinate file : /mnt/meom/MODEL_SET/eNATL60/eNATL60-I/eNATL60_coordinates_v3.nc4
      - mesh mask : /mnt/meom/MODEL_SET/eNATL60/eNATL60-I/mesh_mask_eNATL60_3.6.nc
      - bathymetry : /mnt/meom/MODEL_SET/eNATL60/eNATL60-I/eNATL60_BATHY_GEBCO_2014_2D_msk_v3.1_lb.nc4
   - on [CINES-occigen](https://github.com/AurelieAlbert/extractions/blob/main/platforms/occigen.md) :
      - coordinate file : /store/CT1/hmg2840/lbrodeau/eNATL60/eNATL60-I/eNATL60_coordinates_v3.nc4
      - mesh mask : /store/CT1/hmg2840/lbrodeau/eNATL60/eNATL60-I/mesh_mask_eNATL60_3.6.nc
      - bathymetry : /store/CT1/hmg2840/lbrodeau/eNATL60/eNATL60-I/eNATL60_BATHY_GEBCO_2014_2D_msk_v3.1_lb.nc4
   - on [CNES-hal](https://github.com/AurelieAlbert/extractions/blob/main/platforms/hal.md) :
      - mesh mask : /work/ALT/odatis/eNATL60/mesh_mask_eNATL60_3.6.nc
   - on [PANGEO cloud](https://github.com/AurelieAlbert/extractions/blob/main/platforms/pangeo.md) :                 
      - mesh mask : https://catalog.pangeo.io/browse/master/ocean/MEOM_NEMO/eNATL60_grid/
       ```
        from intake import open_catalog
        cat = open_catalog("https://raw.githubusercontent.com/pangeo-data/pangeo-datastore/master/intake-catalogs/ocean/MEOM-NEMO.yaml")
        ds  = cat["eNATL60_grid"].to_dask()      
        ```
