# Steps to Implement Into DFP

# Index

- [1. Prepare Hike-DFP tag](#HikeTag)
- [2. Set ad unit](#unit)
- [3. Set order](#order)
  - [3-1. In "Advertiser", select "Add a new company"](#order1)
  - [3-2. Input Name and Sizes](#order2)
  - [3-3. Set delivery schedule/delivery rate/goal](#order3)
  - [3-4. Select "Save and Upload creatives"](#order4)
- [4. Set creative](#creative)
- [5. Create DFP tag](#DFPTag)
  - [5-1. Select ad unit](#DFPTag1)
  - [5-2. Select tag type (Web/App)](#DFPTag2)
  - [5-3. Set tag options](#DFPTag3)
  - [5-4. Tag will be generated](#DFPTag4)
- [6. Implement DFP tag](#ImplementTag)
- [7. Start delivery](#delivery)

<a name="HikeTag"></a>
# 1. Prepare Hike-DFP tag
Create Hike tag for DFP with the documents below.

https://github.com/mtburn/MTBurn-JavaScript-SDK-Install-Guide/blob/master/Programming_Guide.md#dfp

<a name="unit"></a>
# 2. Set ad unit
In "Inventory" > "New ad unit", input the basic information and the fixed sizes that determines the ad unit's ad sizes (e.g. 300×250).
When using in-feed, selecting any size would be okay.

![DFP1.png](Install_SDK_Guide_Images/en/DFP1.png)

![DFP2.png](Install_SDK_Guide_Images/en/DFP2.png)

<a name="order"></a>
# 3. Set order
In "Delivery" > "New order", set the ad delivery settings.

<a name="order1"></a>
## 3-1. In "Advertiser", select "Add a new company"

![DFP3.png](Install_SDK_Guide_Images/en/DFP3.png)

<a name="order2"></a>
## 3-2. Input Name and Sizes
Select the same "Inventory sizes" that you selected when you created the ad units in the previous step.

![DFP4.png](Install_SDK_Guide_Images/en/DFP4.png)

<a name="order3"></a>
## 3-3 Set delivery schedule/delivery rate/goal
Select "Network" for "Type", and set the goal as "100".

![DFP5.png](Install_SDK_Guide_Images/en/DFP5.png)

<a name="order4"></a>
## 3-4 Select "Save and Upload creatives"

![DFP6.png](Install_SDK_Guide_Images/en/DFP6.png)

<a name="creative"></a>
# 4. Set creative
Upload creatives at the end of the order setting, or you can also come in "Delivery" > "Creative".

Select "Third Party". Make sure not to select "Native".

![DFP7.png](Install_SDK_Guide_Images/en/DFP7.png)

Here, you upload the Hike DFP Tag.

![DFP8.png](Install_SDK_Guide_Images/en/DFP8.png)

Save. make sure not to check "safeframe". (Recommended)

![DFP9.png](Install_SDK_Guide_Images/en/DFP9.png)

If you check “saferame” , when our ads cannot fill inventory, the empty space will be appear. And if you don’t want to show empty space with safeframe, please set limitation of daily impression.

<a name="DFPTag"></a>
# 5. Create DFP tag

A. How to generate tag for fixed size ( e.g. 300x250)
In "Inventory" > "Generate tags", generate DFP tag.

<a name="DFPTag1"></a>
## 5-1. Select ad unit

![DFP10.png](Install_SDK_Guide_Images/en/DFP10.png)

<a name="DFPTag2"></a>
## 5-2. Select tag type (Web/App)
Select "Google publisher tag"

![DFP11.png](Install_SDK_Guide_Images/en/DFP11.png)

<a name="DFPTag3"></a>
## 5-3. Set tag options
select "Create passback tag" and then "Standard GPT syntax".

![DFP12.png](Install_SDK_Guide_Images/en/DFP12.png)

<a name="DFPTag4"></a>
## 5-4. Tag will be generated

![DFP13.png](Install_SDK_Guide_Images/en/DFP13.png)

![DFP14.png](Install_SDK_Guide_Images/en/DFP14.png)

Also refer this.
https://support.google.com/dfp_premium/answer/177207?hl=en

<a name="ImplementTag"></a>
# 6. Implement DFP tag
Implement tag into your site according to guideline on DFP.

<a name="delivery"></a>
# 7. Start delivery
It seems it takes some time and a few reloads for the request to be sent and for the ad to be shown.

Let's monetise with FreakOut !!
