sqslite
=======

Amazon SQS Lite/Simple CLI for getting messages in and out of SQS

= Send a message =

```
export AWS_ACCESS_KEY_ID=whatever
export AWS_SECRET_ACCESS_KEY=whatever
echo "message" | sqslite -q queue-name -r us-east-1
```

= Receive a message =

```
sqslite -q queue-name -r us-east-1
```

= Delete a message =
```
echo "ReceiptHandlerId" | sqslite -q queue-name -r us-east-1 -d
```