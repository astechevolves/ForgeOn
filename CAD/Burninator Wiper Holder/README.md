The original docking params come through a little bit high for the wiper. 

The original numbers as delviered look like this

```
params_dropoff_path: [{'y':9.5 ,'z':4}, {'y':9.5, 'z':2}, {'y':5.5, 'z':0}, {'z':0, 'y':0, 'f':0.5}, {'z':-10, 'y':0}, {'z':-10, 'y':16}]
params_pickup_path: [{'z':-10, 'y':16}, {'z':-10, 'y':0}, {'z':0, 'y':0, 'f':0.5, 'verify':1}, {'y':5.5, 'z':0}, {'y':9.5, 'z':2}, {'y':9.5 ,'z':4}]
```

The magic values to get a little wipe ont he way in and on the way out is the First Z on drop of and the last Z on pickup. I changed them both from 4 to 2 so it wipes directly across the silicone pad instead of coming up high just across the top of the wiper. 

```
params_dropoff_path: [{'y':9.5 ,'z':2}, {'y':9.5, 'z':2}, {'y':5.5, 'z':0}, {'z':0, 'y':0, 'f':0.5}, {'z':-10, 'y':0}, {'z':-10, 'y':16}]
params_pickup_path: [{'z':-10, 'y':16}, {'z':-10, 'y':0}, {'z':0, 'y':0, 'f':0.5, 'verify':1}, {'y':5.5, 'z':0}, {'y':9.5, 'z':2}, {'y':9.5 ,'z':2}]
```

In order to tune this the Dock_Tuner Macros work great to come at them slowly and test you height requirements with minimal carnage. 