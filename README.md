# AWS - Robo Advisor for Retirement Plans
The purpose of this exercise if to create a robo advisor create that could be used by customers or potential new customers to get investment portfolio recommendations for retirement.

Amazon Web Services and Python are used to create a bot that recommends an investment portfolio for a retirement plan.

## Overview of tasks performed
1. **Initial Robo Advisor Configuration:** </br>
* Define an Amazon Lex bot with a single intent that establishes a conversation about the requirements to suggest an investment portfolio for retirement.
2. **Build and Test the Robo Advisor:** <br/>
* Ensure the bot is working and responding accurately along with the conversation with the user, by building and testing it.

3. **Enhance the Robo Advisor with an Amazon Lambda Function:** <br/>
* Create an Amazon Lambda function that validates the user's input and returns the investment portfolio recommendation. This task includes testing the Amazon Lambda function and making the integration with the bot.

### Files
The following files are generated in support of the solution to the robo advisor: <br/>
* [Robo Advisor Lambda function](robo_advisor.ipynb) - Python script with final lambda function
* Amazon Lex Console components:
   * [AWS Lex - Bot](AWS Lex files/RoboAdvisor_1_Bot_LEX_V1.zip)
   * [AWS Lex - Intent](AWS Lex files/RecommendPortfolio_Intent_LEX_V1.zip)
   * [AWS Lex - Slot](AWS Lex files/RecommendPortfolio_Intent_LEX_V1.zip)
