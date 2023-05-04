# Source:NASS, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC1W8ShdwtfgjRHdbl1Lctcw, language:en-US

## How I digitally restore videos and enhance the faces of videos published on my channel (Timelapse)
 - [https://www.youtube.com/watch?v=jMRjmzmytyA](https://www.youtube.com/watch?v=jMRjmzmytyA)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC1W8ShdwtfgjRHdbl1Lctcw
 - date published: 2022-08-21 00:00:00+00:00

A few techniques: How I digitally restore videos and enhance the faces of videos published on my channel, 

Here are the algorithms of the artificial intelligence I used:
RealESRGAN (Integrate GFPGAN to support face enhancement) for upscale
Real-Time Intermediate Flow Estimation for Video Frame Interpolation

Here are the tool and software used:
Avisynth
Davinci resolve
Filmora 9 (How i make a sound design for videos published on my channel)

Here are the avisynth scripts I used:
#cleaning
RemoveDirtMC(40, false)
#degrain
super = MSuper(pel=2, sharp=1)
bv1 = MAnalyse(super, isb = true, delta = 1, overlap=4)
fv1 = MAnalyse(super, isb = false, delta = 1, overlap=4)
bv2 = MAnalyse(super, isb = true, delta = 2, overlap=4)
fv2 = MAnalyse(super, isb = false, delta = 2, overlap=4)
MDegrain2(super,bv1,fv1,bv2,fv2,thSADC=800, thSAD=800)

return last
#colorcorrection
ConvertToRGB(matrix="Rec601", interlaced=false)
GamMac(LockChan=1,LockVal=130,RedMul=1,GrnMul=1,BluMul=0.9,Show=false,Verbosity=2,hith=0.5,loth=0.5,th=1,scale=2)
ConvertToYV12(interlaced=false)


Before and After 5:41-5:51

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

