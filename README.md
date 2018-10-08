# EA SWBF2 Unity HDRP Shaders

This is a collection of shadergraph shaders designed to make it easy for the end user to import textures exported by Frosty into Unity.
There are a few things to note before you just dive in and have a go:

First off, these are currently a WIP.

Second, they are subject to being updated, and my not represent the most accurate solution. For example, there is no weather influence or AO Slice support for the character shader at this time.

Third, using these shaders means you are using EA's assets, so these shaders cannot be used for any commercial product.

The names at this point are only slightly intuitive, and many updates will be presented as I progress. Generally speaking, the PBR name comes first (e.g. Albedo/Smoothness), followed by the abbreveation given to the texture by Dice as of the latest update (e.g. Some_Object_CS), so as an example, Albedo/Smoothness(CS) would take a texture with CS in the name. 

There are mandatory credits to mention here:

First off, given the chance to thank the Frosty dev, please do so. Thanks to him, these exist. Honestly, most of the work was thanks to him, because I suck at this sort of thing. Being honest, the character shader was 99.9% done by him, all I did was update it with more modifications he sent me later, and rename things to follow my naming scheme.

Secondly, thanks to Unity for finally getting off their arse and making us a node based editor. Without this, I wouldn't have bothered.

Third, thank Sykoo for his support, as well as check out his awesome content. Brackys has been helpful as well, so send him some cheers as well.


Alright, now for the things you NEED to know as you use these:


Firstly, convert the DDS textures to PNG. Frosty will likely have support for exporting to PNG in an update, but for now, you can only export to DDS. Unity has an issue that persists from as far back as 2015 where it doesn't properly import DDS at times. This results in some textures flipping, as I found the hard way when working on the weapon shader.

If you insist on using DDS, take note if a texture flips in Unity and flip it in photoshop (photoshop will show it extracted correctly, but Unity will ignore this, so flip it anyhow).

Photoshop users, make sure you are using the Intel plugin for DDS, not Nvidia's outdated one.

Gimp users are on your own.

If you insist on using DDS, make sure normal maps of any sort have sRGB disabled. I haven't found any issue with other textures using sRGB, and if this is indeed a problem I will update this to reflect that.

The next thing to note is to check the type of shader.

Don't try to use the glove shader on the character's body, or the body shader on a weapon. Each shader is specifically tailored to it's own purpose, just like in Frostbite.


Lastly, I will NOT be taking requests. If and when Frosty spits out some way to poke at shaders, or I need to make one for my specific case, I will addd it in. Feel free to improve on these, or even make new ones in a PR for other aspects of the files, but requests will be ignored.

These should cover most use cases at this point in time from assets pulled from Frosty. I plan to work on vehicles next, but that isn't on my priority list.

![ScreenShot](/Clone.png)
