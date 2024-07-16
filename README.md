## Estimated Time: 120 minutes

Note: Though this lab is split into multiple parts, it is highly recommended it is all completed in one sitting as the project environment may not be persisted. If for any reason that is not possible, please push your changes to git so that the changes are copied to your remote repository and you can start where you left.

## Pre-requisite:

You need to complete [Practice Assignment - Hands-on Lab: Budget Allocation Application](https://cf-courses-data.static.labs.skills.network/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/Practice_Project.md.html) before you start with the final project, as this will be the base code on which you will build the React application for the Final Project.  

## Part A: Git clone the Git repository to have the react code you need to start

1. Open a terminal window by using the menu in the editor: Terminal > New Terminal.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/new-terminal.png)

2. Clone the repository you cloned, edited and git pushed in the [Practice Assignment - Hands-on Lab: Budget Allocation Application](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/Practice_Project.md.html "Practice Assignment - Hands-on Lab: Budget Allocation Application") with all the components added by running the command given below:

1. `git clone <your_repo_name>`

Copied!

3. This will clone the repository with budget allocation app files in your home directory in the lab environment. Check the same with the following command.

1. `ls`

Copied!Executed!

4. Change to the project directory and check its contents.

1. `cd ejtos-react_budget_app && ls`

Copied!Executed!

> Note: Remove the ‘node_modules’ folder in the main project and directories before running npm install command to install the packages. This is necessary to ensure that all package installation commands run correctly.

5. All packages are needed to be installed are listed in package.json. Run npm install -s, to install and save those packages.

1. `npm install -s

## Part B: Launch and view your react app on the browser

1. Make sure you are in the `ejtos-react_budget_app` directory and run the server using the following command.

1. `npm start`

Copied!

2. Click on the Skills Network button on the left, it will open the **“Skills Network Toolbox”**. Then click the **Other** then **Launch Application**. From there you should be able to enter the port `3000`.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/Launch_Application-SN-ToolBox.png)

## Part C: Enhancement of the Budget Allocation Application

_**Disclaimer:** Please note that the screenshots provided in the lab instructions are intended only as a reference and your budget application is not required to replicate the exact styling shown. You are encouraged to unleash your creativity and enhance the visual design of the budget application according to your own vision. It is also important to consider that the hover effect might vary slightly depending on the web browser being used._

### Task 1: Budget allocation Validation

Add validation to the existing budget allocation component.

- It should accept only number value. Take a screenshot and save it as **budget_allocation.png**.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/budget_allocation.PNG)

- The value should not exceed the remaining budget. Take a screenshot and save it as **budget_allocation_error message.png**.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/budget_allocation_error_message.PNG)

### Task 2: Editable budget value

Update the code to make **Budget** editable with option to increase and decrease its value by 10. Take a screenshot and save it as **budget_value.png**.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/task_1.PNG)

Set the upper limit value to 20,000. Take a screenshot of error message when it is more than 20000 and save it as **budget_not_exceeding.png**.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/budget_not_exceeding.PNG)

It should not allow for the budget to be lower than the spending, as that is already allocated. Take a screenshot of error message when it is lower than spending and save it as **budget_morethan_spending.png**.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/budget_morethan_spending.PNG)

### Task 3: Dropdown to change currency

Update the code to change the currency along with the drop-down option. Add these four currencies: $ Dollar,£ Pound,€ Euro,₹ Ruppee. Take a screenshot and save it as **curreny_dropdown.png**.

- Add a **Currency** label in the appropriate place.
- Stylize the dropdown (Use image provided for refernce).

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/task_2.png)

### Task 4: Currency prefix to the **Change allocation** textbox.

Add a currency prefix to the **Change allocation** textbox. Take a screenshot and save it as **budget_allocation_with_currency.png**.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/budget_allocation_with_currency.PNG)

### Task 5: Currency prefix to the **Budget value** textbox.

Add a currency prefix to the **Budget Value** textbox. Take a screenshot and save it as **budget_value_with_currency.png**.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/budget_value_with_currency.PNG)

### Task 6: Change event of the currency dropdown

Add event handler to the dropdown for Currency component change event. On change of the dropdown value, all the currency representation on the screen changes, in the following places.

- Budget
- Remaining
- Spent so far
- Allocated Budget
- Change Allocation

Change the currecy in the dropdown from £ to another symbol and take a screenshot of the whole page reflecting the changes and save it as **currency_change.png**.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/currency_change.PNG)

### Task 7: Decrease and Increase Buttons

Add a decrease button, like the increase button you added in the [Practice Assignment - Hands-on Lab: Budget Allocation Application](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/Practice_Project.md.html "Practice Assignment - Hands-on Lab: Budget Allocation Application"), to all the departments in the allocation, beside increase by 10 as shown in the screenshot. Stylize the button using these images. Styling of buttong should be done according to the reference provided.

- Click the plus button next to **Marketing** department and show that the the value increases by 10. Take a screenshot and save it as **mktgplus10.png**

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/mktgplus10.PNG)

- Click the minus button next to **IT** and show that the the value decreases by 10. Take a screenshot and save it as **itminus10.png**

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/itminus.PNG)

Your final React budget allocation application page should look like this:

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CD0210EN-SkillsNetwork/labs/Final%20project-budget%20app/images/finalbudget.png)

Congratulations! You have completed this Final Project lab and know how to create a budget allocation application.

### Author(s)

#### Pallavi Rai

### © IBM Corporation. All rights reserved.
