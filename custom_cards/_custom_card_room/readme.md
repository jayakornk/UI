### Room

> NOTE
> This card is under active development and is not ready to use!

![Room](../../screenshots/room.png)

<details>
<summary>Usage</summary>

#### Example

```yaml
- type: "custom:button-card"
  template:
    - card_room
  variables:
    entity_id_1: light.living_room_floor_light_1
    entity_id_2: switch.living_room_plug_wall_1
    entity_id_3: sensor.living_room_wall_multi_sensor_temperature
    entity_id_4: media_player.kitchen_speaker_1
    color_icon_1: yellow
    color_icon_2: green
    color_icon_3: red
    color_icon_4: blue
    color_bg_1: yellow
    color_bg_2: green
    color_bg_3: red
    color_bg_4: blue
  entity: climate.anna
  name: Living Room
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

#### Code
Template can be found [here](./custom_card_room.yaml)
