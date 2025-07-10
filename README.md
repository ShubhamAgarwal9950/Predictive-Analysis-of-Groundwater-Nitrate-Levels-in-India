
Selected Parameters 
1. EC (µS/cm at) — Electrical Conductivity 
Indicates the amount of dissolved salts in groundwater. High EC often correlates with increased 
nitrate levels, especially in areas affected by fertilizers or septic runoff. 
2. pH GW — Groundwater pH 
pH influences nitrate solubility and microbial activity. Neutral to alkaline pH levels may stabilize 
nitrate, while low pH may enhance denitrification (reducing NO₃). 
3. PET (Potential Evapotranspiration) 
Reflects the potential for water loss due to evaporation and plant uptake. High PET can 
concentrate nitrates in shallow aquifers by reducing dilution through water loss. 
4. AET (Actual Evapotranspiration) 
Actual water loss from soil and vegetation. Lower AET may indicate reduced biological nitrate 
uptake, leading to accumulation in groundwater. 
5. Precip (Precipitation) 
Major factor in leaching nitrate from surface to groundwater. Moderate rainfall can flush 
nitrates into the water table; excessive rainfall can dilute it. 
6. Aridity 
Ratio of precipitation to evapotranspiration; indicates how dry a region is. High aridity often 
leads to nitrate buildup due to low leaching and high evaporation. 
7. Alpha_Priestley_Taylor 
A climate coefficient for estimating PET. Affects nitrate mobility indirectly by controlling soil 
moisture and plant water use. 
8. Latitude_1 
Geographic position — indirectly reflects climatic zones and agricultural intensity. Areas closer 
to certain latitudes may have higher fertilizer use or irrigation, affecting nitrate loading. 
9. Longitude_1 
Works together with latitude to identify spatial patterns. Helps detect regional differences in 
soil, geology, and land use that influence nitrate levels. 
10. Silt_Subsoil 
Soil texture parameter — influences water retention and nitrate transport. High silt content can 
slow water movement, allowing nitrate to accumulate in shallow zones. 
11. Fluvisols 
A soil type found in river floodplains and alluvial deposits. Often associated with shallow water 
tables and high agricultural activity — prone to nitrate pollution. 
How I get these 11 parameters 
1. Parameter having lot of missing values we had not included that 
2. Correlation Analysis helped detect features with direct linear relationships with nitrate.  
3. Trained a Random Forest Regressor to evaluate the non-linear predictive power of each 
feature. 
4. Used RFE with Random Forest to iteratively eliminate less significant features. 
