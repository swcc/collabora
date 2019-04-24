# collabora
Installs collabora and runs it

## Requirements

Debian or Ubuntu
Webserver to expose Collabora

## Role Variables


| Name                   | Required/Default      | Description                             |
|:-----------------------|:---------------------:|:----------------------------------------|
| `collabora_domain`     | :heavy_check_mark:    | Domain where your nextcloud is running  |
| `collabora_servername` | :heavy_check_mark:    | Domain the collabora instance runs on   |
| `collabora_password`   | :heavy_check_mark:    | Password for the Collabora Admin        |
| `collabora_username`   | `collabora_admin`     | Admin user for the web interface        |


## Example

```yaml
collabora:
  - collabora_domain: nextcloud.example.de
    collabora_username: admin
    collabora_password: YourPassword
    collabora_servername: collabora.example.de
```


## License

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).


## Author Information

 * [Rebekka Riedlinger (Rebexter)](https://github.com/Rebexter)_rebekka.riedlinger@stuvus.uni-stuttgart.de_

 * [Fritz Otlinghaus (Scriptkiddi)](https://github.com/Scriptkiddi) _fritz.otlinghaus@stuvus.uni-stuttgart.de_
