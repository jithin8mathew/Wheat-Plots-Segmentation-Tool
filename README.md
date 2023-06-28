# Wheat-Plots-Segmentation-Tool
A plot segmentation tool for Wheat experimental plot segmentation captured with UAVs.

![](app.gif)

<h3>Wheat Plots Segmentation Tool</h3> <p> is a Python based tool intended for faster dataset creation using a simple GUI. Data captured from drones can be exceedingly huge in terms of Memory. This tool aims at segmenting a large wheat field into smaller individual plots using Python 3 and OpenCV 4.</p>

The cropping can be performed using one of the 3 methods incorported into the tool:

<ol>
  <li> Manual segmentation by selecting the Region of interest</li>
  <li> Semi-manual segmentation where the user inputs the number of subplots a field has and selectes the Region of iterest by clicking and draging the co-ordinates on the image. A grid is drawn in the image indicating individual plots which are automatically cropped and saved upon the click of download button</li>
  <li>Semi-automatic segemntation: User selects the image, filters the color based on the upper and lower RGB values, apply vertical and hoirzontal masks, finally automatic box detection is performed to find the plots. User can save the segmented output to local flolder using save ROI button</li>
</ol>

In adition to the above, images can be corrected by performing a rotation method to align the image to its position

<br>

![Method1](https://github.com/jithin8mathew/Small-Grain-Plots-Segmentation-Tool/blob/main/images/Method1.jpg)
Format: ![](url)

<br>

### Running the file

The code can be run after downloading the requirememts.txt packages by opeing the console and running:

```python 
python deploy.py

or 

python Geotif_tool.py
```
<p><i>**Image processing is performed using CPU, therefore larger files tend to take longer time to upload, process and display. Further improvements will be made in the future updated versions.</i></p>
