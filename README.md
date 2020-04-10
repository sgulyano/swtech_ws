# swtech_ws
Contain notebooks and script for demonstrating folium and tensorflow/keras in GIS application. 

----
## Setup

1. Create Python virtual environment
    ```
    conda env create -f environment.yml
    ```

2. Check that the virtual environment is created successfully by showing all virtual environment in the computer
    ```
    conda info --envs
    ```

3. Select the virtual environment we want
    ```
    conda activate myenv
    ```

4. Make the virtual environment available in the Jupyter by first install the ipykernel
    ```
    conda install ipykernel
    ```

5. Second, register the virtual environment to the Jupyter
    ```
    python -m ipykernel install --user --name=myenv
    ```

6. Some functionality requires folium version 0.10.1, which is not in PyPi so we cannot install it using `pip install folium`. To  install folium 0.10.1, use this script instead (for now, in the future you should be able to install with the previous command). 
    ```
    pip install git+https://github.com/python-visualization/folium.git
    ```


If some errors occurred, you can update your virtual environment again using this command:
```
conda env update –f environment.yml –n myenv
```

If you want to remove the virtual environment, use this command:
```
conda remove --name myenv --all
```

If you want to deselect the virtual environment, use this command:
```
conda deactivate
```

----
## Tutorial
1. [Flood data](https://github.com/sgulyano/swtech_ws/blob/master/flood_viz.ipynb)
2. [Drought data](https://github.com/sgulyano/swtech_ws/blob/master/drought_viz.ipynb)
3. [Satellite Visualization 1](https://github.com/sgulyano/swtech_ws/blob/master/sat_viz1.ipynb)
4. [Satellite Visualization 2](https://github.com/sgulyano/swtech_ws/blob/master/sat_viz2.ipynb)
5. [Satellite Visualization with Time Series](https://github.com/sgulyano/swtech_ws/blob/master/sat_viz_time.ipynb)