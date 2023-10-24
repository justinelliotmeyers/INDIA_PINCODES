# Shapefiles for Pincodes of India

For anyone having issues converting these to geojson

On unix/OSx :
cat india_pincodes.shp.z01 > india_pincodes_full.shp.zip
cat india_pincodes.shp.z02 >> india_pincodes_full.shp.zip
cat india_pincodes.shp.z03 >> india_pincodes_full.shp.zip
cat india_pincodes.shp.z04 >> india_pincodes_full.shp.zip
cat india_pincodes.shp.z05 >> india_pincodes_full.shp.zip
cat india_pincodes.shp.zip >> india_pincodes_full.shp.zip
unzip india_pincodes_full.shp.zip
unzip india_pincodes.cpg.zip
unzip india_pincodes.prj.zip
unzip india_pincodes.sbx.zip
unzip india_pincodes.dbf.zip
unzip india_pincodes.sbn.zip
unzip india_pincodes.shx.zip

Converting to GeoJSON:
ogr2ogr -f GeoJSON india_pincodes_full.geojson india_pincodes_full.shp
