* Frankly, I didn't need to write a code to test the model as the original repository contains the whole needed codes, i.e., inference code for images, videos, and webcams.
* However, I designed some corner cases to test the model robustness. i.e., crowded, night, synthetic, and blurred scenes.

# <font color='blue'>YOLOX Visualizations:</font>
* The whole reported results are produced using YOLOX-S.
* The failure cases only is studied again using YOLOX-X as it is the most powerful variant.

------------------
## Crowded Scenes:
| Input             |  Output |
:-------------------------:|:-------------------------:
![](assets/corner_cases_images/crowded/2.jpg)  |  ![](assets/corner_cases_images/crowded/out_2.jpg)
![](assets/corner_cases_images/crowded/3.jpg)  |  ![](assets/corner_cases_images/crowded/out_3.jpg)
![](assets/corner_cases_images/crowded/4.jpg)  |  ![](assets/corner_cases_images/crowded/out_4.jpg)

### <font color='red'>Failure cases:</font>
| Input             |  Output-S |   Output-X |
:-------------------------:|:-------------------------:|:-------------------------:
![](assets/corner_cases_images/crowded/5.jpg)  |  ![](assets/corner_cases_images/crowded/out_5.jpg)|  ![](assets/corner_cases_images/crowded/out_x5.jpg)
![](assets/corner_cases_images/crowded/6.jpg)  |  ![](assets/corner_cases_images/crowded/out_6.jpg)|  ![](assets/corner_cases_images/crowded/out_x6.jpg)

------------------
## Night Scenes:
| Input             |  Output |
:-------------------------:|:-------------------------:
![](assets/corner_cases_images/night/1.jpg)  |  ![](assets/corner_cases_images/night/out1.jpg)

### <font color='red'>Failure cases:</font>
| Input             |  Output-S |Output-X |
:-------------------------:|:-------------------------:|:-------------------------:
![](assets/corner_cases_images/night/1.jpeg)  |  ![](assets/corner_cases_images/night/out_1.jpeg)|  ![](assets/corner_cases_images/night/out_x1.jpeg)


------------------
## Synthetic Scenes:
| Input             |  Output |
:-------------------------:|:-------------------------:
![](assets/corner_cases_images/synthetic/1.jpg)  |  ![](assets/corner_cases_images/synthetic/out_1.jpg)
![](assets/corner_cases_images/synthetic/2.jpeg)  |  ![](assets/corner_cases_images/synthetic/out_2.jpeg)
![](assets/corner_cases_images/synthetic/3.jpg)  |  ![](assets/corner_cases_images/synthetic/out_3.jpg)
![](assets/corner_cases_images/synthetic/4.jpg)  |  ![](assets/corner_cases_images/synthetic/out_4.jpg)
![](assets/corner_cases_images/synthetic/8.jpg)  |  ![](assets/corner_cases_images/synthetic/out_8.jpg)
![](assets/corner_cases_images/synthetic/7.jpg)  |  ![](assets/corner_cases_images/synthetic/out_7.jpg)

### <font color='red'>Failure cases:</font>
| Input             |  Output-S |  Output-X |
:-------------------------:|:-------------------------:|:-------------------------:
![](assets/corner_cases_images/synthetic/5.jpg)  |  ![](assets/corner_cases_images/synthetic/out_5.jpg)|  ![](assets/corner_cases_images/synthetic/out_x5.jpg)
![](assets/corner_cases_images/synthetic/6.jpg)  |  ![](assets/corner_cases_images/synthetic/out_6.jpg)|  ![](assets/corner_cases_images/synthetic/out_x6.jpg)

------------------
## Blurring Scenes:
| Input             |  Output |
:-------------------------:|:-------------------------:
![](assets/corner_cases_images/bluring/3.jpg)  |  ![](assets/corner_cases_images/bluring/out_3.jpg)
![](assets/corner_cases_images/bluring/5.jpg)  |  ![](assets/corner_cases_images/bluring/out_5.jpg)

### <font color='red'>Failure cases:</font>
| Input             |  Output-S | Output-X |
:-------------------------:|:-------------------------:|:-------------------------:
![](assets/corner_cases_images/bluring/2.jpeg)  |  ![](assets/corner_cases_images/bluring/out_2.jpeg)  |  ![](assets/corner_cases_images/bluring/out_x2.jpeg)
![](assets/corner_cases_images/bluring/4.jpeg)  |  ![](assets/corner_cases_images/bluring/out_4.jpeg)  |  ![](assets/corner_cases_images/bluring/out_x4.jpeg)

# <font color='blue'>Quick Insights from Results:</font>
* In general, YOLOX-small surprisingly performs well in difficult situations like synthetic, night, crowded, and blurring.
* YOLOX-X-Large has boosted the performance in the night and blurring failure cases, however still fails, or maybe we can say perform worse than the small version on synthetic and crowded scenes.

# <font color='green'>Steps to solve the task with an approximated time for each step:</font>
| Steps             |  Approximated time |
:-------------------------:|:-------------------------:
Skim YOLOX report          |     30 Mins
Read YOLOX report in details and create the mind map          |     2.5 Hours
Read OTA[4] paper          |     1 Hours
Clone the code and create an anaconda environment          |     30 Mins
Design and run my testcases and write the readme          |     2.5 Hours


# <font color='green'>Criticising the paper:</font>
[Please refer to this mind map](https://mm.tt/1992748152?t=SWCMNTa0P7)

