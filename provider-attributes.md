## Provider Attributes Information

| Key                         | Type               | Required | Description                                                            |
|---------------------------- |--------------------|----------|------------------------------------------------------------------------|
| host                        | string             | true     | Name of the host. Ex.: 'd3akash.cloud'.                                |
| email                       | string             | true     | Email associated with the provider.                                    |
| organization                | string             | true     | Name of the organization that owns the provider.                       |
| website                     | string             | false    | Link to the organization's website.                                    |
| status-page                 | string             | false    | Link to a status page for the provider.                                |
| location-region             | option             | true     | Geo location region of the provider. Based on the United Nations geoscheme. [UN Geoscheme](https://en.wikipedia.org/wiki/United_Nations_geoscheme) |
| country                     | string             | false    | Country ISO 3166 Alpha-2 code of the provider. [ISO 3166 Country Codes](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes) |
| city                        | string             | false    | City 3 letter code of the provider. [Harbor Codes](https://www.hh-express.com/en/support/three_code/harbor.html) |
| timezone                    | option             | false    | Timezone UTC-12 to UTC+14 of the provider. [Timezone Map](https://www.timeanddate.com/time/map/) |
| location-type               | option             | false    | One of: datacenter, colo, home, office, mix.                            |
| hosting-provider            | string             | false    | Name of the datacenter, colo, public cloud, etc where hosted.          |
| hardware-cpu                | option             | true     | CPU manufacturer.                                                      |
| hardware-cpu-arch           | option             | false    | CPU architecture.                                                      |
| hardware-gpu                | option             | false    | GPU manufacturer.                                                      |
| hardware-gpu-model          | multiple-option    | false    | GPU model.                                                             |
| hardware-disk               | multiple-option    | true     | Storage type.                                                          |
| hardware-memory             | option             | true     | Memory (RAM) type.                                                     |
| network-provider            | string             | false    | Internet service provider.                                             |
| network-speed-up            | number             | false    | Upload Bandwidth in mbps.                                             |
| network-speed-down          | number             | false    | Download Bandwidth in mbps.                                           |
| feat-persistent-storage      | boolean            | true     | True if the provider offers persistent storage.                        |
| feat-persistent-storage-type | option             | false    | Type of persistent storage offered.                                    |
| tier                        | option             | false    | Is this an Akash hosted provider or community hosted?                 |
| workload-support-chia        | boolean            | false    | Does this provider support Chia plotting?                             |
| workload-support-chia-capabilities | option      | false    | Specific capabilities for Chia support.                                |
| feat-endpoint-ip            | boolean            | false    | Does this provider support leasing of IP addresses?                    |
| feat-endpoint-custom-domain  | boolean            | false    | Does this provider support custom domains?                             |
