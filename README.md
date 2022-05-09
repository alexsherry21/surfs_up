# Module 9 Challenge

## Overview

In this module we used Python and Flask to assist W. Avy in evaluating the prospects of the surf and ice cream shop.

## Results

### Queries

#### Temperature

  junquery = session.query(Measurement).filter(extract('month', Measurement.date) == 6).all()

  decquery = session.query(Measurement).filter(extract('month', Measurement.date) == 12).all()
  
#### Precipitation  
  
  aprquery = session.query(Measurement).filter(extract('month', Measurement.date) == 4).all()
  
  octquery = session.query(Measurement).filter(extract('month', Measurement.date) == 10).all()
  
### Figures

#### Temperature

![June_Temps](https://user-images.githubusercontent.com/100380226/167328614-895f5f28-6857-4610-9d3b-2b0ecb554030.png)

![December_Temps](https://user-images.githubusercontent.com/100380226/167328624-3c396952-9493-4656-8804-176ce03abb0a.png)

#### Precipitation

![April_Prcp](https://user-images.githubusercontent.com/100380226/167336573-d8e47853-4ddc-4890-80b3-6773f2603fe9.png)

![October_Prcp](https://user-images.githubusercontent.com/100380226/167336579-def4a0f3-f9b5-4b22-a000-28bc462d6b9a.png)

### Major points

- Near our stations, December has a mean temperature almost four degrees lower than June
- December temperatures have roughly a half degree more of standard deviation
- December's minimum temperature of 56 is significantly lower than June's minimum temperature of 64.

## Summary

While we can see from the tables that December's temperatures vary more and are lower on average, we see that the top 75% of days are over sixty-nine degrees Fahrenheit, which is very desirable for our shop.  If about three quarters of our days are seventy degrees or warmer, we will have lots of potential traffic throughout the year.  Additionally, the max temperatures are eighty-five in June and eighty-three in December.  These upper limits are very comfortable, as once you get into the nineties it can be too hot for many people to stay outside.  We also see that in April, often known as a very rainy month, over 75% of days get a tenth of an inch of precipitation or less.  While the rainiest days max out at 6.25 inches, we will mostly have very sunny days which is good for business.  To look further we also queried precipitation in October, where the maximum was less.  The other benchmarks were pretty close to April, which is a good sign.
