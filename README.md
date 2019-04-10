# collabora
Installs the collabora docker container and runs it

## Requirements

Debian or Ubuntu
An install [docker instance](https://github.com/stuvusIT/docker/)

## Role Variables


| Name                | Required/Default      | Description                            |
|:--------------------|:---------------------:|:---------------------------------------|
| `collabora_domains` | :heavy_check_mark:    | Domain where your nextcloud is running |
| `collabora_ports`   | `127.0.0.1:9980:9980` | Port the docker container listens on   |

Example

```yaml
collabora:
  - collabora_domains: nextcloud.example.com
```


## License

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).


## Author Information

 * [Fritz Otlinghaus (Scriptkiddi)](https://github.com/Scriptkiddi) _fritz.otlinghaus@stuvus.uni-stuttgart.de_
