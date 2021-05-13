---
layout: default
title: John Bear
parent: Case Studies
nav_order: 2
---


# John Bear: Indistinguishable Gestures

Another participant, John Bear, exhibited a very different approach by repeatedly rerecorded samples to make them as similar as possible. They created _jump_ and then added _kick_. They quickly found that these two gestures interfered with one another. In John Bear's Gesture Log, notice that they removed and added _kick_ six times. The gesture was interfering with _jump_ due to similarities between the gestures' accelerometer plots.

## Different Gestures that Look Similar

When Brian Bear described their process for recording three different sleep samples, they explained that it was based on how they sleep, which looks different throughout the night.

### What a Child Sees

When a child acts out a gesture with a stuffed animal, they see very different movements.

![John Bear what a child sees](/img/just-john-bears.svg)

### What a Computer Sees

The micro:bit detects acceleration along the x-, y-, and z-axis, and the resulting shape is compared against what the child's future movements with the stuffed animal. In the case of _sleep_ and _jump_, the computer sees both of these gestures very similarly. 

![John Bear accelerometer data](/img/john-bear-accelerometer-800.svg)

When this occurred, their initial response was to add more samples for _kick_ and _jump_. This revealed that they were aware that the number of samples affects the model. After recording a new _jump_ sample, they inspected the existing samples, counted the three peaks, and then proceeded to record another sample, counting aloud as they moved the bear up and down three times. This again shows their care to make the samples similar while interpreting the sensor data to match peak count with the number of jumps.

## John Bear's Gesture Log

While making their project, John Bear discovered a problem: two of their gestures (_kick_ and _jump_) were **not triggering properly** when tested.

John Bear iterated on their design, **adding** and **removing** _kick_ recordings, in an attempt to fix this. They explained that the computer saw _kick_ and _jump_ very similarly, and would become confused.

<div class='tableauPlaceholder' id='viz1620622687035' style='position: relative'>
  <noscript>
    <a href='#'>
      <img alt='John Bear&#39;s Project ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Jo&#47;JohnBearsProject&#47;JohnBearsProject&#47;1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> 
    <param name='embed_code_version' value='3' /> 
    <param name='site_root' value='' />
    <param name='name' value='JohnBearsProject&#47;JohnBearsProject' />
    <param name='tabs' value='no' /><param name='toolbar' value='yes' />
    <param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Jo&#47;JohnBearsProject&#47;JohnBearsProject&#47;1.png' /> 
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='en' />
  </object>
</div>                

<script type='text/javascript'>
  var divElement = document.getElementById('viz1620622687035');
  var vizElement = divElement.getElementsByTagName('object')[0];
  if ( divElement.offsetWidth > 800 ) { 
    vizElement.style.width='1000px';vizElement.style.height='827px';} 
  else if ( divElement.offsetWidth > 500 ) { 
    vizElement.style.width='1000px';vizElement.style.height='827px';} 
  else { 
    vizElement.style.width='100%';vizElement.style.height='927px';}
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

* * *
Next: [Findings](findings)
