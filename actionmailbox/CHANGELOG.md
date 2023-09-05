*   Added `bounce_now_with` to send the bounce email without going through a mailer queue.

    *Ronan Limon Duparcmeur*

*   Support configured primary key types in generated migrations.

    *Nishiki Liu*

*   Fixed ingress controllers' ability to accept emails that contain no UTF-8 encoded parts.

    Fixes #46297.

    *Jan Honza Sterba*

*   Add X-Forwarded-To addresses to recipients.

    *Andrew Stewart*

*   Add Amazon SES/SNS ingress.

    Configure AWS SES inbound emails to store email content in AWS S3 and trigger AWS SNS notifications
    sent as an API endpoint request to the ActionMailbox inbound emails controller, subsequently creating
    an ActionMailbox::InboundEmail database record. Provides SNS subscription confirmation for configured
    SNS topics.

    *Bob Farrell*
    *Chris Ortman*
    *Marco Borromeo*

Please check [7-0-stable](https://github.com/rails/rails/blob/7-0-stable/actionmailbox/CHANGELOG.md) for previous changes.
