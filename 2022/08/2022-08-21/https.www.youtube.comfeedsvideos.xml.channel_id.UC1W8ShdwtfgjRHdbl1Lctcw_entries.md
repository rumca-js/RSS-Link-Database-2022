# Source:NASS, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC1W8ShdwtfgjRHdbl1Lctcw, language:en-US

## Shanghai 1940s in color [60fps,Remastered] w/sound design added
 - [https://www.youtube.com/watch?v=ABGkTXoyJ5I](https://www.youtube.com/watch?v=ABGkTXoyJ5I)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC1W8ShdwtfgjRHdbl1Lctcw
 - date published: 2022-08-22 00:00:00+00:00

I colorized, restored and worked a sound design of this video of the old Shanghai 1940s . You can see a lot of rickshaws, but not a lot of motorized vehicles, you can also see tramways and big buildings and people living their daily life,

Video Restoration Process:
✔ FPS boosted to 60 frames per second 
✔ Image resolution boosted up to HD 
✔ Improved video sharpness and brightness 
✔ Colorized only for the ambiance (not historically accurate)
✔sound design added only for the ambiance
✔restoration:(stabilisation,denoise,cleand,deblur) 

Please, be aware that colorization colors are not real and fake, colorization was made only for the ambiance and do not represent real historical data.

B&W Video Source from: Internet Archive
B&W Video Source: https://archive.org/details/pet1013r2c

Rights to the black and white 35mm Video Source are held by Internet Archive. under the Creative Commons Attribution License

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

