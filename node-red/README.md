# Node-RED Hass.io Add-On
---------

[Hass.io](https://home-assistant.io/hassio/) add-on for [Node-RED](https://nodered.org/).

## Installation

1. Add my [Hass.io](https://home-assistant.io/hassio/) add-on [repository](https://github.com/notoriousbdg/hassio-addons)
2. Install the "Node-RED" add-on
3. Start the "Node-RED" add-on
4. (Optional) Configure [panel_iframe](https://home-assistant.io/components/panel_iframe/) component to embed Node-RED UI into Home Assistant UI using this example:

```yaml
iframe_panel:
  nodered_flows:
    title: 'Node-RED Flows'
    url: 'http://hassio.local:1880'
    icon: mdi:nodejs
```
5. (Optional) If you install [Node-RED Dashboard](https://github.com/node-red/node-red-dashboard) in Node-RED, you can expose the dashboard in the [Hass.io](https://home-assistant.io/hassio/) UI using this example to your [panel_iframe](https://home-assistant.io/components/panel_iframe/) section:
```yaml
iframe_panel:
  nodered_ui:
    title: 'Node-RED Dashboard'
    url: 'http://hassio.local:1880/ui'
    icon: mdi:nodejs
```

## Support

Something doesn't work as expected? Please open an [issue](https://github.com/notoriousbdg/hassio-addons/issues).