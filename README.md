# PSJ_Sampling

***[This Repository is a Work In Progress]***

This is the implementation of the Point Spread Jitter in Blender.
This algorithm works for Cycles but might be adapted for every ray tracing engine.
The PSJ is used to increment optical realism in rendering, to know more about it please read the related paper.
*We recommend to read the whole README.md before starting*

**How to install the PSJ**

To use this sampling pattern you need to build your own version of Blender (*link below*) and change a file with the one in this the repository.
***After downloading sources and libraries*** you can find the file in:

*C:\blender-git\blender\intern\cycles\kernel\kernel_jitter.h*

You then may proceede building Blender as shown in the guide.
Official blender guide:*https://wiki.blender.org/wiki/Building_Blender*

**How to use the PSJ**

After building Blender you might have an unstable version of it, we suggest to build the scene in an official version and then render in the PSJ version. 
You might have some artifacts in the interface that we hope to fix soon.

In order to have the best performance we recommend the following *Cycles* setting:

    Default Setting +
    Samples: *512*
    Advanced>Patter: *Correlated Multi-jitter*
    Denoising>Render: *NLM*

We also recommend a resolution between 1920x1080px  and 2560x1440px.


**Contacts**

For any advice, critique, comment feel free to contact me: 
leonardo.vezzani@live.com
 



