# Feature selection for intrusion detection using PCA
<p><b>Importance of intrusion detection</b></p> 
<p>Network intrusion detection systems (IDS) play a crucial role for companies by alerting them to possible
malicious activity across variety of gadgets and devices. To this end, machine learning approaches tested
on different datasets such as AWID[1] and “KDD99” have shown diverse procedures to detect
intrusion attacks effectively ranging from more traditional approaches to sophisticated multi-layered
models.</p>
<p>Principal component analysis (PCA) is a method to reduce data complexity with the advantage of
obtaining important patterns. This approach was used for intrusion detection problem in [1], however
authors applied it to KDD dataset.
The method consists of iterative projection observation values on a hyperplane. The coordinates of a
hyperplane are orthogonal to each other and chosen in particular order to capture greater variance and
map it to a new axis. When repeated step by step, this process compresses original input into lower
dimensional space. To be more precise, I obtain a list of sets (eigenvector, eigenvalue) and sort it by
eigenvalue. Then I use this eigenvectors to produce final matrix NxM, where N has the same dimension
as the number of original rows, M – recomputed initial values with respect to principal components.
In this project, I performed PCA part, because it allows to capture unknown patterns of the data, and
combine this compressed input with original one in order to obtain features that contribute most to predicting target class.</p>
<p>Finally I obtained 12 features including one dimension extracted from original data with accuracy rate 98.6%, which is much higher than in [2], where accuracy is 86.34%</b>
<p>[1]. <a href="http://icsdweb.aegean.gr/awid/"><b>“AWID dataset ”</b></a></b>
<p>[2]. B.Zhang, Z.Liu, Y.Jia, J.Ren,and X.Zhao, “Network Intrusion Detection Method Based on PCA and
Bayes Algorithm”, Security and Communication Networks, Hindawi, 2018.<a href="https://www.researchgate.net/publication/328920124_Network_Intrusion_Detection_Method_Based_on_PCA_and_Bayes_Algorithm"></b>



