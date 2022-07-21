# phasenet_demo
Demonstration of PhaseNet for volcanic seismicity, presented as part of the ML in Seismology Summer Group 2022. 

https://github.com/wayneweiqiang/PhaseNet

Zhu, W. and Beroza, G.C., 2019. PhaseNet: a deep-neural-network-based seismic arrival-time picking method. Geophysical Journal International, 216(1), pp.261-273.


### 1) Download data
To run this notebook, you'll need some waveform data. PhaseNet takes in data in csv, hdf5 or miniseed file formats. If you do not have any local data to access then you can download a sample of data to run these notebooks. I use the ObsPy client to download data, and there is an example of how to do this in `demo/prepare_mseed_files`.

My notebook is using seismic data from the IGUANA network at Sierra Negra volcano, Galapagos. This is freely available for download from IRIS. Within the data download notebook, you can change the variables to any network and any stations and any time interval (minutes, hours, seconds) that you are interested in. This notebook is adapted from a demo jupyter notebook available in the PhaseNet repository. It will download and create the correct file names and types to run the examples here and in the PhaseNet repository. 

For more information on the IGUANA network, please see here: http://www.fdsn.org/networks/detail/8G_2018/

You can see information about any other networks here: http://www.fdsn.org/networks/


### 2) Sample notebook

I have provided a walk through of the PhaseNet methods at Sierra Negra on IGUANA stations SN07 and SN14. I have demonstrated two methods to execute PhaseNet:
- Through the QuakeFlow API
- Through your terminal

### 3) Work in progress
This was very much in the **experimenting** stage when presented so there's a few things that aren't working yet. Please feel free to edit and bug fix at leisure! For instance, this notebook uses the pretrained model provided by PhaseNet and I'm still a little unsure about how to train a network. 
