
<p align="center">
  <img src="https://user-images.githubusercontent.com/82110564/152652811-e7f7ea86-d7a8-4148-8f61-add6a5491e65.png">
</p>

# Blend_My_NFTs

## Description
Blend_My_NFTs is an open source, free to use Blender add on that enables you to automatically generate thousands of 3D Models, Animations, and Images. This add on's primary purpose is to aid in the creation of large generative 3D NFT collections. 

For support, help, and questions, please join our Discord where our wonderful community: https://discord.gg/UpZt5Un57t 

This add on was origninal developed to create the NFT project This Cozy Place which is now availabe to mint on our website: https://thiscozystudio.com/


https://user-images.githubusercontent.com/82110564/147833465-965be08b-ca5f-47ba-a159-b92ff775ee14.mov

The video above illustrates the first 10 Cozy Place NFTs generated with Blend_My_NFts.


## Official Links: 

Website: https://thiscozystudio.com/

Discord: https://discord.gg/UpZt5Un57t

Youtube: https://www.youtube.com/c/ThisCozyStudio

Twitter: https://twitter.com/CozyPlaceNFT

Instagram: https://www.instagram.com/this_cozy_studio/

Reddit: https://www.reddit.com/r/ThisCozyPlace/


## Case Studies
This document has a list of projects that use Blend_My_NFTs to help facilitate them in the creation of their collection: 
https://docs.google.com/document/d/e/2PACX-1vSHZS4GRu8xXDYpVPEaxyBeTzms9yrJEC9IoAcP38_U8x0C1kVrbtNZgh0zUmkzBoZQVwNvBf3ldRij/pub


## Quick Disclaimer
Blend_My_NFTs works with Blender 3.0.0 on Windows 10 or macOS Big Sur 11.6. Linux is supported, however I haven't had the chance to test this functionality and guarantee this.

Blend_My_NFTs, this readme documenation, YouTube tutorials, live stream Q/As are all provided for free by This Cozy Studio for anyone to use and access. I only ask in return that you credit this software and kindly share what our team has built. A direct link to the Blend_My_NFTs Github page on your projects website (or equivelant social platform) would sefice. We ask you to share this tool because we feel there are many out there that would benefit from it, our only goal is to help those in need. It warms our hearts that so many people use this add-on. 

Thank you, 

- This Cozy Studio team


## Setup/Installation

Here are the steps you need to take to get the Blend_My_NFTs add-on installed in Blender:

1. Click the green `Code` button at the top of this page.

<img width="328" alt="Screen Shot 2022-02-03 at 4 53 16 PM" src="https://user-images.githubusercontent.com/82110564/152435516-bf49bec3-a00f-4c3f-b632-cdf8028d64c8.png">

2. From the drop down click `Download ZIP`. This will download Blend_My_NFTs-main.zip to your Downloads folder:

<img width="397" alt="Screen Shot 2022-02-03 at 5 17 21 PM" src="https://user-images.githubusercontent.com/82110564/152438471-060f7af7-0624-42be-943a-57bb44b02482.png">

3. Move the Blend_My_NFTs-main.zip file to your desktop:

![Screen Shot 2022-02-03 at 4 57 02 PM](https://user-images.githubusercontent.com/82110564/152436030-bccf33ca-25d4-45f7-997a-89bf2ac858e4.png)

4. Open Blender and navigate to `Edit` -> `Preferences` -> `Add-ons`:

<img width="466" alt="Screen Shot 2022-02-03 at 5 00 27 PM" src="https://user-images.githubusercontent.com/82110564/152436377-b042234e-a791-4e2a-8ffa-f3694d819b4b.png">

<img width="666" alt="Screen Shot 2022-02-03 at 5 00 43 PM" src="https://user-images.githubusercontent.com/82110564/152436410-e02fe611-49b1-45e8-a1b8-336b67e9ecd4.png">

5. Click the `Install` button: 

![Screen Shot 2022-02-03 at 5 05 08 PM](https://user-images.githubusercontent.com/82110564/152436908-8f7d5d8f-eb9c-431f-8ca1-c9a022b1b4eb.png)

6. In the `Blender File View` window, navigate to the Blend_My_NFTs-main.zip file downloaded in step 1., select it, then click `Install Add-on`:

![Screen Shot 2022-02-03 at 5 07 16 PM](https://user-images.githubusercontent.com/82110564/152438040-513222ea-8297-4771-8bf3-3b6af74bb54b.png)


7. Navigate back to the `Add-ons` window in step 4., and search for Blend_My_NFTs:

![Screen Shot 2022-02-03 at 5 02 59 PM](https://user-images.githubusercontent.com/82110564/152436664-e8e135e5-2d36-487a-bf43-4ea200210a4c.png)

8. Click the `Checkbox` to enable the Blend_My_NFTs add-on:

![Screen Shot 2022-02-03 at 5 22 43 PM 1](https://user-images.githubusercontent.com/82110564/152439275-c590db7a-8b5c-48a4-96f5-ac1ce372be38.png)


Now that Blend_My_NFTs is installed in your instance of Blender you can find the main panel in the `3D View` tab in `Layout`, once you are there tap `N` on your keyboard to open the side panel:

![Screen Shot 2022-02-03 at 5 27 41 PM](https://user-images.githubusercontent.com/82110564/152439730-21da93e3-6816-419a-b9d8-5b146dfe3e6e.png)


## Important Terminology

Before you can continue further, there are terms used in this documenation to describe the process of this software. This makes it easier to understand how you need to organize your .blend file to generate NFTs. Refer to this section if you come accross an unfamiliar term. 

Let's say you are creating an NFT collection, the artwork is a .png of a person wearing a hat:

1. ``Attribute`` - A part of the .png that can be changed. The idea of a `Hat` on a man is an Attribute, there are many types of Hats, but the `Hat` itself I will refer to it as an Attribute.

2. ``Variants`` - These are the types of Hats; Red Hat, Blue Hat, Green Hat, Cat Hat, etc. These can be swapped into the `Hat` Attribute to create unique .png NFTs.

3. ``DNA`` - A sequence of numbers that determins what ``Variant`` from every ``Attribute`` to include in a single NFT .png. Blend_My_NFTs creates and stores a uniqe DNA sequence for each NFT you create. These numbers are stored in the ``NFTRecord``.

4. ``NFTRecord`` - The "Ledger" of all ``DNA`` for your NFT collection. This will be generated after you create all the Attribtues and Variants that make up your NFT collection in Blender.

5. ``Batch`` - A randomly selected subset of ``DNA``, taken from the ``NFTRecord``. Blend_My_NFTs can split the ``NFTRecord`` into multiple Batches; This allows you to render or create NFTs on multiple computers, or at seperate instances in time.
