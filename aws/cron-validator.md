# Cron Validator

Source:  [Creating an Amazon EventBridge rule that runs on a schedule - Amazon EventBridge](https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-create-rule-schedule.html#eb-create-scheduled-rule)

1. Open Amazon EventBridge console
2. Select **Rules** from the navigation pane
3. Choose **Create rule**
4. Enter a name for the rule
5. Select the default event bus
6. For **Rule Type**, choose **Schedule**
7. Then click next
8. Enter the expression

⚠️ AWS does not use the standard cron syntax which is what most cron validators that are easy to find on Google use.