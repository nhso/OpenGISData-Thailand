# OpenGISData-Thailand
Open GIS Data Sources in Thailand

## เป็นไฟล์รูปแบบ geojson มีทั้งหมด 3 ไฟล์คือ
- ชั้นข้อมูลขอบเขตจังหวัด 77 จังหวัด (provinces.geojson)
- ชั้นข้อมูลขอบเขตอำเภอ 928 อำเภอ (districts.geojson)
- ชั้นข้อมูลขอบเขตตำบล 7367 ตำบล (subdistricts.geojson)
- ชั้นข้อมูลขอบเขตภูมิภาค 7 ภูมิภาค (region_royin.geojson)
- ชั้นข้อมูลขอบเขตภูมิภาค 6 ภูมิภาค (region_nesdb.geojson)

## Data dictionary
**provinces**

|Field |Type |Key|Description |
|----------------|-------------------------------|-----------------------------|-----------------------------|
|gid|Integer(10)|PK|gid|
|tam_code|String(6)||รหัสตำบล|
|tam_th|String(254)||ชื่อตำบลภาษาไทย|
|tam_en|String(254)||ชื่อตำบลภาษาอังกฤษ|
|amp_code|String(4)||รหัสอำเภอ|
|amp_th|String(254)||ชื่ออำเภอภาษาไทย|
|amp_en|String(254)||ชื่ออำเภอภาษาอังกฤษ|
|pro_code|String(2)||รหัสจังหวัด|
|pro_th|String(254)||ชื่อจังหวัดภาษาไทย|
|pro_en|String(254)||ชื่อจังหวัดภาษาอังกฤษ|
|reg_nesdb|String(254)||เขตภูมิภาค|
|reg_royin|String(254)||เขตภูมิภาค|
|perimeter|Real(18,11)||เส้นรอบรูป กิโลเมตร|
|area_sqkm|Real(18,11)||เนื้อที่ ตารางกิโลเมตร|


----------


**districts**

|Field |Type |Key|Description |
|----------------|-------------------------------|-----------------------------|-----------------------------|
|amp_code|String(4)|PK|รหัสอำเภอ|
|amp_th|String(254)||ชื่ออำเภอภาษาไทย|
|amp_en|String(254)||ชื่ออำเภอภาษาอังกฤษ|
|pro_code|String(2)||รหัสจังหวัด|
|pro_th|String(254)||ชื่อจังหวัดภาษาไทย|
|pro_en|String(254)||ชื่อจังหวัดภาษาอังกฤษ|
|reg_nesdb|String(254)||เขตภูมิภาค|
|reg_royin|String(254)||เขตภูมิภาค|
|perimeter|Real(18,11)||เส้นรอบรูป กิโลเมตร|
|area_sqkm|Real(18,11)||เนื้อที่ ตารางกิโลเมตร|

----------

**subdistricts**

|Field |Type |Key|Description |
|----------------|-------------------------------|-----------------------------|-----------------------------|
|pro_code|String(2)|PK|รหัสจังหวัด|
|pro_th|String(254)||ชื่อจังหวัดภาษาไทย|
|pro_en|String(254)||ชื่อจังหวัดภาษาอังกฤษ|
|reg_nesdb|String(254)||เขตภูมิภาค|
|reg_royin|String(254)||เขตภูมิภาค|
|perimeter|Real(18,11)||เส้นรอบรูป กิโลเมตร|
|area_sqkm|Real(18,11)||เนื้อที่ ตารางกิโลเมตร|

----------

**region_royin**

|Field |Type |Key|Description |
|----------------|-------------------------------|-----------------------------|-----------------------------|
|reg_royin|String(254)||เขตภูมิภาค|
|perimeter|Real(18,11)||เส้นรอบรูป กิโลเมตร|
|area_sqkm|Real(18,11)||เนื้อที่ ตารางกิโลเมตร|

----------

**region_nesdb**

|Field |Type |Key|Description |
|----------------|-------------------------------|-----------------------------|-----------------------------|
|reg_nesdb|String(254)||เขตภูมิภาค|
|perimeter|Real(18,11)||เส้นรอบรูป กิโลเมตร|
|area_sqkm|Real(18,11)||เนื้อที่ ตารางกิโลเมตร|

----------

## แหล่งอ้างอิงข้อมูลอื่นๆ 

- [Data Go : 0205_01_0301](https://data.go.th/dataset/0205_01_0301)
- [Data Thailand : Thailand Provincial Boundaries](https://data.thailand.opendevelopmentmekong.net/th/dataset/thailand-provincial-boundaries)
- [Data Humdata : COD-AB-THA](https://data.humdata.org/dataset/cod-ab-tha?)
- [ThaiGeographers Facebook Post](https://www.facebook.com/ThaiGeographers/posts/%E0%B9%81%E0%B8%9A%E0%B9%88%E0%B8%87%E0%B8%9B%E0%B8%B1%E0%B8%99-shapefile-%E0%B8%88%E0%B8%B2%E0%B8%81-openstreetmap-%E0%B8%97%E0%B8%B1%E0%B9%89%E0%B8%87%E0%B8%9B%E0%B8%A3%E0%B8%B0%E0%B9%80%E0%B8%97%E0%B8%A8%E0%B9%84%E0%B8%97%E0%B8%A2buildings-landuse-water-roads-e/4623659161012952/?locale=hi_IN)
- [GitHub - prasertcbs/thailand_gis](https://github.com/prasertcbs/thailand_gis)
- Test Script -> https://github.com/AhmedKhaled8/Visualizing-Geospatial-Data-in-Python

## Acknowledgement

This project includes major parts that have been forked from [OpenGISData-Thailand](https://github.com/chingchai/OpenGISData-Thailand). We would like to express our gratitude for their valuable contributions and the open sharing of their GIS data. Their work has been instrumental in the development of this project. We recommend visiting their repository for more information and resources related to GIS data in Thailand.

## Contact Information

For more information, please contact:

- Thanasak: [Thanasak.t@nhso.go.th](mailto:Thanasak.t@nhso.go.th)
- Pariyat: [pariyat.l@nhso.go.th](mailto:pariyat.l@nhso.go.th)
