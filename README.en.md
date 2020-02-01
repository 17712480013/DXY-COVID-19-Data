# 2019-nCoV Time Series Infection Data Warehouse

[简体中文](README.md) | English

2019-nCoV time series infection data warehouse, the data source is [Ding Xiang Yuan](https://3g.dxy.cn/newh5/view/pneumonia).

**Researchers**  
Recently, many college teachers and students contacted me, 
hoping to use these data for scientific research. 
However, not everyone is familiar with the use of APIs and the format of JSON, 
so here is the [data warehouse](https://github.com/BlankerL/DXY-2019-nCoV-Data) 
to publish the latest data in CSV format, 
which can be easily processed and loaded by most software.

The data is obtained by [2019-nCoV Infection Data Realtime Crawler](https://github.com/BlankerL/DXY-2019-nCoV-Crawler).

The project is under beta test, so the data will be published in every hours. 
The frequency will be adjusted in the future. 

File List：
1. Overall Data [DXYOverall.csv](https://github.com/BlankerL/DXY-2019-nCoV-Data/blob/master/DXYOverall.csv)
2. Regional Data [DXYArea.csv](https://github.com/BlankerL/DXY-2019-nCoV-Data/blob/master/DXYArea.csv)
3. News [DXYNews.csv](https://github.com/BlankerL/DXY-2019-nCoV-Data/blob/master/DXYNews.csv)
4. Rumors [DXYRumors.csv](https://github.com/BlankerL/DXY-2019-nCoV-Data/blob/master/DXYRumors.csv)

Regional data ([DXYArea.csv](https://github.com/BlankerL/DXY-2019-nCoV-Data/blob/master/DXYArea.csv))
only contains all the city-level data. 
Data from Hong Kong SAR, Macao SAR, Tai Wan and Tibet are province-level, 
and not city-level data available from DXY, so they are not in this file. 

If needed, you can modify the [dumper function](https://github.com/BlankerL/DXY-2019-nCoV-Data/blob/8e21a7e27604a9d2b1dcf0fa3d0266aa68576753/script.py#L71)
to customize your own files. 

Data customization is not accepted. 
If you have more requirements for data, please handle it on your own.

## Noise Data
At present, some time series data in Zhejiang and Hubei are found containing noises. 
The possible reason is the manually processed data were recorded by mistake. 

The crawler just crawl what it sees, do not deal with any noise data. 
Therefore, if you use the data for scientific research, please preprocess and clean the data properly. 

In the meantime, I opened an [issue](https://github.com/BlankerL/DXY-2019-nCoV-Crawler/issues/34) 
for you to report the potential noise data. I will check and remove them periodically. 

**Wish you all the best.**
