---
layout: default
title: Case Studies
nav_order: 4
---


# Case Studies

Each child's project was unique and developed out of their own interests and experiences. Two stories stood out based on their experieces using the machine learning tool.

## Brian Bear and Varied Data Sampling

Brian Bear (a pseudonym for the child based on their stuffed animal's name) created gestures for their stuffed animal to respond to in a bedroom: _sleeping_, _playing board games_, and _dancing_. While recording samples of each of these gestures, the researcher noticed that Brian Bear performed each gesture differently. When asked to explain their intentions, Brian Bear explained that they wanted a wider range of movements for the computer to recognize as one gesture. In the example of _sleeping_, this resulted in three different gesture samples: lying still, sleeping on one side, and rolling over.

![sleeping gestures](/img/sleeping-gestures-1.svg){: width="700" }

While this mindset could work on a large data set with many sample recordings, it's not ideal to have such varied recordings for a small sample size of N=3.

<div class='tableauPlaceholder' id='viz1620602511003' style='position: relative'>
  <noscript><a href='#'>
    <img alt='Brian Bear&#39;s Project ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Br&#47;BrianBearsProject&#47;BrianBearsProject&#47;1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz'  style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> 
    <param name='embed_code_version' value='3' /> 
    <param name='site_root' value='' />
    <param name='name' value='BrianBearsProject&#47;BrianBearsProject' />
    <param name='tabs' value='no' /><param name='toolbar' value='yes' />
    <param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Br&#47;BrianBearsProject&#47;BrianBearsProject&#47;1.png' /> 
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='en' />
  </object>
</div>                

<script type='text/javascript'>
  var divElement = document.getElementById('viz1620602511003');
  var vizElement = divElement.getElementsByTagName('object')[0];
  if ( divElement.offsetWidth > 800 ) { 
    vizElement.style.width='1000px';vizElement.style.height='827px';}
  else if ( divElement.offsetWidth > 500 ) { 
    vizElement.style.width='1000px';vizElement.style.height='827px';} 
  else { 
    vizElement.style.width='100%';vizElement.style.height='777px';}
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

## John Bear: Similarities Across Gestures 

Another participant, John Bear, exhibited a very different approach to data sampling than Brian Bear. They repeatedly rerecorded samples to make them as similar as possible. Initially creating _jump_ and _run_ from a warm-up exercise, he added _kick_ for kicking a soccer ball and quickly found that the gestures interfered with one another. In John Bear's Gesture Log, notice that they removed and added kick six times. The gesture was interfering with _jump_ due to similarities between the gestures' accelerometer plots.

![John Bear accelerometer data](/img/john-bear-accel-1.png){: width="640" }

When this occurred, his initial response was, “More data?," at which point he added another sample for both _kick_ and _jump_. This revealed that he was aware that the number of samples affects the model. After recording a new _jump_ sample, he inspected the existing samples, counted the three peaks, and then proceeded to record another sample, counting aloud as he moved the bear up and down three times. This again shows his care to make the samples similar while interpreting the sensor data to match peak count with the number of jumps.

<div class='tableauPlaceholder' id='viz1619917080298' style='position: relative'>
  <noscript>
    <a href='#'>
    <img alt='John Bear&#39;s Gesture Log ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Jo&#47;JohnBear&#47;JohnBear&#47;1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz'  style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> 
    <param name='embed_code_version' value='3' /> 
    <param name='site_root' value='' />
    <param name='name' value='JohnBear&#47;JohnBear' />
    <param name='tabs' value='no' /><param name='toolbar' value='yes' />
    <param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Jo&#47;JohnBear&#47;JohnBear&#47;1.png' /> 
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='en' />
  </object>
</div>

<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1619917080298');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';
  vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>
