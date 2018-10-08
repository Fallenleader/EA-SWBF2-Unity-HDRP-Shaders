# EA SWBF2 Unity HDRP Shaders

This is a collection of shadergraph shaders designed to make it easy for the end user to import textures exported by frosty into Unity.
There are a few things to not before you just dive in and have a go:

First off, these are currently a WIP.
Second, they are subject to being updated, and my not represent the most accurate solution. For example, there is no weather influence or AO Slice support for the character shader at this time.
Third, using these shaders means you are using EA's assets, so these shaders cannot be used for any commercial product.

The names at this point are unintuitive, and many updates will be presented as I progress.

There are mandatory credits to mention here. First off, given the chance to thank the Frosty dev, please do so. Thanks to him, these exist. Honestly, most of tthe work was thanks to him, because I suck at this sort of thing.
Secondly, thanks to Unity for finally getting off their arse and making us a node based editor. Without this, I wouldn't have bothered.
Third, thank Sykoo for his support, as well as check out his awesome content. Brackys has been helpful as well, so send him some cheers as well.

Alright, now for the things to seriously note as you use these:
Firstly, convert the DDS textures to PNG. Frosty will likely have support for exporting to PNG in an update, but for now, you can only export to DDS.
Unity has an issue that persists from 2015 where it doesn't properly import DDS at times. This results in some textures flipping, as I found the hard way when working on the weapon shader.
The next thing to note is to check how the input is split up. Don't try to use the glove shader on the character's body, or the body shader on a weapon. each shader is specifically tailored to it's own purpose, just like in Frostbite.
And lastly, I will NOT be taking requests. If and when Frosty spits out some way to poke at shaders, or I need to make one for my specific case, I will addd it in. Feel free to improve on these, or even make new ones in a PR for other aspects of the files, but requests will be ignored. These should cover most use cases at this point in time from assets pulled from Frosty. I plan to work on vehicles next, but that isn't on my priority list.
