# AWS - Robo Advisor for Retirement Plans
The purpose of this exercise if to create a robo advisor that could be used by customers or potential new customers to get investment portfolio recommendations for retirement.

Amazon Web Services and Python are used to create a bot that recommends an investment portfolio for a retirement plan.

## Overview of tasks performed:
1. **Initial Robo Advisor Configuration:** </br>
   * Define an Amazon Lex bot with a single intent that establishes a conversation about the requirements to suggest an investment portfolio for retirement. 
   * Add an intent with 4 corresponding slots, of which 3 are built-in and 1 is a custom slot that retrieves the risk level that the user is willing to take.

2. **Build and Test the Robo Advisor:** <br/>
   * Ensure the bot is working and responding accurately along with the conversation with the user, by building and testing it.

3. **Enhance the Robo Advisor with an Amazon Lambda Function:** <br/>
   * Amazon Lambda function is created that validates the user's input and returns the investment portfolio recommendation. This task includes testing the Amazon Lambda function with test cases supplied and making the integration with the bot.

   * User Input Validation:
      * The user age should be greater than zero and less than 65.
      * The investment amount should be equal to or greater than 5000.

   * Investment portfolio recommendation:
      * **none:** "100% bonds (AGG), 0% equities (SPY)"
      * **very low:** "80% bonds (AGG), 20% equities (SPY)"
      * **low:** "60% bonds (AGG), 40% equities (SPY)"
      * **medium:** "40% bonds (AGG), 60% equities (SPY)"
      * **high:** "20% bonds (AGG), 80% equities (SPY)"
      * **very high:** "0% bonds (AGG), 100% equities (SPY)"

## Files:
The following files are generated as the solution for the robo advisor: <br/>
* [Robo Advisor Lambda function](robo_advisor.ipynb) - Python script with final lambda function
* Amazon Lex Console components:
   * [AWS Lex Bot](AWS_Lex_files/RoboAdvisor_1_Bot_LEX_V1.zip)
   * [AWS Lex Intent](AWS_Lex_files/RecommendPortfolio_Intent_LEX_V1.zip)
   * [AWS Lex Slot](AWS_Lex_files/RecommendPortfolio_Intent_LEX_V1.zip)
* [Robo Advisor Solution Screen recording](RoboAdvisor_screen_recording) - short video showing a demo of Robo Advisor in action from the test window in Amazon Lex.<br/>
* Amazon Lex Lamda Function Test cases
   * [Age error test case](/test_cases/age_error.txt)
   * [Correct dialog](correct_dialog.txt)
   * [Incorrect amount](incorrect_amount_error.txt)
   * [Negative age](negative_age_error.txt)
