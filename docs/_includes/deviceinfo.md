{% assign device = site.data.devices[page.codename] %}
[Home]({{ "/" | relative_url }})

# {{ page.title }} ({{ page.codename }})



{% assign ota_url = site.lineage_ota_base_url-19_1 | append: page.codename | append: ".json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>
<a href="{{ device.xda_191 }}">XDA forum thread for LineageOS-19.1</a><br>
[Changelog for LineageOS-19.1]({{ "/changes/" | append: page.codename | append: ".html" | relative_url }}) 

{% assign ota_url = site.lineage_ota_base_url-18_1 | append: page.codename | append: ".json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>
<a href="{{ device.xda_181 }}">XDA forum thread for LineageOS-18.1</a>

{% if device.shipped_version == "Android 6.0" %}

{% assign ota_url = site.lineage_ota_base_url-17_1 | append: page.codename | append: ".json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>
<a href="{{ device.xda_171 }}">XDA forum thread for LineageOS-17.1</a>
{% endif %}

{% if device.shipped_version == "Android 6.0" %}
If you want to use Zygisk please use Magisk 24.1 for time being due to [regression in Magisk](https://github.com/topjohnwu/Magisk/issues/5395)
{% endif %}
[Telegram support group]({{device.tg}})

{% include donations.md %}

## Device specifications

<table>
    <tbody>
        <tr>
            <td align="left" colspan="2"><img src="{{ "/images/" | append: page.codename | append: ".png" | relative_url}}" style="max-height: 500px"></td>
        </tr>
        <tr>
            <td align="left">Released on</td>
            <td align="left">{{ device.released }}</td>
        </tr>
        <tr>
            <td align="left">Chipset</td>
            <td align="left">{{ device.chipset }}</td>
        </tr>
        <tr>
            <td align="left">CPU</td>
            <td align="left">{{ device.cpu }}</td>
        </tr>
        <tr>
            <td align="left">GPU</td>
            <td align="left">{{ device.gpu }}</td>
        </tr>
        <tr>
            <td align="left">RAM</td>
            <td align="left">{{ device.ram }}</td>
        </tr>
        <tr>
            <td align="left">Shipped Android Version</td>
            <td align="left">{{ device.shipped_version }}</td>
        </tr>
        <tr>
            <td align="left">Storage</td>
            <td align="left">{{ device.storage }}</td>
        </tr>
        <tr>
            <td align="left">Battery</td>
            <td align="left">{{ device.battery }}</td>
        </tr>
        <tr>
            <td align="left">Dimensions</td>
            <td align="left">{{ device.dimensions }}</td>
        </tr>
        <tr>
            <td align="left">Display</td>
            <td align="left">{{ device.display }}</td>
        </tr>
{% for rear_camera in device.rear_camera %}
        <tr>
            <td align="left">Rear Camera</td>
            <td align="left">{{ rear_camera }}</td>
        </tr>
{% endfor %}
{% for front_camera in device.front_camera %}
        <tr>
            <td align="left">Front Camera</td>
            <td align="left">{{ front_camera }}</td>
        </tr>
{% endfor %}
        <tr>
            <td align="left">Sensors</td>
            <td align="left">{{ device.sensors }}</td>
        </tr>
    </tbody>
</table>
