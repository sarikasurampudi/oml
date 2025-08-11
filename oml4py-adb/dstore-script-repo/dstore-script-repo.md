# Store and manage Python objects and user-defined functions

## Introduction

This lab walks you through the steps to use and work with OML4Py datastores and the script repository.

Estimated Time: 20 minutes

### About datastores
Datastores exist in the user’s Oracle database schema. A datastore, and the objects it contains, persist in the database until explicitly deleted. By using a datastore, you can store Python objects in a named datastore entry. This named datastore can then be used in subsequent Python sessions, and even be made available to other users or programs by granting/revoking read permissions.

Python objects, including Oracle Machine Learning for Python (OML4Py) proxy objects, exist for the duration of the current Python session unless you explicitly save them. You can save one or more Python objects, including OML proxy objects, to a named datastore and then load those objects in a later Python session. This is also useful when using embedded Python execution.
By using a datastore, you can:
* Save OML4Py and other Python objects for use across Python sessions.
* Grant or revoke read privilege access to a datastore or its objects to one or more users. You can restore the saved objects in another Python session.
* Easily pass multiple and non-scalar arguments to Python functions for use in embedded Python execution from Python, REST, and SQL  API.
  >**Note:** SQL and REST APIs support passing scalar values, such as datastore name or numeric values, only.

* List available datastores and explore datastore contents.

### About the Python script repository

OML4Py stores named user-defined functions called scripts in the script repository. You can make scripts either private or global. A private script is available only to the owner. A global script is available to any user. For private scripts, the owner of the script may grant the read privilege to other users or revoke that privilege.

* `oml.script.create` - Creates a script, which contains a single Python function definition, in the script repository.
* `oml.script.dir` - Lists the scripts present in the script repository.
* `oml.script.drop` - Drops a script from the script repository.
* `oml.script.load` - Loads a script from the script repository into a Python session.
* `oml.grant` - Grants read privilege permission to another user to a datastore or script owned by the current user.
* `oml.revoke` - Revokes the read privilege permission that was granted to another user to a datastore or script owned by the current user.

### Objectives

In this lab, you will learn how to:

**Datastores**
  * Move objects between datastore and a Python sessions
  * Save Python objects in a datastore
  * Save model objects in a datastore
  * Load datastore objects into memory
  * View datastore and its details
  * Manage datastore privileges
  * Delete datastores

**Python script repository**
  * Use the Python Script Repository
  * Create Scripts in Repository
  * Store a function as a global function
  * Drop scripts from the Script Repository

### Prerequisites

1. We need to access and run the OML notebook for this lab.

    > **NOTE:** If you have problems with downloading and extracting the ZIP file in Lab 1 Task 2, please [**CLICK HERE** to download the "Lab 4 - Store and manage Python objects and UDFs" notebook DSNB file](<./../notebooks/Lab 4 - Store and manage Python objects and UDFs.dsnb?download=1>). This notebook contains the scripts for **Lab 4**. Save it to your local machine and import it like illustrated in **Lab 1, Task 2, Step 1**.

    Go back to the main Notebooks page by clicking on the Cloud menu icon ![](images/cloud-menu-icon.png) on the upper left of the screen to open the left navigation pane, and then click **Notebooks**. 

    ![Go to main Notebooks EA](images/go-back-to-notebooks-rw.png " ")

    Click the **Lab 4** notebook to view it.

    <if type="freetier">
    ![Open Lab 4 notebook ft](images/click-on-lab4-ft.png " ") </if>
    <if type="livelabs">
    ![Open Lab 4 notebook ll](images/click-on-lab4-ft.png " ") </if>
    <if type="freetier-ocw23">
    ![Open Lab 4 notebook ft](images/click-on-lab4-ft-ocw23.png " ") </if>
    <if type="livelabs-ocw23">
    ![Open Lab 4 notebook ll](images/click-on-lab4-ft-ocw23.png " ") </if>

    OML Notebooks will create a session and make the notebook available for editing.

    You can optionally click the **Run all paragraphs** (![](images/run-all-paragraphs.png =20x*)) icon, and then click **Confirm** to refresh the content with your data, or just scroll down and read the pre-recorded results.  

    ![Lab 4 main screen](images/lab4-main.png " ")

## Task 1: Import libraries supporting OML4Py and create data table

1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 1.

  ![Import libraries supporting OML4Py](images/lab4-task1.png " ")  

## Task 2: Create pandas dataFrames and load them into Oracle Autonomous Database

1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 2.

  ![Create pandas dataFrames and load them](images/lab4-task2.png " ")  

## Task 3: Save Python objects to a datastore instance
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 3.

  ![Save Python objects to a datastore](images/lab4-task3.png " ")  

## Task 4: Save model objects in a datastore instance
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 4.

  ![Save model objects in a datastore](images/lab4-task4.png " ")  

## Task 5:  Load datastore objects into memory
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 5.

  ![Load datastore objects into memory](images/lab4-task5.png " ")  

## Task 6: View datastores and other details
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 6.

  ![View datastores and other details](images/lab4-task6.png " ")  

## Task 7: View contents of a datastore
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 7.

  ![View contents of a datastore](images/lab4-task7.png " ")     

## Task 8: Manage datastore privileges
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 8.

  ![Manage datastore privileges](images/lab4-task8.png " ")  

## Task 9: Delete datastore content
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 9.

  ![Delete datastore content](images/lab4-task9.png " ")

## Task 10: Use the Python Script Repository
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 10.

  ![Use the Python Script Repository](images/lab4-task10.png " ")  

## Task 11: Create scripts in repository
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 11.

  ![Create scripts in repository](images/lab4-task11.png " ")  

## Task 12: Store a function as a global function
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 12.

  ![Store a function as a global function](images/lab4-task12.png " ")  

## Task 13: Drop scripts from the script repository
1. Follow the flow of the notebook by scrolling to view and run each paragraph of this lab.

  Scroll down to the beginning of Task 13.

  ![Drop scripts from the script repository](images/lab4-task13.png " ")  

After you reach the end of Lab 4, you can *proceed to the next lab*.

## Learn More

* [Get started with OML4Py Datastores](https://docs.oracle.com/en/database/oracle/machine-learning/oml4py/2/mlpug/get-started-oracle-machine-learning-python1.html#GUID-C02396D1-2B30-47A0-AE27-37B123E15710)
* [Get started with OML4Py Script Repository](https://docs.oracle.com/en/database/oracle/machine-learning/oml4py/2/mlpug/save-and-manage-functions-for-embedded-python-execution.html#GUID-74671038-15FE-44BB-A657-C89C16C1EF43)
* [Oracle Machine Learning Notebooks](https://docs.oracle.com/en/database/oracle/machine-learning/oml-notebooks/)

## Acknowledgements
* **Authors** - Marcos Arancibia, Product Manager, Machine Learning; Jie Liu, Data Scientist; Moitreyee Hazarika, Principal User Assistance Developer; Dhanish Kumar, Senior Member of Technical Staff
* **Contributors** -  Mark Hornick, Senior Director, Data Science and Machine Learning; Sherry LaMonica, Principal Member of Tech Staff, Machine Learning
* **Last Updated By/Date** - Dhanish Kumar, July 2025
