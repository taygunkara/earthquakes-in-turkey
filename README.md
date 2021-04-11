**Research related to the earthquake in Turkey with Python.**

**The purpose of this project, learn to data manipulation. Numpy, Pandas, Matplotlib, Seaborn, Geocoder are used. http://kepler.gl/ is used for mapping.**


**All Versions**
**General Information:**

The data taken from; REPUBLIC OF TURKEY PRIME MINISTRY - Disaster & Emergency Management Authority Presidential of Earthquake Department (https://deprem.afad.gov.tr/)

The data contains 4.0 - 10 (max = 7.9) magnitudes in Turkey coordinates (latitude = between 36 - 42 ,longitude = between 26 - 45)

**Version 1:**

**Processes:**

- Read data
- Organize columns and index
- Slicing data according to mangitudes of earthquakes
- Describe of earthquakes
- Visualization of earthquakes
- Find location (place/city) from latitude and longtitude
- Re-organize data (clean out of Turkey's place, change Turkish characters )
- Find and visualize largest earthquakes in Turkey

**Version 2:**

**Processes:**

- Read data from version - 1
- Re-organize columns and create new main data
- Basic covariance and correlation analysis
- Visualizing:
    - covariance and correlation
    - distributions of earthquakes
- Descriptive statements of cities
- Basic analysis of city (Balikesir)
- Summary

**Note :** Regions were not found due to their restrictions with Geocoder. I tried to find it using the Google API, but the region information was not found. I showed in version 1 how to find it with Geocoder. If anyone wants, he/she can try and find himself. Since I do not have time, there are no regions in this version ( In addition, new information can be retrieved with the Google API and region can be found with another function). I will try to add again if I have time and update later. Another problem was the Geocoder running slowly, but it cannot be solved due to restrictions. ( It can be resolved from paid platforms like the Google API, without time restrictions.)

---

**Dataset**

**Content**

There are 5 different csv files.

- catalogue.csv is main data and there is no any changing. Columns:
  (No , Zaman (UTC), Ref1, Kaynak Aç?klama 1, Enlem, Boylam,Derinlik ,Sabit Derinlik ,Kaynak No 2, Kaynak Aç?klama 2, Kaynak Aç?klama 2, Tip, Büyüklük, Kaynak No 3, Kaynak Aç?klama 3, Yer)
- f_moderate.csv was created by me. (Magnitude = 5.0 - 5.9)
- f_strong.csv was created by me. (Magnitude = 6.0 - 6.9)
- f_major.csv was created by me. (Magnitude = 7.0 - 7.9)
- final.csv = fmoderate + fstrong + f_major

- New Columns of 2,3,4,5:
['date', 'latitude', 'longitude', 'depth', 'magnitude', 'type', 'place', 'year']

**What are the news ?**

- Organize columns and index.
- Slicing data according to mangitudes of earthquakes.
- Find location (place/city) from latitude and longtitude.
- Re-organize data (clean out of Turkey's place, change Turkish characters ,add years column)

**Acknowledgements**

The data taken from; REPUBLIC OF TURKEY PRIME MINISTRY - Disaster & Emergency Management Authority Presidential of Earthquake Department (https://deprem.afad.gov.tr/)

The data contains 4.0 - 10 (max = 7.9) magnitudes in Turkey coordinates (latitude = between 36 - 42 ,longitude = between 26 - 45)
Inspiration

I hope we can show people better analysis of earthquakes and take the earthquake seriously.

---

[Notebook in Kaggle](https://www.kaggle.com/taygunkara/earthquakes-in-turkey)
[Dataset in Kaggle](https://www.kaggle.com/taygunkara/earthquakes-of-republic-of-turkey)
