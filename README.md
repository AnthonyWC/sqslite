sqslite
=======

Amazon SQS Lite/Simple CLI for getting messages in and out of Amazon SQS

### Send a message

```
export AWS_ACCESS_KEY_ID=whatever
export AWS_SECRET_ACCESS_KEY=whatever
echo "message" | sqslite -q queue-name -c s
```

### Receive a message

```
sqslite -q queue-name
```

### Delete a message
```
echo "ReceiptHandlerId" | sqslite -q queue-name -c d
```

### Full Example

See examples folder for the work script. You can run the script like this:

```
QUEUE_NAME=sqslite QUEUE_REGION=us-east-1 ./work job
```
