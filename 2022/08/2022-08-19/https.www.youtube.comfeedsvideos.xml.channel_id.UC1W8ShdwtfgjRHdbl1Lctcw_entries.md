# Source:NASS, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC1W8ShdwtfgjRHdbl1Lctcw, language:en-US

## My advanced black and white video colorization process (Timelapse)
 - [https://www.youtube.com/watch?v=gFosPTJjkw4](https://www.youtube.com/watch?v=gFosPTJjkw4)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC1W8ShdwtfgjRHdbl1Lctcw
 - date published: 2022-08-20 00:00:00+00:00

Hello everyone I hope you are well, I wanted to show you the colorization technique I have developed to have a realistic colorization with artificial intelligence algorithms and manual work

For the cleaning of this video I used Avisynth and davinci resolve:
Avisynth script:
SpotLess(RadT=6, ThSAD2=900, pel=4, chroma=true)
davinci resolve plugins: automatic dirt removal, dustbuster (Manual work)

Artificial intelligence algorithms for colorization: deoldify, Deep Exemplar-based Video Colorization
Preparing Reference Images: colorizer pro software (Manual work)

Artificial intelligence algorithms for upscale to HD and face restoration
RealESRGAN (Integrate GFPGAN to support face enhancement)

For Resize Avisynth script:
nnedi3_rpow2(cshift="Spline64ResizeMT", rfactor=2, fwidth=960, fheight=720, nsize=4, nns=4, qual=1, etype=0, pscrn=2, threads=0, csresize=true, mpeg2=true, threads_rs=0, logicalCores_rs=true, MaxPhysCore_rs=true, SetAffinity_rs=false, opt=3)

## A few techniques: how I restore black and white videos before colorization
 - [https://www.youtube.com/watch?v=0d9T7Fj2dJs](https://www.youtube.com/watch?v=0d9T7Fj2dJs)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC1W8ShdwtfgjRHdbl1Lctcw
 - date published: 2022-08-19 00:00:00+00:00

Here are some techniques I used for cleaning and denoise & degraine and sharpening the black and white videos before colorization that I publish on my channel,

Here are the tool and software used:
Avisynth
Davinci resolve

Here are the avisynth scripts I used:

#cleaning
SpotLess(RadT=6, ThSAD2=900, pel=4, chroma=true)

#Denoising and #Degraining

super = MSuper(pel=2, sharp=1)
bv1 = MAnalyse(super, isb = true, delta = 1, overlap=4)
fv1 = MAnalyse(super, isb = false, delta = 1, overlap=4)
bv2 = MAnalyse(super, isb = true, delta = 2, overlap=4)
fv2 = MAnalyse(super, isb = false, delta = 2, overlap=4)
MDegrain2(super,bv1,fv1,bv2,fv2,thSADC=800, thSAD=800)

return last

FFT3DFilter(sigma=3.0, beta=1.0, plane=4, bw=16, bh=16, ow=8, oh=8, bt=3, kratio=3.0, sharpen=1.0, scutoff=0.3, svr=1.0, smin=4.0, smax=30.0, measure=true, interlaced=false, wintype=0, degrid=1.0, dehalo=1.0, hr=2.0, ht=50.0)

#Sharpening
aWarpSharp2(thresh=180, blur=3, type=0, depth=35, depthC=10, chroma=4)

Overview 00:00-1.30
Cleaning 1:30- 6:30
Denoising and Degraining 6:30-8:20
Sharpening: 8:20-10-26
Before and After : 10:26-10:37

