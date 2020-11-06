
<!-- wp:image {"align":"center","id":617,"width":329,"height":270,"sizeSlug":"large"} 
<div class="wp-block-image"><figure class="aligncenter size-large is-resized"><img src="https://vedantdave117com.files.wordpress.com/2019/12/fraud-detection-and-prevention-market-1.png?w=702" alt="" class="wp-image-617" width="329" height="270"/><figcaption>Security is Main Concern in Trustful Business</figcaption></figure></div>
<!-- /wp:image --> -->

<!-- wp:heading {"level":3} -->
<h3><strong>Banking Financial Fraudulent Transactions analysis ( Kaggle dataset)</strong>  </h3>
<!-- /wp:heading -->

<!-- wp:heading {"level":3} -->
<h3><strong>Business Problem</strong> </h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Given dataset of reputed company (Bank or Financial Institute) recently faced transactinal fraud, and our main objective is to get data insights from the data set and identify the following questions.</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>What is the common in all fradulent Transactions?</li><li>Finding hiddent pattern to detect fraud sequence for future planning</li><li>Is our Fraud Flagged data are correct in own manner?</li><li>Which kind of customers / clients involved in such activity? Are they outsiders or other genuine looking profiles?</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3><strong>Data Understanding</strong></h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>We have around 500 MB dataset with  (6362620, 11)&nbsp; matrix.</li><li> It has 11 features with type of transactions, amount, customer name(modified id), Original balance , new balance, original account destination, new account destination, fraud , fruadflegged labeling.</li><li>Its in form of excel spread sheet </li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3><strong>Data Explotary Analysis &amp; Preprocessing</strong></h3>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li>Type of Fruad Transfer type and thier actual Numbers.</li><li>Total Flagged Transfer and their transfer type ( finding method of froud scenario)</li><li>Min and Max amount of Flagged raised during transaction</li><li>No of flagged when (isFlaggedFraud = 0, yet oldBalanceDest = 0 and newBalanceDest = 0) because of security concern account blocking</li><li>Finding maximum attempt of fraud from one accont (to get intensity of fraud)</li><li>Customer of client type of fraud to ensure perticular profession or account type involvement in cheating (helpful to ensure future planning of security stage improvement)</li><li>Get destination accounts and match them with CASH_OUT from same account to ensure the fraud (require for trust breaching concern from financial institute level)</li><li>Identified fraudulent desitnation accounts whose CASH_OUT origin is looking genuine (due to CASH_OUT before fraud  transaction happened to account) </li></ol>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3><strong>Data Cleaning</strong></h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Why?</strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Separate required data for better prediction, and to reduce computational power requirement and time requirement, machine modeling perfomance imporvement.</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Check fraction of zero balance in fraud and nonfraud transaction to determine our focus concern during machine learning modeling.</li><li>Modify zero balance to -1 (from 0) to classify betterly in modeling stage.</li><li>Now, modify null value to zero (from null) to reduce missing data barrier for machine learning modeling. </li><li>Check the requirement of new features for further classifications.</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3>Featu<strong>re Engineering</strong></h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Create error balance in Originator and Destination Accounts </li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3><strong>Data Visulization</strong></h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>To identify our best classification algorithm for final result.</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Visulize fraud transactions for TRANSFER and CASH_OUT types</li><li>Create genuine account fingure print ( may involved in faud transfer) .</li><li>3D visualization for our new features' importance</li><li>Heatmapping of correlation difference in Genuine VS Fraud accounts</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3><strong>Machine learning Modeling</strong></h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>I tried boosing algorithm on random forest , simple decision tree , svm (not actully use due to data distribution in 3D space) and get better result in <strong>Gradiant boosting Dicision tree</strong> modeling. (Also take help from kernel notebook of top Kaggler) </p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Found out ascending order of most useful features.</li><li>get model output (preety impresive for training &amp; validation more than 99.5 percent) - weight base modeling</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3><strong>Bias -variance Tradeoff</strong></h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>This phase is somewhat disapponting because of underfitting of model. </li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3><strong>Reasons and Solution Approach</strong></h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Possibility of further training ( it require time ) by increase depthsize, or chainging data spliting ratio 90:10 from 80:10 because our model need more data for training.</li><li>We must use scalling od data due to unaspected ratio of genuine vs fradulent data set (only 16 fraud exist in 6362620 transactions)</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3><strong>Attachment</strong></h3>
<!-- /wp:heading -->

<!-- wp:heading {"level":4} -->
<h4><a href="https://github.com/vedantdave77/PROJECT_Financial_Fraud_Analysis-/blob/master/Fraud_Analysis.ipynb">Code</a></h4>
<!-- /wp:heading -->

<!-- wp:paragraph {"align":"justify","textColor":"very-light-gray","backgroundColor":"vivid-red","fontSize":"normal"} -->
<p class="has-text-color has-background has-text-align-justify has-normal-font-size has-very-light-gray-color has-vivid-red-background-color"><strong>Thank you for reading, here I want to acknoledge kaggle for providing data sets and contribution of some kaggler's notebooks which I used for understanding sets and its process pattern.</strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph {"textColor":"very-light-gray","backgroundColor":"very-dark-gray"} -->
<p class="has-text-color has-background has-very-light-gray-color has-very-dark-gray-background-color">Plz give me advised if you find anything wrong or new intution for applying. Thank you for reading. <strong><em><span style="text-decoration: underline;">Keep Learning ,get empowering</span></em></strong>.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->
