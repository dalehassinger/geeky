---
title: "vRealize Operations 8.x - New Features"
description: "description"
image: "images/post/vro.png"
date: 2021-02-20T00:00:00-05:00
categories: ["vRealize Operations"]
tags:
- vROPS
- vRealize Operations
- Donut Charts
- Top-N Charts
- Ping Monitoring
type: "regular" # available types: [featured/regular]
draft: false
---

<div>
  <b>The New vRealize Operations Features I use the most.</b>
</div>
<div>
  <br>
</div>

---

1. <b>Donut Charts.</b>
   * This is one of my favorite new features.
   * The donut chart allows you to show a lot of information in a smaller space and makes the Dashboards look more modern and clean looking.
   * I have been replacing the Heat Map Widgets on some of my custom Dashboards with Donut Charts.
   * If you click on the colors of the Donut charts you will then get a list of the data that makes up that color.
2. <b>Top-N Chart and Color Method.</b>
   * Adding color to the Top-N makes it so much more usable. With the previous version where is was just blue it didn't grab your eye like adding the color.
   * Using the Top-N chart and the Donut chart together makes a GREAT looking Dashboard. See my example below.
3. <b>Ping Monitoring.</b>
   * This feature always us to monitor non VMware devices. In a short period of time I learned a lot about latency and packet drops in our environment.
4. <b>Troubleshooting Workbench.</b>
   * In previous versions of vROPS I would create Dashboards to help with trouble shooting.
   * With Trouble Shooting work bench I don't need to create those custom Dashboards anymore.
   * The included Trouble Shooting workbench is like what I did on steroids.

###### Donut Chart and Top-N Example:

{{< image title="" w="" h="" o="webp q1" p="center" c="rounded" src="images/post/vrops8-01.png" >}}
<a href="https://github.com/dalehassinger/geeky/raw/main/assets/images/post/vrops8-01.png" target="_blank">Click Here to see Larger Image of Screen Shot</a>


This single Dashboard has a lot of info that would has taken several Dashboards to show same amount of data using Heat Maps. This would be a good example of a Dashboard that managers may want to see.

{{< image title="" w="" h="" o="webp q1" p="center" c="rounded" src="images/post/vrops8-05.png" >}}
<a href="https://github.com/dalehassinger/geeky/raw/main/assets/images/post/vrops8-05.png" target="_blank">Click Here to see Larger Image of Screen Shot</a>


###### Donut Chart Config:
* Create a Distribution View. 
* Make the visualization a Donut Chart. 
* Use Manual distribution.
* Create Buckets and set the values/colors for the Buckets.
* Add the View to a Dashboard.

{{< image title="" w="" h="" o="webp q1" p="center" c="rounded" src="images/post/vrops8-02.png" >}}
<a href="https://github.com/dalehassinger/geeky/raw/main/assets/images/post/vrops8-02.png" target="_blank">Click Here to see Larger Image of Screen Shot</a>

{{< image title="" w="" h="" o="webp q1" p="center" c="rounded" src="images/post/vrops8-03.png" >}}
<a href="https://github.com/dalehassinger/geeky/raw/main/assets/images/post/vrops8-03.png" target="_blank">Click Here to see Larger Image of Screen Shot</a>

###### Top-N Chart Config:
* Add Top-N Widget to Dashboard
* Define configuration and Input Transformation.
* Output Data:Color Method:Custom is where you define the color values.

{{< image title="" w="" h="" o="webp q1" p="center" c="rounded" src="images/post/vrops8-04.png" >}}
<a href="https://github.com/dalehassinger/geeky/raw/main/assets/images/post/vrops8-04.png" target="_blank">Click Here to see Larger Image of Screen Shot</a>
