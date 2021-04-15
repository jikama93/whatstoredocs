# SMTP

You will need to have SMTP \( way to send mail \) because the system will use it to

This is probably the easiest way to obtain SMTP data. Create an email in your hosting and get note of the credentials. You will need them in the install process.

Then click on "Connect Device". You will find all required info there

SendGrid is the leading SMTP provider. Easy to set up and reliable service.

```text
MAIL_MAILER=smtpMAIL_HOST=smtp.sendgrid.netMAIL_PORT=587MAIL_USERNAME=apikeyMAIL_PASSWORD=xxxxxxxxxxxxxxxxxMAIL_ENCRYPTION=null​MAIL_FROM_NAME='Your Project name'
```

