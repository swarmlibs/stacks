# About

Open-source cron job and background task monitoring service, written in Python & Django

> [!NOTE]
> For the sake of simplicity, the sample configuration starts a single database
> node and a single web server node, both on the same host. It does not handle TLS
> termination.

## Environment Variables

* `ALLOWED_HOSTS` – the domain name of your Healthchecks instance. Example: `ALLOWED_HOSTS=hc.example.org`.
* `DEFAULT_FROM_EMAIL` – the "From:" address for outbound emails.
* `EMAIL_HOST` – the SMTP server.
* `EMAIL_HOST_PASSWORD` – the SMTP password.
* `EMAIL_HOST_USER` – the SMTP username.
* `SECRET_KEY` – secures HTTP sessions, set to a random value.
* `SITE_ROOT` – The base public URL of your Healthchecks instance. Example: `SITE_ROOT=https://hc.example.org`.
