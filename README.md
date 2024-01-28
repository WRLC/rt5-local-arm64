# rt5-local
Local dev environment for Request Tracker 5 via Docker Compose

## Requirements

- Docker Desktop

## Usage

1. Clone this repo
2. Run `docker-compose up -d`
3. Open http://localhost:8080/ in your browser
4. Login with username `root` and password `secret`

## Notes
Customizations to the RT instance can be made by editing the `rt5/etc/RT_SiteConfig.pm` file.

Customizations to the Apache config can be made by editing the `rt5/etc/apache2/sites-available/000-default.conf` file. 

Changes will be applied when the container is restarted.

The only additional RT module installed by default is `RT::Extension::MergeUsers`. 