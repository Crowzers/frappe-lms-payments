# Frappe LMS + Payments (Docker / Coolify)

Self-hosted Learning Management System built with **Frappe LMS** and **Frappe Payments**, ready to deploy with Docker or Coolify.

This setup includes:

* Frappe Framework v15
* Frappe LMS
* Frappe Payments
* MariaDB
* Redis
* Docker deployment

## Features

* Online courses
* Paid course enrollment
* Stripe payments
* Self-hosted LMS
* Works with Coolify or Docker

## Requirements

* Docker
* Docker Compose
* 2GB RAM minimum recommended

## Deployment (Coolify)

1. Create a new **Application** in Coolify
2. Connect this repository
3. Coolify will automatically detect the **Dockerfile**
4. Deploy

After deployment, create the site:

```bash
bench new-site frontend \
--admin-password admin \
--db-root-username root \
--db-root-password admin \
--install-app lms \
--install-app payments
```

Enable scheduler:

```bash
bench --site frontend enable-scheduler
```

## Access

LMS will be available on:

```
http://your-domain:8080
```

## Apps Included

* frappe
* lms
* payments

## Use Case

Perfect for:

* selling online courses
* memberships
* coaching programs
* creator academies

## License

Open Source – based on Frappe Framework and Frappe LMS.
