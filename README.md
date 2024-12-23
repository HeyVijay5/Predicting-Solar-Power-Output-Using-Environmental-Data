<h2 align=center> Predicting Solar Power Output Using Environmental Data </h2>


### Predicting Solar Power Output Using Environmental Data  

This project focuses on predicting the power output of a solar plant using environmental factors. Solar power forecasting plays a vital role in ensuring the smooth operation and control of solar plants. Power generation depends not only on the design and doping level of photovoltaic (PV) arrays but also on key environmental factors such as solar radiation, temperature, humidity, and dust accumulation. These parameters are naturally variable, influencing the energy output.  

Since solar irradiance and environmental conditions fluctuate throughout the day, periodic measurements (e.g., hourly averages) provide better insights for accurate predictions. A higher sampling rate leads to more precise forecasts of power output for PV modules and solar plants.  

### Dataset Overview  

The dataset includes the following features:  
- **distance-to-solar-noon**: Angular distance to solar noon in radians.  
- **temperature**: Daily average temperature in degrees Celsius.  
- **wind-direction**: Daily average wind direction in degrees (0-360).  
- **wind-speed**: Daily average wind speed in meters per second.  
- **sky-cover**: Sky conditions on a scale from 0 (clear) to 4 (fully covered).  
- **visibility**: Visibility in kilometers.  
- **humidity**: Daily average humidity in percentage.  
- **average-wind-speed-(period)**: Wind speed during the 3-hour period, in meters per second.  
- **average-pressure-(period)**: Barometric pressure during the 3-hour period, in mercury inches.  
- **power-generated**: Energy generated in joules for each 3-hour period.  

### Dependencies  

The project uses the following tools and libraries:  
- **Python 3.8**  
- **Pandas**  
- **TensorFlow 2.2**  
- **Keras**  
- **Matplotlib**  
- **Seaborn**  
- **NumPy**  

Model Architecture
--------
<p float="left">
  <img src="results/Network%20Architecture.png" alt="drawing" width="500"/>
  <img src="results/spfnet_model.png" alt="drawing" width="300"/>
</p>

Results
-------
<p float="left">
  <img src="results/train%20pred%20vs%20real%20data.png" alt="drawing" width="400"/>
  <img src="results/test%20pred%20vs%20real%20data.png" alt="drawing" width="400"/>
</p>

- lasso regressor feature importance

![alt](results/lasso%20regressor%20feature%20importance.png)

| Evaluation Parameter  | Value  |
| --------- | -------|
|R2 Score of Whole Data Frame	|0.881888|
|R2 Score of Training Set|	0.921727|
|R2 Score of Test Set|	0.767884|
|Mean of Test Set|	1204.179810|
|Standard Deviation of Test Set	|930.158020|
|Relative Standard Deviation	|0.772441|

Refrences
------
- [Neural Designer](https://www.neuraldesigner.com/)
- [Get Data](https://www.neuraldesigner.com/files/datasets/solarpowergeneration.csv)
