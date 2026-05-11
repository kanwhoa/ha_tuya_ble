# Home Assistant support for Tuya BLE devices

## Overview

This integration supports Tuya devices connected via BLE.

_Fork of the [@PlusPlus-ua ha_tuya_ble](https://github.com/PlusPlus-ua/ha_tuya_ble) project_

## Installation

Place the `custom_components` folder in your configuration directory (or add its contents to an existing `custom_components` folder). <!-- Alternatively install via [HACS](https://hacs.xyz/). -->

<!--
[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=PlusPlus-ua&repository=ha_tuya_ble&category=integration)
-->

## Usage

After adding to Home Assistant integration should discover all supported Bluetooth devices, or you can add discoverable devices manually.

The integration works locally, but connection to Tuya BLE device requires device ID and encryption key from Tuya IOT cloud. It could be obtained using the same credentials as in official Tuya integration. To obtain the credentials, please refer to official Tuya integration [documentation](https://www.home-assistant.io/integrations/tuya/)

## Supported devices list

<table>
    <thead>
        <tr>
            <th>Category identifier</th>
            <th>Product Identifier</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan="14"><code>szjqr</code></td>
            <td><code>ltak7e1p</code></td>
            <td rowspan="7">Fingerbot - original device, first in category, powered by CR2 battery</td>
        </tr>
        <tr>
            <td><code>y6kttvd6</code></td>
        </tr>
        <tr>
            <td><code>yrnk7mnn</code></td>
        </tr>
        <tr>
            <td><code>nvr2rocq</code></td>
        </tr>
        <tr>
            <td><code>bnt7wajf</code></td>
        </tr>
        <tr>
            <td><code>rvdceqjh</code></td>
        </tr>
        <tr>
            <td><code>5xhbk964</code></td>
        </tr>
        <tr>
            <td><code>y6kttvd6</code></td>
            <td>Adaprox Fingerbot - built-in battery with USB type C charging</td>
        </tr>
        <tr>
            <td><code>blliqpsj</code></td>
            <td rowspan="4">Fingerbot Plus - almost same as original, has sensor button for manual control</td>
        </tr>
        <tr>
            <td><code>ndvkgsrm</code></td>
        </tr>
        <tr>
            <td><code>yiihr7zh</code></td>
        </tr>
        <tr>
            <td><code>neq16kgd</code></td>
        </tr>
        <tr>
            <td><code>3yqdo5yt</code></td>
            <td>CubeTouch 1s - built-in battery with USB type C charging.</td>
        </tr>
        <tr>
            <td><code>xhf790if</code></td>
            <td>CubeTouch II - built-in battery with USB type C charging.</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td><code>wsdcg</code></td>
            <td><code>ojzlzzsw</code></td>
            <td>Soil moisture sensor</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td><code>co2bj</code></td>
            <td><code>59s19z5m</code></td>
            <td>CO2 Detector</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan="2"><code>ms</code></td>
            <td><code>ludzroix</code></td>
            <td rowspan="2">Smart Lock</td>
        </tr>
        <tr>
            <td><code>isk2p555</code></td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan="2"><code>wk</code></td>
            <td><code>drlajpqc</code></td>
            <td rowspan="2">Thermostatic Radiator Valve</td>
        </tr>
        <tr>
            <td><code>nhj2j7su</code></td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td><code>znhsb</code></td>
            <td><code>cdlandip</code></td>
            <td>Smart water bottle</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td><code>ggq</code></td>
            <td><code>6pahkcau</code></td>
            <td>Irrigation computer</td>
        </tr>
    </tbody>
</table>

### Fingerbot notes

All features available in Home Assistant, programming (series of actions) is implemented for Fingerbot Plus.
For programming exposed entities 'Program' (switch), 'Repeat forever', 'Repeats count', 'Idle position' and 'Program' (text). Format of program text is: 'position\[/time\];...' where position is in percents, optional time is in seconds (zero if missing).

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
