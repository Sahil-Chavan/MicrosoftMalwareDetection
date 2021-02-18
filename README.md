# MicrosoftMalwareDetection
<h1>1.Business/Real-world Problem</h1>

<h2>1.1. What is Malware? </h2>
<p>
The term malware is a contraction of malicious software. Put simply, malware is any piece of software that was written with the intent of doing harm to data, devices or to people. <br> 
Source: https://www.avg.com/en/signal/what-is-malware
<p>

<h2> 1.2. Problem Statement </h2>
<p>
    In the past few years, the malware industry has grown very rapidly that, the syndicates invest heavily in technologies to evade traditional protection, forcing the anti-malware groups/communities to build more robust softwares to detect and terminate these attacks. The major part of protecting a computer system from a malware attack is to <b>identify whether a given piece of file/software<b> is a malware. 
</p>

<h2>1.3 Source/Useful Links </h2>
<p>    Microsoft has been very active in building anti-malware products over the years  and it runs it’s anti-malware utilities over <b>150 million computers</b> around the world. This generates tens of millions of daily data points to be analyzed as potential malware. In order to be effective in analyzing and classifying such large amounts of data, we need to be able to group them into groups and identify their respective families. 
<br>
<br>
This dataset provided by Microsoft contains about 9 classes of malware.
</p>
<b> Source: </b> https://www.kaggle.com/c/malware-classification
<p>
</p>

<h2>1.4. Real-world/Business objectives and constraints.</h2>
1. Minimize multi-class error. <br>
2. Multi-class probability estimates.<br>
3. Malware detection should not take hours and block the user's computer. It should fininsh in a few seconds or a minute.

<h1>2. Mapping the real-world problem to an ML problem</h1>

<h2>2.2.1. Type of Machine Learning Problem</h2>
<p>
    
            There are nine different classes of malware that we need to classify a given a data point => Multi class classification problem    
</p>

<h2>2.2.2. Performance Metric</h2>
Source: https://www.kaggle.com/c/malware-classification#evaluation

Metric(s): 
* Multi class log-loss 
* Confusion matrix 

<h2>2.2.3. Machine Learing Objectives and Constraints</h2>
<p> Objective: Predict the probability of each data-point belonging to each of the nine classes.
</p>
<p> Constraints:
</p>

- Class probabilities are needed.
- Penalize the errors in class probabilites => Metric is Log-loss.
- Some Latency constraints.
