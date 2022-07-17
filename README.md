# balena-seafile

[Seafile](https://seafile.com) is an open source file sync & share solution designed for high reliability, performance and productivity.

## Getting Started

You can one-click-deploy this project to balena using the button below:

[![deploy-with-balena](https://balena.io/deploy.svg)](https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/klutchell/balena-seafile)

## Manual Deployment

Alternatively, deployment can be carried out by manually creating a [balenaCloud account](https://dashboard.balena-cloud.com) and application, flashing a device, downloading the project and pushing it via the [balena CLI](https://github.com/balena-io/balena-cli).

## Usage

Once your device joins the fleet you'll need to allow some time for it to download the various services.

When it's done you should be able to access the access the dashboard at <http://seafile.local>.

Documentation for Seafile can be found at <https://manual.seafile.com/>.

## Customization

### Environment Variables

| Name                     | Description                                                                                                       |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------- |
| `TIME_ZONE`              | Inform services of the [timezone](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) in your location. |
| `SEAFILE_ADMIN_EMAIL`    | Specifies Seafile admin user, default is `admin@example.com`.                                                        |
| `SEAFILE_ADMIN_PASSWORD` | Specifies Seafile admin password, default is `asecret`.                                                           |

### Backups

Encrypted offsite backups can be enabled with the included [restic block](https://github.com/klutchell/balena-restic).

### Hostname

The device hostname will automatically be changed to `seafile` via the included [hostname block](https://github.com/balenablocks/hostname).

## Contributing

Please open an issue or submit a pull request with any features, fixes, or changes.
