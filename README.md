# Sending-Email-WhatsApp-Tweets-SNS-from-Linux-CLI
# 1️⃣ Send an Email from Linux CLI

Using mail or mutt (configured with SMTP):
```
echo "Hello, this is a test email from Linux CLI" | mail -s "Test Email" user@example.com
```

Or with ```ssmtp``` / ```msmtp``` configured for Gmail/SMTP.

# 2️⃣ Send WhatsApp Messages

With yowsup (unofficial WhatsApp CLI library):
```
yowsup-cli demos -c config.example --send 91xxxxxxxxxx "Hello from Linux Terminal!"
```

⚠️ Note: ```yowsup``` is unofficial and may break due to WhatsApp changes.

# 3️⃣ Send a Tweet from Linux

With t (Twitter CLI tool):
```
t update "Hello World from Linux Terminal! #Linux #Automation"
```

👉 You’ll need to authenticate once with your Twitter account.

# 4️⃣ Send an AWS SNS Notification

Using AWS CLI:
```
aws sns publish \
  --topic-arn arn:aws:sns:us-east-1:123456789012:MyTopic \
  --message "This is a Linux CLI SNS test notification"
```
