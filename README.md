# collabora
Installs collabora and runs it

## Requirements

Debian or Ubuntu with a webserver that exposes Collabora.
Note that SSL included in Collabora is deactivated and should be configured in your webserver.

## Role Variables


| Name                     | Required/Default   | Description                                                                      |
|:-------------------------|:------------------:|:---------------------------------------------------------------------------------|
| `collabora_domain`       | :heavy_check_mark: | Domain where your nextcloud is running                                           |
| `collabora_servername`   | :heavy_check_mark: | Domain the collabora instance runs on                                            |
| `collabora_password`     | :heavy_check_mark: | Password for the Collabora Admin                                                 |
| `collabora_username`     | `collabora_admin`  | Admin user for the web interface                                                 |
| `collabora_version`      | `6.4`              | The version of collabora to install                                              |
| `collabora_extra_params` | `{}`               | Configure extra collabora system parameters. Use a dot separated string as keys. |


## Example

```yaml
collabora:
  - collabora_domain: nextcloud.example.de
    collabora_username: admin
    collabora_password: YourPassword
    collabora_servername: collabora.example.de
    collabora_extra_params:
      'welcome.enable': false
```


## License

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).


## Author Information

 * [Rebekka Riedlinger (Rebexter)](https://github.com/Rebexter)_rebekka.riedlinger@stuvus.uni-stuttgart.de_
 * [Fritz Otlinghaus (Scriptkiddi)](https://github.com/Scriptkiddi) _fritz.otlinghaus@stuvus.uni-stuttgart.de_
