# MTA Drop
Sends an email to a **single recipient** straight to his MTA.
Looks up for the MX DNS records of the recipient SMTP server and attempts the delivery through them.

## Requirements
* PHP 5.5.9-1

## Install
Just download and give it execution permissions:
```
curl -o ./mtadrop https://raw.githubusercontent.com/jorgebg/mtadrop/master/mtadrop && chmod +x ./mtadrop
```

## Usage
```
usage: mtadrop [-fSENDER] [-mMESSAGE] RECIPIENT [SUBJECT]
```

## Examples
```
./mtadrop recipient@example.com
./mtadrop recipient@example.com "To infinity..."
./mtadrop -f"sender@example.com" recipient@example.com "To infinity..."
./mtadrop -m"...and beyond!" recipient@example.com "To infinity..."
```
