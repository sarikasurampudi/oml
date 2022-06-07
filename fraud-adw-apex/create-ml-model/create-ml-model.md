# Build a Machine Learning Model

## Introduction

This is the lab where you’re going to do the work of building and training a machine learning model that will help identify fraudulent auto claims.

### Before You Begin

Remember that we are trying to help predict when an auto claim is fraudulent. We use Oracle Machine Learning's 1-Class Support Vector Machine to train on "normal" records and apply the 1-Class SVM model to our insurance claims to flag those claims that are most dissimilar from the training population.

[](youtube:IkOz2rrB7hU)

In this lab, you will use Apache Zeppelin notebooks to do this work.

Estimated time: 20 - 30 minutes

### Objectives

- Import an Apache Zeppelin notebook.
- Become familiar with Oracle Machine Learning Algorithms.
- Create a machine learning model to determine factors that predict fraud.

### Prerequisites

This lab assumes you have completed the following labs:
<if type="freetier">
- Sign Up for Free Tier Account/Login to Oracle Cloud
- Provision and Setup ADB
</if>
<if type="livelabs">
- Launch the workshop (in the Introduction)
</if>

## Task 1: Import ML Notebooks

We have built the steps that are normally followed when exploring data and building a machine learning model. This has been saved to the file you can download. We will import this notebook and review it. It is important to note that you *must execute all the steps in this notebook*. Executing the steps takes only a few minutes.

1. From the tab on your browser with your ADW instance, in the Tools tab, select **Open Oracle ML Administration** and (if required) login with the admin credentials. <if type="livelabs">Your admin password is the password you copied from the Launch page.</if>

    ![](images/adw-open-ml-user-admin.png)

    ![](images/login_user.png)

2. Click the home button to login in with the OMLUSER.

    ![](images/oml-user-homebutton.png)

3. Sign in with the omluser using the password <if type="freetier">you created</if><if type="livelabs">`AAbbcc123456`</if>.

    ![](images/login_user.png)

4. Click on Notebooks from the Quick Actions menu.

    ![](images/open-notebooks.png)

5. [**CLICK HERE** to download the AutoInsuranceClaimsFraudUnsupervisedLearning.json notebook file](files/AutoInsuranceClaimsFraudUnsupervisedLearning.json?download=1).

6. [**CLICK HERE** to download the AutoInsuranceClaimsFraudSupervisedLearning.json notebook file](files/AutoInsuranceClaimsFraudSupervisedLearning.json?download=1).

7. Click on **Import**.

    ![](images/import-notebook.png)

6. Go to the directory where you downloaded the files and import the **Auto-Insurance-Claims-Fraud-Unsupervised-Learning.json** notebook.

    ![](images/import-unsuper-notebook.png)

7. Repeat and import the **Auto-Insurance-Claims-Fraud-Supervised-Learning.json** notebook.

    ![](images/import-super-notebook.png)

## Task 2: - Working Unsupervised Auto Claims

1.  Select the **Auto Insurance Claims Fraud - Unsupervised Learning** notebook to open it.

    ![](./images/unsuper-learning-notebook.png  " ")

2.  Before you start working the **Auto Insurance Claims Fraud - Unsupervised Learning** you need to set the interpreter binging. Click on the gear icon.

    ![](./images/unsuper-learning-notebook-binding-1.png  " ")

3.  Click the low and medium bindings to disable them and click **Save**.

    ![](./images/unsuper-learning-notebook-binding-2.png  " ")

4.  Click on the **Run All Paragraphs** icon to run all paragraphs in the notebook, then click **OK**.

    ![](./images/run-all.png  " ")

    ![](images/run-all-ok.png)

5.  Click on the **Show/Hide the Output** icon to show the output and ensure that all the paragraphs are in **Finished** state.

    ![](./images/show-hide-output-2.png  " ")

    Click the **Show/Hide the Output** icon again to return to the paragraphs.

## Task 3: About this Notebook

This step discusses the result of each portion of the notebook.

1. Lets use Python to access the datasets. You can access the datasets directly from Github or the database.

    ![](images/unsuper-1.png)

2. Create dataset without the fraud flag column for unsupervised learning task(CLAIMS_UNSPV).

    ![](images/unsuper-2.png)

3. The next section illustrates how we can graph our understanding of the data.

    ![](images/unsuper-3.png)

4. Data Exploration - Use Visualizations to better understand the data (Find any missing Patterns etc.)
    
    ![](images/unsuper-4.png)

5. Build the Anomaly Detection Model - Using 1-Class SVM.

    ![](images/unsuper-5.png)

6. Examples of possible setting overrides for SVM - Update the Model Settings if required.

    ![](images/unsuper-6.png)

7. Apply ML model to CLAIMS to flag which Claims are likely to be fraudulent.

    ![](images/unsuper-9.png)

8. Display Suspicious Claims by Number of Cars in Accident and Age of the Policy Holder.

    ![](images/unsuper-7.png)

9. Build the table of suspicious claims - Visualize using Oracle Analytics Cloud (OAC).

    ![](images/unsuper-10.png)

10. Finally, lets explore those suspicious claims.

    ![](images/unsuper-8.png)



You may now [proceed to the next lab](#next).

## Acknowledgements

- **Author** - Mark Hornick , Sr. Director, Data Science / Machine Learning PM

- **Last Updated By/Date** - Siddesh Ujjni, Senior Cloud Engineer, October 2021

