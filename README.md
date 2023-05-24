# snowcover_products

The snow surface is quite straightforward to detect from high resolution optical imagery. Discriminating cloud and snow pixels is the challenging part in snow cover mapping. 

## Potential products for snowcover

| Data Source | Name | Spatial Resolution | Spatial Domain | Timeliness | Period | Link | More Info |
|-------------|------|--------------------|----------------|------------|--------|------|-----------|
| Copernicus Global Land Service | Fractional Snow Cover (FSC) and Gap-Filled Fractional Snow Cover (GFSC) | | | | | [Snow Cover](https://land.copernicus.eu/pan-european/biophysical-parameters/high-resolution-snow-and-ice-monitoring/snow-products/snow-cover) | Just provide information about the Sentinel-2 L1C and L2A products |
| EUMETSAT    | SN-OBS-1 (Snow detection (snow mask) by VIS/IR radiometry) | 1 to 5 km | ~Europe| 6h | mid-November 2007 - today | [Snow Products](https://hsaf.meteoam.it/Products/ProductsList?type=snow) | Format: HDF5 and PNG. Instrument: SEVIRI |
| EUMETSAT    | SN-OBS-3 (Effective snow cover by VIS/IR radiometry) | | ~EUROPE | | | | Instrument: AVHRR/3, **MODIS** | 
| VIIRS       | VNP10A1F (Snow Cover Cloud-Gap-Filled Daily L3 Global 375m SIN Grid) | 375m | Global | 1day | 19 January 2012 to present | [VNP10A1F](https://nsidc.org/data/vnp10a1f/versions/1) | Format: HDF-EOS5. Instrument: VIIRS |
| MODIS       | MOD10A1 (Terra) &	MYD10A1 (AQUA) (MODIS Snow Cover Daily L3 Global 500m Grid) | 500m | Global | | | [MODIS Snow Cover](https://modis.gsfc.nasa.gov/data/dataprod/mod10.php) | Instrument: MODIS |
| Sentinel-2  | 


## Algorithms

Most of the algorithms are based on the normalized-difference snow index (NDSI) and a digital elevation model



## Notes

### EUMETSAT

More snow-cover products from EUMETSAT: [available here](https://hsaf.meteoam.it/Products/ProductsList?type=snow)

### NDSI

The Normalized Difference Snow Index (NDSI) snow cover is an index that is related to the presence of snow in a pixel and is a more accurate description of snow detection as compared to Fractional Snow Cover (FSC). Snow typically has very high visible (VIS) reflectance and very low reflectance in the shortwave infrared (SWIR), a characteristic used to detect snow by distinguishing between snow and most cloud types. Snow cover is detected using the NDSI ratio of the difference in VIS and SWIR reflectance; NDSI = ((band 4-band 6) / (band 4 + band 6)). A pixel with NDSI > 0.0 is considered to have some snow present. A pixel with NDSI <= 0.0 is a snow free land surface (Riggs et al., 2016).   

## References

- [Let-It-Snow](file:///E:/fioragu/Downloads/ATBD_CES-Neige.pdf)

- Riggs, George A., Dorothy K. Hall, and Miguel O. Román. 2015. VIIRS Snow Cover Algorithm Theoretical Basis Document.


