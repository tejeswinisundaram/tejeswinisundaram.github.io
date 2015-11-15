---
layout: post
title: Voice Forensics
---

The following is a summary of the work done by my team at the CMU IPTSE Winter School 2014. 

<div dir="ltr" style="text-align: left;" trbidi="on">
<div class="MsoNormal" style="text-align: justify;">
<b><span style="font-size: 14.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">OBJECTIVE</span></b><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<span style="font-size: 12pt; line-height: 115%;">To build a
voice forensics system that would identify bodily features such as height,
weight, age, sex, region of origin and various other demographic information
about a miscreant from the voice evidence collected. The end objective is to
build an extensive, if not comprehensive, one-of-a-kind &nbsp;voice print</span><span style="font-size: 12pt; line-height: 115%;">&nbsp;database to
enable authorities to track criminals.</span><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<b><span style="font-size: 14.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">ABSTRACT</span></b><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Security
has become a great concern for the citizens of our nation. With incidents such
as bomb attacks, ransom calls, and threat calls to life and property occurring
more frequently, it is important to develop a mechanism to help curb them. It
is vital for the government to devise a mechanism to deal with threats and
ransom calls in an effective and promising way. Voice Forensics has potential to
help the law enforcement agencies by providing valuable information such as
height, weight, age, sex of the suspect from the voice evidence available. In
the current scenario of crime investigation in India, we are technologically
ill-equipped to investigate cases that have only audio as their evidence. Our
project tries to solve this problem. Through this project we wish to explore
and improvise the area of Voice Forensics. The ultimate aim of the project is
to equip law enforcement agencies with the tools to process voice samples and
provide physical and demographic information about the miscreant that could be
used as an important evidence for investigation purposes. We propose to build a
unique one-of-a-kind voice print database for further research and analysis.</span><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<b><span style="font-size: 14.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">INTRODUCTION</span></b><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">During the
process of criminal investigations, it is imperative to extract as much
information as possible from the available evidences. Currently, the National
Crime Records Bureau cites two methods of Criminal identification, one using
fingerprints, and the other is a portrait building system. Fingerprint matching
could provide accurate information about the criminal, but in cases where
evidence is not available, or if the person is not recorded in the database, we
will not be able to make any predictions. In case of fingerprints, it is
impossible to approximate predictions about the person, if he/she is not
recorded in the database. Presently, there are 11 divisions under the CBI for
forensics and crime investigations in India. Surprisingly, voice forensics is
not one of them yet. With the technology we are developing, it would be
possible for the CBI to investigate cases with the evidences obtained from
voice and speech also.</span><span style="font-size: 10.0pt; line-height: 115%;"> </span><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">With this
tool, voice could be used as a reliable evidence in a court proceeding as per
Section 65B of the Indian Evidence Act, 1972.</span><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Exploration
of voice as a possible evidence is quite recent, and there are some advanced
voice identification software’s being developed, such as VoiceGrid. While,
voice based technologies such as Siri and Cortana are used as personal digital
assistants in mobile phones, VoiceGrid is a database intensive tool that has
been adopted by various state police organizations in the USA and Russia for
identification of miscreants based on the voice sample captured. These systems
rely largely on an existing database to make exact or close-to matches.
However, in cases when the exact voice samples cannot be matched, or is
unavailable in the database, it is very useful to extract physical and
geographical information of the miscreant from the voice sample available.
Hence, there is scope to develop much smarter and efficient systems for the
purpose of voice forensic study. In addition to this problem, there are no
publicly available benchmarks to test an attribute identification method. This
is mainly due to the difficulty in procuring a large dataset for the models to
work on and the absence of a framework for testing. Moreover, there exists no
framework that does the work of:</span><o:p></o:p></div>
<div class="MsoNormal" style="margin-left: 0.15pt; text-align: left;">
<br /></div>
<div class="MsoListParagraphCxSpFirst" style="text-align: left; text-indent: -0.25in;">
<!--[if !supportLists]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">1.<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Collecting
a large quantity of audio data from the citizens of our nation</span><o:p></o:p></div>
<div class="MsoListParagraphCxSpMiddle" style="text-align: left; text-indent: -0.25in;">
<!--[if !supportLists]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">2.<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Storing,
Analyzing, Validating the audio samples collected and managing it securely.</span><o:p></o:p></div>
<div class="MsoListParagraphCxSpMiddle" style="text-align: left; text-indent: -0.25in;">
<!--[if !supportLists]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">3.<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Perform
formal research on the collected voice samples. There is no framework that
allows for testing different models that predict physical attribute of a person
from their voice.</span><o:p></o:p></div>
<div class="MsoListParagraphCxSpLast" style="text-align: left; text-indent: -0.25in;">
<!--[if !supportLists]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">4.<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Provides
aids to the work of researchers across the country to use this nationwide audio
database for other interesting applications. (Anonymity of persons will be maintained
for security purposes).<o:p></o:p></span></div>
<div class="MsoNormal" style="text-align: justify; text-indent: -17.95pt;">
<br /></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Within this
project, we propose to build a framework that would solve these problems. We
aim to build the necessary technology for voice forensics and investigation.
The long term aim of this project is to equip law enforcement agencies with the
required tools to perform voice forensics and provide necessary evidence for
enforcement of law and order. With the system we build, the officials should be
able to estimate with good accuracy, the physical and geographical features of
the suspect.</span><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<b><span style="font-size: 14.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">DATA COLLECTION</span></b><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Voice
samples were collected from 40 students who participated in the IPTSE CMU-NITK
Winter School 2014. The age group of the participants was in the range of 19-22
years. The height, weight, age and sex of the students were recorded. Each
student was asked to speak a set of 25 phonetically rich sentences randomly
selected from the large TIMIT database. Thus, there were 25 recordings per
person, making a total of 1000 recordings. The samples were recorded using an
external microphone on Audacity, in a relatively quiet room. We ensured that
the recordings were lossless. All other necessary conditions like distance
between the speaker and the microphone were taken care of while recording the
voice samples.</span><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<b><span style="font-size: 14.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">METHODOLOGY</span></b><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .25in;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">The
Framework we are developing consists of machine learning tools, classification
and regression algorithms that extract and analyze features of the voice and
learn the correlations of the physical features and voice of the speaker. The
framework depicts the pipeline of computations and analysis. The pipeline
mainly consists of the following:</span><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoListParagraphCxSpFirst" style="mso-list: l2 level1 lfo2; text-align: justify; text-indent: -.25in;">
<!--[if !supportLists]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">1.<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Feature
Extraction</span><o:p></o:p></div>
<div class="MsoListParagraphCxSpMiddle" style="mso-list: l2 level1 lfo2; text-align: justify; text-indent: -.25in;">
<!--[if !supportLists]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">2.<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Normalization
of data</span><o:p></o:p></div>
<div class="MsoListParagraphCxSpMiddle" style="mso-list: l2 level1 lfo2; text-align: justify; text-indent: -.25in;">
<!--[if !supportLists]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">3.<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Clustering
(Bag of Words Model)</span><o:p></o:p></div>
<div class="MsoListParagraphCxSpLast" style="mso-list: l2 level1 lfo2; text-align: justify; text-indent: -.25in;">
<!--[if !supportLists]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">4.<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Machine
Learning Algorithms </span><o:p></o:p></div>
<div class="MsoNormalCxSpFirst" style="margin-left: .75in; mso-add-space: auto; mso-list: l1 level1 lfo3; text-align: justify; text-indent: -.25in;">
<!--[if !supportLists]--><span style="font-family: Wingdings; font-size: 12.0pt; line-height: 115%; mso-bidi-font-family: Wingdings; mso-bidi-font-size: 10.0pt; mso-fareast-font-family: Wingdings;">Ø<span style="font-family: 'Times New Roman'; font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Classifier
Models<o:p></o:p></span></div>
<div class="MsoNormalCxSpMiddle" style="margin-left: .75in; mso-add-space: auto; mso-list: l1 level1 lfo3; text-align: justify; text-indent: -.25in;">
<!--[if !supportLists]--><span style="font-family: Wingdings; font-size: 12.0pt; line-height: 115%; mso-bidi-font-family: Wingdings; mso-bidi-font-size: 10.0pt; mso-fareast-font-family: Wingdings;">Ø<span style="font-family: 'Times New Roman'; font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp; </span></span><!--[endif]--><span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">Regression
Models<o:p></o:p></span></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="separator" style="clear: both; text-align: center;">
<a href="http://1.bp.blogspot.com/-TymARnbQxKQ/VLA83B4oS5I/AAAAAAAACDo/DJ8qifmkzUs/s1600/pipeline.png" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="http://1.bp.blogspot.com/-TymARnbQxKQ/VLA83B4oS5I/AAAAAAAACDo/DJ8qifmkzUs/s1600/pipeline.png" height="238" width="400" /></a></div>
<div class="MsoNormal" style="text-align: justify;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></div>
<div class="MsoNormal" style="text-align: justify;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">The
pipeline followed is depicted in the picture demonstrated above.
The following sections will explain the above sections in detail.</span></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<b><span style="font-size: 14.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">RESULTS </span></b><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<span style="background: white; font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt; mso-highlight: white;">The initial results that we obtained was itself a
proof of concept for what we were trying to build. Given that the data set we used to test our system was
meagre and biased (male-female ratio was 3:1), we were still able to generate
results with good accuracy. We could predict the gender of an unknown person’s
voice with an accuracy of 95.2% and predict his/her height with an error of
6.5cm. With more data, and fine-tuning, our system could become reliable enough
to finally reach our desired goals.</span><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<span style="background: white; font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt; mso-highlight: white;"><br /></span></div>
<div class="separator" style="clear: both; text-align: center;">
<a href="http://2.bp.blogspot.com/-wDb0LnN5rzE/VLA_Ka7n_yI/AAAAAAAACD0/ZnyRkff6ab4/s1600/resutls.png" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="http://2.bp.blogspot.com/-wDb0LnN5rzE/VLA_Ka7n_yI/AAAAAAAACD0/ZnyRkff6ab4/s1600/resutls.png" height="213" width="400" /></a></div>
<div class="separator" style="clear: both; text-align: center;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<b><span style="font-size: 14.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">WEBSITE</span></b><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">To make our tool publicly usable,
we have developed a website. The website allows a user to upload a voice sample
(only .wav files are accepted as of now) and outputs the physical
characteristics of the owner of that voice in the sample. To predict the
physical features, the voice sample inputed is run on the already trained model.
In future, we intend to make a provision for users to contribute training data
as well. To ensure authenticity and security, only validated users shall be
allowed to upload their voice samples and their physical characteristics. After
inspection of the samples collected from the website for genuineness, it will
be used for training of our models.</span></div>
<div class="MsoNormal" style="text-align: justify;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;"><br /></span></div>
<div class="separator" style="clear: both; text-align: center;">
<a href="http://4.bp.blogspot.com/-7I_-M850lZM/VLBCiNdOTsI/AAAAAAAACEA/qNUVQ8s-tQE/s1600/website.png" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="http://4.bp.blogspot.com/-7I_-M850lZM/VLBCiNdOTsI/AAAAAAAACEA/qNUVQ8s-tQE/s1600/website.png" height="223" width="400" /></a></div>
<div class="MsoNormal" style="text-align: justify;">
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;"><br /></span></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<b><span style="font-size: 14.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">FURTHER WORK</span></b><o:p></o:p></div>
<div class="MsoNormal" style="text-align: justify;">
<br /></div>
<div class="MsoNormalCxSpMiddle" style="line-height: 150%; margin-bottom: .0001pt; margin-bottom: 0in; margin-left: .5in; margin-right: -44.95pt; margin-top: 0in; mso-add-space: auto; mso-list: l0 level1 lfo1; text-align: justify; text-indent: -17.95pt;">
<!--[if !supportLists]-->●<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp;&nbsp;
</span><!--[endif]--><span style="font-size: 12.0pt; line-height: 150%; mso-bidi-font-size: 10.0pt;">LASSO regression for height estimation,</span><o:p></o:p></div>
<div class="MsoNormalCxSpMiddle" style="line-height: 150%; margin-bottom: .0001pt; margin-bottom: 0in; margin-left: .5in; margin-right: -44.95pt; margin-top: 0in; mso-add-space: auto; mso-list: l0 level1 lfo1; text-align: justify; text-indent: -17.95pt;">
<!--[if !supportLists]-->●<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp;&nbsp;
</span><!--[endif]--><span style="font-size: 12.0pt; line-height: 150%; mso-bidi-font-size: 10.0pt;">Augmenting 6000 features(speaker traits) with bags of words
features,</span><o:p></o:p></div>
<div class="MsoNormalCxSpMiddle" style="line-height: 150%; margin-left: .5in; mso-add-space: auto; mso-list: l0 level1 lfo1; text-align: justify; text-indent: -17.95pt;">
<!--[if !supportLists]-->●<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp;&nbsp;
</span><!--[endif]--><span style="font-size: 12.0pt; line-height: 150%; mso-bidi-font-size: 10.0pt;">Since we have got high accuracy for gender classification, we
would now hope to see better results by using the predicted gender itself as a
feature for height prediction.</span><o:p></o:p></div>
<div class="MsoNormalCxSpMiddle" style="margin-left: 0.5in; text-align: justify; text-indent: -17.95pt;">
<!--[if !supportLists]--><span style="font-size: 12pt; line-height: 150%;">●<span style="font-size: 7pt; font-stretch: normal; line-height: normal;">&nbsp;&nbsp;&nbsp;&nbsp;
</span></span><!--[endif]--><span style="font-size: 12pt; line-height: 150%;">The data collected was biased, we had a girls to boys
ratio of 1:3. We need to test our models on a larger&nbsp;</span><span style="line-height: 24px;">data set</span><span style="font-size: 12pt; line-height: 150%;">&nbsp;with unbiased
inputs and check for the performance.<o:p></o:p></span></div>
<div class="MsoNormalCxSpMiddle" style="text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<b><span style="font-size: 14.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;">ACKNOWLEDGMENT<o:p></o:p></span></b></div>
<div class="MsoNormal" style="line-height: 150%; text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<span style="background: white; font-size: 12.0pt; line-height: 150%; mso-fareast-font-family: &quot;Times New Roman&quot;;"><span style="line-height: 150%;">We would like to extend our gratitude to our guides Prof
Bhiksha Raj, Prof Rita Singh from CMU and Mr. Pulkit Agrawal, PhD student from
University of California, Berkeley. A special thanks to the entire IPTSE Winter
School Team for providing us the opportunity and resources to work on this
project.</span><br /><br /><b>POSTER&nbsp;</b><span style="line-height: 150%;"><o:p></o:p></span></span><br />
<span style="background: white; font-size: 12.0pt; line-height: 150%; mso-fareast-font-family: &quot;Times New Roman&quot;;"><b><br /></b></span>
<span style="background: white; font-size: 12.0pt; line-height: 150%; mso-fareast-font-family: &quot;Times New Roman&quot;;"><b><br /></b></span>
<br />
<div class="separator" style="clear: both; line-height: 150%; text-align: left;">
<a href="http://4.bp.blogspot.com/-wGx8aCjjLk4/VLBHdpzquZI/AAAAAAAACEY/SY3v-z_ihiU/s1600/Screenshot%2B2015-01-10%2B02.52.01%2B(2).png" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="http://4.bp.blogspot.com/-wGx8aCjjLk4/VLBHdpzquZI/AAAAAAAACEY/SY3v-z_ihiU/s1600/Screenshot%2B2015-01-10%2B02.52.01%2B(2).png" height="230" width="400" /></a></div>
</div>
<div class="MsoNormal" style="line-height: 150%; text-align: justify;">
<br />
<br /></div>
<div class="MsoNormal" style="line-height: 150%;">
<span style="font-size: 12.0pt; line-height: 150%;">Team Voice Forensics: <o:p></o:p></span></div>
<div class="MsoNormal" style="line-height: 150%;">
<span style="font-size: 12.0pt; line-height: 150%;">1. Tejeswini Sundaram, BTech Computer Science, MIT Manipal<o:p></o:p></span></div>
<div class="MsoNormal" style="line-height: 150%;">
<span style="font-size: 12.0pt; line-height: 150%;">2. Priya Soundararajan, Int. M.Sc. Applied Mathematics, IIT
Roorkee<o:p></o:p></span></div>
<div class="MsoNormal" style="line-height: 150%;">
<span style="font-size: 12.0pt; line-height: 150%;">3. Utkarsh Patange, BTech Computer Science, IIT Kanpur<o:p></o:p></span></div>
<div class="MsoNormal" style="line-height: 150%;">
<span style="font-size: 12.0pt; line-height: 150%;">4. Sakthivel Sivaraman, BTech Mechanical Engineering, NITK
Surathkal<o:p></o:p></span></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
</div>
<div class="MsoNormal" style="line-height: 150%; text-align: justify;">
<br /></div>
<div class="MsoNormal" style="text-align: justify; text-indent: .5in;">
<br /></div>
<div class="MsoNormal" style="text-align: justify;">
<div class="separator" style="clear: both; text-align: left;">
<a href="http://2.bp.blogspot.com/-A5dfH6JB0rQ/VLBEhdTb8kI/AAAAAAAACEM/DIZ8G03V7EU/s1600/team%2Bpic.jpg" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="http://2.bp.blogspot.com/-A5dfH6JB0rQ/VLBEhdTb8kI/AAAAAAAACEM/DIZ8G03V7EU/s1600/team%2Bpic.jpg" height="200" width="200" /></a></div>
<span style="font-size: 12.0pt; line-height: 115%; mso-bidi-font-size: 10.0pt;"><br /></span></div>
</div>

