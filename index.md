# PlushPal Study

## What is PlushPal?
[PlushPal](https://ttseng.github.io/plushie/) is a new digital tool for kids to use make their stuffed animals interactive using machine learning (ML). Kids make their own custom gesture and sound pairings, and use a [micro:bit](https://microbit.org) to detect specific movements that their stuffed animal makes. 

![plushpal gif](/img/plushpal-demo.gif){: width="400" }

# How it Works
### Set-up

![set up micro:bit](/img/set-up.png){: width="250" }

Start by attaching a micro:bit to a stuffed animal and pair it to PlushPal using web Bluetooth.

### Record Gestures

![record gestures](/img/record-gestures.png){: width="400" }

Create a new gesture and perform the gesture multiple times while recording it.

### Evaluate and Play

![evaluate and play](/img/evaluate.png){: width="250" }

Test if ML models correctly detect gestures and make adjustments as needed and add sound to each gesture.

## What is the PlushPal study?
PlushPal was introduced to eleven kids, ages 8-14 years old, over Zoom and in person during the COVID-19 pandemic. Children brought their own stuffed animals to the playtest and used a micro:bit and PlushPal to make their toys interactive. After a brief introduction to the tool, machine learning, and a presurvey, children were asked to make custom gestures for their stuffed animals (ex. walking, eating, sleeping). These gestures were performed multiple times by the children, and it was suggested that they should perform and record each gesture at least three times. 

## Demographics
We had eleven children participate in the study that were eight to fourteen years old. Most had prior programming experience through block based editors like Scratch and MakeCode, and a few had experience using a micro:bit.

![demographics](/img/demographics.png){: width="400" }

## What Kids Made

There were 42 unique gestures that were created across all eleven projects. Some gestures were common amongst projects (ex: _run_ and _jump_) and others were unique only to one project. For anonymity, the child's name is replaced with the of their stuffed animal (ex: Cat, Dog, Unicorn). Since multiple children brought teddy bears, their names start with the name they gave to their stuffed animal followed by bear (ex: Brian Bear, John Bear).

In the following visualization, each gesture is listed next to a circle. The circle size corresponds to the number of times that gesture was used across all stuffed animal projects. For instance, _run_ was used more often than _fly_. To see which stuffed animals used each gesture, hover over the gesture name to reveal the stuffed animals associated with it (each stuffed animal's name corresponds to its own color) and what other gestures were also used.

#### Stuffed Animal Names
<html>
<iframe width="100%" height="109" frameborder="0"
  src="https://observablehq.com/embed/@deannagelosi/plushpal-gesture-visualization?cells=swatch"></iframe>
</html>

### Gesture Exploration

<html>
  <iframe width="945px" height="984px" frameborder="0" src="https://observablehq.com/embed/@deannagelosi/plushpal-gesture-visualization?cells=NodesAndLabels"></iframe>
</html>

## Case Studies

Each child's project was unique and developed out of their own interests and experiences. Two stories stood out based on their experieces using the machine learning tool.

### Brian Bear and Varied Data Sampling

Brian Bear (a pseudonym for the child based on their stuffed animal's name) created gestures for their stuffed animal to respond to in a bedroom: _sleeping_, _playing board games_, and _dancing_. While recording samples of each of these gestures, the researcher noticed that Brian Bear performed each gesture differently. When asked to explain their intentions, Brian Bear explained that they wanted a wider range of movements for the computer to recognize as one gesture. In the example of _sleeping_, this resulted in three different gesture samples: lying still, sleeping on one side, and rolling over.

![Brian Bear accelerometer data](/img/sleep-gestures.png){: width="640" }

While this mindset could work on a large data set with many sample recordings, it's not ideal to have such varied recordings for a small sample size of N=3.

<div class='tableauPlaceholder' id='viz1619886289792' style='position: relative'>
  <noscript>
    <a href='#'>
      <img alt='Brian Bear&#39;s Gesture Log ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Br&#47;BrianBear&#47;BrianBear&#47;1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> 
    <param name='embed_code_version' value='3' /> 
    <param name='site_root' value='' />
    <param name='name' value='BrianBear&#47;BrianBear' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Br&#47;BrianBear&#47;BrianBear&#47;1.png' /> 
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='en' />
  </object>
</div>   

<script type='text/javascript'>
  var divElement = document.getElementById('viz1619886289792');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width='100%';
  vizElement.style.height=(divElement.offsetWidth*0.75)+'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

### John Bear: Similarities Across Gestures 

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

## Findings

Children were asked pre- and post-tests around topics related to machine learning. After their experience with PlushPal, 70% of children who answered the post-survey questions could provide a technical definition of machine learning (one that defines machine learning as a human training a computer to detect something specified). Before PlushPal, only 10% of children were able to provide such a definition. 

![data literacy](/img/data literacy.png){: width="400" }

Researchers saw through this study that children have different approaches to collecting data samples and highlight some misconceptions, including how machine learning models work. Children had a wide variety of gesture ideas to record, but could use support around how the quantity of sample sizes and similiarities between sample recordings impacts the accuracy of their machine learning models. 
