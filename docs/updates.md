# Updates Card

## Screenshot
<img src="../screenshots/updates.png" raw=true alt="Updates"/>  
<br/><br/>

# Requirements
* [HACS](https://hacs.xyz/) Installed and `sensor.hacs` enabled
* [auto-entities](https://github.com/thomasloven/lovelace-auto-entities) card (can be installed via HACS)
* Home Assistant Supervisor and enabled `binary_sensor` entities for desired Add-ons (available since core release 2021.4)
* _Optional:_ [Vertical Stack in Card](https://github.com/ofekashery/vertical-stack-in-card) instead of `vertical-stack` for a sleeker design
<br/><br/>

# Code
```
type: vertical-stack
cards:
  - type: conditional
    conditions:
      - entity: sensor.hacs
        state_not: '0'
    card:
      type: markdown
      content: >-
        {% for repo in state_attr('sensor.hacs', 'repositories') %}

        **{{ repo.display_name }}** _{{ repo["installed_version"] }}_ -> _{{ repo["available_version"] }}_

        {% endfor %}
      title: Hacs Updates
  - type: custom:auto-entities
    card:
      type: entities
      title: Add-on Updates
      show_header_toggle: false
    filter:
      include:
        - entity_id: binary_sensor.*update*
          state: 'on'
          options:
            secondary_info: last-changed
      exclude: []
    sort:
      method: entity_id
    show_empty: false
```

## Thanks
The content of the HACS markdown card is inspired by [this automation recipe](https://hacs.xyz/docs/basic/automation/#updates-pending) from HACS Team, regarding updates notifications.