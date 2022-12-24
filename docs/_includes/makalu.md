{% assign device = 982X %}
[Home]({{ "/" | relative_url }})

# LineageOS 20 builds for Exynos 9820/9825 devices 


Rom will disable Encryption if it detects that twrp is being used, you can find copy of lineageos recovery inside of rom zip 
and flash that if you want to enable encryption (install rom from lineageos recovery in that case) <br><br>

Builds will be updated once a month to merge latest security updates and other changes<br>
<details>
  <summary>Changelog</summary>
- Added support for signature spoofing<br>
- OTA Updated built-in<br>
- Vendor partition is using ext4 so it can be modified by user<br>
- Kernel side wireguard support<br>
- Works on latest and older 12 firmwares<br>
- Rom will dynamically chose to encrypt or not to encrypt data based on installed recovery (if TWRP is installed encryption will be disabled)<br>
- Merged December 2022. Security update<br>
- Synced with LineageOS source<br><br><br>
</details>

{% assign ota_url = "https://raw.githubusercontent.com/ivanmeler/ota_provider/master/20.0/beyond2lte.json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>

{% assign ota_url = "https://raw.githubusercontent.com/ivanmeler/ota_provider/master/20.0/beyond1lte.json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>

{% assign ota_url = "https://raw.githubusercontent.com/ivanmeler/ota_provider/master/20.0/beyond0lte.json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>

{% assign ota_url = "https://raw.githubusercontent.com/ivanmeler/ota_provider/master/20.0/beyondx.json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>

{% assign ota_url = "https://raw.githubusercontent.com/ivanmeler/ota_provider/master/20.0/d2x.json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>

{% assign ota_url = "https://raw.githubusercontent.com/ivanmeler/ota_provider/master/20.0/d2s.json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>

{% assign ota_url = "https://raw.githubusercontent.com/ivanmeler/ota_provider/master/20.0/d1.json" %}
{% fetch builds_raw ota_url %}
{% json builds builds_raw %}
{% assign build = builds.response[0] %}
<a href="{{ build.url }}">Download {{ build.filename }}</a><br>

[Telegram support group](https://t.me/Exynos9820AOSP)<br>
Source used in builds can be found at [GitHub](https://github.com/SealsPlayground)

{% include donations.md %}
