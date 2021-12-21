### Room

> NOTE
> This card is under active development and is not ready to use!

![Room](./screenshots/room.png)

<details>
<summary>Usage</summary>

#### Example

```yaml
- type: 'custom:button-card'
  template:
    - card_room
    - blue
  entity: climate.vicare_heating
  name: Living
  icon: mdi:sofa-outline
```

#### Variables
<table>
<tr>
<th>Variable</th>
<th>Example</th>
<th>Required</th>
<th>Explanation</th>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</table>
<br />
</details>

<details>
<summary>Template code</summary>

```yaml
card_room:
  tap_action:
    action: more-info
  color: var(--google-grey-500)
  show_icon: true
  show_name: true
  show_label: true
  size: 55px
  label: |-
      [[[
          var temperature = entity.attributes.room_temperature;
          if (temperature == null) {
            var temperature = '-';
          }
          return temperature + '°C'
      ]]]
  styles:
    card:
      - border-radius: 20px
      - box-shadow: var(--box-shadow)
      - padding: 1px
    grid:
      - grid-template-areas: '"n n" "l l" "i icon1"'
      - grid-template-columns: 1fr 1fr
      - grid-template-rows: min-content
    icon:
      - left: 4px
      - bottom: 10px
      - color: 'rgba(var(--color-theme),0.2)'
    img_cell:
      - background-color: 'rgba(var(--color-theme),0.05)'
      - border-radius: 50%
      - place-self: end
      - width: 102px
      - height: 82px
      - margin-left: -30px
      - top: 22px
      - padding: 10px
    name:
      - align-self: end
      - justify-self: start
      - font-weight: bold
      - font-size: 20px
      - margin-left: 15px
      - margin-top: 8px
    label:
      - justify-self: start
      - align-self: start
      - font-weight: bolder
      - font-size: 12px
      - filter: opacity(40%)
      - margin-left: 15px
    state:
      - justify-self: start
      - align-self: start
      - font-weight: bolder
      - font-size: 12px
      - filter: opacity(40%)
      - margin-left: 12px
```
</details>
